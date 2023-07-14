# Comparing `tmp/geneplexus-1.0.0.dev4.tar.gz` & `tmp/geneplexus-1.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneplexus-1.0.0.dev4.tar", last modified: Mon Jun 27 20:04:20 2022, max compression
+gzip compressed data, was "geneplexus-1.0.0.dev5.tar", last modified: Wed Aug 10 17:24:14 2022, max compression
```

## Comparing `geneplexus-1.0.0.dev4.tar` & `geneplexus-1.0.0.dev5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:04:20.151391 geneplexus-1.0.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5271 2022-06-27 20:04:20.151391 geneplexus-1.0.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:04:20.151391 geneplexus-1.0.0.dev4/geneplexus/
--rw-r--r--   0 runner    (1001) docker     (121)     5410 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:04:20.151391 geneplexus-1.0.0.dev4/geneplexus/_config/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/_config/config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5355 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/_config/data_filenames.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/_config/logger_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    10849 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/_geneplexus.py
--rw-r--r--   0 runner    (1001) docker     (121)     9432 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5477 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/custom.py
--rw-r--r--   0 runner    (1001) docker     (121)    10721 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/download.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16043 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/geneplexus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9278 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/geneplexus/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:04:20.151391 geneplexus-1.0.0.dev4/geneplexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5271 2022-06-27 20:04:20.000000 geneplexus-1.0.0.dev4/geneplexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-06-27 20:04:20.000000 geneplexus-1.0.0.dev4/geneplexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 20:04:20.000000 geneplexus-1.0.0.dev4/geneplexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-27 20:04:20.000000 geneplexus-1.0.0.dev4/geneplexus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-27 20:04:20.000000 geneplexus-1.0.0.dev4/geneplexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-27 20:04:20.000000 geneplexus-1.0.0.dev4/geneplexus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-06-27 20:04:20.151391 geneplexus-1.0.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 20:04:20.151391 geneplexus-1.0.0.dev4/test/
--rw-r--r--   0 runner    (1001) docker     (121)     5340 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/test/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/test/test_geneplexus.py
--rw-r--r--   0 runner    (1001) docker     (121)     8140 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-06-27 20:04:12.000000 geneplexus-1.0.0.dev4/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 17:24:14.550348 geneplexus-1.0.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5251 2022-08-10 17:24:14.550348 geneplexus-1.0.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 17:24:14.546348 geneplexus-1.0.0.dev5/geneplexus/
+-rw-r--r--   0 runner    (1001) docker     (121)     5495 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 17:24:14.550348 geneplexus-1.0.0.dev5/geneplexus/_config/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/_config/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5355 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/_config/data_filenames.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/_config/logger_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10841 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/_geneplexus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9432 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5477 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/custom.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10721 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16314 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/geneplexus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9278 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/geneplexus/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 17:24:14.550348 geneplexus-1.0.0.dev5/geneplexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5251 2022-08-10 17:24:14.000000 geneplexus-1.0.0.dev5/geneplexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-08-10 17:24:14.000000 geneplexus-1.0.0.dev5/geneplexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 17:24:14.000000 geneplexus-1.0.0.dev5/geneplexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-10 17:24:14.000000 geneplexus-1.0.0.dev5/geneplexus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-10 17:24:14.000000 geneplexus-1.0.0.dev5/geneplexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-10 17:24:14.000000 geneplexus-1.0.0.dev5/geneplexus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-08-10 17:24:14.550348 geneplexus-1.0.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 17:24:14.550348 geneplexus-1.0.0.dev5/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     5340 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/test/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/test/test_geneplexus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-08-10 17:24:04.000000 geneplexus-1.0.0.dev5/test/test_util.py
```

### Comparing `geneplexus-1.0.0.dev4/PKG-INFO` & `geneplexus-1.0.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: geneplexus
-Version: 1.0.0.dev4
+Version: 1.0.0.dev5
 Summary: Network based gene classification
 Home-page: https://github.com/krishnanlab/PyGenePlexus
 Author: Remy Liu and Christopher A. Mancuso
 Author-email: liurenmi@msu.edu, mancus16@msu.edu
 License: Creative Commons License: Attribution 4.0 International
 Project-URL: Documentation, https://pygeneplexus.readthedocs.io
 Keywords: Network Biology,Supervised Learning,Gene Classification
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -125,9 +124,7 @@
 1. Install doc dependencies ``pip install -r docs/requirements.txt``
 2. Build
 ```bash
 cd docs
 make html
 ```
 3. Open doc ``open build/html/index.html``
