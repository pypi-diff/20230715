# Comparing `tmp/py_grama-0.3.5.tar.gz` & `tmp/py_grama-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grama-0.3.5.tar", last modified: Sat Jul 15 15:45:56 2023, max compression
+gzip compressed data, was "py_grama-0.3.6.tar", last modified: Sat Jul 15 16:11:59 2023, max compression
```

## Comparing `py_grama-0.3.5.tar` & `py_grama-0.3.6.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.759787 py_grama-0.3.5/
--rw-r--r--   0 zach       (501) staff       (20)     1076 2019-08-18 16:39:35.000000 py_grama-0.3.5/LICENSE
--rw-r--r--   0 zach       (501) staff       (20)     5347 2023-07-15 15:45:56.759567 py_grama-0.3.5/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     4188 2021-03-26 22:43:20.000000 py_grama-0.3.5/README.md
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.731833 py_grama-0.3.5/grama/
--rw-r--r--   0 zach       (501) staff       (20)     1143 2022-04-03 13:32:37.000000 py_grama-0.3.5/grama/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)    19793 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/comp_building.py
--rw-r--r--   0 zach       (501) staff       (20)     1643 2022-01-08 17:46:40.000000 py_grama-0.3.5/grama/comp_metamodels.py
--rw-r--r--   0 zach       (501) staff       (20)    37950 2023-07-15 15:40:33.000000 py_grama-0.3.5/grama/core.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.739378 py_grama-0.3.5/grama/data/
--rw-r--r--   0 zach       (501) staff       (20)     1690 2023-04-24 17:11:41.000000 py_grama-0.3.5/grama/data/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     1719 2022-01-28 00:02:51.000000 py_grama-0.3.5/grama/data/datasets.py
--rw-r--r--   0 zach       (501) staff       (20)  2571905 2020-03-08 22:57:01.000000 py_grama-0.3.5/grama/data/diamonds.csv
--rw-r--r--   0 zach       (501) staff       (20)    52696 2022-01-28 00:02:51.000000 py_grama-0.3.5/grama/data/psaap.csv
--rw-r--r--   0 zach       (501) staff       (20)      307 2020-12-17 02:04:23.000000 py_grama-0.3.5/grama/data/ruff.csv
--rw-rw-rw-   0 zach       (501) staff       (20)     1345 2021-09-15 12:49:03.000000 py_grama-0.3.5/grama/data/shewhart1931-table3.csv
--rw-r--r--   0 zach       (501) staff       (20)      562 2019-12-16 22:02:29.000000 py_grama-0.3.5/grama/data/stang.csv
--rw-r--r--   0 zach       (501) staff       (20)     2845 2019-12-19 01:09:10.000000 py_grama-0.3.5/grama/data/stang_long.csv
--rw-r--r--   0 zach       (501) staff       (20)      539 2020-07-28 14:02:47.000000 py_grama-0.3.5/grama/data/trajectory_full.csv
--rw-r--r--   0 zach       (501) staff       (20)      271 2020-07-28 16:04:52.000000 py_grama-0.3.5/grama/data/trajectory_windowed.csv
--rw-r--r--   0 zach       (501) staff       (20)     4408 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dataframe.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.742892 py_grama-0.3.5/grama/dfply/
--rw-r--r--   0 zach       (501) staff       (20)      433 2022-04-10 03:10:37.000000 py_grama-0.3.5/grama/dfply/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)    11028 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/dfply/base.py
--rw-r--r--   0 zach       (501) staff       (20)     1088 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/count.py
--rw-r--r--   0 zach       (501) staff       (20)      414 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/dfply/group.py
--rw-r--r--   0 zach       (501) staff       (20)    11626 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/join.py
--rw-r--r--   0 zach       (501) staff       (20)     1523 2023-01-03 18:10:43.000000 py_grama-0.3.5/grama/dfply/mask_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)    16220 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/reshape.py
--rw-r--r--   0 zach       (501) staff       (20)     7693 2023-01-03 18:22:07.000000 py_grama-0.3.5/grama/dfply/select.py
--rw-r--r--   0 zach       (501) staff       (20)     6129 2022-03-01 22:38:38.000000 py_grama-0.3.5/grama/dfply/set_ops.py
--rw-r--r--   0 zach       (501) staff       (20)     4401 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/dfply/string_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)     6763 2022-03-16 12:14:46.000000 py_grama-0.3.5/grama/dfply/subset.py
--rw-r--r--   0 zach       (501) staff       (20)     3090 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/summarize.py
--rw-r--r--   0 zach       (501) staff       (20)    23971 2022-11-04 16:41:23.000000 py_grama-0.3.5/grama/dfply/summary_functions.py
--rw-r--r--   0 zach       (501) staff       (20)     2533 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/transform.py
--rw-r--r--   0 zach       (501) staff       (20)    10097 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/vector.py
--rw-r--r--   0 zach       (501) staff       (20)     6084 2022-01-08 17:46:40.000000 py_grama-0.3.5/grama/dfply/window_functions.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.743261 py_grama-0.3.5/grama/eval/
--rw-r--r--   0 zach       (501) staff       (20)       26 2020-04-22 14:56:37.000000 py_grama-0.3.5/grama/eval/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     2425 2022-01-27 23:25:14.000000 py_grama-0.3.5/grama/eval/eval_pyDOE.py
--rw-r--r--   0 zach       (501) staff       (20)    12304 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/eval_contour.py
--rw-r--r--   0 zach       (501) staff       (20)    23653 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/eval_defaults.py
--rw-r--r--   0 zach       (501) staff       (20)    14508 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/eval_opt.py
--rw-r--r--   0 zach       (501) staff       (20)    12250 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/eval_pnd.py
--rw-r--r--   0 zach       (501) staff       (20)    10120 2023-03-17 12:30:25.000000 py_grama-0.3.5/grama/eval_random.py
--rw-r--r--   0 zach       (501) staff       (20)    18515 2022-11-04 16:20:43.000000 py_grama-0.3.5/grama/eval_tail.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.743963 py_grama-0.3.5/grama/fit/
--rw-r--r--   0 zach       (501) staff       (20)       86 2020-08-06 18:23:32.000000 py_grama-0.3.5/grama/fit/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     4783 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/fit/fit_lolo.py
--rw-r--r--   0 zach       (501) staff       (20)    15804 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/fit/fit_scikitlearn.py
--rw-r--r--   0 zach       (501) staff       (20)     2104 2022-01-27 23:25:14.000000 py_grama-0.3.5/grama/fit/fit_statsmodels.py
--rw-r--r--   0 zach       (501) staff       (20)     8453 2022-10-25 16:55:34.000000 py_grama-0.3.5/grama/fit_synonyms.py
--rw-r--r--   0 zach       (501) staff       (20)    23217 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/marginals.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.746267 py_grama-0.3.5/grama/models/
--rw-r--r--   0 zach       (501) staff       (20)      347 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/models/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     3195 2022-02-14 13:31:19.000000 py_grama-0.3.5/grama/models/cantilever_beam.py
--rw-r--r--   0 zach       (501) staff       (20)     8442 2022-01-28 00:02:51.000000 py_grama-0.3.5/grama/models/channel1d.py
--rw-r--r--   0 zach       (501) staff       (20)     2356 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/circuit_RLC.py
--rw-r--r--   0 zach       (501) staff       (20)     1564 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/ishigami.py
--rw-r--r--   0 zach       (501) staff       (20)      615 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/linear_normal.py
--rw-r--r--   0 zach       (501) staff       (20)     1635 2022-03-01 22:38:38.000000 py_grama-0.3.5/grama/models/pareto_random.py
--rw-r--r--   0 zach       (501) staff       (20)     2107 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/pipe_flow.py
--rw-r--r--   0 zach       (501) staff       (20)    14077 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/plane_laminate.py
--rw-r--r--   0 zach       (501) staff       (20)     1873 2022-02-03 20:27:56.000000 py_grama-0.3.5/grama/models/plate_buckling.py
--rw-r--r--   0 zach       (501) staff       (20)      645 2022-01-08 17:46:40.000000 py_grama-0.3.5/grama/models/poly.py
--rw-r--r--   0 zach       (501) staff       (20)     5505 2022-11-14 14:44:52.000000 py_grama-0.3.5/grama/models/sir.py
--rw-r--r--   0 zach       (501) staff       (20)      681 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/test.py
--rw-r--r--   0 zach       (501) staff       (20)     1035 2022-01-27 23:25:14.000000 py_grama-0.3.5/grama/models/trajectory_linear_drag.py
--rw-r--r--   0 zach       (501) staff       (20)    12175 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/mutate_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)    20525 2023-03-17 15:26:35.000000 py_grama-0.3.5/grama/plot_auto.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.749146 py_grama-0.3.5/grama/psdr/
--rw-r--r--   0 zach       (501) staff       (20)       26 2022-03-02 19:36:18.000000 py_grama-0.3.5/grama/psdr/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)    14559 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/psdr/basis.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.750197 py_grama-0.3.5/grama/psdr/domains/
--rw-r--r--   0 zach       (501) staff       (20)       41 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     2444 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/box.py
--rw-r--r--   0 zach       (501) staff       (20)     1555 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/domain.py
--rw-r--r--   0 zach       (501) staff       (20)    11274 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/psdr/domains/euclidean.py
--rw-r--r--   0 zach       (501) staff       (20)     4621 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/linineq.py
--rw-r--r--   0 zach       (501) staff       (20)    11623 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/linquad.py
--rw-r--r--   0 zach       (501) staff       (20)     5488 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/tensor.py
--rw-r--r--   0 zach       (501) staff       (20)      417 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/exceptions.py
--rw-r--r--   0 zach       (501) staff       (20)      715 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/function.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.750980 py_grama-0.3.5/grama/psdr/geometry/
--rw-r--r--   0 zach       (501) staff       (20)      111 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      369 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/cdist.py
--rw-r--r--   0 zach       (501) staff       (20)     2610 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/fill.py
--rw-r--r--   0 zach       (501) staff       (20)     1930 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/geometry.py
--rw-r--r--   0 zach       (501) staff       (20)      658 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/miniball.py
--rw-r--r--   0 zach       (501) staff       (20)    10529 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/vertex.py
--rw-r--r--   0 zach       (501) staff       (20)     7277 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/gn.py
--rw-r--r--   0 zach       (501) staff       (20)      841 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/initialization.py
--rw-r--r--   0 zach       (501) staff       (20)     6183 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/psdr/local_linear.py
--rw-r--r--   0 zach       (501) staff       (20)      724 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/misc.py
--rw-r--r--   0 zach       (501) staff       (20)     2732 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/pgf.py
--rw-r--r--   0 zach       (501) staff       (20)     3775 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/poly.py
--rw-r--r--   0 zach       (501) staff       (20)    17487 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/polyridge.py
--rw-r--r--   0 zach       (501) staff       (20)     8692 2022-03-02 19:36:18.000000 py_grama-0.3.5/grama/psdr/psdr_tools.py
--rw-r--r--   0 zach       (501) staff       (20)      921 2022-03-01 22:38:38.000000 py_grama-0.3.5/grama/psdr/quadrature.py
--rw-r--r--   0 zach       (501) staff       (20)     1801 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/ridge.py
--rw-r--r--   0 zach       (501) staff       (20)     9189 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/seqlp.py
--rw-r--r--   0 zach       (501) staff       (20)     7473 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/subspace.py
--rw-r--r--   0 zach       (501) staff       (20)     9809 2023-04-25 19:26:35.000000 py_grama-0.3.5/grama/spc.py
--rw-r--r--   0 zach       (501) staff       (20)     6995 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/string_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)     5876 2022-11-04 17:50:26.000000 py_grama-0.3.5/grama/support.py
--rw-r--r--   0 zach       (501) staff       (20)    13267 2022-04-20 12:57:11.000000 py_grama-0.3.5/grama/tools.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.751698 py_grama-0.3.5/grama/tran/
--rw-r--r--   0 zach       (501) staff       (20)       86 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/tran/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     2657 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran/tran_matminer.py
--rw-r--r--   0 zach       (501) staff       (20)     5356 2022-12-28 15:10:00.000000 py_grama-0.3.5/grama/tran/tran_scikitlearn.py
--rw-r--r--   0 zach       (501) staff       (20)     3434 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran/tran_umap.py
--rw-r--r--   0 zach       (501) staff       (20)     6346 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran_is.py
--rw-r--r--   0 zach       (501) staff       (20)    18443 2023-04-25 19:26:35.000000 py_grama-0.3.5/grama/tran_pivot.py
--rw-r--r--   0 zach       (501) staff       (20)     5836 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran_shapley.py
--rw-r--r--   0 zach       (501) staff       (20)    13351 2023-03-17 15:26:35.000000 py_grama-0.3.5/grama/tran_summaries.py
--rw-r--r--   0 zach       (501) staff       (20)    14018 2022-11-04 16:42:06.000000 py_grama-0.3.5/grama/tran_tools.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.752374 py_grama-0.3.5/py_grama.egg-info/
--rw-r--r--   0 zach       (501) staff       (20)     5347 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     3540 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (501) staff       (20)        1 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (501) staff       (20)      280 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/requires.txt
--rw-r--r--   0 zach       (501) staff       (20)        6 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/top_level.txt
--rw-r--r--   0 zach       (501) staff       (20)       38 2023-07-15 15:45:56.759848 py_grama-0.3.5/setup.cfg
--rw-r--r--   0 zach       (501) staff       (20)     1486 2023-07-15 15:41:48.000000 py_grama-0.3.5/setup.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.759095 py_grama-0.3.5/tests/
--rw-r--r--   0 zach       (501) staff       (20)     2454 2023-03-17 15:26:35.000000 py_grama-0.3.5/tests/test_autoplot.py
--rw-r--r--   0 zach       (501) staff       (20)     4927 2022-04-17 03:06:58.000000 py_grama-0.3.5/tests/test_contour.py
--rw-r--r--   0 zach       (501) staff       (20)    15210 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_core.py
--rw-r--r--   0 zach       (501) staff       (20)      463 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_data.py
--rw-r--r--   0 zach       (501) staff       (20)     1434 2022-04-03 13:32:37.000000 py_grama-0.3.5/tests/test_dataframe.py
--rw-r--r--   0 zach       (501) staff       (20)     1014 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_dfply_count.py
--rw-r--r--   0 zach       (501) staff       (20)      659 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_filter_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)      583 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_group.py
--rw-r--r--   0 zach       (501) staff       (20)     4133 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_join.py
--rw-r--r--   0 zach       (501) staff       (20)     3008 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_dfply_mutate_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)     9110 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_reshape.py
--rw-r--r--   0 zach       (501) staff       (20)    14801 2023-01-03 18:22:07.000000 py_grama-0.3.5/tests/test_dfply_select.py
--rw-r--r--   0 zach       (501) staff       (20)      870 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_subset.py
--rw-r--r--   0 zach       (501) staff       (20)     3339 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_summarize.py
--rw-r--r--   0 zach       (501) staff       (20)    20877 2022-04-19 22:57:07.000000 py_grama-0.3.5/tests/test_dfply_summary_functions.py
--rw-r--r--   0 zach       (501) staff       (20)     2697 2022-01-28 00:02:51.000000 py_grama-0.3.5/tests/test_dfply_transform.py
--rw-r--r--   0 zach       (501) staff       (20)     4619 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_vector.py
--rw-r--r--   0 zach       (501) staff       (20)    10725 2022-09-19 17:26:49.000000 py_grama-0.3.5/tests/test_eval_pnd.py
--rw-r--r--   0 zach       (501) staff       (20)    25250 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_evals.py
--rw-r--r--   0 zach       (501) staff       (20)     9763 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_fit.py
--rw-r--r--   0 zach       (501) staff       (20)     2398 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_is.py
--rw-r--r--   0 zach       (501) staff       (20)     4785 2022-02-03 20:27:56.000000 py_grama-0.3.5/tests/test_marginals.py
--rw-r--r--   0 zach       (501) staff       (20)     8871 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_mbi.py
--rw-r--r--   0 zach       (501) staff       (20)     2994 2022-06-16 13:35:20.000000 py_grama-0.3.5/tests/test_models.py
--rw-r--r--   0 zach       (501) staff       (20)      309 2021-03-26 22:43:20.000000 py_grama-0.3.5/tests/test_mp_restart.py
--rw-r--r--   0 zach       (501) staff       (20)     2603 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_pipes.py
--rw-r--r--   0 zach       (501) staff       (20)    21403 2022-04-14 13:54:09.000000 py_grama-0.3.5/tests/test_pivot.py
--rw-r--r--   0 zach       (501) staff       (20)     2643 2022-03-02 19:36:18.000000 py_grama-0.3.5/tests/test_psdr.py
--rw-r--r--   0 zach       (501) staff       (20)      633 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_shapley.py
--rw-r--r--   0 zach       (501) staff       (20)     2093 2023-04-25 19:26:35.000000 py_grama-0.3.5/tests/test_spc.py
--rw-r--r--   0 zach       (501) staff       (20)     4711 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_string_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)     1294 2022-12-01 14:56:07.000000 py_grama-0.3.5/tests/test_support.py
--rw-r--r--   0 zach       (501) staff       (20)     4340 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_tail.py
--rw-r--r--   0 zach       (501) staff       (20)      430 2022-04-03 13:32:37.000000 py_grama-0.3.5/tests/test_tools.py
--rw-r--r--   0 zach       (501) staff       (20)    12415 2022-12-28 15:10:00.000000 py_grama-0.3.5/tests/test_transforms.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.597320 py_grama-0.3.6/
+-rw-r--r--   0 zach       (501) staff       (20)     1076 2019-08-18 16:39:35.000000 py_grama-0.3.6/LICENSE
+-rw-r--r--   0 zach       (501) staff       (20)     5347 2023-07-15 16:11:59.597119 py_grama-0.3.6/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     4188 2021-03-26 22:43:20.000000 py_grama-0.3.6/README.md
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.569344 py_grama-0.3.6/grama/
+-rw-r--r--   0 zach       (501) staff       (20)     1143 2022-04-03 13:32:37.000000 py_grama-0.3.6/grama/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)    19793 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/comp_building.py
+-rw-r--r--   0 zach       (501) staff       (20)     1643 2022-01-08 17:46:40.000000 py_grama-0.3.6/grama/comp_metamodels.py
+-rw-r--r--   0 zach       (501) staff       (20)    37950 2023-07-15 15:40:33.000000 py_grama-0.3.6/grama/core.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.575473 py_grama-0.3.6/grama/data/
+-rw-r--r--   0 zach       (501) staff       (20)     1690 2023-04-24 17:11:41.000000 py_grama-0.3.6/grama/data/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     1719 2022-01-28 00:02:51.000000 py_grama-0.3.6/grama/data/datasets.py
+-rw-r--r--   0 zach       (501) staff       (20)  2571905 2020-03-08 22:57:01.000000 py_grama-0.3.6/grama/data/diamonds.csv
+-rw-r--r--   0 zach       (501) staff       (20)    52696 2022-01-28 00:02:51.000000 py_grama-0.3.6/grama/data/psaap.csv
+-rw-r--r--   0 zach       (501) staff       (20)      307 2020-12-17 02:04:23.000000 py_grama-0.3.6/grama/data/ruff.csv
+-rw-rw-rw-   0 zach       (501) staff       (20)     1345 2021-09-15 12:49:03.000000 py_grama-0.3.6/grama/data/shewhart1931-table3.csv
+-rw-r--r--   0 zach       (501) staff       (20)      562 2019-12-16 22:02:29.000000 py_grama-0.3.6/grama/data/stang.csv
+-rw-r--r--   0 zach       (501) staff       (20)     2845 2019-12-19 01:09:10.000000 py_grama-0.3.6/grama/data/stang_long.csv
+-rw-r--r--   0 zach       (501) staff       (20)      539 2020-07-28 14:02:47.000000 py_grama-0.3.6/grama/data/trajectory_full.csv
+-rw-r--r--   0 zach       (501) staff       (20)      271 2020-07-28 16:04:52.000000 py_grama-0.3.6/grama/data/trajectory_windowed.csv
+-rw-r--r--   0 zach       (501) staff       (20)     4408 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/dataframe.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.579114 py_grama-0.3.6/grama/dfply/
+-rw-r--r--   0 zach       (501) staff       (20)      433 2022-04-10 03:10:37.000000 py_grama-0.3.6/grama/dfply/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)    11028 2021-07-07 12:13:10.000000 py_grama-0.3.6/grama/dfply/base.py
+-rw-r--r--   0 zach       (501) staff       (20)     1088 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/dfply/count.py
+-rw-r--r--   0 zach       (501) staff       (20)      414 2021-07-07 12:13:10.000000 py_grama-0.3.6/grama/dfply/group.py
+-rw-r--r--   0 zach       (501) staff       (20)    11626 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/dfply/join.py
+-rw-r--r--   0 zach       (501) staff       (20)     1523 2023-01-03 18:10:43.000000 py_grama-0.3.6/grama/dfply/mask_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)    16220 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/dfply/reshape.py
+-rw-r--r--   0 zach       (501) staff       (20)     7693 2023-01-03 18:22:07.000000 py_grama-0.3.6/grama/dfply/select.py
+-rw-r--r--   0 zach       (501) staff       (20)     6129 2022-03-01 22:38:38.000000 py_grama-0.3.6/grama/dfply/set_ops.py
+-rw-r--r--   0 zach       (501) staff       (20)     4401 2022-03-10 14:13:00.000000 py_grama-0.3.6/grama/dfply/string_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     6763 2022-03-16 12:14:46.000000 py_grama-0.3.6/grama/dfply/subset.py
+-rw-r--r--   0 zach       (501) staff       (20)     3090 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/dfply/summarize.py
+-rw-r--r--   0 zach       (501) staff       (20)    23971 2022-11-04 16:41:23.000000 py_grama-0.3.6/grama/dfply/summary_functions.py
+-rw-r--r--   0 zach       (501) staff       (20)     2533 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/dfply/transform.py
+-rw-r--r--   0 zach       (501) staff       (20)    10097 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/dfply/vector.py
+-rw-r--r--   0 zach       (501) staff       (20)     6084 2022-01-08 17:46:40.000000 py_grama-0.3.6/grama/dfply/window_functions.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.579536 py_grama-0.3.6/grama/eval/
+-rw-r--r--   0 zach       (501) staff       (20)       26 2020-04-22 14:56:37.000000 py_grama-0.3.6/grama/eval/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     2425 2022-01-27 23:25:14.000000 py_grama-0.3.6/grama/eval/eval_pyDOE.py
+-rw-r--r--   0 zach       (501) staff       (20)    12304 2022-09-19 17:26:49.000000 py_grama-0.3.6/grama/eval_contour.py
+-rw-r--r--   0 zach       (501) staff       (20)    23653 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/eval_defaults.py
+-rw-r--r--   0 zach       (501) staff       (20)    14508 2022-09-19 17:26:49.000000 py_grama-0.3.6/grama/eval_opt.py
+-rw-r--r--   0 zach       (501) staff       (20)    12250 2022-09-19 17:26:49.000000 py_grama-0.3.6/grama/eval_pnd.py
+-rw-r--r--   0 zach       (501) staff       (20)    10120 2023-03-17 12:30:25.000000 py_grama-0.3.6/grama/eval_random.py
+-rw-r--r--   0 zach       (501) staff       (20)    18515 2022-11-04 16:20:43.000000 py_grama-0.3.6/grama/eval_tail.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.580316 py_grama-0.3.6/grama/fit/
+-rw-r--r--   0 zach       (501) staff       (20)       86 2020-08-06 18:23:32.000000 py_grama-0.3.6/grama/fit/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     4783 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/fit/fit_lolo.py
+-rw-r--r--   0 zach       (501) staff       (20)    15804 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/fit/fit_scikitlearn.py
+-rw-r--r--   0 zach       (501) staff       (20)     2104 2022-01-27 23:25:14.000000 py_grama-0.3.6/grama/fit/fit_statsmodels.py
+-rw-r--r--   0 zach       (501) staff       (20)     8453 2022-10-25 16:55:34.000000 py_grama-0.3.6/grama/fit_synonyms.py
+-rw-r--r--   0 zach       (501) staff       (20)    23213 2023-07-15 16:11:44.000000 py_grama-0.3.6/grama/marginals.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.582898 py_grama-0.3.6/grama/models/
+-rw-r--r--   0 zach       (501) staff       (20)      347 2022-09-19 17:26:49.000000 py_grama-0.3.6/grama/models/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     3195 2022-02-14 13:31:19.000000 py_grama-0.3.6/grama/models/cantilever_beam.py
+-rw-r--r--   0 zach       (501) staff       (20)     8442 2022-01-28 00:02:51.000000 py_grama-0.3.6/grama/models/channel1d.py
+-rw-r--r--   0 zach       (501) staff       (20)     2356 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/models/circuit_RLC.py
+-rw-r--r--   0 zach       (501) staff       (20)     1564 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/models/ishigami.py
+-rw-r--r--   0 zach       (501) staff       (20)      615 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/models/linear_normal.py
+-rw-r--r--   0 zach       (501) staff       (20)     1635 2022-03-01 22:38:38.000000 py_grama-0.3.6/grama/models/pareto_random.py
+-rw-r--r--   0 zach       (501) staff       (20)     2107 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/models/pipe_flow.py
+-rw-r--r--   0 zach       (501) staff       (20)    14077 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/models/plane_laminate.py
+-rw-r--r--   0 zach       (501) staff       (20)     1873 2022-02-03 20:27:56.000000 py_grama-0.3.6/grama/models/plate_buckling.py
+-rw-r--r--   0 zach       (501) staff       (20)      645 2022-01-08 17:46:40.000000 py_grama-0.3.6/grama/models/poly.py
+-rw-r--r--   0 zach       (501) staff       (20)     5505 2022-11-14 14:44:52.000000 py_grama-0.3.6/grama/models/sir.py
+-rw-r--r--   0 zach       (501) staff       (20)      681 2023-06-20 16:22:27.000000 py_grama-0.3.6/grama/models/test.py
+-rw-r--r--   0 zach       (501) staff       (20)     1035 2022-01-27 23:25:14.000000 py_grama-0.3.6/grama/models/trajectory_linear_drag.py
+-rw-r--r--   0 zach       (501) staff       (20)    12175 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/mutate_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)    20525 2023-03-17 15:26:35.000000 py_grama-0.3.6/grama/plot_auto.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.585918 py_grama-0.3.6/grama/psdr/
+-rw-r--r--   0 zach       (501) staff       (20)       26 2022-03-02 19:36:18.000000 py_grama-0.3.6/grama/psdr/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)    14559 2022-03-10 14:13:00.000000 py_grama-0.3.6/grama/psdr/basis.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.587088 py_grama-0.3.6/grama/psdr/domains/
+-rw-r--r--   0 zach       (501) staff       (20)       41 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/domains/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     2444 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/domains/box.py
+-rw-r--r--   0 zach       (501) staff       (20)     1555 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/domains/domain.py
+-rw-r--r--   0 zach       (501) staff       (20)    11274 2022-03-10 14:13:00.000000 py_grama-0.3.6/grama/psdr/domains/euclidean.py
+-rw-r--r--   0 zach       (501) staff       (20)     4621 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/domains/linineq.py
+-rw-r--r--   0 zach       (501) staff       (20)    11623 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/domains/linquad.py
+-rw-r--r--   0 zach       (501) staff       (20)     5488 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/domains/tensor.py
+-rw-r--r--   0 zach       (501) staff       (20)      417 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/exceptions.py
+-rw-r--r--   0 zach       (501) staff       (20)      715 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/function.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.587896 py_grama-0.3.6/grama/psdr/geometry/
+-rw-r--r--   0 zach       (501) staff       (20)      111 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/geometry/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      369 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/geometry/cdist.py
+-rw-r--r--   0 zach       (501) staff       (20)     2610 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/geometry/fill.py
+-rw-r--r--   0 zach       (501) staff       (20)     1930 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/geometry/geometry.py
+-rw-r--r--   0 zach       (501) staff       (20)      658 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/geometry/miniball.py
+-rw-r--r--   0 zach       (501) staff       (20)    10529 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/geometry/vertex.py
+-rw-r--r--   0 zach       (501) staff       (20)     7277 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/gn.py
+-rw-r--r--   0 zach       (501) staff       (20)      841 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/initialization.py
+-rw-r--r--   0 zach       (501) staff       (20)     6183 2022-03-10 14:13:00.000000 py_grama-0.3.6/grama/psdr/local_linear.py
+-rw-r--r--   0 zach       (501) staff       (20)      724 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/misc.py
+-rw-r--r--   0 zach       (501) staff       (20)     2732 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/pgf.py
+-rw-r--r--   0 zach       (501) staff       (20)     3775 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/poly.py
+-rw-r--r--   0 zach       (501) staff       (20)    17487 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/polyridge.py
+-rw-r--r--   0 zach       (501) staff       (20)     8692 2022-03-02 19:36:18.000000 py_grama-0.3.6/grama/psdr/psdr_tools.py
+-rw-r--r--   0 zach       (501) staff       (20)      921 2022-03-01 22:38:38.000000 py_grama-0.3.6/grama/psdr/quadrature.py
+-rw-r--r--   0 zach       (501) staff       (20)     1801 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/ridge.py
+-rw-r--r--   0 zach       (501) staff       (20)     9189 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/seqlp.py
+-rw-r--r--   0 zach       (501) staff       (20)     7473 2022-02-23 18:18:30.000000 py_grama-0.3.6/grama/psdr/subspace.py
+-rw-r--r--   0 zach       (501) staff       (20)     9809 2023-04-25 19:26:35.000000 py_grama-0.3.6/grama/spc.py
+-rw-r--r--   0 zach       (501) staff       (20)     6995 2021-07-07 12:13:10.000000 py_grama-0.3.6/grama/string_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     5876 2022-11-04 17:50:26.000000 py_grama-0.3.6/grama/support.py
+-rw-r--r--   0 zach       (501) staff       (20)    13263 2023-07-15 16:11:44.000000 py_grama-0.3.6/grama/tools.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.588813 py_grama-0.3.6/grama/tran/
+-rw-r--r--   0 zach       (501) staff       (20)       86 2021-07-07 12:13:10.000000 py_grama-0.3.6/grama/tran/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     2657 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/tran/tran_matminer.py
+-rw-r--r--   0 zach       (501) staff       (20)     5356 2022-12-28 15:10:00.000000 py_grama-0.3.6/grama/tran/tran_scikitlearn.py
+-rw-r--r--   0 zach       (501) staff       (20)     3434 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/tran/tran_umap.py
+-rw-r--r--   0 zach       (501) staff       (20)     6346 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/tran_is.py
+-rw-r--r--   0 zach       (501) staff       (20)    18443 2023-04-25 19:26:35.000000 py_grama-0.3.6/grama/tran_pivot.py
+-rw-r--r--   0 zach       (501) staff       (20)     5836 2022-04-17 03:06:58.000000 py_grama-0.3.6/grama/tran_shapley.py
+-rw-r--r--   0 zach       (501) staff       (20)    13351 2023-03-17 15:26:35.000000 py_grama-0.3.6/grama/tran_summaries.py
+-rw-r--r--   0 zach       (501) staff       (20)    14018 2022-11-04 16:42:06.000000 py_grama-0.3.6/grama/tran_tools.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.589545 py_grama-0.3.6/py_grama.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     5347 2023-07-15 16:11:59.000000 py_grama-0.3.6/py_grama.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     3540 2023-07-15 16:11:59.000000 py_grama-0.3.6/py_grama.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-07-15 16:11:59.000000 py_grama-0.3.6/py_grama.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (501) staff       (20)      292 2023-07-15 16:11:59.000000 py_grama-0.3.6/py_grama.egg-info/requires.txt
+-rw-r--r--   0 zach       (501) staff       (20)        6 2023-07-15 16:11:59.000000 py_grama-0.3.6/py_grama.egg-info/top_level.txt
+-rw-r--r--   0 zach       (501) staff       (20)       38 2023-07-15 16:11:59.597378 py_grama-0.3.6/setup.cfg
+-rw-r--r--   0 zach       (501) staff       (20)     1509 2023-07-15 16:11:44.000000 py_grama-0.3.6/setup.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 16:11:59.596682 py_grama-0.3.6/tests/
+-rw-r--r--   0 zach       (501) staff       (20)     2454 2023-03-17 15:26:35.000000 py_grama-0.3.6/tests/test_autoplot.py
+-rw-r--r--   0 zach       (501) staff       (20)     4927 2022-04-17 03:06:58.000000 py_grama-0.3.6/tests/test_contour.py
+-rw-r--r--   0 zach       (501) staff       (20)    15210 2023-06-20 16:22:27.000000 py_grama-0.3.6/tests/test_core.py
+-rw-r--r--   0 zach       (501) staff       (20)      463 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_data.py
+-rw-r--r--   0 zach       (501) staff       (20)     1434 2022-04-03 13:32:37.000000 py_grama-0.3.6/tests/test_dataframe.py
+-rw-r--r--   0 zach       (501) staff       (20)     1014 2022-01-27 23:25:14.000000 py_grama-0.3.6/tests/test_dfply_count.py
+-rw-r--r--   0 zach       (501) staff       (20)      659 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_dfply_filter_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)      583 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_dfply_group.py
+-rw-r--r--   0 zach       (501) staff       (20)     4133 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_dfply_join.py
+-rw-r--r--   0 zach       (501) staff       (20)     3008 2022-01-27 23:25:14.000000 py_grama-0.3.6/tests/test_dfply_mutate_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     9110 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_dfply_reshape.py
+-rw-r--r--   0 zach       (501) staff       (20)    14801 2023-01-03 18:22:07.000000 py_grama-0.3.6/tests/test_dfply_select.py
+-rw-r--r--   0 zach       (501) staff       (20)      870 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_dfply_subset.py
+-rw-r--r--   0 zach       (501) staff       (20)     3339 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_dfply_summarize.py
+-rw-r--r--   0 zach       (501) staff       (20)    20877 2022-04-19 22:57:07.000000 py_grama-0.3.6/tests/test_dfply_summary_functions.py
+-rw-r--r--   0 zach       (501) staff       (20)     2697 2022-01-28 00:02:51.000000 py_grama-0.3.6/tests/test_dfply_transform.py
+-rw-r--r--   0 zach       (501) staff       (20)     4619 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_dfply_vector.py
+-rw-r--r--   0 zach       (501) staff       (20)    10725 2022-09-19 17:26:49.000000 py_grama-0.3.6/tests/test_eval_pnd.py
+-rw-r--r--   0 zach       (501) staff       (20)    25250 2023-06-20 16:22:27.000000 py_grama-0.3.6/tests/test_evals.py
+-rw-r--r--   0 zach       (501) staff       (20)     9763 2023-06-20 16:22:27.000000 py_grama-0.3.6/tests/test_fit.py
+-rw-r--r--   0 zach       (501) staff       (20)     2398 2022-01-27 23:25:14.000000 py_grama-0.3.6/tests/test_is.py
+-rw-r--r--   0 zach       (501) staff       (20)     4785 2022-02-03 20:27:56.000000 py_grama-0.3.6/tests/test_marginals.py
+-rw-r--r--   0 zach       (501) staff       (20)     8871 2023-06-20 16:22:27.000000 py_grama-0.3.6/tests/test_mbi.py
+-rw-r--r--   0 zach       (501) staff       (20)     2994 2022-06-16 13:35:20.000000 py_grama-0.3.6/tests/test_models.py
+-rw-r--r--   0 zach       (501) staff       (20)      309 2021-03-26 22:43:20.000000 py_grama-0.3.6/tests/test_mp_restart.py
+-rw-r--r--   0 zach       (501) staff       (20)     2603 2022-01-27 23:25:14.000000 py_grama-0.3.6/tests/test_pipes.py
+-rw-r--r--   0 zach       (501) staff       (20)    21403 2022-04-14 13:54:09.000000 py_grama-0.3.6/tests/test_pivot.py
+-rw-r--r--   0 zach       (501) staff       (20)     2643 2022-03-02 19:36:18.000000 py_grama-0.3.6/tests/test_psdr.py
+-rw-r--r--   0 zach       (501) staff       (20)      633 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_shapley.py
+-rw-r--r--   0 zach       (501) staff       (20)     2093 2023-04-25 19:26:35.000000 py_grama-0.3.6/tests/test_spc.py
+-rw-r--r--   0 zach       (501) staff       (20)     4711 2021-11-12 12:20:36.000000 py_grama-0.3.6/tests/test_string_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     1294 2022-12-01 14:56:07.000000 py_grama-0.3.6/tests/test_support.py
+-rw-r--r--   0 zach       (501) staff       (20)     4340 2023-06-20 16:22:27.000000 py_grama-0.3.6/tests/test_tail.py
+-rw-r--r--   0 zach       (501) staff       (20)      430 2022-04-03 13:32:37.000000 py_grama-0.3.6/tests/test_tools.py
+-rw-r--r--   0 zach       (501) staff       (20)    12415 2022-12-28 15:10:00.000000 py_grama-0.3.6/tests/test_transforms.py
```

### Comparing `py_grama-0.3.5/LICENSE` & `py_grama-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/PKG-INFO` & `py_grama-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_grama
-Version: 0.3.5
+Version: 0.3.6
 Summary: A grammar of model analysis
 Home-page: https://github.com/zdelrosario/py_grama
 Author: Zachary del Rosario
 Author-email: zdelrosario@outlook.com
 License: MIT
 Description: # py_grama
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.02462/status.svg)](https://doi.org/10.21105/joss.02462) [![PyPI version](https://badge.fury.io/py/py-grama.svg)](https://badge.fury.io/py/py-grama) [![Documentation Status](https://readthedocs.org/projects/py_grama/badge/?version=latest)](https://py_grama.readthedocs.io/en/latest/?badge=latest) ![Python package test](https://github.com/zdelrosario/py_grama/workflows/Python%20package%20test/badge.svg) [![codecov](https://codecov.io/gh/zdelrosario/py_grama/branch/master/graph/badge.svg)](https://codecov.io/gh/zdelrosario/py_grama) [![CodeFactor](https://www.codefactor.io/repository/github/zdelrosario/py_grama/badge/master)](https://www.codefactor.io/repository/github/zdelrosario/py_grama/overview/master)
```

### Comparing `py_grama-0.3.5/README.md` & `py_grama-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/__init__.py` & `py_grama-0.3.6/grama/__init__.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/comp_building.py` & `py_grama-0.3.6/grama/comp_building.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/comp_metamodels.py` & `py_grama-0.3.6/grama/comp_metamodels.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/core.py` & `py_grama-0.3.6/grama/core.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/__init__.py` & `py_grama-0.3.6/grama/data/__init__.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/datasets.py` & `py_grama-0.3.6/grama/data/datasets.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/diamonds.csv` & `py_grama-0.3.6/grama/data/diamonds.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/psaap.csv` & `py_grama-0.3.6/grama/data/psaap.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/shewhart1931-table3.csv` & `py_grama-0.3.6/grama/data/shewhart1931-table3.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/stang.csv` & `py_grama-0.3.6/grama/data/stang.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/stang_long.csv` & `py_grama-0.3.6/grama/data/stang_long.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/data/trajectory_full.csv` & `py_grama-0.3.6/grama/data/trajectory_full.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dataframe.py` & `py_grama-0.3.6/grama/dataframe.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/base.py` & `py_grama-0.3.6/grama/dfply/base.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/count.py` & `py_grama-0.3.6/grama/dfply/count.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/join.py` & `py_grama-0.3.6/grama/dfply/join.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/mask_helpers.py` & `py_grama-0.3.6/grama/dfply/mask_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/reshape.py` & `py_grama-0.3.6/grama/dfply/reshape.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/select.py` & `py_grama-0.3.6/grama/dfply/select.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/set_ops.py` & `py_grama-0.3.6/grama/dfply/set_ops.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/string_helpers.py` & `py_grama-0.3.6/grama/dfply/string_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/subset.py` & `py_grama-0.3.6/grama/dfply/subset.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/summarize.py` & `py_grama-0.3.6/grama/dfply/summarize.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/summary_functions.py` & `py_grama-0.3.6/grama/dfply/summary_functions.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/transform.py` & `py_grama-0.3.6/grama/dfply/transform.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/vector.py` & `py_grama-0.3.6/grama/dfply/vector.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/dfply/window_functions.py` & `py_grama-0.3.6/grama/dfply/window_functions.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/eval/eval_pyDOE.py` & `py_grama-0.3.6/grama/eval/eval_pyDOE.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/eval_contour.py` & `py_grama-0.3.6/grama/eval_contour.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/eval_defaults.py` & `py_grama-0.3.6/grama/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/eval_opt.py` & `py_grama-0.3.6/grama/eval_opt.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/eval_pnd.py` & `py_grama-0.3.6/grama/eval_pnd.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/eval_random.py` & `py_grama-0.3.6/grama/eval_random.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/eval_tail.py` & `py_grama-0.3.6/grama/eval_tail.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/fit/fit_lolo.py` & `py_grama-0.3.6/grama/fit/fit_lolo.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/fit/fit_scikitlearn.py` & `py_grama-0.3.6/grama/fit/fit_scikitlearn.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/fit/fit_statsmodels.py` & `py_grama-0.3.6/grama/fit/fit_statsmodels.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/fit_synonyms.py` & `py_grama-0.3.6/grama/fit_synonyms.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/marginals.py` & `py_grama-0.3.6/grama/marginals.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pandas import DataFrame
 from scipy.optimize import root_scalar, root
 from scipy.stats import alpha, anglit, arcsine, argus, beta, betaprime, \
     bradford, burr, burr12, cauchy, chi, chi2, cosine, crystalball, dgamma, \
     dweibull, erlang, expon, exponnorm, exponweib, exponpow, f, fatiguelife, \
     fisk, foldcauchy, foldnorm, gaussian_kde, genlogistic, gennorm, genpareto, \
     genexpon, genextreme, gausshyper, gamma, gengamma, genhalflogistic, \
-    gilbrat, gompertz, gumbel_r, gumbel_l, halfcauchy, halflogistic, \
+    gibrat, gompertz, gumbel_r, gumbel_l, halfcauchy, halflogistic, \
     halfnorm, halfgennorm, hypsecant, invgamma, invgauss, invweibull, \
     johnsonsb, johnsonsu, kappa4, kappa3, ksone, kstwobign, laplace, levy, \
     levy_l, levy_stable, logistic, loggamma, loglaplace, lognorm, lomax, \
     maxwell, mielke, moyal, nakagami, ncx2, ncf, nct, norm, norminvgauss, \
     pareto, pearson3, powerlaw, powerlognorm, powernorm, rdist, rayleigh, \
     rice, recipinvgauss, skewnorm, t, trapz, triang, truncexpon, truncnorm, \
     tukeylambda, uniform, vonmises, vonmises_line, wald, weibull_min, \
@@ -71,15 +71,15 @@
     "genexpon": genexpon,
     "genextreme": genextreme,
     "gausshyper": gausshyper,
     "gamma": gamma,
     "gengamma": gengamma,
     "genhalflogistic": genhalflogistic,
     # "geninvgauss": geninvgauss,
-    "gilbrat": gilbrat,
+    "gibrat": gibrat,
     "gompertz": gompertz,
     "gumbel_r": gumbel_r,
     "gumbel_l": gumbel_l,
     "halfcauchy": halfcauchy,
     "halflogistic": halflogistic,
     "halfnorm": halfnorm,
     "halfgennorm": halfgennorm,
@@ -172,15 +172,15 @@
     "genexpon": ["a", "b", "c", "loc", "scale"],
     "genextreme": ["c", "loc", "scale"],
     "gausshyper": ["a", "b", "c", "z", "loc", "scale"],
     "gamma": ["a", "loc", "scale"],
     "gengamma": ["a", "c", "loc", "scale"],
     "genhalflogistic": ["c", "loc", "scale"],
     "geninvgauss": ["p", "b", "loc", "scale"],
-    "gilbrat": ["loc", "scale"],
+    "gibrat": ["loc", "scale"],
     "gompertz": ["c", "loc", "scale"],
     "gumbel_r": ["loc", "scale"],
     "gumbel_l": ["loc", "scale"],
     "halfcauchy": ["loc", "scale"],
     "halflogistic": ["loc", "scale"],
     "halfnorm": ["loc", "scale"],
     "halfgennorm": ["beta", "loc", "scale"],
```

### Comparing `py_grama-0.3.5/grama/models/cantilever_beam.py` & `py_grama-0.3.6/grama/models/cantilever_beam.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/channel1d.py` & `py_grama-0.3.6/grama/models/channel1d.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/circuit_RLC.py` & `py_grama-0.3.6/grama/models/circuit_RLC.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/ishigami.py` & `py_grama-0.3.6/grama/models/ishigami.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/linear_normal.py` & `py_grama-0.3.6/grama/models/linear_normal.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/pareto_random.py` & `py_grama-0.3.6/grama/models/pareto_random.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/pipe_flow.py` & `py_grama-0.3.6/grama/models/pipe_flow.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/plane_laminate.py` & `py_grama-0.3.6/grama/models/plane_laminate.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/plate_buckling.py` & `py_grama-0.3.6/grama/models/plate_buckling.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/poly.py` & `py_grama-0.3.6/grama/models/poly.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/sir.py` & `py_grama-0.3.6/grama/models/sir.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/test.py` & `py_grama-0.3.6/grama/models/test.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/models/trajectory_linear_drag.py` & `py_grama-0.3.6/grama/models/trajectory_linear_drag.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/mutate_helpers.py` & `py_grama-0.3.6/grama/mutate_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/plot_auto.py` & `py_grama-0.3.6/grama/plot_auto.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/basis.py` & `py_grama-0.3.6/grama/psdr/basis.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/domains/box.py` & `py_grama-0.3.6/grama/psdr/domains/box.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/domains/domain.py` & `py_grama-0.3.6/grama/psdr/domains/domain.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/domains/euclidean.py` & `py_grama-0.3.6/grama/psdr/domains/euclidean.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/domains/linineq.py` & `py_grama-0.3.6/grama/psdr/domains/linineq.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/domains/linquad.py` & `py_grama-0.3.6/grama/psdr/domains/linquad.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/domains/tensor.py` & `py_grama-0.3.6/grama/psdr/domains/tensor.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/function.py` & `py_grama-0.3.6/grama/psdr/function.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/geometry/fill.py` & `py_grama-0.3.6/grama/psdr/geometry/fill.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/geometry/geometry.py` & `py_grama-0.3.6/grama/psdr/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/geometry/miniball.py` & `py_grama-0.3.6/grama/psdr/geometry/miniball.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/geometry/vertex.py` & `py_grama-0.3.6/grama/psdr/geometry/vertex.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/gn.py` & `py_grama-0.3.6/grama/psdr/gn.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/initialization.py` & `py_grama-0.3.6/grama/psdr/initialization.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/local_linear.py` & `py_grama-0.3.6/grama/psdr/local_linear.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/misc.py` & `py_grama-0.3.6/grama/psdr/misc.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/pgf.py` & `py_grama-0.3.6/grama/psdr/pgf.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/poly.py` & `py_grama-0.3.6/grama/psdr/poly.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/polyridge.py` & `py_grama-0.3.6/grama/psdr/polyridge.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/psdr_tools.py` & `py_grama-0.3.6/grama/psdr/psdr_tools.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/quadrature.py` & `py_grama-0.3.6/grama/psdr/quadrature.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/ridge.py` & `py_grama-0.3.6/grama/psdr/ridge.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/seqlp.py` & `py_grama-0.3.6/grama/psdr/seqlp.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/psdr/subspace.py` & `py_grama-0.3.6/grama/psdr/subspace.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/spc.py` & `py_grama-0.3.6/grama/spc.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/string_helpers.py` & `py_grama-0.3.6/grama/string_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/support.py` & `py_grama-0.3.6/grama/support.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tools.py` & `py_grama-0.3.6/grama/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 from pandas.testing import assert_frame_equal
 from scipy.stats import alpha, anglit, arcsine, argus, beta, betaprime, \
     bradford, burr, burr12, cauchy, chi, chi2, cosine, crystalball, dgamma, \
     dweibull, erlang, expon, exponnorm, exponweib, exponpow, f, fatiguelife, \
     fisk, foldcauchy, foldnorm, gaussian_kde, genlogistic, gennorm, genpareto, \
     genexpon, genextreme, gausshyper, gamma, gengamma, genhalflogistic, \
-    gilbrat, gompertz, gumbel_r, gumbel_l, halfcauchy, halflogistic, \
+    gibrat, gompertz, gumbel_r, gumbel_l, halfcauchy, halflogistic, \
     halfnorm, halfgennorm, hypsecant, invgamma, invgauss, invweibull, \
     johnsonsb, johnsonsu, kappa4, kappa3, ksone, kstwobign, laplace, levy, \
     levy_l, levy_stable, logistic, loggamma, loglaplace, lognorm, lomax, \
     maxwell, mielke, moyal, nakagami, ncx2, ncf, nct, norm, norminvgauss, \
     pareto, pearson3, powerlaw, powerlognorm, powernorm, rdist, rayleigh, \
     rice, recipinvgauss, skewnorm, t, trapz, triang, truncexpon, truncnorm, \
     tukeylambda, uniform, vonmises, vonmises_line, wald, weibull_min, \
@@ -78,15 +78,15 @@
     "genexpon": genexpon,
     "genextreme": genextreme,
     "gausshyper": gausshyper,
     "gamma": gamma,
     "gengamma": gengamma,
     "genhalflogistic": genhalflogistic,
     # "geninvgauss": geninvgauss,
-    "gilbrat": gilbrat,
+    "gibrat": gibrat,
     "gompertz": gompertz,
     "gumbel_r": gumbel_r,
     "gumbel_l": gumbel_l,
     "halfcauchy": halfcauchy,
     "halflogistic": halflogistic,
     "halfnorm": halfnorm,
     "halfgennorm": halfgennorm,
@@ -179,15 +179,15 @@
     "genexpon": ["a", "b", "c", "loc", "scale"],
     "genextreme": ["c", "loc", "scale"],
     "gausshyper": ["a", "b", "c", "z", "loc", "scale"],
     "gamma": ["a", "loc", "scale"],
     "gengamma": ["a", "c", "loc", "scale"],
     "genhalflogistic": ["c", "loc", "scale"],
     "geninvgauss": ["p", "b", "loc", "scale"],
-    "gilbrat": ["loc", "scale"],
+    "gibrat": ["loc", "scale"],
     "gompertz": ["c", "loc", "scale"],
     "gumbel_r": ["loc", "scale"],
     "gumbel_l": ["loc", "scale"],
     "halfcauchy": ["loc", "scale"],
     "halflogistic": ["loc", "scale"],
     "halfnorm": ["loc", "scale"],
     "halfgennorm": ["beta", "loc", "scale"],
```

### Comparing `py_grama-0.3.5/grama/tran/tran_matminer.py` & `py_grama-0.3.6/grama/tran/tran_matminer.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tran/tran_scikitlearn.py` & `py_grama-0.3.6/grama/tran/tran_scikitlearn.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tran/tran_umap.py` & `py_grama-0.3.6/grama/tran/tran_umap.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tran_is.py` & `py_grama-0.3.6/grama/tran_is.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tran_pivot.py` & `py_grama-0.3.6/grama/tran_pivot.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tran_shapley.py` & `py_grama-0.3.6/grama/tran_shapley.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tran_summaries.py` & `py_grama-0.3.6/grama/tran_summaries.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/grama/tran_tools.py` & `py_grama-0.3.6/grama/tran_tools.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/py_grama.egg-info/PKG-INFO` & `py_grama-0.3.6/py_grama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grama
-Version: 0.3.5
+Version: 0.3.6
 Summary: A grammar of model analysis
 Home-page: https://github.com/zdelrosario/py_grama
 Author: Zachary del Rosario
 Author-email: zdelrosario@outlook.com
 License: MIT
 Description: # py_grama
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.02462/status.svg)](https://doi.org/10.21105/joss.02462) [![PyPI version](https://badge.fury.io/py/py-grama.svg)](https://badge.fury.io/py/py-grama) [![Documentation Status](https://readthedocs.org/projects/py_grama/badge/?version=latest)](https://py_grama.readthedocs.io/en/latest/?badge=latest) ![Python package test](https://github.com/zdelrosario/py_grama/workflows/Python%20package%20test/badge.svg) [![codecov](https://codecov.io/gh/zdelrosario/py_grama/branch/master/graph/badge.svg)](https://codecov.io/gh/zdelrosario/py_grama) [![CodeFactor](https://www.codefactor.io/repository/github/zdelrosario/py_grama/badge/master)](https://www.codefactor.io/repository/github/zdelrosario/py_grama/overview/master)
```

### Comparing `py_grama-0.3.5/py_grama.egg-info/SOURCES.txt` & `py_grama-0.3.6/py_grama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/setup.py` & `py_grama-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="py_grama",
     author="Zachary del Rosario",
     author_email="zdelrosario@outlook.com",
-    version="0.3.5",
+    version="0.3.6",
     packages=[
         "grama",
         "grama.data",
         "grama.dfply",
         "grama.eval",
         "grama.fit",
         "grama.models",
@@ -28,14 +28,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8, <3.10",
     install_requires=[
         "matplotlib",
         "numpy>=1.15",
+        "scipy>=1.10",
         "pandas<=1.5.3",
         "plotnine>=0.8.0",
         "scipy",
         "toolz",
         "networkx",
     ],
     extras_require={
```

### Comparing `py_grama-0.3.5/tests/test_autoplot.py` & `py_grama-0.3.6/tests/test_autoplot.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_contour.py` & `py_grama-0.3.6/tests/test_contour.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_core.py` & `py_grama-0.3.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dataframe.py` & `py_grama-0.3.6/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_count.py` & `py_grama-0.3.6/tests/test_dfply_count.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_filter_helpers.py` & `py_grama-0.3.6/tests/test_dfply_filter_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_group.py` & `py_grama-0.3.6/tests/test_dfply_group.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_join.py` & `py_grama-0.3.6/tests/test_dfply_join.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_mutate_helpers.py` & `py_grama-0.3.6/tests/test_dfply_mutate_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_reshape.py` & `py_grama-0.3.6/tests/test_dfply_reshape.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_select.py` & `py_grama-0.3.6/tests/test_dfply_select.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_subset.py` & `py_grama-0.3.6/tests/test_dfply_subset.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_summarize.py` & `py_grama-0.3.6/tests/test_dfply_summarize.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_summary_functions.py` & `py_grama-0.3.6/tests/test_dfply_summary_functions.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_transform.py` & `py_grama-0.3.6/tests/test_dfply_transform.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_dfply_vector.py` & `py_grama-0.3.6/tests/test_dfply_vector.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_eval_pnd.py` & `py_grama-0.3.6/tests/test_eval_pnd.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_evals.py` & `py_grama-0.3.6/tests/test_evals.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_fit.py` & `py_grama-0.3.6/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_is.py` & `py_grama-0.3.6/tests/test_is.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_marginals.py` & `py_grama-0.3.6/tests/test_marginals.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_mbi.py` & `py_grama-0.3.6/tests/test_mbi.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_models.py` & `py_grama-0.3.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_pipes.py` & `py_grama-0.3.6/tests/test_pipes.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_pivot.py` & `py_grama-0.3.6/tests/test_pivot.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_psdr.py` & `py_grama-0.3.6/tests/test_psdr.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_shapley.py` & `py_grama-0.3.6/tests/test_shapley.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_spc.py` & `py_grama-0.3.6/tests/test_spc.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_string_helpers.py` & `py_grama-0.3.6/tests/test_string_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_support.py` & `py_grama-0.3.6/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_tail.py` & `py_grama-0.3.6/tests/test_tail.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.5/tests/test_transforms.py` & `py_grama-0.3.6/tests/test_transforms.py`

 * *Files identical despite different names*

