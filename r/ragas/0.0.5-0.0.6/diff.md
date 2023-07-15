# Comparing `tmp/ragas-0.0.5.tar.gz` & `tmp/ragas-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.5.tar", last modified: Mon Jul 10 10:56:29 2023, max compression
+gzip compressed data, was "ragas-0.0.6.tar", last modified: Sat Jul 15 06:28:35 2023, max compression
```

## Comparing `ragas-0.0.5.tar` & `ragas-0.0.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:18.000000 ragas-0.0.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-10 10:56:18.000000 ragas-0.0.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-10 10:56:18.000000 ragas-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-10 10:56:18.000000 ragas-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 10:56:18.000000 ragas-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-10 10:56:18.000000 ragas-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-10 10:56:29.196072 ragas-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-10 10:56:18.000000 ragas-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-10 10:56:18.000000 ragas-0.0.5/docs/assets/bar-graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-10 10:56:18.000000 ragas-0.0.5/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-10 10:56:18.000000 ragas-0.0.5/docs/guides/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-10 10:56:18.000000 ragas-0.0.5/docs/metrics.md
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-10 10:56:18.000000 ragas-0.0.5/docs/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 10:56:18.000000 ragas-0.0.5/experiments/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/experiments/assesments/
--rw-r--r--   0 runner    (1001) docker     (123)    26468 2023-07-10 10:56:18.000000 ragas-0.0.5/experiments/assesments/metrics_assesments.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/experiments/baselines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/experiments/baselines/fiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-10 10:56:18.000000 ragas-0.0.5/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-10 10:56:18.000000 ragas-0.0.5/experiments/baselines/fiqa/improving-baselines.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/experiments/baselines/hotpotqa/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-10 10:56:18.000000 ragas-0.0.5/experiments/baselines/hotpotqa/explore-dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/experiments/baselines/wikiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-10 10:56:18.000000 ragas-0.0.5/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-10 10:56:18.000000 ragas-0.0.5/experiments/baselines/wikiqa/failed_wikis
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-10 10:56:18.000000 ragas-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-10 10:56:18.000000 ragas-0.0.5/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 10:56:18.000000 ragas-0.0.5/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 10:56:18.000000 ragas-0.0.5/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:56:29.196072 ragas-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 10:56:29.000000 ragas-0.0.5/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/metrics/answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/metrics/context_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/metrics/factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/metrics/llms.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 10:56:18.000000 ragas-0.0.5/src/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-10 10:56:29.000000 ragas-0.0.5/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-10 10:56:29.000000 ragas-0.0.5/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:56:29.000000 ragas-0.0.5/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 10:56:29.000000 ragas-0.0.5/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 10:56:29.000000 ragas-0.0.5/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.192072 ragas-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-10 10:56:18.000000 ragas-0.0.5/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-10 10:56:18.000000 ragas-0.0.5/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:56:29.196072 ragas-0.0.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-10 10:56:18.000000 ragas-0.0.5/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 10:56:18.000000 ragas-0.0.5/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:22.000000 ragas-0.0.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.619446 ragas-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-15 06:28:22.000000 ragas-0.0.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-15 06:28:22.000000 ragas-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-15 06:28:22.000000 ragas-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 06:28:22.000000 ragas-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-15 06:28:22.000000 ragas-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-15 06:28:35.631446 ragas-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-15 06:28:22.000000 ragas-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/assets/bar-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/guides/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/experiments/assesments/
+-rw-r--r--   0 runner    (1001) docker     (123)    47692 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/assesments/metrics_assesments.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.623446 ragas-0.0.6/experiments/baselines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/experiments/baselines/fiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/fiqa/improving-baselines.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/experiments/baselines/hotpotqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/hotpotqa/explore-dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/experiments/baselines/wikiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/wikiqa/failed_wikis
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-15 06:28:22.000000 ragas-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-15 06:28:22.000000 ragas-0.0.6/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 06:28:22.000000 ragas-0.0.6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 06:28:22.000000 ragas-0.0.6/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:28:35.631446 ragas-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.623446 ragas-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/context_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/faithfulnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.623446 ragas-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/unit/test_simple.py
```

### Comparing `ragas-0.0.5/.github/workflows/ci.yaml` & `ragas-0.0.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/.github/workflows/python-publish.yml` & `ragas-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/.gitignore` & `ragas-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/LICENSE` & `ragas-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/Makefile` & `ragas-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/PKG-INFO` & `ragas-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
-  <i>SOTA metrics for evaluating Retrieval Augmented Generation (RAG)</i>
+  <i>Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines</i>
 </p>
 
 <p align="center">
     <a href="https://github.com/explodinggradients/ragas/releases">
         <img alt="GitHub release" src="https://img.shields.io/github/release/explodinggradients/ragas.svg">
     </a>
     <a href="https://www.python.org/">