-
-
```

### Comparing `geneplexus-1.0.0.dev4/README.md` & `geneplexus-1.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus/__init__.py` & `geneplexus-1.0.0.dev5/geneplexus/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 .. currentmodule:: geneplexus.GenePlexus
 
 PyGenePlexus enables researchers to predict novel genes similar to their
 genes of interest based on their patterns of connectivity in genome-scale
 molecular interaction networks.
 
 .. figure:: ../figures/mainfigure.png
-  :scale: 30 %
+  :scale: 20 %
   :align: center
   :alt: My Text
 
-  Probably put Figure from the paper here?
+  Overview of PyGenePlexus
 
 Given a list of input genes and a geneset collection (:term:`GSC`) to help
 select negative examples, the package trains a logistic regression model
 using one of three network derived features (:term:`adjacency`,
 :term:`influence`, or :term:`embedding`) and generates the following outputs
 
 #. Genome-wide prediction of how **functionally similar** a gene is  to the \
@@ -36,14 +36,16 @@
 <https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkac335/6586869?login=true>`_
     * `GenePlexus Benchmarking Paper \
 <https://academic.oup.com/bioinformatics/article/36/11/3457/5780279>`_
     * `GenePlexus Benchmarking Paper Repo \
 <https://github.com/krishnanlab/GenePlexus>`_
     * `PyGenePlexus PyPi Package <https://pypi.org/project/geneplexus/>`_
     * `PyGenePlexus GitHub Repo <https://github.com/krishnanlab/PyGenePlexus>`_
+    * `PyGenePlexus Paper \
+<https://www.biorxiv.org/content/10.1101/2022.07.02.498552v1.abstract>`_
 
 Quick start
 -----------
 
 PyGenePlexus comes with an easy to use command line interface (CLI) to run the
 full GenePlexus pipeline given an input gene list. Go get started, install via
 pip and run a quick example as follows.
```

### Comparing `geneplexus-1.0.0.dev4/geneplexus/_config/config.py` & `geneplexus-1.0.0.dev5/geneplexus/_config/config.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus/_config/data_filenames.txt` & `geneplexus-1.0.0.dev5/geneplexus/_config/data_filenames.txt`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus/_config/logger_util.py` & `geneplexus-1.0.0.dev5/geneplexus/_config/logger_util.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus/_geneplexus.py` & `geneplexus-1.0.0.dev5/geneplexus/_geneplexus.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from scipy.stats import hypergeom
 from scipy.stats import rankdata
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import average_precision_score
 from sklearn.model_selection import StratifiedKFold
 from sklearn.preprocessing import StandardScaler
 
-from . import config
 from . import util
 from ._config import logger
 from ._config.config import DEFAULT_LOGREG_KWARGS
 
 
 def _initial_id_convert(input_genes, file_loc):
     # load all the possible conversion dictionaries
@@ -52,15 +51,15 @@
 
 
 def _make_validation_df(df_convert_out, file_loc):
     table_summary = []
     input_count = df_convert_out.shape[0]
     converted_genes = df_convert_out["Entrez ID"].to_numpy()
 
-    for anet in config.ALL_NETWORKS:
+    for anet in util.get_all_net_types(file_loc):
         net_genes = util.load_node_order(file_loc, anet)
         df_tmp = df_convert_out[df_convert_out["Entrez ID"].isin(net_genes)]
         pos_genes_in_net = np.intersect1d(converted_genes, net_genes)
         table_row = {"Network": anet, "NetworkGenes": len(net_genes), "PositiveGenes": len(pos_genes_in_net)}
         table_summary.append(dict(table_row))
         tmp_ins = np.full(len(converted_genes), "N", dtype=str)
         tmp_ins[df_tmp.index.to_numpy()] = "Y"
```

### Comparing `geneplexus-1.0.0.dev4/geneplexus/cli.py` & `geneplexus-1.0.0.dev5/geneplexus/cli.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus/custom.py` & `geneplexus-1.0.0.dev5/geneplexus/custom.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus/download.py` & `geneplexus-1.0.0.dev5/geneplexus/download.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus/geneplexus.py` & `geneplexus-1.0.0.dev5/geneplexus/geneplexus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """GenePlexus API."""
 import os
 import os.path as osp
+import warnings
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import pystow
 import yaml
