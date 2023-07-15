# Comparing `tmp/checkatlas-0.3.2.tar.gz` & `tmp/checkatlas-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.3.2.tar", max compression
+gzip compressed data, was "checkatlas-0.3.3.tar", max compression
```

## Comparing `checkatlas-0.3.2.tar` & `checkatlas-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1506 2023-07-14 14:21:31.935068 checkatlas-0.3.2/LICENSE
--rw-r--r--   0        0        0     4452 2023-07-14 14:21:31.939068 checkatlas-0.3.2/README.md
--rw-r--r--   0        0        0      111 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/__init__.py
--rw-r--r--   0        0        0     4648 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/__main__.py
--rw-r--r--   0        0        0    24201 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/atlas.py
--rw-r--r--   0        0        0     4715 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/cellranger.py
--rw-r--r--   0        0        0     8494 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/checkatlas.py
--rw-r--r--   0        0        0       45 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4108 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0    20177 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/seurat.py
--rw-r--r--   0        0        0      107 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/__init__.py
--rw-r--r--   0        0        0     4544 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/checkatlas_arguments.py
--rw-r--r--   0        0        0     2230 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/files.py
--rw-r--r--   0        0        0     2065 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/folders.py
--rw-r--r--   0        0        0     6267 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/obsolete_arguments.py
--rw-r--r--   0        0        0     1350 2023-07-14 14:21:32.131070 checkatlas-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 checkatlas-0.3.2/setup.py
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-15 15:46:21.660234 checkatlas-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4452 2023-07-15 15:46:21.660234 checkatlas-0.3.3/README.md
+-rw-r--r--   0        0        0      111 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4652 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24201 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/atlas.py
+-rw-r--r--   0        0        0     4715 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/cellranger.py
+-rw-r--r--   0        0        0     8485 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0     2785 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/checkatlas_workflow.py
+-rw-r--r--   0        0        0       45 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4108 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20177 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/seurat.py
+-rw-r--r--   0        0        0      107 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4563 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     4239 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/checkatlas_workflow_arguments.py
+-rw-r--r--   0        0        0     2759 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     2065 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1410 2023-07-15 15:46:21.852237 checkatlas-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 checkatlas-0.3.3/setup.py
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.3/PKG-INFO
```

### Comparing `checkatlas-0.3.2/LICENSE` & `checkatlas-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/README.md` & `checkatlas-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/__main__.py` & `checkatlas-0.3.3/checkatlas/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,8 +105,8 @@
         elif process == checkatlas.PROCESS_TYPE[3]:
             seurat_data = seurat.read_atlas(atlas_info)
             seurat.create_metric_annot(seurat_data, atlas_info, args)
         elif process == checkatlas.PROCESS_TYPE[4]:
             seurat_data = seurat.read_atlas(atlas_info)
             seurat.create_metric_dimred(seurat_data, atlas_info, args)
     else:
-        logger.debug("TO DO : Seurat is no longer managed here !!!")
+        logger.debug("TO DO : Spatial Transcriptomics not yet managed.")
```

### Comparing `checkatlas-0.3.2/checkatlas/atlas.py` & `checkatlas-0.3.3/checkatlas/atlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/cellranger.py` & `checkatlas-0.3.3/checkatlas/cellranger.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/checkatlas.py` & `checkatlas-0.3.3/checkatlas/checkatlas.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,42 +139,42 @@
             if qc_fig.endswith(".png"):
                 atlas_name = os.path.splitext(os.path.basename(qc_fig))[0]
                 print(atlas_name)
                 print("qc", qc_fig)
                 qc_dict[atlas_name] = qc_fig
         html = create_img_html_content(type_viz, qc_dict)
         with open(
-            os.path.join("../", qc_fig_path, "QC_report_mqc.html"), "w"
+            chk_files.get_html_qc_report_path(checkatlas_path), "w"
         ) as html_report:
             html_report.write(html)
     elif type_viz == "reductions":
         umap_dict = dict()
         umap_fig_path = folders.get_folder(checkatlas_path, folders.UMAP)
         for umap_fig in os.listdir(umap_fig_path):
             if umap_fig.endswith(".png"):
                 atlas_name = os.path.splitext(os.path.basename(umap_fig))[0]
                 print(umap_fig)
                 umap_dict[atlas_name] = umap_fig
         html = create_img_html_content(type_viz, umap_dict)
         with open(
-            os.path.join("../", umap_fig_path, "Umap_report_mqc.html"), "w"
+            chk_files.get_html_umap_report_path(checkatlas_path), "w"
         ) as html_report:
             html_report.write(html)
 
         tsne_dict = dict()
         tsne_fig_path = folders.get_folder(checkatlas_path, folders.TSNE)
         for tsne_fig in os.listdir(tsne_fig_path):
             if tsne_fig.endswith(".png"):
                 atlas_name = os.path.splitext(os.path.basename(tsne_fig))[0]
                 print(atlas_name)
                 print("tsne", tsne_fig)
                 tsne_dict[atlas_name] = tsne_fig
         html = create_img_html_content(type_viz, tsne_dict)
         with open(
-            os.path.join(tsne_fig_path, "Tsne_report_mqc.html"), "w"
+            chk_files.get_html_tsne_report_path(checkatlas_path), "w"
         ) as html_report:
             html_report.write(html)
     else:
         logger.error(f"Type of vsualization not recognized {type_viz}")
 
 
 def create_img_html_content(type_viz, data):