@@ -84,15 +84,16 @@
 # 'faithfulness': 0.892, 'answer_relevancy': 0.874}
 ```
 If you want a more in-depth explanation of core components, check out our [quick-start notebook](./docs/quickstart.ipynb)
 ## :luggage: Metrics
 
 Ragas measures your pipeline's performance against two dimensions
 1. **Faithfulness**: measures the information consistency of the generated answer against the given context. If any claims made in the answer that cannot be deduced from context is penalized. 
-2. **Relevancy**:  measures how relevant retrieved contexts and the generated answer are to the question. The presence of extra or redundant information is penalized. 
+2. **Context Relevancy**:  measures how relevant retrieved contexts is to the question. Ideally the context should only contain information necessary to answer the question. The presence of redundant information in the context is penalized.
+3. **Answer Relevancy**: measures how relevant generated answer is to the question. This do not ensure factuality of the generated answer rather penalizes the presence of redundant information in the generated answer.
 
 Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors. 
 
 To read more about our metrics, checkout [docs](/docs/metrics.md).
 ## 🫂 Community
 If you want to get more involved with Ragas, check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out about LLM, Retrieval, Production issues and more.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.5 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.6 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
-       SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
+ Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
 external data to augment the LLMâs context. There are existing tools and
 frameworks that help you build these pipelines but evaluating it and
@@ -23,40 +23,44 @@
 num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) #
 {'ragas_score': 0.860, 'context_relavency': 0.817, # 'faithfulness': 0.892,
 'answer_relevancy': 0.874} ``` If you want a more in-depth explanation of core
 components, check out our [quick-start notebook](./docs/quickstart.ipynb) ## :
 luggage: Metrics Ragas measures your pipeline's performance against two
 dimensions 1. **Faithfulness**: measures the information consistency of the
 generated answer against the given context. If any claims made in the answer