@@ -43,25 +44,31 @@
                 later if not specified at init time by simply calling
                 :meth:`load_genes` (default: :obj:`None`).
             auto_download: Automatically download necessary files if set.
             log_level: Logging level.
 
         """
         set_stream_level(logger, log_level)
+        self._is_custom: bool = False
         self.file_loc = file_loc  # type: ignore
         self.features = features
         self.gsc = gsc
         self.net_type = net_type
         self.log_level = log_level
         self.auto_download = auto_download
         self.input_genes: List[str] = []
 
         self.check_custom()
 
-        if self.auto_download:
+        if self.auto_download and self._is_custom:
+            warnings.warn(
+                f"Skipping auto download for custom network {self.net_type}. "
+                "Unset auto_download option to suppress this message.",
+            )
+        elif self.auto_download:
             download_select_data(
                 self.file_loc,
                 "All",
                 self.net_type,
                 self.features,
                 ["GO", "DisGeNet"],
                 log_level=log_level,
@@ -110,22 +117,22 @@
     @property
     def net_type(self) -> config.NET_TYPE:
         """Network to use."""
         return self._net_type  # type: ignore
 
     @net_type.setter
     def net_type(self, net_type: config.NET_TYPE):
-        self._standard_net_type = self._custom_net_type = None
         util.check_param("network", net_type, util.get_all_net_types(self.file_loc))
         if net_type not in config.ALL_NETWORKS:
             data_files = os.listdir(self.file_loc)
             node_order_fn = f"NodeOrder_{net_type}.txt"
             if node_order_fn not in data_files:
                 raise ValueError(f"Missing file {node_order_fn} for custom network {net_type}")
 
+            self._is_custom = True
             logger.info(f"Using custom network {net_type!r}")
 
         self._net_type = net_type
 
     @property
     def features(self) -> config.FEATURE_TYPE:
         """Features to use."""
```

### Comparing `geneplexus-1.0.0.dev4/geneplexus/util.py` & `geneplexus-1.0.0.dev5/geneplexus/util.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/geneplexus.egg-info/PKG-INFO` & `geneplexus-1.0.0.dev5/geneplexus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: geneplexus
-Version: 1.0.0.dev4
+Version: 1.0.0.dev5
 Summary: Network based gene classification
 Home-page: https://github.com/krishnanlab/PyGenePlexus
 Author: Remy Liu and Christopher A. Mancuso
 Author-email: liurenmi@msu.edu, mancus16@msu.edu
 License: Creative Commons License: Attribution 4.0 International
 Project-URL: Documentation, https://pygeneplexus.readthedocs.io
 Keywords: Network Biology,Supervised Learning,Gene Classification
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -125,9 +124,7 @@
 1. Install doc dependencies ``pip install -r docs/requirements.txt``
 2. Build
 ```bash
 cd docs
 make html
 ```
 3. Open doc ``open build/html/index.html``
-
-
```

### Comparing `geneplexus-1.0.0.dev4/geneplexus.egg-info/SOURCES.txt` & `geneplexus-1.0.0.dev5/geneplexus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/setup.cfg` & `geneplexus-1.0.0.dev5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geneplexus
-version = 1.0.0-dev.4
+version = 1.0.0-dev.5
 description = Network based gene classification
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/krishnanlab/PyGenePlexus
 project_urls = 
 	Documentation = https://pygeneplexus.readthedocs.io
 author = Remy Liu and Christopher A. Mancuso
```

### Comparing `geneplexus-1.0.0.dev4/test/test_custom.py` & `geneplexus-1.0.0.dev5/test/test_custom.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/test/test_download.py` & `geneplexus-1.0.0.dev5/test/test_download.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/test/test_geneplexus.py` & `geneplexus-1.0.0.dev5/test/test_geneplexus.py`

 * *Files identical despite different names*

### Comparing `geneplexus-1.0.0.dev4/test/test_pipeline.py` & `geneplexus-1.0.0.dev5/test/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         df_convert_out = self.gp.df_convert_out.copy()
         columns = ["Original ID", "Entrez ID"]
         df_convert_out[columns] = df_convert_out[columns].astype(int)
 
         path = osp.join(pytest.ANSWERDIR, "df_convert_out.tsv")
         df_convert_out_expected = pd.read_csv(path, sep="\t")
         self.assertEqual(
-            df_convert_out.values.tolist(),
+            df_convert_out[df_convert_out_expected.columns].values.tolist(),
             df_convert_out_expected.values.tolist(),
         )
 
     @pytest.mark.order(3)
     def test_get_pos_and_neg_genes(self):
         self.gp._get_pos_and_neg_genes()
```

### Comparing `geneplexus-1.0.0.dev4/test/test_util.py` & `geneplexus-1.0.0.dev5/test/test_util.py`

 * *Files identical despite different names*