```

### Comparing `checkatlas-0.3.2/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.3.3/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/metrics/metrics.py` & `checkatlas-0.3.3/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.3.3/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.3.3/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.3.3/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.3.3/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/seurat.py` & `checkatlas-0.3.3/checkatlas/seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/utils/checkatlas_arguments.py` & `checkatlas-0.3.3/checkatlas/utils/checkatlas_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from checkatlas import atlas, checkatlas
 from checkatlas.metrics import annot, cluster, dimred
 
 
 def create_parser():
     parser = argparse.ArgumentParser(
         prog="checkatlas",
-        usage="checkatlas [OPTIONS] your_search_folder/",
+        usage="checkatlas [OPTIONS] process atlas_name your_search_folder/",
         description="CheckAtlas is a one liner tool to check the "
         "quality of your single-cell atlases. For "
         "every atlas, it produces the quality control "
         "tables and figures which can be then processed "
         "by multiqc. CheckAtlas is able to load Scanpy, "
         "Seurat, and CellRanger files.",
         epilog="Enjoy the checkatlas functionality!",
```

### Comparing `checkatlas-0.3.2/checkatlas/utils/files.py` & `checkatlas-0.3.3/checkatlas/utils/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,7 +76,28 @@
     for table_info in clean_seurat_list:
         df_summary.loc[
             table_info[checkatlas.ATLAS_NAME_KEY]
         ] = table_info.values()
     df_summary.to_csv(
         get_table_seurat_path(checkatlas_path), index=False, sep=","
     )
+
+
+def get_html_qc_report_path(checkatlas_path: str):
+    return os.path.join(
+        folders.get_folder(checkatlas_path, folders.QC_FIG),
+        "QC_report_mqc.html",
+    )
+
+
+def get_html_umap_report_path(checkatlas_path: str):
+    return os.path.join(
+        folders.get_folder(checkatlas_path, folders.UMAP),
+        "UMAP_report_mqc.html",
+    )
+
+
+def get_html_tsne_report_path(checkatlas_path: str):
+    return os.path.join(
+        folders.get_folder(checkatlas_path, folders.TSNE),
+        "tSNE_report_mqc.html",
+    )
```

### Comparing `checkatlas-0.3.2/checkatlas/utils/folders.py` & `checkatlas-0.3.3/checkatlas/utils/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/checkatlas/utils/obsolete_arguments.py` & `checkatlas-0.3.3/checkatlas/utils/obsolete_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.2/pyproject.toml` & `checkatlas-0.3.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.3.2"
+version = "0.3.3"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
@@ -52,7 +52,8 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 checkatlas = 'checkatlas.__main__:main'
+checkatlas-workflow = 'checkatlas.checkatlas_workflow:main'
```

### Comparing `checkatlas-0.3.2/setup.py` & `checkatlas-0.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,21 @@
  'poetry>=1.5.1,<2.0.0',
  'rpy2==3.5.10',
  'scanpy>=1.9.1,<2.0.0',
  'scikit-learn>=1.2.1,<2.0.0',
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
 entry_points = \
-{'console_scripts': ['checkatlas = checkatlas.__main__:main']}
+{'console_scripts': ['checkatlas = checkatlas.__main__:main',
+                     'checkatlas-workflow = '
+                     'checkatlas.checkatlas_workflow:main']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
```

### Comparing `checkatlas-0.3.2/PKG-INFO` & `checkatlas-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.3.2
+Version: 0.3.3
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: BSD 3-Clause
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