-that cannot be deduced from context is penalized. 2. **Relevancy**: measures
-how relevant retrieved contexts and the generated answer are to the question.
-The presence of extra or redundant information is penalized. Through repeated
-experiments, we have found that the quality of a RAG pipeline is highly
-dependent on these two dimensions. The final `ragas_score` is the harmonic mean
-of these two factors. To read more about our metrics, checkout [docs](/docs/
-metrics.md). ## ð« Community If you want to get more involved with Ragas,
-check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun
-community where we geek out about LLM, Retrieval, Production issues and more.
-## ð Open Analytics We track very basic usage metrics to guide us to figure
-out what our users want, what is working and what's not. As a young startup, we
-have to be brutally honest about this which is why we are tracking these
-metrics. But as an Open Startup we open-source all the data we collect. You can
-read more about this [here](https://github.com/explodinggradients/ragas/issues/
-49). **Ragas doesnot track any information that can be used to identify you or
-your company**. You can take a look at exactly what we track in the [code](./
-src/ragas/_analytics.py) To disable usage-tracking you set the
-`RAGAS_DO_NOT_TRACK` flag to true. ## :raising_hand_man: FAQ 1. Why harmonic
-mean? Harmonic mean penalizes extreme values. For example, if your generated
-answer is fully factually consistent with the context (faithfulness = 1) but is
-not relevant to the question (relevancy = 0), a simple average would give you a
-score of 0.5 but a harmonic mean will give you 0.0 2. How to use Ragas to
-improve your pipeline? *"Measurement is the first step that leads to control
-and eventually to improvement" - James Harrington* Here we assume that you
-already have your RAG pipeline ready. When it comes to RAG pipelines, there are
-mainly two parts - Retriever and generator. A change in any of this should also
-impact your pipelines's quality. 1. First, decide one parameter that you're
-interested in adjusting. for example the number of retrieved documents, K. 2.
-Collect a set of sample prompts (min 20) to form your test set. 3. Run your
-pipeline using the test set before and after the change. Each time record the
-prompts with context and generated output. 4. Run ragas evaluation for each of
-them to generate evaluation scores. 5. Compare the scores and you will know how
-much the change has affected your pipelines' performance.
+that cannot be deduced from context is penalized. 2. **Context Relevancy**:
+measures how relevant retrieved contexts is to the question. Ideally the
+context should only contain information necessary to answer the question. The
+presence of redundant information in the context is penalized. 3. **Answer
+Relevancy**: measures how relevant generated answer is to the question. This do
+not ensure factuality of the generated answer rather penalizes the presence of
+redundant information in the generated answer. Through repeated experiments, we
+have found that the quality of a RAG pipeline is highly dependent on these two
+dimensions. The final `ragas_score` is the harmonic mean of these two factors.
+To read more about our metrics, checkout [docs](/docs/metrics.md). ## ð«
+Community If you want to get more involved with Ragas, check out our [discord
+server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out
+about LLM, Retrieval, Production issues and more. ## ð Open Analytics We
+track very basic usage metrics to guide us to figure out what our users want,
+what is working and what's not. As a young startup, we have to be brutally
+honest about this which is why we are tracking these metrics. But as an Open
+Startup we open-source all the data we collect. You can read more about this
+[here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot
+track any information that can be used to identify you or your company**. You
+can take a look at exactly what we track in the [code](./src/ragas/
+_analytics.py) To disable usage-tracking you set the `RAGAS_DO_NOT_TRACK` flag
+to true. ## :raising_hand_man: FAQ 1. Why harmonic mean? Harmonic mean
+penalizes extreme values. For example, if your generated answer is fully
+factually consistent with the context (faithfulness = 1) but is not relevant to
+the question (relevancy = 0), a simple average would give you a score of 0.5
+but a harmonic mean will give you 0.0 2. How to use Ragas to improve your
+pipeline? *"Measurement is the first step that leads to control and eventually
+to improvement" - James Harrington* Here we assume that you already have your
+RAG pipeline ready. When it comes to RAG pipelines, there are mainly two parts
+- Retriever and generator. A change in any of this should also impact your
+pipelines's quality. 1. First, decide one parameter that you're interested in
+adjusting. for example the number of retrieved documents, K. 2. Collect a set
+of sample prompts (min 20) to form your test set. 3. Run your pipeline using
+the test set before and after the change. Each time record the prompts with
+context and generated output. 4. Run ragas evaluation for each of them to
+generate evaluation scores. 5. Compare the scores and you will know how much
+the change has affected your pipelines' performance.
```

### Comparing `ragas-0.0.5/README.md` & `ragas-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
-  <i>SOTA metrics for evaluating Retrieval Augmented Generation (RAG)</i>
+  <i>Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines</i>
 </p>
 
 <p align="center">
     <a href="https://github.com/explodinggradients/ragas/releases">
         <img alt="GitHub release" src="https://img.shields.io/github/release/explodinggradients/ragas.svg">
     </a>
     <a href="https://www.python.org/">
@@ -78,15 +78,16 @@
 # 'faithfulness': 0.892, 'answer_relevancy': 0.874}
 ```
 If you want a more in-depth explanation of core components, check out our [quick-start notebook](./docs/quickstart.ipynb)
 ## :luggage: Metrics
 
 Ragas measures your pipeline's performance against two dimensions
 1. **Faithfulness**: measures the information consistency of the generated answer against the given context. If any claims made in the answer that cannot be deduced from context is penalized. 
-2. **Relevancy**:  measures how relevant retrieved contexts and the generated answer are to the question. The presence of extra or redundant information is penalized. 
+2. **Context Relevancy**:  measures how relevant retrieved contexts is to the question. Ideally the context should only contain information necessary to answer the question. The presence of redundant information in the context is penalized.
+3. **Answer Relevancy**: measures how relevant generated answer is to the question. This do not ensure factuality of the generated answer rather penalizes the presence of redundant information in the generated answer.
 
 Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors. 
 
 To read more about our metrics, checkout [docs](/docs/metrics.md).
 ## 🫂 Community
 If you want to get more involved with Ragas, check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out about LLM, Retrieval, Production issues and more.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                     ****** [./docs/assets/logo.png] ******
-       SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
+ Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
 external data to augment the LLMâs context. There are existing tools and
 frameworks that help you build these pipelines but evaluating it and
@@ -21,40 +21,44 @@
 num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) #
 {'ragas_score': 0.860, 'context_relavency': 0.817, # 'faithfulness': 0.892,
 'answer_relevancy': 0.874} ``` If you want a more in-depth explanation of core
 components, check out our [quick-start notebook](./docs/quickstart.ipynb) ## :
 luggage: Metrics Ragas measures your pipeline's performance against two
 dimensions 1. **Faithfulness**: measures the information consistency of the
 generated answer against the given context. If any claims made in the answer
-that cannot be deduced from context is penalized. 2. **Relevancy**: measures
-how relevant retrieved contexts and the generated answer are to the question.
-The presence of extra or redundant information is penalized. Through repeated
-experiments, we have found that the quality of a RAG pipeline is highly
-dependent on these two dimensions. The final `ragas_score` is the harmonic mean
-of these two factors. To read more about our metrics, checkout [docs](/docs/
-metrics.md). ## ð« Community If you want to get more involved with Ragas,
-check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun
-community where we geek out about LLM, Retrieval, Production issues and more.
-## ð Open Analytics We track very basic usage metrics to guide us to figure
-out what our users want, what is working and what's not. As a young startup, we
-have to be brutally honest about this which is why we are tracking these
-metrics. But as an Open Startup we open-source all the data we collect. You can
-read more about this [here](https://github.com/explodinggradients/ragas/issues/
-49). **Ragas doesnot track any information that can be used to identify you or
-your company**. You can take a look at exactly what we track in the [code](./
-src/ragas/_analytics.py) To disable usage-tracking you set the
-`RAGAS_DO_NOT_TRACK` flag to true. ## :raising_hand_man: FAQ 1. Why harmonic
-mean? Harmonic mean penalizes extreme values. For example, if your generated
-answer is fully factually consistent with the context (faithfulness = 1) but is
-not relevant to the question (relevancy = 0), a simple average would give you a
-score of 0.5 but a harmonic mean will give you 0.0 2. How to use Ragas to
-improve your pipeline? *"Measurement is the first step that leads to control
-and eventually to improvement" - James Harrington* Here we assume that you
-already have your RAG pipeline ready. When it comes to RAG pipelines, there are
-mainly two parts - Retriever and generator. A change in any of this should also
-impact your pipelines's quality. 1. First, decide one parameter that you're
-interested in adjusting. for example the number of retrieved documents, K. 2.
-Collect a set of sample prompts (min 20) to form your test set. 3. Run your
-pipeline using the test set before and after the change. Each time record the
-prompts with context and generated output. 4. Run ragas evaluation for each of
-them to generate evaluation scores. 5. Compare the scores and you will know how
-much the change has affected your pipelines' performance.
+that cannot be deduced from context is penalized. 2. **Context Relevancy**:
+measures how relevant retrieved contexts is to the question. Ideally the
+context should only contain information necessary to answer the question. The
+presence of redundant information in the context is penalized. 3. **Answer
+Relevancy**: measures how relevant generated answer is to the question. This do
+not ensure factuality of the generated answer rather penalizes the presence of
+redundant information in the generated answer. Through repeated experiments, we
+have found that the quality of a RAG pipeline is highly dependent on these two
+dimensions. The final `ragas_score` is the harmonic mean of these two factors.
+To read more about our metrics, checkout [docs](/docs/metrics.md). ## ð«
+Community If you want to get more involved with Ragas, check out our [discord
+server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out
+about LLM, Retrieval, Production issues and more. ## ð Open Analytics We
+track very basic usage metrics to guide us to figure out what our users want,
+what is working and what's not. As a young startup, we have to be brutally
+honest about this which is why we are tracking these metrics. But as an Open
+Startup we open-source all the data we collect. You can read more about this
+[here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot
+track any information that can be used to identify you or your company**. You
+can take a look at exactly what we track in the [code](./src/ragas/
+_analytics.py) To disable usage-tracking you set the `RAGAS_DO_NOT_TRACK` flag
+to true. ## :raising_hand_man: FAQ 1. Why harmonic mean? Harmonic mean
+penalizes extreme values. For example, if your generated answer is fully
+factually consistent with the context (faithfulness = 1) but is not relevant to
+the question (relevancy = 0), a simple average would give you a score of 0.5
+but a harmonic mean will give you 0.0 2. How to use Ragas to improve your
+pipeline? *"Measurement is the first step that leads to control and eventually
+to improvement" - James Harrington* Here we assume that you already have your
+RAG pipeline ready. When it comes to RAG pipelines, there are mainly two parts
+- Retriever and generator. A change in any of this should also impact your
+pipelines's quality. 1. First, decide one parameter that you're interested in
+adjusting. for example the number of retrieved documents, K. 2. Collect a set
+of sample prompts (min 20) to form your test set. 3. Run your pipeline using
+the test set before and after the change. Each time record the prompts with
+context and generated output. 4. Run ragas evaluation for each of them to
+generate evaluation scores. 5. Compare the scores and you will know how much
+the change has affected your pipelines' performance.
```

### Comparing `ragas-0.0.5/docs/assets/bar-graph.svg` & `ragas-0.0.6/docs/assets/bar-graph.svg`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/docs/assets/logo.png` & `ragas-0.0.6/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/docs/guides/data_prep.py` & `ragas-0.0.6/docs/guides/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/docs/metrics.md` & `ragas-0.0.6/docs/metrics.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 # Metrics
 
 1. `faithfulness` : measures the factual consistency of the generated answer against the given context. This is done using a multi step paradigm that includes creation of statements from the generated answer followed by verifying each of these statements against the context. The answer is scaled to (0,1) range. Higher the better.
 ```python
-from ragas.metrics import faithfulness
+from ragas.metrics.factuality import Faithfulness
+faithfulness = Faithfulness()
+
 # Dataset({
 #     features: ['question','contexts','answer'],
 #     num_rows: 25
 # })
 dataset: Dataset
 
-results = evaluate(dataset, metrics=[faithfulness])
+results = faithfulness.score(dataset)
 ```
-2. `answer_relevancy`: measures how relevant is the generated answer to the prompt. This is quantified using conditional likelihood of an LLM generating the question given the answer. This is implemented using a custom model. Values range (0,1), higher the better.
+
+2. `context_relevancy`: measures how relevant is the retrieved context to the prompt. This is done using a combination of OpenAI models and cross-encoder models. To improve the score one can try to optimize the amount of information present in the retrieved context. 
 ```python
-from ragas.metrics import answer_relevancy
+from ragas.metrics.context_relevancy import ContextRelevancy
+context_rel = ContextRelevancy(strictness=3)
 # Dataset({
-#     features: ['question','answer'],
+#     features: ['question','contexts'],
 #     num_rows: 25
 # })
 dataset: Dataset
 
-results = evaluate(dataset, metrics=[answer_relevancy])
+results = context_rel.score(dataset)
 ```
 
-3. `context_relevancy`: measures how relevant is the retrieved context to the prompt. This is quantified using a custom trained cross encoder model. Values range (0,1), higher the better.
+3. `answer_relevancy`: measures how relevant is the generated answer to the prompt. This is quantified using conditional likelihood of an LLM generating the question given the answer. This is implemented using a custom model. Values range (0,1), higher the better.
 ```python
-from ragas.metrics import context_relevancy
+from ragas.metrics.answer_relevancy import AnswerRelevancy
+answer_relevancy = AnswerRelevancy(model_name="t5-small")
 # Dataset({
-#     features: ['question','contexts'],
+#     features: ['question','answer'],
 #     num_rows: 25
 # })
 dataset: Dataset
 
-results = evaluate(dataset, metrics=[context_relevancy])
+results = answer_relevancy.score(dataset)
 ```
+
+
 ## Why is ragas better than scoring using GPT 3.5 directly.
 LLM like GPT 3.5 struggle when it comes to scoring generated text directly. For instance, these models would always only generate integer scores and these scores vary when invoked differently. Advanced paradigms and techniques leveraging LLMs to minimize this bias is the solution ragas presents.
 <h1 align="center">
   <img style="vertical-align:middle" height="350"
   src="./assets/bar-graph.svg">
 </h1>
```

### Comparing `ragas-0.0.5/docs/quickstart.ipynb` & `ragas-0.0.6/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/experiments/README.md` & `ragas-0.0.6/experiments/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.6/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/experiments/baselines/fiqa/improving-baselines.ipynb` & `ragas-0.0.6/experiments/baselines/fiqa/improving-baselines.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/experiments/baselines/hotpotqa/explore-dataset.ipynb` & `ragas-0.0.6/experiments/baselines/hotpotqa/explore-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.6/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/pyproject.toml` & `ragas-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/references.md` & `ragas-0.0.6/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/src/ragas/_analytics.py` & `ragas-0.0.6/src/ragas/_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/src/ragas/evaluation.py` & `ragas-0.0.6/src/ragas/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     Run the evaluation on the dataset with different metrics
 
     Parameters
     ----------
     dataset : Dataset[question: list[str], contexts: list[list[str]], answer: list[str]]
         The dataset in the format of ragas which the metrics will use to score the RAG
         pipeline with
-
     metrics : list[Metric] , optional
         List of metrics to use for evaluation. If not provided then ragas will run the
         evaluation on the best set of metrics to give a complete view.
 
     Returns
     -------
     result : Result
@@ -82,14 +81,15 @@
 
     # run the evaluation on dataset with different metrics
     # initialize all the models in the metrics
     [m.init_model() for m in metrics]
 
     scores = []
     for metric in metrics:
+        print(f"evaluating with [{metric.name}]")
         scores.append(metric.score(dataset).select_columns(metric.name))
 
     # log the evaluation event
     metrics_names = [m.name for m in metrics]
     track(
         EvaluationEvent(
             event_type="evaluation",
```

### Comparing `ragas-0.0.5/src/ragas/metrics/answer_relevance.py` & `ragas-0.0.6/src/ragas/metrics/answer_relevance.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
         )
 
         if show_progress:
             dataloader = tqdm(dataloader)
 
         for _, data in enumerate(dataloader):
             inputs, labels = data
+            inputs = {k: v.to(self._target_device) for k, v in inputs.items()}
+            labels = labels.to(self._target_device)
             with torch.no_grad():
                 logits = self.model(**inputs, output_hidden_states=False).logits
                 loss = self.get_loss(logits, labels)
                 predictions.append(loss)
 
         return np.hstack(predictions)
```

### Comparing `ragas-0.0.5/src/ragas/metrics/base.py` & `ragas-0.0.6/src/ragas/metrics/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/src/ragas/metrics/factual.py` & `ragas-0.0.6/src/ragas/metrics/faithfulnes.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/src/ragas/metrics/llms.py` & `ragas-0.0.6/src/ragas/metrics/llms.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/src/ragas/utils.py` & `ragas-0.0.6/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.5/src/ragas.egg-info/PKG-INFO` & `ragas-0.0.6/src/ragas.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
-  <i>SOTA metrics for evaluating Retrieval Augmented Generation (RAG)</i>
+  <i>Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines</i>
 </p>
 
 <p align="center">
     <a href="https://github.com/explodinggradients/ragas/releases">
         <img alt="GitHub release" src="https://img.shields.io/github/release/explodinggradients/ragas.svg">
     </a>
     <a href="https://www.python.org/">
@@ -84,15 +84,16 @@
 # 'faithfulness': 0.892, 'answer_relevancy': 0.874}
 ```
 If you want a more in-depth explanation of core components, check out our [quick-start notebook](./docs/quickstart.ipynb)
 ## :luggage: Metrics
 
 Ragas measures your pipeline's performance against two dimensions
 1. **Faithfulness**: measures the information consistency of the generated answer against the given context. If any claims made in the answer that cannot be deduced from context is penalized. 
-2. **Relevancy**:  measures how relevant retrieved contexts and the generated answer are to the question. The presence of extra or redundant information is penalized. 
+2. **Context Relevancy**:  measures how relevant retrieved contexts is to the question. Ideally the context should only contain information necessary to answer the question. The presence of redundant information in the context is penalized.
+3. **Answer Relevancy**: measures how relevant generated answer is to the question. This do not ensure factuality of the generated answer rather penalizes the presence of redundant information in the generated answer.
 
 Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors. 
 
 To read more about our metrics, checkout [docs](/docs/metrics.md).
 ## 🫂 Community
 If you want to get more involved with Ragas, check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out about LLM, Retrieval, Production issues and more.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.5 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.6 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
-       SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
+ Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
 external data to augment the LLMâs context. There are existing tools and
 frameworks that help you build these pipelines but evaluating it and
@@ -23,40 +23,44 @@
 num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) #
 {'ragas_score': 0.860, 'context_relavency': 0.817, # 'faithfulness': 0.892,
 'answer_relevancy': 0.874} ``` If you want a more in-depth explanation of core
 components, check out our [quick-start notebook](./docs/quickstart.ipynb) ## :
 luggage: Metrics Ragas measures your pipeline's performance against two
 dimensions 1. **Faithfulness**: measures the information consistency of the
 generated answer against the given context. If any claims made in the answer
-that cannot be deduced from context is penalized. 2. **Relevancy**: measures
-how relevant retrieved contexts and the generated answer are to the question.
-The presence of extra or redundant information is penalized. Through repeated
-experiments, we have found that the quality of a RAG pipeline is highly
-dependent on these two dimensions. The final `ragas_score` is the harmonic mean
-of these two factors. To read more about our metrics, checkout [docs](/docs/
-metrics.md). ## ð« Community If you want to get more involved with Ragas,
-check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun
-community where we geek out about LLM, Retrieval, Production issues and more.
-## ð Open Analytics We track very basic usage metrics to guide us to figure
-out what our users want, what is working and what's not. As a young startup, we
-have to be brutally honest about this which is why we are tracking these
-metrics. But as an Open Startup we open-source all the data we collect. You can
-read more about this [here](https://github.com/explodinggradients/ragas/issues/
-49). **Ragas doesnot track any information that can be used to identify you or
-your company**. You can take a look at exactly what we track in the [code](./
-src/ragas/_analytics.py) To disable usage-tracking you set the
-`RAGAS_DO_NOT_TRACK` flag to true. ## :raising_hand_man: FAQ 1. Why harmonic
-mean? Harmonic mean penalizes extreme values. For example, if your generated
-answer is fully factually consistent with the context (faithfulness = 1) but is
-not relevant to the question (relevancy = 0), a simple average would give you a
-score of 0.5 but a harmonic mean will give you 0.0 2. How to use Ragas to
-improve your pipeline? *"Measurement is the first step that leads to control
-and eventually to improvement" - James Harrington* Here we assume that you
-already have your RAG pipeline ready. When it comes to RAG pipelines, there are
-mainly two parts - Retriever and generator. A change in any of this should also
-impact your pipelines's quality. 1. First, decide one parameter that you're
-interested in adjusting. for example the number of retrieved documents, K. 2.
-Collect a set of sample prompts (min 20) to form your test set. 3. Run your
-pipeline using the test set before and after the change. Each time record the
-prompts with context and generated output. 4. Run ragas evaluation for each of
-them to generate evaluation scores. 5. Compare the scores and you will know how
-much the change has affected your pipelines' performance.
+that cannot be deduced from context is penalized. 2. **Context Relevancy**:
+measures how relevant retrieved contexts is to the question. Ideally the
+context should only contain information necessary to answer the question. The
+presence of redundant information in the context is penalized. 3. **Answer
+Relevancy**: measures how relevant generated answer is to the question. This do
+not ensure factuality of the generated answer rather penalizes the presence of
+redundant information in the generated answer. Through repeated experiments, we
+have found that the quality of a RAG pipeline is highly dependent on these two
+dimensions. The final `ragas_score` is the harmonic mean of these two factors.
+To read more about our metrics, checkout [docs](/docs/metrics.md). ## ð«
+Community If you want to get more involved with Ragas, check out our [discord
+server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out
+about LLM, Retrieval, Production issues and more. ## ð Open Analytics We
+track very basic usage metrics to guide us to figure out what our users want,
+what is working and what's not. As a young startup, we have to be brutally
+honest about this which is why we are tracking these metrics. But as an Open
+Startup we open-source all the data we collect. You can read more about this
+[here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot
+track any information that can be used to identify you or your company**. You
+can take a look at exactly what we track in the [code](./src/ragas/
+_analytics.py) To disable usage-tracking you set the `RAGAS_DO_NOT_TRACK` flag
+to true. ## :raising_hand_man: FAQ 1. Why harmonic mean? Harmonic mean
+penalizes extreme values. For example, if your generated answer is fully
+factually consistent with the context (faithfulness = 1) but is not relevant to
+the question (relevancy = 0), a simple average would give you a score of 0.5
+but a harmonic mean will give you 0.0 2. How to use Ragas to improve your
+pipeline? *"Measurement is the first step that leads to control and eventually
+to improvement" - James Harrington* Here we assume that you already have your
+RAG pipeline ready. When it comes to RAG pipelines, there are mainly two parts
+- Retriever and generator. A change in any of this should also impact your
+pipelines's quality. 1. First, decide one parameter that you're interested in
+adjusting. for example the number of retrieved documents, K. 2. Collect a set
+of sample prompts (min 20) to form your test set. 3. Run your pipeline using
+the test set before and after the change. Each time record the prompts with
+context and generated output. 4. Run ragas evaluation for each of them to
+generate evaluation scores. 5. Compare the scores and you will know how much
+the change has affected your pipelines' performance.
```

### Comparing `ragas-0.0.5/src/ragas.egg-info/SOURCES.txt` & `ragas-0.0.6/src/ragas.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 src/ragas.egg-info/dependency_links.txt
 src/ragas.egg-info/requires.txt
 src/ragas.egg-info/top_level.txt
 src/ragas/metrics/__init__.py
 src/ragas/metrics/answer_relevance.py
 src/ragas/metrics/base.py
 src/ragas/metrics/context_relevance.py
-src/ragas/metrics/factual.py
+src/ragas/metrics/faithfulnes.py
 src/ragas/metrics/llms.py
 tests/benchmarks/benchmark_eval.py
 tests/benchmarks/utils.py
 tests/unit/test_metric.py
 tests/unit/test_simple.py
```

### Comparing `ragas-0.0.5/tests/benchmarks/utils.py` & `ragas-0.0.6/tests/benchmarks/utils.py`

 * *Files identical despite different names*

