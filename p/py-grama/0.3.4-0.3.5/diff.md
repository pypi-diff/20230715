# Comparing `tmp/py_grama-0.3.4.tar.gz` & `tmp/py_grama-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grama-0.3.4.tar", last modified: Thu Apr 14 14:10:23 2022, max compression
+gzip compressed data, was "py_grama-0.3.5.tar", last modified: Sat Jul 15 15:45:56 2023, max compression
```

## Comparing `py_grama-0.3.4.tar` & `py_grama-0.3.5.tar`

### file list

```diff
@@ -1,124 +1,161 @@
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.753760 py_grama-0.3.4/
--rw-r--r--   0 zach       (501) staff       (20)     1076 2019-08-18 16:39:35.000000 py_grama-0.3.4/LICENSE
--rw-r--r--   0 zach       (501) staff       (20)     5361 2022-04-14 14:10:23.753597 py_grama-0.3.4/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     4188 2021-03-26 22:43:20.000000 py_grama-0.3.4/README.md
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.734458 py_grama-0.3.4/grama/
--rw-r--r--   0 zach       (501) staff       (20)     1143 2022-04-03 13:32:37.000000 py_grama-0.3.4/grama/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)    14751 2022-02-03 14:52:46.000000 py_grama-0.3.4/grama/comp_building.py
--rw-r--r--   0 zach       (501) staff       (20)     1643 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/comp_metamodels.py
--rw-r--r--   0 zach       (501) staff       (20)    37919 2022-02-10 01:59:07.000000 py_grama-0.3.4/grama/core.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.740671 py_grama-0.3.4/grama/data/
--rw-r--r--   0 zach       (501) staff       (20)     1606 2021-09-15 12:50:05.000000 py_grama-0.3.4/grama/data/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     1719 2022-01-28 00:02:51.000000 py_grama-0.3.4/grama/data/datasets.py
--rw-r--r--   0 zach       (501) staff       (20)  2571905 2020-03-08 22:57:01.000000 py_grama-0.3.4/grama/data/diamonds.csv
--rw-r--r--   0 zach       (501) staff       (20)    52696 2022-01-28 00:02:51.000000 py_grama-0.3.4/grama/data/psaap.csv
--rw-r--r--   0 zach       (501) staff       (20)      307 2020-12-17 02:04:23.000000 py_grama-0.3.4/grama/data/ruff.csv
--rw-rw-rw-   0 zach       (501) staff       (20)     1345 2021-09-15 12:49:03.000000 py_grama-0.3.4/grama/data/shewhart1931-table3.csv
--rw-r--r--   0 zach       (501) staff       (20)      562 2019-12-16 22:02:29.000000 py_grama-0.3.4/grama/data/stang.csv
--rw-r--r--   0 zach       (501) staff       (20)     2845 2019-12-19 01:09:10.000000 py_grama-0.3.4/grama/data/stang_long.csv
--rw-r--r--   0 zach       (501) staff       (20)      539 2020-07-28 14:02:47.000000 py_grama-0.3.4/grama/data/trajectory_full.csv
--rw-r--r--   0 zach       (501) staff       (20)      271 2020-07-28 16:04:52.000000 py_grama-0.3.4/grama/data/trajectory_windowed.csv
--rw-r--r--   0 zach       (501) staff       (20)     4507 2022-04-03 13:32:37.000000 py_grama-0.3.4/grama/dataframe.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.743793 py_grama-0.3.4/grama/dfply/
--rw-r--r--   0 zach       (501) staff       (20)      433 2022-04-10 03:10:37.000000 py_grama-0.3.4/grama/dfply/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)    11028 2021-07-07 12:13:10.000000 py_grama-0.3.4/grama/dfply/base.py
--rw-r--r--   0 zach       (501) staff       (20)     1149 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/dfply/count.py
--rw-r--r--   0 zach       (501) staff       (20)      414 2021-07-07 12:13:10.000000 py_grama-0.3.4/grama/dfply/group.py
--rw-r--r--   0 zach       (501) staff       (20)    10836 2021-07-21 20:39:06.000000 py_grama-0.3.4/grama/dfply/join.py
--rw-r--r--   0 zach       (501) staff       (20)     1523 2022-03-10 14:13:00.000000 py_grama-0.3.4/grama/dfply/mask_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)    16209 2022-03-10 14:13:00.000000 py_grama-0.3.4/grama/dfply/reshape.py
--rw-r--r--   0 zach       (501) staff       (20)     7113 2022-04-14 13:54:09.000000 py_grama-0.3.4/grama/dfply/select.py
--rw-r--r--   0 zach       (501) staff       (20)     6129 2022-03-01 22:38:38.000000 py_grama-0.3.4/grama/dfply/set_ops.py
--rw-r--r--   0 zach       (501) staff       (20)     4401 2022-03-10 14:13:00.000000 py_grama-0.3.4/grama/dfply/string_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)     6763 2022-03-16 12:14:46.000000 py_grama-0.3.4/grama/dfply/subset.py
--rw-r--r--   0 zach       (501) staff       (20)     3088 2022-04-14 13:57:56.000000 py_grama-0.3.4/grama/dfply/summarize.py
--rw-r--r--   0 zach       (501) staff       (20)    18897 2022-04-02 02:40:17.000000 py_grama-0.3.4/grama/dfply/summary_functions.py
--rw-r--r--   0 zach       (501) staff       (20)     2527 2022-03-10 14:13:00.000000 py_grama-0.3.4/grama/dfply/transform.py
--rw-r--r--   0 zach       (501) staff       (20)    10144 2022-03-31 12:06:10.000000 py_grama-0.3.4/grama/dfply/vector.py
--rw-r--r--   0 zach       (501) staff       (20)     6084 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/dfply/window_functions.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.744063 py_grama-0.3.4/grama/eval/
--rw-r--r--   0 zach       (501) staff       (20)       26 2020-04-22 14:56:37.000000 py_grama-0.3.4/grama/eval/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     2425 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/eval/eval_pyDOE.py
--rw-r--r--   0 zach       (501) staff       (20)    12063 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/eval_contour.py
--rw-r--r--   0 zach       (501) staff       (20)    13403 2022-02-10 14:17:54.000000 py_grama-0.3.4/grama/eval_defaults.py
--rw-r--r--   0 zach       (501) staff       (20)    14185 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/eval_opt.py
--rw-r--r--   0 zach       (501) staff       (20)    12001 2022-03-01 22:38:38.000000 py_grama-0.3.4/grama/eval_pnd.py
--rw-r--r--   0 zach       (501) staff       (20)     9851 2022-02-09 14:54:15.000000 py_grama-0.3.4/grama/eval_random.py
--rw-r--r--   0 zach       (501) staff       (20)    13420 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/eval_tail.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.744621 py_grama-0.3.4/grama/fit/
--rw-r--r--   0 zach       (501) staff       (20)       86 2020-08-06 18:23:32.000000 py_grama-0.3.4/grama/fit/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     4726 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/fit/fit_lolo.py
--rw-r--r--   0 zach       (501) staff       (20)    15876 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/fit/fit_scikitlearn.py
--rw-r--r--   0 zach       (501) staff       (20)     2104 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/fit/fit_statsmodels.py
--rw-r--r--   0 zach       (501) staff       (20)     8452 2022-04-14 11:18:15.000000 py_grama-0.3.4/grama/fit_synonyms.py
--rw-r--r--   0 zach       (501) staff       (20)    23490 2022-02-03 20:27:56.000000 py_grama-0.3.4/grama/marginals.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.746603 py_grama-0.3.4/grama/models/
--rw-r--r--   0 zach       (501) staff       (20)      303 2022-03-01 22:38:38.000000 py_grama-0.3.4/grama/models/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     3195 2022-02-14 13:31:19.000000 py_grama-0.3.4/grama/models/cantilever_beam.py
--rw-r--r--   0 zach       (501) staff       (20)     8442 2022-01-28 00:02:51.000000 py_grama-0.3.4/grama/models/channel1d.py
--rw-r--r--   0 zach       (501) staff       (20)     2352 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/models/circuit_RLC.py
--rw-r--r--   0 zach       (501) staff       (20)     1574 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/models/ishigami.py
--rw-r--r--   0 zach       (501) staff       (20)      626 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/models/linear_normal.py
--rw-r--r--   0 zach       (501) staff       (20)     1635 2022-03-01 22:38:38.000000 py_grama-0.3.4/grama/models/pareto_random.py
--rw-r--r--   0 zach       (501) staff       (20)    14076 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/models/plane_laminate.py
--rw-r--r--   0 zach       (501) staff       (20)     1873 2022-02-03 20:27:56.000000 py_grama-0.3.4/grama/models/plate_buckling.py
--rw-r--r--   0 zach       (501) staff       (20)      645 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/models/poly.py
--rw-r--r--   0 zach       (501) staff       (20)      691 2022-01-08 17:46:40.000000 py_grama-0.3.4/grama/models/test.py
--rw-r--r--   0 zach       (501) staff       (20)     1095 2019-12-24 21:45:05.000000 py_grama-0.3.4/grama/models/time_cantilever.py
--rw-r--r--   0 zach       (501) staff       (20)     1035 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/models/trajectory_linear_drag.py
--rw-r--r--   0 zach       (501) staff       (20)    11760 2022-03-29 11:03:43.000000 py_grama-0.3.4/grama/mutate_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)    15070 2022-03-08 15:46:59.000000 py_grama-0.3.4/grama/plot_auto.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.749235 py_grama-0.3.4/grama/psdr/
--rw-r--r--   0 zach       (501) staff       (20)       26 2022-03-02 19:36:18.000000 py_grama-0.3.4/grama/psdr/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)    14559 2022-03-10 14:13:00.000000 py_grama-0.3.4/grama/psdr/basis.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.750972 py_grama-0.3.4/grama/psdr/domains/
--rw-r--r--   0 zach       (501) staff       (20)       41 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/domains/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     2444 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/domains/box.py
--rw-r--r--   0 zach       (501) staff       (20)     1555 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/domains/domain.py
--rw-r--r--   0 zach       (501) staff       (20)    11274 2022-03-10 14:13:00.000000 py_grama-0.3.4/grama/psdr/domains/euclidean.py
--rw-r--r--   0 zach       (501) staff       (20)     4621 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/domains/linineq.py
--rw-r--r--   0 zach       (501) staff       (20)    11623 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/domains/linquad.py
--rw-r--r--   0 zach       (501) staff       (20)     5488 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/domains/tensor.py
--rw-r--r--   0 zach       (501) staff       (20)      417 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/exceptions.py
--rw-r--r--   0 zach       (501) staff       (20)      715 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/function.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.751815 py_grama-0.3.4/grama/psdr/geometry/
--rw-r--r--   0 zach       (501) staff       (20)      111 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/geometry/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      369 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/geometry/cdist.py
--rw-r--r--   0 zach       (501) staff       (20)     2610 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/geometry/fill.py
--rw-r--r--   0 zach       (501) staff       (20)     1930 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/geometry/geometry.py
--rw-r--r--   0 zach       (501) staff       (20)      658 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/geometry/miniball.py
--rw-r--r--   0 zach       (501) staff       (20)    10529 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/geometry/vertex.py
--rw-r--r--   0 zach       (501) staff       (20)     7277 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/gn.py
--rw-r--r--   0 zach       (501) staff       (20)      841 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/initialization.py
--rw-r--r--   0 zach       (501) staff       (20)     6183 2022-03-10 14:13:00.000000 py_grama-0.3.4/grama/psdr/local_linear.py
--rw-r--r--   0 zach       (501) staff       (20)      724 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/misc.py
--rw-r--r--   0 zach       (501) staff       (20)     2732 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/pgf.py
--rw-r--r--   0 zach       (501) staff       (20)     3775 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/poly.py
--rw-r--r--   0 zach       (501) staff       (20)    17487 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/polyridge.py
--rw-r--r--   0 zach       (501) staff       (20)     8692 2022-03-02 19:36:18.000000 py_grama-0.3.4/grama/psdr/psdr_tools.py
--rw-r--r--   0 zach       (501) staff       (20)      921 2022-03-01 22:38:38.000000 py_grama-0.3.4/grama/psdr/quadrature.py
--rw-r--r--   0 zach       (501) staff       (20)     1801 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/ridge.py
--rw-r--r--   0 zach       (501) staff       (20)     9189 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/seqlp.py
--rw-r--r--   0 zach       (501) staff       (20)     7473 2022-02-23 18:18:30.000000 py_grama-0.3.4/grama/psdr/subspace.py
--rw-r--r--   0 zach       (501) staff       (20)     7865 2022-04-14 13:57:58.000000 py_grama-0.3.4/grama/spc.py
--rw-r--r--   0 zach       (501) staff       (20)     6995 2021-07-07 12:13:10.000000 py_grama-0.3.4/grama/string_helpers.py
--rw-r--r--   0 zach       (501) staff       (20)     5949 2022-02-09 15:00:00.000000 py_grama-0.3.4/grama/support.py
--rw-r--r--   0 zach       (501) staff       (20)    12730 2022-04-03 13:32:37.000000 py_grama-0.3.4/grama/tools.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.752667 py_grama-0.3.4/grama/tran/
--rw-r--r--   0 zach       (501) staff       (20)       86 2021-07-07 12:13:10.000000 py_grama-0.3.4/grama/tran/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)     2679 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/tran/tran_matminer.py
--rw-r--r--   0 zach       (501) staff       (20)     5226 2022-01-27 23:25:14.000000 py_grama-0.3.4/grama/tran/tran_scikitlearn.py
--rw-r--r--   0 zach       (501) staff       (20)     3146 2022-03-10 15:43:06.000000 py_grama-0.3.4/grama/tran/tran_umap.py
--rw-r--r--   0 zach       (501) staff       (20)     6617 2022-02-03 20:27:56.000000 py_grama-0.3.4/grama/tran_is.py
--rw-r--r--   0 zach       (501) staff       (20)    17803 2022-04-14 13:54:09.000000 py_grama-0.3.4/grama/tran_pivot.py
--rw-r--r--   0 zach       (501) staff       (20)     5969 2021-07-21 20:39:06.000000 py_grama-0.3.4/grama/tran_shapley.py
--rw-r--r--   0 zach       (501) staff       (20)    12901 2022-02-08 18:37:53.000000 py_grama-0.3.4/grama/tran_summaries.py
--rw-r--r--   0 zach       (501) staff       (20)    13519 2022-01-07 20:57:15.000000 py_grama-0.3.4/grama/tran_tools.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2022-04-14 14:10:23.753378 py_grama-0.3.4/py_grama.egg-info/
--rw-r--r--   0 zach       (501) staff       (20)     5361 2022-04-14 14:10:23.000000 py_grama-0.3.4/py_grama.egg-info/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     2685 2022-04-14 14:10:23.000000 py_grama-0.3.4/py_grama.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (501) staff       (20)        1 2022-04-14 14:10:23.000000 py_grama-0.3.4/py_grama.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (501) staff       (20)      295 2022-04-14 14:10:23.000000 py_grama-0.3.4/py_grama.egg-info/requires.txt
--rw-r--r--   0 zach       (501) staff       (20)        6 2022-04-14 14:10:23.000000 py_grama-0.3.4/py_grama.egg-info/top_level.txt
--rw-r--r--   0 zach       (501) staff       (20)       38 2022-04-14 14:10:23.753810 py_grama-0.3.4/setup.cfg
--rw-r--r--   0 zach       (501) staff       (20)     1522 2022-04-14 13:57:24.000000 py_grama-0.3.4/setup.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.759787 py_grama-0.3.5/
+-rw-r--r--   0 zach       (501) staff       (20)     1076 2019-08-18 16:39:35.000000 py_grama-0.3.5/LICENSE
+-rw-r--r--   0 zach       (501) staff       (20)     5347 2023-07-15 15:45:56.759567 py_grama-0.3.5/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     4188 2021-03-26 22:43:20.000000 py_grama-0.3.5/README.md
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.731833 py_grama-0.3.5/grama/
+-rw-r--r--   0 zach       (501) staff       (20)     1143 2022-04-03 13:32:37.000000 py_grama-0.3.5/grama/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)    19793 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/comp_building.py
+-rw-r--r--   0 zach       (501) staff       (20)     1643 2022-01-08 17:46:40.000000 py_grama-0.3.5/grama/comp_metamodels.py
+-rw-r--r--   0 zach       (501) staff       (20)    37950 2023-07-15 15:40:33.000000 py_grama-0.3.5/grama/core.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.739378 py_grama-0.3.5/grama/data/
+-rw-r--r--   0 zach       (501) staff       (20)     1690 2023-04-24 17:11:41.000000 py_grama-0.3.5/grama/data/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     1719 2022-01-28 00:02:51.000000 py_grama-0.3.5/grama/data/datasets.py
+-rw-r--r--   0 zach       (501) staff       (20)  2571905 2020-03-08 22:57:01.000000 py_grama-0.3.5/grama/data/diamonds.csv
+-rw-r--r--   0 zach       (501) staff       (20)    52696 2022-01-28 00:02:51.000000 py_grama-0.3.5/grama/data/psaap.csv
+-rw-r--r--   0 zach       (501) staff       (20)      307 2020-12-17 02:04:23.000000 py_grama-0.3.5/grama/data/ruff.csv
+-rw-rw-rw-   0 zach       (501) staff       (20)     1345 2021-09-15 12:49:03.000000 py_grama-0.3.5/grama/data/shewhart1931-table3.csv
+-rw-r--r--   0 zach       (501) staff       (20)      562 2019-12-16 22:02:29.000000 py_grama-0.3.5/grama/data/stang.csv
+-rw-r--r--   0 zach       (501) staff       (20)     2845 2019-12-19 01:09:10.000000 py_grama-0.3.5/grama/data/stang_long.csv
+-rw-r--r--   0 zach       (501) staff       (20)      539 2020-07-28 14:02:47.000000 py_grama-0.3.5/grama/data/trajectory_full.csv
+-rw-r--r--   0 zach       (501) staff       (20)      271 2020-07-28 16:04:52.000000 py_grama-0.3.5/grama/data/trajectory_windowed.csv
+-rw-r--r--   0 zach       (501) staff       (20)     4408 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dataframe.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.742892 py_grama-0.3.5/grama/dfply/
+-rw-r--r--   0 zach       (501) staff       (20)      433 2022-04-10 03:10:37.000000 py_grama-0.3.5/grama/dfply/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)    11028 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/dfply/base.py
+-rw-r--r--   0 zach       (501) staff       (20)     1088 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/count.py
+-rw-r--r--   0 zach       (501) staff       (20)      414 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/dfply/group.py
+-rw-r--r--   0 zach       (501) staff       (20)    11626 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/join.py
+-rw-r--r--   0 zach       (501) staff       (20)     1523 2023-01-03 18:10:43.000000 py_grama-0.3.5/grama/dfply/mask_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)    16220 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/reshape.py
+-rw-r--r--   0 zach       (501) staff       (20)     7693 2023-01-03 18:22:07.000000 py_grama-0.3.5/grama/dfply/select.py
+-rw-r--r--   0 zach       (501) staff       (20)     6129 2022-03-01 22:38:38.000000 py_grama-0.3.5/grama/dfply/set_ops.py
+-rw-r--r--   0 zach       (501) staff       (20)     4401 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/dfply/string_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     6763 2022-03-16 12:14:46.000000 py_grama-0.3.5/grama/dfply/subset.py
+-rw-r--r--   0 zach       (501) staff       (20)     3090 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/summarize.py
+-rw-r--r--   0 zach       (501) staff       (20)    23971 2022-11-04 16:41:23.000000 py_grama-0.3.5/grama/dfply/summary_functions.py
+-rw-r--r--   0 zach       (501) staff       (20)     2533 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/transform.py
+-rw-r--r--   0 zach       (501) staff       (20)    10097 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/dfply/vector.py
+-rw-r--r--   0 zach       (501) staff       (20)     6084 2022-01-08 17:46:40.000000 py_grama-0.3.5/grama/dfply/window_functions.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.743261 py_grama-0.3.5/grama/eval/
+-rw-r--r--   0 zach       (501) staff       (20)       26 2020-04-22 14:56:37.000000 py_grama-0.3.5/grama/eval/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     2425 2022-01-27 23:25:14.000000 py_grama-0.3.5/grama/eval/eval_pyDOE.py
+-rw-r--r--   0 zach       (501) staff       (20)    12304 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/eval_contour.py
+-rw-r--r--   0 zach       (501) staff       (20)    23653 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/eval_defaults.py
+-rw-r--r--   0 zach       (501) staff       (20)    14508 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/eval_opt.py
+-rw-r--r--   0 zach       (501) staff       (20)    12250 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/eval_pnd.py
+-rw-r--r--   0 zach       (501) staff       (20)    10120 2023-03-17 12:30:25.000000 py_grama-0.3.5/grama/eval_random.py
+-rw-r--r--   0 zach       (501) staff       (20)    18515 2022-11-04 16:20:43.000000 py_grama-0.3.5/grama/eval_tail.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.743963 py_grama-0.3.5/grama/fit/
+-rw-r--r--   0 zach       (501) staff       (20)       86 2020-08-06 18:23:32.000000 py_grama-0.3.5/grama/fit/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     4783 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/fit/fit_lolo.py
+-rw-r--r--   0 zach       (501) staff       (20)    15804 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/fit/fit_scikitlearn.py
+-rw-r--r--   0 zach       (501) staff       (20)     2104 2022-01-27 23:25:14.000000 py_grama-0.3.5/grama/fit/fit_statsmodels.py
+-rw-r--r--   0 zach       (501) staff       (20)     8453 2022-10-25 16:55:34.000000 py_grama-0.3.5/grama/fit_synonyms.py
+-rw-r--r--   0 zach       (501) staff       (20)    23217 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/marginals.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.746267 py_grama-0.3.5/grama/models/
+-rw-r--r--   0 zach       (501) staff       (20)      347 2022-09-19 17:26:49.000000 py_grama-0.3.5/grama/models/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     3195 2022-02-14 13:31:19.000000 py_grama-0.3.5/grama/models/cantilever_beam.py
+-rw-r--r--   0 zach       (501) staff       (20)     8442 2022-01-28 00:02:51.000000 py_grama-0.3.5/grama/models/channel1d.py
+-rw-r--r--   0 zach       (501) staff       (20)     2356 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/circuit_RLC.py
+-rw-r--r--   0 zach       (501) staff       (20)     1564 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/ishigami.py
+-rw-r--r--   0 zach       (501) staff       (20)      615 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/linear_normal.py
+-rw-r--r--   0 zach       (501) staff       (20)     1635 2022-03-01 22:38:38.000000 py_grama-0.3.5/grama/models/pareto_random.py
+-rw-r--r--   0 zach       (501) staff       (20)     2107 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/pipe_flow.py
+-rw-r--r--   0 zach       (501) staff       (20)    14077 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/plane_laminate.py
+-rw-r--r--   0 zach       (501) staff       (20)     1873 2022-02-03 20:27:56.000000 py_grama-0.3.5/grama/models/plate_buckling.py
+-rw-r--r--   0 zach       (501) staff       (20)      645 2022-01-08 17:46:40.000000 py_grama-0.3.5/grama/models/poly.py
+-rw-r--r--   0 zach       (501) staff       (20)     5505 2022-11-14 14:44:52.000000 py_grama-0.3.5/grama/models/sir.py
+-rw-r--r--   0 zach       (501) staff       (20)      681 2023-06-20 16:22:27.000000 py_grama-0.3.5/grama/models/test.py
+-rw-r--r--   0 zach       (501) staff       (20)     1035 2022-01-27 23:25:14.000000 py_grama-0.3.5/grama/models/trajectory_linear_drag.py
+-rw-r--r--   0 zach       (501) staff       (20)    12175 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/mutate_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)    20525 2023-03-17 15:26:35.000000 py_grama-0.3.5/grama/plot_auto.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.749146 py_grama-0.3.5/grama/psdr/
+-rw-r--r--   0 zach       (501) staff       (20)       26 2022-03-02 19:36:18.000000 py_grama-0.3.5/grama/psdr/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)    14559 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/psdr/basis.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.750197 py_grama-0.3.5/grama/psdr/domains/
+-rw-r--r--   0 zach       (501) staff       (20)       41 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     2444 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/box.py
+-rw-r--r--   0 zach       (501) staff       (20)     1555 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/domain.py
+-rw-r--r--   0 zach       (501) staff       (20)    11274 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/psdr/domains/euclidean.py
+-rw-r--r--   0 zach       (501) staff       (20)     4621 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/linineq.py
+-rw-r--r--   0 zach       (501) staff       (20)    11623 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/linquad.py
+-rw-r--r--   0 zach       (501) staff       (20)     5488 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/domains/tensor.py
+-rw-r--r--   0 zach       (501) staff       (20)      417 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/exceptions.py
+-rw-r--r--   0 zach       (501) staff       (20)      715 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/function.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.750980 py_grama-0.3.5/grama/psdr/geometry/
+-rw-r--r--   0 zach       (501) staff       (20)      111 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      369 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/cdist.py
+-rw-r--r--   0 zach       (501) staff       (20)     2610 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/fill.py
+-rw-r--r--   0 zach       (501) staff       (20)     1930 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/geometry.py
+-rw-r--r--   0 zach       (501) staff       (20)      658 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/miniball.py
+-rw-r--r--   0 zach       (501) staff       (20)    10529 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/geometry/vertex.py
+-rw-r--r--   0 zach       (501) staff       (20)     7277 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/gn.py
+-rw-r--r--   0 zach       (501) staff       (20)      841 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/initialization.py
+-rw-r--r--   0 zach       (501) staff       (20)     6183 2022-03-10 14:13:00.000000 py_grama-0.3.5/grama/psdr/local_linear.py
+-rw-r--r--   0 zach       (501) staff       (20)      724 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/misc.py
+-rw-r--r--   0 zach       (501) staff       (20)     2732 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/pgf.py
+-rw-r--r--   0 zach       (501) staff       (20)     3775 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/poly.py
+-rw-r--r--   0 zach       (501) staff       (20)    17487 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/polyridge.py
+-rw-r--r--   0 zach       (501) staff       (20)     8692 2022-03-02 19:36:18.000000 py_grama-0.3.5/grama/psdr/psdr_tools.py
+-rw-r--r--   0 zach       (501) staff       (20)      921 2022-03-01 22:38:38.000000 py_grama-0.3.5/grama/psdr/quadrature.py
+-rw-r--r--   0 zach       (501) staff       (20)     1801 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/ridge.py
+-rw-r--r--   0 zach       (501) staff       (20)     9189 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/seqlp.py
+-rw-r--r--   0 zach       (501) staff       (20)     7473 2022-02-23 18:18:30.000000 py_grama-0.3.5/grama/psdr/subspace.py
+-rw-r--r--   0 zach       (501) staff       (20)     9809 2023-04-25 19:26:35.000000 py_grama-0.3.5/grama/spc.py
+-rw-r--r--   0 zach       (501) staff       (20)     6995 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/string_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     5876 2022-11-04 17:50:26.000000 py_grama-0.3.5/grama/support.py
+-rw-r--r--   0 zach       (501) staff       (20)    13267 2022-04-20 12:57:11.000000 py_grama-0.3.5/grama/tools.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.751698 py_grama-0.3.5/grama/tran/
+-rw-r--r--   0 zach       (501) staff       (20)       86 2021-07-07 12:13:10.000000 py_grama-0.3.5/grama/tran/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)     2657 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran/tran_matminer.py
+-rw-r--r--   0 zach       (501) staff       (20)     5356 2022-12-28 15:10:00.000000 py_grama-0.3.5/grama/tran/tran_scikitlearn.py
+-rw-r--r--   0 zach       (501) staff       (20)     3434 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran/tran_umap.py
+-rw-r--r--   0 zach       (501) staff       (20)     6346 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran_is.py
+-rw-r--r--   0 zach       (501) staff       (20)    18443 2023-04-25 19:26:35.000000 py_grama-0.3.5/grama/tran_pivot.py
+-rw-r--r--   0 zach       (501) staff       (20)     5836 2022-04-17 03:06:58.000000 py_grama-0.3.5/grama/tran_shapley.py
+-rw-r--r--   0 zach       (501) staff       (20)    13351 2023-03-17 15:26:35.000000 py_grama-0.3.5/grama/tran_summaries.py
+-rw-r--r--   0 zach       (501) staff       (20)    14018 2022-11-04 16:42:06.000000 py_grama-0.3.5/grama/tran_tools.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.752374 py_grama-0.3.5/py_grama.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     5347 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     3540 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (501) staff       (20)      280 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/requires.txt
+-rw-r--r--   0 zach       (501) staff       (20)        6 2023-07-15 15:45:56.000000 py_grama-0.3.5/py_grama.egg-info/top_level.txt
+-rw-r--r--   0 zach       (501) staff       (20)       38 2023-07-15 15:45:56.759848 py_grama-0.3.5/setup.cfg
+-rw-r--r--   0 zach       (501) staff       (20)     1486 2023-07-15 15:41:48.000000 py_grama-0.3.5/setup.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-07-15 15:45:56.759095 py_grama-0.3.5/tests/
+-rw-r--r--   0 zach       (501) staff       (20)     2454 2023-03-17 15:26:35.000000 py_grama-0.3.5/tests/test_autoplot.py
+-rw-r--r--   0 zach       (501) staff       (20)     4927 2022-04-17 03:06:58.000000 py_grama-0.3.5/tests/test_contour.py
+-rw-r--r--   0 zach       (501) staff       (20)    15210 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_core.py
+-rw-r--r--   0 zach       (501) staff       (20)      463 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_data.py
+-rw-r--r--   0 zach       (501) staff       (20)     1434 2022-04-03 13:32:37.000000 py_grama-0.3.5/tests/test_dataframe.py
+-rw-r--r--   0 zach       (501) staff       (20)     1014 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_dfply_count.py
+-rw-r--r--   0 zach       (501) staff       (20)      659 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_filter_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)      583 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_group.py
+-rw-r--r--   0 zach       (501) staff       (20)     4133 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_join.py
+-rw-r--r--   0 zach       (501) staff       (20)     3008 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_dfply_mutate_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     9110 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_reshape.py
+-rw-r--r--   0 zach       (501) staff       (20)    14801 2023-01-03 18:22:07.000000 py_grama-0.3.5/tests/test_dfply_select.py
+-rw-r--r--   0 zach       (501) staff       (20)      870 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_subset.py
+-rw-r--r--   0 zach       (501) staff       (20)     3339 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_summarize.py
+-rw-r--r--   0 zach       (501) staff       (20)    20877 2022-04-19 22:57:07.000000 py_grama-0.3.5/tests/test_dfply_summary_functions.py
+-rw-r--r--   0 zach       (501) staff       (20)     2697 2022-01-28 00:02:51.000000 py_grama-0.3.5/tests/test_dfply_transform.py
+-rw-r--r--   0 zach       (501) staff       (20)     4619 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_dfply_vector.py
+-rw-r--r--   0 zach       (501) staff       (20)    10725 2022-09-19 17:26:49.000000 py_grama-0.3.5/tests/test_eval_pnd.py
+-rw-r--r--   0 zach       (501) staff       (20)    25250 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_evals.py
+-rw-r--r--   0 zach       (501) staff       (20)     9763 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_fit.py
+-rw-r--r--   0 zach       (501) staff       (20)     2398 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_is.py
+-rw-r--r--   0 zach       (501) staff       (20)     4785 2022-02-03 20:27:56.000000 py_grama-0.3.5/tests/test_marginals.py
+-rw-r--r--   0 zach       (501) staff       (20)     8871 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_mbi.py
+-rw-r--r--   0 zach       (501) staff       (20)     2994 2022-06-16 13:35:20.000000 py_grama-0.3.5/tests/test_models.py
+-rw-r--r--   0 zach       (501) staff       (20)      309 2021-03-26 22:43:20.000000 py_grama-0.3.5/tests/test_mp_restart.py
+-rw-r--r--   0 zach       (501) staff       (20)     2603 2022-01-27 23:25:14.000000 py_grama-0.3.5/tests/test_pipes.py
+-rw-r--r--   0 zach       (501) staff       (20)    21403 2022-04-14 13:54:09.000000 py_grama-0.3.5/tests/test_pivot.py
+-rw-r--r--   0 zach       (501) staff       (20)     2643 2022-03-02 19:36:18.000000 py_grama-0.3.5/tests/test_psdr.py
+-rw-r--r--   0 zach       (501) staff       (20)      633 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_shapley.py
+-rw-r--r--   0 zach       (501) staff       (20)     2093 2023-04-25 19:26:35.000000 py_grama-0.3.5/tests/test_spc.py
+-rw-r--r--   0 zach       (501) staff       (20)     4711 2021-11-12 12:20:36.000000 py_grama-0.3.5/tests/test_string_helpers.py
+-rw-r--r--   0 zach       (501) staff       (20)     1294 2022-12-01 14:56:07.000000 py_grama-0.3.5/tests/test_support.py
+-rw-r--r--   0 zach       (501) staff       (20)     4340 2023-06-20 16:22:27.000000 py_grama-0.3.5/tests/test_tail.py
+-rw-r--r--   0 zach       (501) staff       (20)      430 2022-04-03 13:32:37.000000 py_grama-0.3.5/tests/test_tools.py
+-rw-r--r--   0 zach       (501) staff       (20)    12415 2022-12-28 15:10:00.000000 py_grama-0.3.5/tests/test_transforms.py
```

### Comparing `py_grama-0.3.4/LICENSE` & `py_grama-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/PKG-INFO` & `py_grama-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_grama
-Version: 0.3.4
+Version: 0.3.5
 Summary: A grammar of model analysis
 Home-page: https://github.com/zdelrosario/py_grama
 Author: Zachary del Rosario
 Author-email: zdelrosario@outlook.com
 License: MIT
 Description: # py_grama
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.02462/status.svg)](https://doi.org/10.21105/joss.02462) [![PyPI version](https://badge.fury.io/py/py-grama.svg)](https://badge.fury.io/py/py-grama) [![Documentation Status](https://readthedocs.org/projects/py_grama/badge/?version=latest)](https://py_grama.readthedocs.io/en/latest/?badge=latest) ![Python package test](https://github.com/zdelrosario/py_grama/workflows/Python%20package%20test/badge.svg) [![codecov](https://codecov.io/gh/zdelrosario/py_grama/branch/master/graph/badge.svg)](https://codecov.io/gh/zdelrosario/py_grama) [![CodeFactor](https://www.codefactor.io/repository/github/zdelrosario/py_grama/badge/master)](https://www.codefactor.io/repository/github/zdelrosario/py_grama/overview/master) 
@@ -76,16 +76,15 @@
         }
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8, <3.10
 Description-Content-Type: text/markdown
-Provides-Extra: lolo
 Provides-Extra: matminer
 Provides-Extra: sklearn
 Provides-Extra: statsmodels
 Provides-Extra: pyDOE
 Provides-Extra: umap
 Provides-Extra: dev
```

### Comparing `py_grama-0.3.4/README.md` & `py_grama-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/__init__.py` & `py_grama-0.3.5/grama/__init__.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/comp_metamodels.py` & `py_grama-0.3.5/grama/comp_metamodels.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/core.py` & `py_grama-0.3.5/grama/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,17 @@
                     self.name
                 )
             )
 
         ## Set up output
         n_rows = df.shape[0]
         results = zeros((n_rows, len(self.out)))
+
         for ind in range(n_rows):
-            results[ind] = self.func(df.loc[ind, self.var])
+            results[ind] = self.func(*df.loc[ind, self.var])
 
         ## Package output as DataFrame
         return DataFrame(data=results, columns=self.out)
 
     def summary(self):
         """Returns a summary string
         """
@@ -821,14 +822,16 @@
         """
         if functions is None:
             functions = []
         if domain is None:
             domain = Domain()
         if density is None:
             density = Density()
+        if name is None:
+            name = "(no name)"
 
         self.name = name
         self.functions = functions
         self.domain = domain
         self.density = density
 
         self.update()
@@ -882,35 +885,40 @@
             float: Estimated runtime, in seconds
 
         """
         rate = 0
         for fun in self.functions:
             rate = rate + fun.runtime
 
-        return rate * n
+        return float(rate * n)
 
     def runtime_message(self, df):
         """Runtime message
 
         Estimate total runtime based on proposed DataFrame, prepare a message
-        for console print. Print no message if runtime is negligible.
+        for console print.
 
         Args:
             self (gr.Model):
             df (DataFrame): Data to evaluate
 
         Returns:
             str: Runtime message
 
         """
         runtime = self.runtime(df.shape[0])
 
-        if runtime < RUNTIME_LOWER:
-            return None
-        return "Estimated runtime: {0:3.4f} sec".format(runtime)
+        if runtime is None:
+            return "Runtime estimate unavailable; model has no timing data."
+        elif runtime >= 3600:
+            return "Estimated runtime: {0:3.4f} hr".format(runtime / 3600)
+        elif runtime >= 60:
+            return "Estimated runtime: {0:3.4f} min".format(runtime / 60)
+        else:
+            return "Estimated runtime: {0:3.4f} sec".format(runtime)
 
     def det_nom(self):
         """Return nominal conditions for deterministic variables
 
         Returns:
             DataFrame: Nominal values for deterministic variables
 
@@ -960,23 +968,16 @@
             DataFrame: Outer product of samples
 
         """
         ## Pass-through if no var_det
         if self.n_var_det == 0:
             return df_rand
 
-        ## Error-throwing default value
-        if df_det is None:
-            raise ValueError("df_det must be DataFrame or 'nom'")
-        ## String shortcut
-        elif isinstance(df_det, str):
-            if df_det == "nom":
-                df_det = self.det_nom()
-            else:
-                raise ValueError("df_det shortcut string invalid")
+        elif isinstance(df_det, str) and df_det == "nom":
+            df_det = self.det_nom()
         ## DataFrame
         else:
             ## Check invariant; model inputs must be subset of df columns
             if not set(self.var_det).issubset(set(df_det.columns)):
                 raise ValueError("model.var_det not a subset of given columns")
 
         ## Pass-through if no var_rand
```

### Comparing `py_grama-0.3.4/grama/data/__init__.py` & `py_grama-0.3.5/grama/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         y: Projectile height (meters)
 
     df_shewhart: Aluminum die cast data from Table 3 in Shewhart (1931)
 
         specimen: Specimen identifier
 
-        tensile_strength: Specimen tensile strength (psi)
+        tensile_strength: Specimen tensile strength (psi). The original reference does not specify if this is the yield or ultimate strength.
 
         hardness: Specimen hardness (Rockwell's "E")
 
         density: Specimen density (gm/cm^3)
 
 References:
     Stang, Greenspan, and Newman, "Poisson's ratio of some structural alloys for
```

### Comparing `py_grama-0.3.4/grama/data/datasets.py` & `py_grama-0.3.5/grama/data/datasets.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/data/diamonds.csv` & `py_grama-0.3.5/grama/data/diamonds.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/data/psaap.csv` & `py_grama-0.3.5/grama/data/psaap.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/data/shewhart1931-table3.csv` & `py_grama-0.3.5/grama/data/shewhart1931-table3.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/data/stang.csv` & `py_grama-0.3.5/grama/data/stang.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/data/stang_long.csv` & `py_grama-0.3.5/grama/data/stang_long.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/data/trajectory_full.csv` & `py_grama-0.3.5/grama/data/trajectory_full.csv`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/dataframe.py` & `py_grama-0.3.5/grama/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,40 +21,38 @@
         return 1
 
 
 ## DataFrame constructor utility
 def df_make(**kwargs):
     r"""Construct a DataFrame
 
-    Helper function to construct a DataFrame.
+    Helper function to construct a DataFrame. A common use-case is to use df_make() to pass values to the df (and related) keyword arguments succinctly.
+
+    Kwargs:
+        varname (iterable): Column for constructed dataframe; column name inferred from variable name.
 
-    Keyword Args:
-        varname (iterable): Column for constructed dataframe; column
-                            name inferred from variable name.
     Returns:
         DataFrame: Constructed DataFrame
 
     Preconditions:
-        All provided iterables must have identical length or be of
-        length one.
-
+        All provided iterables must have identical length or be of length one.
         All provided variable names (keyword arguments) must be distinct.
 
-    Examples:
-        A common use-case is to use df_make() to pass values to
-        the df_det keyword argument succinctly;
-
-        >>> import grama as gr
-        >>> from models import make_test
-        >>> md = make_test()
-        >>> md >> \
-        >>>     gr.ev_monte_carlo(
-        >>>         n=1e3,
-        >>>         df_det=gr.df_make(x2=[1, 2])
-        >>>     )
+    Examples::
+
+        import grama as gr
+        from models import make_test
+        md = make_test()
+        (
+            md
+            >> gr.ev_sample(
+                n=1e3,
+                df_det=gr.df_make(x2=[1, 2])
+            )
+        )
 
     """
     ## Catch passed Intention operator
     if any([isinstance(v, Intention) for v in kwargs.values()]):
         raise ValueError(
             "df_make() does not support the Intention operator; " +
             "did you mean to use a DataFrame argument?\n\n" +
@@ -85,16 +83,15 @@
     return df_res
 
 
 ## DataFrame equality checker
 def df_equal(df1, df2, close=False, precision=3):
     """Check DataFrame equality
 
-    Check that two dataframes have the same columns and values. Allow column
-    order to differ.
+    Check that two dataframes have the same columns and values. Allows column order to differ.
 
     Args:
         df1 (DataFrame): Comparison input 1
         df2 (DataFrame): Comparison input 2
 
     Returns:
         bool: Result of comparison
@@ -119,27 +116,27 @@
     else:
         return df1[df2.columns].equals(df2)
 
 ## DataFrame constructor utility; outer product
 def df_grid(**kwargs):
     r"""Construct a DataFrame as outer-product
 
-    Helper function to construct a DataFrame as an outer-product of the given
-    columns.
+    Helper function to construct a DataFrame as an outer-product of the given columns.
+
+    Kwargs:
+        varname (iterable): Column for constructed dataframe; column name inferred from variable name.
 
-    Keyword Args:
-        varname (iterable): Column for constructed dataframe; column
-                            name inferred from variable name.
     Returns:
         DataFrame: Constructed DataFrame
 
     Preconditions:
         All provided variable names (keyword arguments) must be distinct.
 
-    Examples:
+    Examples::
+
         import grama as gr
         ## Make an empty DataFrame
         gr.df_grid()
         ## Create a row for every pair of values (6 rows total)
         gr.df_grid(x=["A", "B"], y=[1, 2, 3])
 
     """
```

### Comparing `py_grama-0.3.4/grama/dfply/base.py` & `py_grama-0.3.5/grama/dfply/base.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/dfply/join.py` & `py_grama-0.3.5/grama/dfply/join.py`

 * *Files 17% similar despite different names*

```diff
@@ -59,20 +59,24 @@
     Kwargs:
         by (str or list): Columns to join on. If a single string, will join
             on that column. If a list of lists which contain strings or
             integers, the right/left columns to join on.
         suffixes (list): String suffixes to append to column names in left
             and right DataFrames.
 
-    Example:
-        a >> inner_join(b, by='x1')
+    Examples::
+
+        import grama as gr
+        df_1 = gr.df_make(key=["A", "B", "C"], x=[1, 2, 3])
+        df_2 = gr.df_make(key=["B", "A", "D"], y=[4, 5, 6])
+        (
+            df_1
+            >> gr.tf_inner_join(df_2, by="key")
+        )
 
-          x1  x2     x3
-        0  A   1   True
-        1  B   2  False
     """
 
     left_on, right_on, suffixes = get_join_parameters(kwargs)
     joined = df.merge(
         other, how="inner", left_on=left_on, right_on=right_on, suffixes=suffixes
     )
     return joined
@@ -92,22 +96,24 @@
     Kwargs:
         by (str or list): Columns to join on. If a single string, will join
             on that column. If a list of lists which contain strings or
             integers, the right/left columns to join on.
         suffixes (list): String suffixes to append to column names in left
             and right DataFrames.
 
-    Example:
-        a >> outer_join(b, by='x1')
+    Examples::
+
+        import grama as gr
+        df_1 = gr.df_make(key=["A", "B", "C"], x=[1, 2, 3])
+        df_2 = gr.df_make(key=["B", "A", "D"], y=[4, 5, 6])
+        (
+            df_1
+            >> gr.tf_full_join(df_2, by="key")
+        )
 
-          x1   x2     x3
-        0  A  1.0   True
-        1  B  2.0  False
-        2  C  3.0    NaN
-        3  D  NaN   True
     """
 
     left_on, right_on, suffixes = get_join_parameters(kwargs)
     joined = df.merge(
         other, how="outer", left_on=left_on, right_on=right_on, suffixes=suffixes
     )
     return joined
@@ -127,22 +133,24 @@
     Kwargs:
         by (str or list): Columns to join on. If a single string, will join
             on that column. If a list of lists which contain strings or
             integers, the right/left columns to join on.
         suffixes (list): String suffixes to append to column names in left
             and right DataFrames.
 
-    Example:
-        a >> full_join(b, by='x1')
+    Examples::
+
+        import grama as gr
+        df_1 = gr.df_make(key=["A", "B", "C"], x=[1, 2, 3])
+        df_2 = gr.df_make(key=["B", "A", "D"], y=[4, 5, 6])
+        (
+            df_1
+            >> gr.tf_outer_join(df_2, by="key")
+        )
 
-          x1   x2     x3
-        0  A  1.0   True
-        1  B  2.0  False
-        2  C  3.0    NaN
-        3  D  NaN   True
     """
 
     left_on, right_on, suffixes = get_join_parameters(kwargs)
     joined = df.merge(
         other, how="outer", left_on=left_on, right_on=right_on, suffixes=suffixes
     )
     return joined
@@ -162,21 +170,24 @@
     Kwargs:
         by (str or list): Columns to join on. If a single string, will join
             on that column. If a list of lists which contain strings or
             integers, the right/left columns to join on.
         suffixes (list): String suffixes to append to column names in left
             and right DataFrames.
 
-    Example:
-        a >> left_join(b, by='x1')
+    Examples::
+
+        import grama as gr
+        df_1 = gr.df_make(key=["A", "B", "C"], x=[1, 2, 3])
+        df_2 = gr.df_make(key=["B", "A", "D"], y=[4, 5, 6])
+        (
+            df_1
+            >> gr.tf_left_join(df_2, by="key")
+        )
 
-          x1  x2     x3
-        0  A   1   True
-        1  B   2  False
-        2  C   3    NaN
     """
 
     left_on, right_on, suffixes = get_join_parameters(kwargs)
     joined = df.merge(
         other, how="left", left_on=left_on, right_on=right_on, suffixes=suffixes
     )
     return joined
@@ -196,21 +207,24 @@
     Kwargs:
         by (str or list): Columns to join on. If a single string, will join
             on that column. If a list of lists which contain strings or
             integers, the right/left columns to join on.
         suffixes (list): String suffixes to append to column names in left
             and right DataFrames.
 
-    Example:
-        a >> right_join(b, by='x1')
+    Examples::
+
+        import grama as gr
+        df_1 = gr.df_make(key=["A", "B", "C"], x=[1, 2, 3])
+        df_2 = gr.df_make(key=["B", "A", "D"], y=[4, 5, 6])
+        (
+            df_1
+            >> gr.tf_right_join(df_2, by="key")
+        )
 
-          x1   x2     x3
-        0  A  1.0   True
-        1  B  2.0  False
-        2  D  NaN   True
     """
 
     left_on, right_on, suffixes = get_join_parameters(kwargs)
     joined = df.merge(
         other, how="right", left_on=left_on, right_on=right_on, suffixes=suffixes
     )
     return joined
@@ -229,20 +243,24 @@
         other (pandas.DataFrame): Right DataFrame
 
     Kwargs:
         by (str or list): Columns to join on. If a single string, will join
             on that column. If a list of lists which contain strings or
             integers, the right/left columns to join on.
 
-    Example:
-        a >> semi_join(b, by='x1')
+    Examples::
+
+        import grama as gr
+        df_1 = gr.df_make(key=["A", "B", "C"], x=[1, 2, 3])
+        df_2 = gr.df_make(key=["B", "A", "D"], y=[4, 5, 6])
+        (
+            df_1
+            >> gr.tf_semi_join(df_2, by="key")
+        )
 
-          x1  x2
-        0  A   1
-        1  B   2
     """
 
     left_on, right_on, suffixes = get_join_parameters(kwargs)
     if not right_on:
         right_on = [
             col_name
             for col_name in df.columns.values.tolist()
@@ -276,19 +294,24 @@
         other (pandas.DataFrame): Right DataFrame
 
     Kwargs:
         by (str or list): Columns to join on. If a single string, will join
             on that column. If a list of lists which contain strings or
             integers, the right/left columns to join on.
 
-    Example:
-        a >> anti_join(b, by='x1')
+    Examples::
+
+        import grama as gr
+        df_1 = gr.df_make(key=["A", "B", "C"], x=[1, 2, 3])
+        df_2 = gr.df_make(key=["B", "A", "D"], y=[4, 5, 6])
+        (
+            df_1
+            >> gr.tf_anti_join(df_2, by="key")
+        )
 
-          x1  x2
-        2  C   3
     """
 
     left_on, right_on, suffixes = get_join_parameters(kwargs)
     if not right_on:
         right_on = [
             col_name
             for col_name in df.columns.values.tolist()
```

### Comparing `py_grama-0.3.4/grama/dfply/mask_helpers.py` & `py_grama-0.3.5/grama/dfply/mask_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/dfply/reshape.py` & `py_grama-0.3.5/grama/dfply/reshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
         df (pandas.DataFrame): DataFrame
 
     Kwargs:
         **kwargs: Renaming pair
             the name of the argument (left of `=`) will be the new column name,
             the value of the argument (right of `=`) is the old column name (as a string).
 
-    Examples:
+    Examples::
+
         ## Setup
         import grama as gr
         DF = gr.Intention()
         ## Load example dataset
         from grama.data import df_stang
 
         ## Rename columns
@@ -134,15 +135,16 @@
             into they key and value columns.
 
     Kwargs:
         add_id (bool): Boolean value indicating whether to add a `"_ID"`
             column that will preserve information about the original rows
             (useful for being able to re-widen the data later).
 
-    Example:
+    Example ::
+
         diamonds >> gather('variable', 'value', ['price', 'depth','x','y','z']) >> head(5)
 
            carat      cut color clarity  table variable  value
         0   0.23    Ideal     E     SI2   55.0    price  326.0
         1   0.21  Premium     E     SI1   61.0    price  326.0
         2   0.23     Good     E     VS1   65.0    price  327.0
         3   0.29  Premium     I     VS2   58.0    price  334.0
@@ -217,15 +219,16 @@
         values (str, int, or symbolic): Label for the values column.
 
     Kwargs:
         convert (bool): Boolean indicating whether or not to try and convert
             the spread columns to more appropriate data types.
 
 
-    Example:
+    Examples::
+
         widened = elongated >> spread(X.variable, X.value)
         widened >> head(5)
 
             _ID carat clarity color        cut depth price table     x     y     z
         0     0  0.23     SI2     E      Ideal  61.5   326    55  3.95  3.98  2.43
         1     1  0.21     SI1     E    Premium  59.8   326    61  3.89  3.84  2.31
         2    10   0.3     SI1     J       Good    64   339    55  4.25  4.28  2.73
@@ -308,15 +311,16 @@
         convert (bool): Boolean indicating whether the new columns should be converted to the appropriate type.
         extra (str): either `'drop'`, where split pieces beyond the specified new columns are dropped, or `'merge'`, where the final split piece contains the remainder of the original column.
         fill (str): either `'right'`, where `np.nan` values are filled in the right-most columns for missing pieces, or `'left'` where `np.nan` values are filled in the left-most columns.
 
     Returns:
         pandas.DataFrame: Modified data
 
-    Examples:
+    Examples::
+
         import grama as gr
         DF = gr.Intention
 
         ## Simple example
         df = gr.df_make(x=["a_1", "b_2", "c_3"])
         (
             df
@@ -475,15 +479,15 @@
     Kwargs:
         convert (bool): Boolean indicating whether or not to try and convert
             the spread columns to more appropriate data types.
 
     Returns:
         DataFrame:
 
-    Example:
+    Example::
 
     """
 
     df_res = df.explode(col).reset_index(drop=True)
 
     if convert and (df_res[col].dtype.kind in "OSaU"):
         return convert_type(df_res, [col])
```

### Comparing `py_grama-0.3.4/grama/dfply/select.py` & `py_grama-0.3.5/grama/dfply/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     "tf_select",
     "tran_select_if",
     "tf_select_if",
     "tran_drop",
     "tf_drop",
     "tran_drop_if",
     "tf_drop_if",
+    "is_numeric",
     "starts_with",
     "ends_with",
     "contains",
     "matches",
     "everything",
     "num_range",
     "one_of",
@@ -18,19 +19,20 @@
     "columns_from",
     "columns_to",
     "resolve_selection"
 ]
 
 import re
 from .base import Intention, dfdelegate, symbolic_evaluation, \
-    group_delegation, flatten
+    group_delegation, flatten, make_symbolic
 from .. import add_pipe
 from numpy import zeros, where, ones
 from numpy import max as npmax
 from pandas import Index, Series
+from pandas.api.types import is_numeric_dtype
 
 
 # ------------------------------------------------------------------------------
 # Select and drop operators
 # ------------------------------------------------------------------------------
 
 
@@ -269,7 +271,29 @@
 
 
 @selection_filter
 def columns_to(columns, end_col, inclusive=False):
     if isinstance(end_col, str):
         end_col = columns.index(end_col)
     return columns[: end_col + int(inclusive)]
+
+
+@make_symbolic
+def is_numeric(series):
+    """Determine if column is numeric
+
+    Returns True if the provided column is numeric, False otherwise. Intended for calls to select_if() or mutate_if().
+
+    Args:
+        bool: Boolean corresponding to the datatype of the given column
+
+    Examples::
+        import grama as gr
+        from grama.data import df_diamonds
+
+        (
+            df_diamonds
+            gr.tf_select_if(gr.is_numeric)
+        )
+
+    """
+    return is_numeric_dtype(series)
```

### Comparing `py_grama-0.3.4/grama/dfply/set_ops.py` & `py_grama-0.3.5/grama/dfply/set_ops.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/dfply/string_helpers.py` & `py_grama-0.3.5/grama/dfply/string_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/dfply/subset.py` & `py_grama-0.3.5/grama/dfply/subset.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/dfply/summarize.py` & `py_grama-0.3.5/grama/dfply/summarize.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         **kwargs (array-like or summary expression): Summaries to assign;
             the name of the argument (left of `=`) will be the new column name,
             the value of the argument (right of `=`) defines the summary
 
     Returns:
         DataFrame: Summarized data
 
-    Examples:
+    Examples::
+
         ## Setup
         import grama as gr
         DF = gr.Intention()
         ## Load example dataset
         from grama.data import df_diamonds
 
         ## Compute some summary statistics
```

### Comparing `py_grama-0.3.4/grama/dfply/summary_functions.py` & `py_grama-0.3.5/grama/dfply/summary_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,18 @@
     "binomial_ci",
     "corr",
     "mean",
     "mean_lo",
     "mean_up",
     "IQR",
     "quant",
+    "pint_lo",
+    "pint_lo_index",
+    "pint_up",
+    "pint_up_index",
     "pr",
     "pr_lo",
     "pr_up",
     "var",
     "sd",
     "skew",
     "kurt",
@@ -23,24 +27,26 @@
     "last",
 
     "n",
     "nth",
     "n_distinct",
     "neff_is",
 
+    "mad",
+    "mead",
     "mse",
     "rmse",
     "ndme",
     "rsq",
 ]
 
 from .base import make_symbolic, Intention
 from .vector import order_series_by
 from numpy import array, sqrt, power, nan, isnan
-from scipy.stats import norm, pearsonr, spearmanr, kurtosis
+from scipy.stats import norm, pearsonr, spearmanr, kurtosis, nhypergeom
 from scipy.stats import skew as spskew
 
 
 # ------------------------------------------------------------------------------
 # Series summary functions
 # ------------------------------------------------------------------------------
 
@@ -59,64 +65,66 @@
     # else:
     #     return np.nan
     return series.mean()
 
 
 # Mean CI helpers
 @make_symbolic
-def mean_lo(series, alpha=0.01):
+def mean_lo(series, alpha=0.005):
     """Return a confidence interval (lower bound) for the mean
 
     Uses a central limit approximation for a lower confidence bound of an estimated mean. That is:
 
         m - q(alpha) * s / sqrt(n)
 
     where
 
         m = sample mean
         s = sample standard deviation
         n = sample size
         q(alpha) = alpha-level lower-quantile of standard normal
                  = (-norm.ppf(alpha))
 
+    For a two-sided interval at a confidence level of ``C``, set ``alpha = 1 - C`` and use ``[gr.mean_lo(X, alpha=alpha/2), gr.mean_up(X, alpha=alpha/2)``. Note that the default ``alpha`` level for both helpers is calibrated for a two-sided interval with ``C = 0.99``.
+
     Args:
         series (pandas.Series): column to summarize
-        alpha (float): alpha-level for calculation
-            Note that the confidence level C is given by C = 1 - alpha
+        alpha (float): alpha-level for calculation. Note that the confidence level C is given by ``C = 1 - alpha``.
 
     Returns:
         float: Lower confidence interval for the mean
     """
     m = mean(series)
     s = sd(series)
     n_sample = len(series)
 
     return m - (-norm.ppf(alpha)) * s / sqrt(n_sample)
 
 
 @make_symbolic
-def mean_up(series, alpha=0.01):
+def mean_up(series, alpha=0.005):
     """Return a confidence interval (upper bound) for the mean
 
     Uses a central limit approximation for a upper confidence bound of an estimated mean. That is:
 
         m + q(alpha) * s / sqrt(n)
 
     where
 
         m = sample mean
         s = sample standard deviation
         n = sample size
         q(alpha) = alpha-level lower-quantile of standard normal
                  = (-norm.ppf(alpha))
 
+    For a two-sided interval at a confidence level of ``C``, set ``alpha = 1 - C`` and use ``[gr.mean_lo(X, alpha=alpha/2), gr.mean_up(X, alpha=alpha/2)``. Note that the default ``alpha`` level for both helpers is calibrated for a two-sided interval with ``C = 0.99``.
+
     Args:
         series (pandas.Series): column to summarize
-        alpha (float): alpha-level for calculation
-            Note that the confidence level C is given by C = 1 - alpha
+        alpha (float): alpha-level for calculation. Note that the confidence level C is given by ``C = 1 - alpha``.
 
     Returns:
         float: Upper confidence interval for the mean
     """
     m = mean(series)
     s = sd(series)
     n_sample = len(series)
@@ -224,15 +232,16 @@
 def n(series=None):
     """
     Returns the length of a series.
 
     Args:
         series (pandas.Series): column to summarize. Default is the size of the parent DataFrame.
 
-    Examples:
+    Examples::
+
         import grama as gr
         from grama.data import df_diamonds
         DF = gr.Intention()
 
         ## Count entries in series
         gr.n(df_diamonds.cut)
         ## Use implicit mode to get size of current DataFrame
@@ -383,14 +392,50 @@
         series (pandas.Series): column to summarize.
     """
 
     return series.sum()
 
 
 @make_symbolic
+def mad(series_pred, series_meas):
+    """Compute MAD
+
+    Returns the mean absolute deviation (MAD) between predicted and measured
+    values.
+
+    Args:
+        series_pred (pandas.Series): column of predicted values
+        series_meas (pandas.Series): column of measured values
+
+    Returns:
+        float: Mean absolute deviation (MAD)
+    """
+
+    return (series_pred - series_meas).abs().mean()
+
+
+@make_symbolic
+def mead(series_pred, series_meas):
+    """Compute median absolute deviation
+
+    Returns the median absolute deviation (MEAD) between predicted and measured
+    values.
+
+    Args:
+        series_pred (pandas.Series): column of predicted values
+        series_meas (pandas.Series): column of measured values
+
+    Returns:
+        float: Median absolute deviation (MEAD)
+    """
+
+    return (series_pred - series_meas).abs().median()
+
+
+@make_symbolic
 def mse(series_pred, series_meas):
     """Compute MSE
 
     Returns the mean-square-error (MSE) between predicted and measured
     values.
 
     Args:
@@ -520,118 +565,125 @@
     Estimate a probability from a random sample. Provided series must be boolean, with 1 corresponding to the event of interest.
 
     Use logical statements together with column values to construct a boolean indicator for the event you're interested in. Remember that you can chain multiple statements with logical and `&` and or `|` operators. See the examples below for more details.
 
     Args:
         series (pandas.Series): Column to summarize; must be boolean or 0/1.
 
-    Examples:
-        >>> import grama as gr
-        >>> DF = gr.Intention()
-        >>> ## Cantilever beam examples
-        >>> from grama.models import make_cantilever_beam
-        >>> md_beam = make_cantilever_beam()
-        >>>
-        >>> ## Estimate probabilities
-        >>> (
-        >>>     md_beam
-        >>>     # Generate large
-        >>>     >> gr.ev_sample(n=1e5, df_det="nom")
-        >>>     # Estimate probabilities of failure
-        >>>     >> gr.tf_summarize(
-        >>>         pof_stress=gr.pr(DF.g_stress <= 0),
-        >>>         pof_disp=gr.pr(DF.g_disp <= 0),
-        >>>         pof_joint=gr.pr( (DF.g_stress <= 0) & (DF.g_disp) ),
-        >>>         pof_either=gr.pr( (DF.g_stress <= 0) | (DF.g_disp) ),
-        >>>     )
-        >>> )
+    Examples::
+
+        import grama as gr
+        DF = gr.Intention()
+        ## Cantilever beam examples
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+
+        ## Estimate probabilities
+        (
+            md_beam
+            # Generate large
+            >> gr.ev_sample(n=1e5, df_det="nom")
+            # Estimate probabilities of failure
+            >> gr.tf_summarize(
+                pof_stress=gr.pr(DF.g_stress <= 0),
+                pof_disp=gr.pr(DF.g_disp <= 0),
+                pof_joint=gr.pr( (DF.g_stress <= 0) & (DF.g_disp) ),
+                pof_either=gr.pr( (DF.g_stress <= 0) | (DF.g_disp) ),
+            )
+        )
 
     """
     return series.mean()
 
 
 @make_symbolic
-def pr_lo(series, alpha=0.01):
+def pr_lo(series, alpha=0.005):
     r"""Estimate a confidence interval for a probability
 
     Estimate the lower side of a confidence interval for a probability from a random sample. Provided series must be boolean, with 1 corresponding to the event of interest.
 
     Uses Wilson interval method.
 
     Use logical statements together with column values to construct a boolean indicator for the event you're interested in. Remember that you can chain multiple statements with logical and `&` and or `|` operators. See the documentation for `gr.pr()` for more details and examples.
 
+    For a two-sided interval at a confidence level of ``C``, set ``alpha = 1 - C`` and use ``[gr.mean_lo(X, alpha=alpha/2), gr.mean_up(X, alpha=alpha/2)``. Note that the default ``alpha`` level for both helpers is calibrated for a two-sided interval with ``C = 0.99``.
+
     Args:
         series (pandas.Series): Column to summarize; must be boolean or 0/1.
         alpha (float): alpha-level for calculation, in (0, 1)
             Note that the confidence level C is given by C = 1 - alpha
 
     Returns:
         float: Lower confidence interval
 
-    Examples:
-        >>> import grama as gr
-        >>> DF = gr.Intention()
-        >>> ## Cantilever beam examples
-        >>> from grama.models import make_cantilever_beam
-        >>> md_beam = make_cantilever_beam()
-        >>>
-        >>> ## Estimate probabilities
-        >>> (
-        >>>     md_beam
-        >>>     # Generate large
-        >>>     >> gr.ev_sample(n=1e5, df_det="nom")
-        >>>     # Estimate probabilities with a confidence interval
-        >>>     >> gr.tf_summarize(
-        >>>         pof_lo=gr.pr_lo(DF.g_stress <= 0),
-        >>>         pof=gr.pr(DF.g_stress <= 0),
-        >>>         pof_up=gr.pr_up(DF.g_stress <= 0),
-        >>>     )
-        >>> )
+    Examples::
+
+        import grama as gr
+        DF = gr.Intention()
+        ## Cantilever beam examples
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+
+        ## Estimate probabilities
+        (
+            md_beam
+            # Generate large
+            >> gr.ev_sample(n=1e5, df_det="nom")
+            # Estimate probabilities with a confidence interval
+            >> gr.tf_summarize(
+                pof_lo=gr.pr_lo(DF.g_stress <= 0),
+                pof=gr.pr(DF.g_stress <= 0),
+                pof_up=gr.pr_up(DF.g_stress <= 0),
+            )
+        )
     """
     up = binomial_ci(series, alpha=alpha, side="lo")
     return up
 
 
 @make_symbolic
-def pr_up(series, alpha=0.01):
+def pr_up(series, alpha=0.005):
     r"""
 
     Estimate the upper side of a confidence interval for a probability from a random sample. Provided series must be boolean, with 1 corresponding to the event of interest.
 
     Uses Wilson interval method.
 
     Use logical statements together with column values to construct a boolean indicator for the event you're interested in. Remember that you can chain multiple statements with logical and `&` and or `|` operators. See the documentation for `gr.pr()` for more details and examples.
 
+    For a two-sided interval at a confidence level of ``C``, set ``alpha = 1 - C`` and use ``[gr.mean_lo(X, alpha=alpha/2), gr.mean_up(X, alpha=alpha/2)``. Note that the default ``alpha`` level for both helpers is calibrated for a two-sided interval with ``C = 0.99``.
+
     Args:
         series (pandas.Series): Column to summarize; must be boolean or 0/1.
         alpha (float): alpha-level for calculation, in (0, 1)
             Note that the confidence level C is given by C = 1 - alpha
 
     Returns:
         float: Upper confidence interval
 
-    Examples:
-        >>> import grama as gr
-        >>> DF = gr.Intention()
-        >>> ## Cantilever beam examples
-        >>> from grama.models import make_cantilever_beam
-        >>> md_beam = make_cantilever_beam()
-        >>>
-        >>> ## Estimate probabilities
-        >>> (
-        >>>     md_beam
-        >>>     # Generate large
-        >>>     >> gr.ev_sample(n=1e5, df_det="nom")
-        >>>     # Estimate probabilities with a confidence interval
-        >>>     >> gr.tf_summarize(
-        >>>         pof_lo=gr.pr_lo(DF.g_stress <= 0),
-        >>>         pof=gr.pr(DF.g_stress <= 0),
-        >>>         pof_up=gr.pr_up(DF.g_stress <= 0),
-        >>>     )
-        >>> )
+    Examples::
+
+        import grama as gr
+        DF = gr.Intention()
+        ## Cantilever beam examples
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+
+        ## Estimate probabilities
+        (
+            md_beam
+            # Generate large
+            >> gr.ev_sample(n=1e5, df_det="nom")
+            # Estimate probabilities with a confidence interval
+            >> gr.tf_summarize(
+                pof_lo=gr.pr_lo(DF.g_stress <= 0),
+                pof=gr.pr(DF.g_stress <= 0),
+                pof_up=gr.pr_up(DF.g_stress <= 0),
+            )
+        )
     """
     up = binomial_ci(series, alpha=alpha, side="up")
     return up
 
 
 @make_symbolic
 def corr(series1, series2, method="pearson", res="corr", nan_drop=False):
@@ -666,26 +718,107 @@
         return r
     if res == "both":
         return r, p
     else:
         raise ValueError("res {} not supported".format(res))
 
 
+# Distribution-free Prediction Intervals
+# --------------------------------------------------
+def pint_lo_index(n, m, j, alpha):
+    r"""PI lower bound index
+
+    Compute the order statistic index for the lower bound of a distribution-free
+    prediction interval.
+
+    """
+    l = int(n - nhypergeom.ppf(1 - alpha, m + n, n, m - j  + 1))
+    if l <= 0:
+        raise ValueError(
+            "Insufficient series length for requested `alpha` level; " +
+            "obtain more observations or choose a larger value for `alpha`."
+        )
+    return l
+
+
+def pint_up_index(n, m, j, alpha):
+    r"""PI upper bound index
+
+    Compute the order statistic index for the upper bound of a distribution-free
+    prediction interval.
+
+    """
+    u = int(nhypergeom.ppf(1 - alpha, m + n, n, j) + 1)
+    if u >= n + 1:
+        raise ValueError(
+            "Insufficient series length for requested `alpha` level; " +
+            "obtain more observations or choose a larger value for `alpha`."
+        )
+    return u
+
+
+@make_symbolic
+def pint_lo(series, m=1, j=1, alpha=0.005):
+    r"""Lower prediction interval
+
+    Compute a one-sided lower prediction interval using a distribution-free approach.
+
+    For a two-sided interval at a confidence level of ``C``, set ``alpha = 1 - C`` and use ``[gr.pint_lo(X, alpha=alpha/2), gr.pint_up(X, alpha=alpha/2)``. Note that the default ``alpha`` level for both helpers is calibrated for a two-sided interval with ``C = 0.99``.
+
+    Args:
+        series (pd.Series): Dataset to analyze
+
+    Kwargs:
+        m (int): Number of observations in future dataset (Default m=1)
+        j (int): Order statistic to target; 1 <= j <= m (Default j=1)
+        alpha (float): alpha-level for calculation, in (0, 1). Note that the confidence level C is given by ``C = 1 - alpha``.
+
+    References:
+        Hahn, Gerald J., and William Q. Meeker. Statistical intervals: a guide for practitioners. Vol. 92. John Wiley & Sons, 2011.
+
+    """
+    n = len(series)
+    l = pint_lo_index(n, m, j, alpha)
+    return series.sort_values().iloc[l - 1] # for 0-based indexing
+
+@make_symbolic
+def pint_up(series, m=1, j=1, alpha=0.005):
+    r"""Upper prediction interval
+
+    Compute a one-sided upper prediction interval using a distribution-free approach.
+
+    For a two-sided interval at a confidence level of ``C``, set ``alpha = 1 - C`` and use ``[gr.pint_lo(X, alpha=alpha/2), gr.pint_up(X, alpha=alpha/2)``. Note that the default ``alpha`` level for both helpers is calibrated for a two-sided interval with ``C = 0.99``.
+
+    Args:
+        series (pd.Series): Dataset to analyze
+
+    Kwargs:
+        m (int): Number of observations in future dataset (Default m=1)
+        j (int): Order statistic to target; 1 <= j <= m (Default j=1)
+        alpha (float): alpha-level for calculation, in (0, 1). Note that the confidence level C is given by ``C = 1 - alpha``.
+
+    References:
+        Hahn, Gerald J., and William Q. Meeker. Statistical intervals: a guide for practitioners. Vol. 92. John Wiley & Sons, 2011.
+
+    """
+    n = len(series)
+    u = pint_up_index(n, m, j, alpha)
+    return series.sort_values().iloc[u - 1] # for 0-based indexing
+
 # ------------------------------------------------------------------------------
 # Effective Sample Size helpers
 # ------------------------------------------------------------------------------
 @make_symbolic
 def neff_is(series):
     """Importance sampling n_eff
 
-    Computes the effective sample size according to Equation 9.13 of Owen
-    (2013).
+    Computes the effective sample size based on importance sampling weights. See Equation 9.13 of Owen (2013) for details. See ``gr.tran_reweight()`` for more details.
 
     Args:
-        series (pandas.Series): column to summarize.
+        series (pandas.Series): column of importance sampling weights.
 
     References:
         A.B. Owen, "Monte Carlo theory, methods and examples" (2013)
 
     """
 
     w = series.mean()
```

### Comparing `py_grama-0.3.4/grama/dfply/transform.py` & `py_grama-0.3.5/grama/dfply/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         df (pandas.DataFrame): Data to modify
 
     Kwargs:
         **kwargs: Compute new column values
             the name of the argument (left of `=`) will be the new column name,
             the value of the argument (right of `=`) defines the new column's value
 
-    Example:
+    Examples::
+
         ## Setup
         import grama as gr
         DF = gr.Intention()
         ## Load example dataset
         from grama.data import df_diamonds
 
         ## Compute a rough estimate of volume
@@ -53,15 +54,16 @@
     """
     Modifies columns in place if the specified predicate is true.
     Args:
         df (pandas.DataFrame): data passed in through the pipe.
         predicate: a function applied to columns that returns a boolean value
         fun: a function that will be applied to columns where predicate returns True
 
-    Example:
+    Examples::
+
         diamonds >> mutate_if(lambda col: min(col) < 1 and mean(col) < 4, lambda row: 2 * row) >> head(3)
            carat      cut color clarity  depth  table  price     x     y     z
         0   0.46    Ideal     E     SI2   61.5   55.0    326  3.95  3.98  4.86
         1   0.42  Premium     E     SI1   59.8   61.0    326  3.89  3.84  4.62
         2   0.46     Good     E     VS1   56.9   65.0    327  4.05  4.07  4.62
         (columns 'carat' and 'z', both having a min < 1 and mean < 4, are doubled, while the
         other rows remain as they were)
```

### Comparing `py_grama-0.3.4/grama/dfply/vector.py` & `py_grama-0.3.5/grama/dfply/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         series (:obj:`pandas.Series`): pandas series to be inverted prior to
             ordering/sorting.
 
     Returns:
         inverted `pandas.Series`. The returned series will be numeric (integers),
             regardless of the type of the original series.
 
-    Example:
+    Examples::
 
         First group by cut, then find the first value of price when ordering by
         price ascending, and ordering by price descending using the `desc` function.
 
         diamonds >> group_by(X.cut) >> summarize(carat_low=first(X.price, order_by=X.price),
                                                  carat_high=first(X.price, order_by=desc(X.price)))
 
@@ -95,15 +95,16 @@
     Takes the first non-NaN value in order across the specified series,
     returning a new series. Mimics the coalesce function in dplyr and SQL.
 
     Args:
         *series: Series objects, typically represented in their symbolic form
             (like X.series).
 
-    Example:
+    Examples::
+
         df = pd.DataFrame({
             'a':[1,np.nan,np.nan,np.nan,np.nan],
             'b':[2,3,np.nan,np.nan,np.nan],
             'c':[np.nan,np.nan,4,5,np.nan],
             'd':[6,7,8,9,np.nan]
         })
         df >> transmute(coal=coalesce(X.a, X.b, X.c, X.d))
@@ -163,15 +164,16 @@
 
     Args:
         *conditions: Each condition should be a list with two values. The first
             value is a boolean or vector of booleans that specify indices in
             which the condition is met. The second value is a vector of values
             or single value specifying the outcome where that condition is met.
 
-    Example:
+    Example::
+
         df = pd.DataFrame({
             'num':np.arange(16)
         })
         df >> mutate(strnum=case_when([X.num % 15 == 0, 'fizzbuzz'],
                                       [X.num % 3 == 0, 'fizz'],
                                       [X.num % 5 == 0, 'buzz'],
                                       [True, X.num.astype(str)]))
@@ -238,29 +240,30 @@
         condition: A boolean vector representing the condition. This is often
             a logical statement with a symbolic series.
         when_true: A vector the same length as the condition vector or a single
             value to apply when the condition is `True`.
         otherwise: A vector the same length as the condition vector or a single
             value to apply when the condition is `False`.
 
-    Example:
-        >>> import grama as gr
-        >>> from grama.data import df_diamonds
-        >>> DF = gr.Intention()
-        >>> (
-        >>>     df_diamonds
-        >>>     >> gr.tf_mutate(
-        >>>         # Recode nonsensical x values
-        >>>         x=gr.if_else(
-        >>>             DF.x == 0
-        >>>             gr.NaN,
-        >>>             DF.x,
-        >>>         )
-        >>>     )
-        >>> )
+    Example::
+
+        import grama as gr
+        from grama.data import df_diamonds
+        DF = gr.Intention()
+        (
+            df_diamonds
+            >> gr.tf_mutate(
+                # Recode nonsensical x values
+                x=gr.if_else(
+                    DF.x == 0
+                    gr.NaN,
+                    DF.x,
+                )
+            )
+        )
     """
 
     if not isinstance(when_true, collections.abc.Iterable) or isinstance(when_true, str):
         when_true = repeat(when_true, len(condition))
     if not isinstance(otherwise, collections.abc.Iterable) or isinstance(otherwise, str):
         otherwise = repeat(otherwise, len(condition))
     assert (len(condition) == len(when_true)) and (len(condition) == len(otherwise))
```

### Comparing `py_grama-0.3.4/grama/dfply/window_functions.py` & `py_grama-0.3.5/grama/dfply/window_functions.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/eval/eval_pyDOE.py` & `py_grama-0.3.5/grama/eval/eval_pyDOE.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/eval_contour.py` & `py_grama-0.3.5/grama/eval_contour.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __all__ = [
     "eval_contour",
     "ev_contour",
 ]
 
 from grama import eval_df, add_pipe, tf_outer
+from grama.eval_defaults import invariants_eval_model, invariants_eval_df
 from numpy import array, linspace, isfinite, reshape, full
 from pandas import concat, DataFrame
 from toolz import curry
 from warnings import formatwarning, catch_warnings, simplefilter, warn
 
 class Square():
     # D -- C
@@ -184,83 +185,85 @@
         df=None,
         levels=None,
         n_side=20,
         n_levels=5,
 ):
     r"""Generate contours from a model
 
-    Generates contours from a model. Evaluates the model on a dense grid, then
-    runs marching squares to generate contours. Supports targeting multiple
-    outputs and handling auxiliary inputs not included in the contour map.
+    Generates contours from a model. Evaluates the model on a dense grid, then runs marching squares to generate contours. Supports targeting multiple outputs and handling auxiliary inputs not included in the contour map.
 
     Args:
         model (gr.Model): Model to evaluate.
-        var (list of str): Model inputs to target; must provide exactly
-            two inputs, and both must have finite domain width.
+        var (list of str): Model inputs to target; must provide exactly two inputs, and both must have finite domain width.
         out (list of str): Model output(s) for contour generation.
-        df (DataFrame): Levels for model variables not included in var (auxiliary inputs).
-        levels (dict): Specific output levels for contour generation;
-            overrides n_levels.
+        df (DataFrame or None): Levels for model variables not included in var 
+            (auxiliary inputs). If provided var and model.var contain the same
+            values, then df may equal None.
+        levels (dict): Specific output levels for contour generation; overrides n_levels.
         n_side (int): Side resolution for grid; n_side**2 total evaluations.
         n_levels (int): Number of contour levels.
 
     Returns:
         DataFrame: Points along contours, organized by output and auxiliary variable levels.
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> ## Multiple outputs
-        >>> (
-        >>>     gr.Model()
-        >>>     >> gr.cp_vec_function(
-        >>>         fun=lambda df: gr.df_make(
-        >>>             f=df.x**2 + df.y**2,
-        >>>             g=df.x + df.y,
-        >>>         ),
-        >>>         var=["x", "y"],
-        >>>         out=["f", "g"],
-        >>>     )
-        >>>     >> gr.cp_bounds(
-        >>>         x=(-1, +1),
-        >>>         y=(-1, +1),
-        >>>     )
-        >>>     >> gr.ev_contour(
-        >>>         var=["x", "y"],
-        >>>         out=["f", "g"],
-        >>>     )
-        >>>     # Contours with no auxiliary variables can autoplot
-        >>>     >> gr.pt_auto()
-        >>> )
-        >>> ## Auxiliary inputs
-        >>> (
-        >>>     gr.Model()
-        >>>     >> gr.cp_vec_function(
-        >>>         fun=lambda df: gr.df_make(
-        >>>             f=df.c * df.x + (1 - df.c) * df.y,
-        >>>         ),
-        >>>         var=["x", "y"],
-        >>>         out=["f", "g"],
-        >>>     )
-        >>>     >> gr.cp_bounds(
-        >>>         x=(-1, +1),
-        >>>         y=(-1, +1),
-        >>>     )
-        >>>     >> gr.ev_contour(
-        >>>         var=["x", "y"],
-        >>>         out=["f"],
-        >>>         df=gr.df_make(c=[0, 1])
-        >>>     )
-        >>>
-        >>>     >> gr.ggplot(gr.aes("x", "y"))
-        >>>     + gr.geom_segment(gr.aes(xend="x_end", yend="y_end", group="level", color="c"))
-        >>> )
+        import grama as gr
+        ## Multiple outputs
+        (
+            gr.Model()
+            >> gr.cp_vec_function(
+                fun=lambda df: gr.df_make(
+                    f=df.x**2 + df.y**2,
+                    g=df.x + df.y,
+                ),
+                var=["x", "y"],
+                out=["f", "g"],
+            )
+            >> gr.cp_bounds(
+                x=(-1, +1),
+                y=(-1, +1),
+            )
+            >> gr.ev_contour(
+                var=["x", "y"],
+                out=["f", "g"],
+            )
+            # Contours with no auxiliary variables can autoplot
+            >> gr.pt_auto()
+        )
+
+        ## Auxiliary inputs
+        (
+            gr.Model()
+            >> gr.cp_vec_function(
+                fun=lambda df: gr.df_make(
+                    f=df.c * df.x + (1 - df.c) * df.y,
+                ),
+                var=["x", "y"],
+                out=["f", "g"],
+            )
+            >> gr.cp_bounds(
+                x=(-1, +1),
+                y=(-1, +1),
+            )
+            >> gr.ev_contour(
+                var=["x", "y"],
+                out=["f"],
+                df=gr.df_make(c=[0, 1])
+            )
+
+            # Contours with auxiliary variables should be manually plotted
+            >> gr.ggplot(gr.aes("x", "y"))
+            + gr.geom_segment(gr.aes(xend="x_end", yend="y_end", group="level", color="c"))
+        )
 
     """
     ## Check invariants
+    invariants_eval_model(model)
+    invariants_eval_df(df, acc_none=True)
     # Argument given
     if var is None:
         raise ValueError("No `var` given")
     # Correct number of inputs
     if len(var) != 2:
         raise ValueError("Must provide exactly 2 inputs in `var`.")
     # Inputs available
@@ -273,14 +276,18 @@
     var_diff = set(model.var).difference(set(var))
     if len(var_diff) > 0:
         if df is None:
             raise ValueError(
                 "Must provide values for remaining model variables using df; " +
                 "missing values: {}".format(var_diff)
             )
+        # Drop the swept variables
+        df = df.drop(columns=var, errors="ignore")
+
+        # Check for unsupported inputs
         var_diff2 = var_diff.difference(set(df.columns))
         if len(var_diff2) > 0:
             raise ValueError(
                 "All model variables need values in provided df; " +
                 "missing values: {}".format(var_diff2)
             )
```

### Comparing `py_grama-0.3.4/grama/eval_defaults.py` & `py_grama-0.3.5/grama/tran_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,425 +1,449 @@
 __all__ = [
-    "eval_df",
-    "ev_df",
-    "eval_nominal",
-    "ev_nominal",
-    "eval_grad_fd",
-    "ev_grad_fd",
-    "eval_sample",
-    "ev_sample",
-    "eval_conservative",
-    "ev_conservative",
+    "tran_angles",
+    "tf_angles",
+    "tran_bootstrap",
+    "tf_bootstrap",
+    "tran_copula_corr",
+    "tf_copula_corr",
+    "tran_kfolds",
+    "tf_kfolds",
+    "tran_md",
+    "tf_md",
 ]
 
-import itertools
-from grama import add_pipe, tran_outer, custom_formatwarning
+from grama import add_pipe, pipe, copy_meta, Intention, mse, rsq, mead
+from grama import (
+    tf_bind_cols,
+    tf_filter,
+    tf_summarize,
+    tf_drop,
+    tf_mutate,
+    var_in,
+    ev_df,
+)
+from collections import ChainMap
 from numbers import Integral
-from numpy import ones, eye, tile, atleast_2d
+from numpy import arange, ceil, zeros, std, quantile, nan, triu_indices, unique
+from numpy.random import choice, permutation
 from numpy.random import seed as set_seed
-from pandas import DataFrame, concat
+from pandas import concat, DataFrame, melt
+from pandas.api.types import is_numeric_dtype
+from scipy.linalg import subspace_angles
+from scipy.stats import norm
+from .string_helpers import str_detect, str_replace
 from toolz import curry
-from warnings import formatwarning, catch_warnings, simplefilter
 
-formatwarning = custom_formatwarning
+X = Intention()
 
-## Default evaluation function
+
+## k-Fold CV utility
 # --------------------------------------------------
 @curry
-def eval_df(model, df=None, append=True, verbose=True):
-    r"""Evaluate model at given values
+def tran_kfolds(
+    df,
+    k=None,
+    ft=None,
+    out=None,
+    var_fold=None,
+    suffix="_mean",
+    summaries=None,
+    tf=tf_summarize,
+    shuffle=True,
+    seed=None,
+):
+    r"""Perform k-fold CV
 
-    Evaluates a given model at a given dataframe.
+    Perform k-fold cross-validation (CV) using a given fitting procedure (ft). Optionally provide a fold identifier column, or (randomly) assign folds.
 
     Args:
-        model (gr.Model): Model to evaluate
-        df (DataFrame): Input dataframe to evaluate
-        append (bool): Append results to original dataframe?
+        df (DataFrame): Data to pass to given fitting procedure
+        ft (gr.ft_): Partially-evaluated grama fit function; defines model fitting
+            procedure and outputs to aggregate
+        tf (gr.tf_): Partially-evaluated grama transform function; evaluation of
+            fitted model will be passed to tf and provided with keyword arguments
+            from summaries
+        out (list or None): Outputs for which to compute `summaries`; None uses ft.out
+        var_fold (str or None): Column to treat as fold identifier; overrides `k`
+        suffix (str): Suffix for predicted value; used to distinguish between predicted and actual
+        summaries (dict of functions): Summary functions to pass to tf; will be evaluated
+            for outputs of ft. Each summary must have signature summary(f_pred, f_meas).
+            Grama includes builtin options: gr.mse, gr.rmse, gr.rel_mse, gr.rsq, gr.ndme
+        k (int): Number of folds; k=5 to k=10 recommended [1]
+        shuffle (bool): Shuffle the data before CV? True recommended [1]
+
+    Notes:
+        - Many grama functions support *partial evaluation*; this allows one to specify things like hyperparameters in fitting functions without providing data and executing the fit. You can take advantage of this functionality to easly do hyperparameter studies.
 
     Returns:
-        DataFrame: Results of model evaluation
+        DataFrame: Aggregated results within each of k-folds using given model and
+            summary transform
+
+    References:
+        [1] James, Witten, Hastie, and Tibshirani, "An introduction to statistical learning" (2017), Chapter 5. Resampling Methods
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.models import make_test
-        >>> md = make_test()
-        >>> df = gr.df_make(x0=0, x1=1, x2=2)
-        >>> md >> gr.ev_df(df=df)
+        import grama as gr
+        from grama.data import df_stang
+        df_kfolds = (
+            df_stang
+            >> gr.tf_kfolds(
+                k=5,
+                ft=gr.ft_rf(out=["thick"], var=["E", "mu"]),
+            )
+        )
 
     """
-    if df is None:
-        raise ValueError("No input df given")
-    if len(model.functions) == 0:
-        raise ValueError("Given model has no functions")
-    out_intersect = set(df.columns).intersection(model.out)
-    if (len(out_intersect) > 0) and verbose:
-        print(
-            "... provided columns intersect model output.\n"
-            + "eval_df() is dropping {}".format(out_intersect)
+    ## Check invariants
+    if ft is None:
+        raise ValueError("Must provide ft keyword argument")
+    if (k is None) and (var_fold is None):
+        print("... tran_kfolds is using default k=5")
+        k = 5
+    if summaries is None:
+        print("... tran_kfolds is using default summaries mse, mead, and rsq")
+        summaries = dict(mse=mse, mead=mead, rsq=rsq)
+
+    n = df.shape[0]
+    ## Handle custom folds
+    if not (var_fold is None):
+        ## Check for a valid var_fold
+        if not (var_fold in df.columns):
+            raise ValueError("var_fold must be in df.columns or None")
+        ## Build folds
+        levels = unique(df[var_fold])
+        k = len(levels)
+        print("... tran_kfolds found {} levels via var_folds".format(k))
+        Is = []
+        for l in levels:
+            Is.append(list(arange(n)[df[var_fold] == l]))
+
+    else:
+        ## Shuffle data indices
+        if shuffle:
+            if seed:
+                set_seed(seed)
+            I = permutation(n)
+        else:
+            I = arange(n)
+        ## Build folds
+        di = int(ceil(n / k))
+        Is = [I[i * di : min((i + 1) * di, n)] for i in range(k)]
+
+    ## Iterate over folds
+    df_res = DataFrame()
+    for i in range(k):
+        ## Train by out-of-fold data
+        md_fit = df >> tf_filter(~var_in(X.index, Is[i])) >> ft
+
+        ## Determine predicted and actual
+        if out is None:
+            out = str_replace(md_fit.out, suffix, "")
+        else:
+            out = str_replace(out, suffix, "")
+
+        ## Test by in-fold data
+        df_pred = md_fit >> ev_df(
+            df=df >> tf_filter(var_in(X.index, Is[i])), append=False
         )
 
-    df_res = model.evaluate_df(df)
+        ## Specialize summaries for output names
+        summaries_all = ChainMap(
+            *[
+                {
+                    key + "_" + o: fun(X[o + suffix], X[o])
+                    for key, fun in summaries.items()
+                }
+                for o in out
+            ]
+        )
 
-    if append:
-        df_res = concat(
-            [
-                df.reset_index(drop=True).drop(model.out, axis=1, errors="ignore"),
-                df_res,
-            ],
-            axis=1,
+        ## Aggregate
+        df_summary_tmp = (
+            df_pred
+            >> tf_bind_cols(df[out] >> tf_filter(var_in(X.index, Is[i])))
+            >> tf(**summaries_all)
+            # >> tf_mutate(_kfold=i)
         )
 
+        if var_fold is None:
+            df_summary_tmp = df_summary_tmp >> tf_mutate(_kfold=i)
+        else:
+            df_summary_tmp[var_fold] = levels[i]
+
+        df_res = concat((df_res, df_summary_tmp), axis=0).reset_index(drop=True)
+
     return df_res
 
 
-ev_df = add_pipe(eval_df)
+tf_kfolds = add_pipe(tran_kfolds)
 
-## Nominal evaluation
+## Bootstrap utility
 # --------------------------------------------------
 @curry
-def eval_nominal(model, df_det=None, append=True, skip=False):
-    r"""Evaluate model at nominal values
+def tran_bootstrap(
+    df, tran=None, n_boot=500, n_sub=25, con=0.90, col_sel=None, seed=None
+):
+    r"""Estimate bootstrap confidence intervals
 
-    Evaluates a given model at a model nominal conditions (median).
+    Estimate bootstrap confidence intervals for a given transform. Uses the
+    "bootstrap-t" procedure discussed in Efron and Tibshirani (1993).
 
     Args:
-        model (gr.Model): Model to evaluate
-        df_det (DataFrame): Deterministic levels for evaluation; use "nom"
-            for nominal deterministic levels.
-        append (bool): Append results to nominal inputs?
-        skip (bool): Skip evaluation of the functions?
+        df (DataFrame): Data to bootstrap
+        tran (grama tran_ function): Transform procedure which generates statistic
+        n_boot (numeric): Monte Carlo resamples for bootstrap
+        n_sub (numeric): Nested resamples to estimate SE
+        con (float): Confidence level
+        col_sel (list(string)): Columns to include in bootstrap calculation
 
     Returns:
-        DataFrame: Results of nominal model evaluation or unevaluated design
+        DataFrame: Results of tran(df), plus _lo and _up columns for
+        numeric columns
 
-    Examples:
+    References and notes:
+       Efron and Tibshirani (1993) "The bootstrap-t procedure... is
+       particularly applicable to location statistics like the sample mean....
+       The bootstrap-t method, at least in its simple form, cannot be trusted
+       for more general problems, like setting a confidence interval for a
+       correlation coefficient."
 
-        >>> import grama as gr
-        >>> from grama.models import make_test
-        >>> md = make_test()
-        >>> md >> gr.ev_nominal(df_det="nom")
+    Examples::
 
     """
-    ## Draw from underlying gaussian
-    quantiles = ones((1, model.n_var_rand)) * 0.5  # Median
+    ## Set seed only if given
+    if seed is not None:
+        set_seed(seed)
+
+    ## Ensure sample count is int
+    if not isinstance(n_boot, Integral):
+        print("tran_bootstrap() is rounding n_boot...")
+        n_boot = int(n_boot)
+    if not isinstance(n_sub, Integral):
+        print("tran_bootstrap() is rounding n_sub...")
+        n_sub = int(n_sub)
+
+    ## Base results
+    df_base = tran(df)
+
+    ## Select columns for bootstrap
+    col_numeric = list(df_base.select_dtypes(include="number").columns)
+    if not (col_sel is None):
+        col_numeric = list(set(col_numeric).intersection(set(col_sel)))
+
+    ## Setup
+    n_samples = df.shape[0]
+    n_row = df_base.shape[0]
+    n_col = len(col_numeric)
+    alpha = (1 - con) / 2
+    theta_hat = df_base[col_numeric].values
+
+    theta_all = zeros((n_boot, n_row, n_col))
+    se_boot_all = zeros((n_boot, n_row, n_col))
+    z_all = zeros((n_boot, n_row, n_col))
+    theta_sub = zeros((n_sub, n_row, n_col))
+
+    ## Main loop
+    for ind in range(n_boot):
+        ## Construct resample
+        Ib = choice(n_samples, size=n_samples, replace=True)
+        df_tmp = copy_meta(df, df.iloc[Ib,])
+        theta_all[ind] = tran(df_tmp)[col_numeric].values
+
+        ## Internal loop to approximate SE
+        for jnd in range(n_sub):
+            Isub = Ib[choice(n_samples, size=n_samples, replace=True)]
+            df_tmp = copy_meta(df, df.iloc[Isub,])
+            theta_sub[jnd] = tran(df_tmp)[col_numeric].values
+        se_boot_all[ind] = std(theta_sub, axis=0)
+
+        ## Construct approximate pivot
+        z_all[ind] = (theta_all[ind] - theta_hat) / se_boot_all[ind]
+
+    ## Compute bootstrap table
+    t_lo, t_hi = quantile(z_all, q=[1 - alpha, alpha], axis=0)
+
+    ## Estimate bootstrap intervals
+    se = std(theta_all, axis=0)
+    theta_lo = theta_hat - t_lo * se
+    theta_hi = theta_hat - t_hi * se
+
+    ## Assemble output data
+    col_lo = list(map(lambda s: s + "_lo", col_numeric))
+    col_hi = list(map(lambda s: s + "_up", col_numeric))
+
+    df_lo = DataFrame(data=theta_lo, columns=col_lo)
+    df_hi = DataFrame(data=theta_hi, columns=col_hi)
+
+    df_ci = concat((df_lo, df_hi), axis=1).sort_index(axis=1)
+    df_ci.index = df_base.index
 
-    ## Convert samples to desired marginals
-    df_pr = DataFrame(data=quantiles, columns=model.var_rand)
-    df_rand = model.density.pr2sample(df_pr)
-    ## Construct outer-product DOE
-    df_samp = model.var_outer(df_rand, df_det=df_det)
+    return concat((df_base, df_ci), axis=1)
 
-    if skip:
-        return df_samp
-    return eval_df(model, df=df_samp, append=append)
 
+tf_bootstrap = add_pipe(tran_bootstrap)
 
-ev_nominal = add_pipe(eval_nominal)
 
-## Gradient finite-difference evaluation
+## Assess subspace angles
 # --------------------------------------------------
-@curry
-def eval_grad_fd(model, h=1e-8, df_base=None, var=None, append=True, skip=False):
-    r"""Finite-difference gradient approximation
+def tran_angles(df, df2):
+    r"""Subspace angles
 
-    Evaluates a given model with a central-difference stencil to approximate the
-    gradient.
+    Compute the subspace angles between two matrices. A wrapper for scipy.linalg.subspace_angles that corrects for column ordering. Row ordering is assumed.
 
     Args:
-        model (gr.Model): Model to differentiate
-        h (numeric): finite difference stepsize,
-            single (scalar): or per-input (array)
-        df_base (DataFrame): Base-points for gradient calculations
-        var (list(str) or string): list of variables to differentiate,
-            or flag; "rand" for var_rand, "det" for var_det
-        append (bool): Append results to base point inputs?
-        skip (bool): Skip evaluation of the functions?
+        df (DataFrame): First matrix to compare
+        df2 (DataFrame): Second matrix to compare
 
     Returns:
-        DataFrame: Gradient approximation or unevaluated design
-
-    @pre (not isinstance(h, collections.Sequence)) |
-         (h.shape[0] == df_base.shape[1])
+        array: Array of angles (in radians)
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.models import make_cantilever_beam
-        >>> md = make_cantilever_beam()
-        >>> df_nom = md >> gr.ev_nominal(df_det="nom")
-        >>> df_grad = md >> gr.ev_grad_fd(df_base=df_nom)
-        >>> df_grad >> gr.tf_gather("var", "val", gr.everything())
+        import grama as gr
+        import pandas as pd
+        df = pd.DataFrame(dict(v=[+1, +1]))
+        df_v1 = pd.DataFrame(dict(w=[+1, -1]))
+        df_v2 = pd.DataFrame(dict(w=[+1, +1]))
+        theta1 = angles(df, df_v1)
+        theta2 = angles(df, df_v2)
 
     """
-    ## Check invariants
-    if not set(model.var).issubset(set(df_base.columns)):
-        raise ValueError("model.var must be subset of df_base.columns")
-    if var is None:
-        var = model.var
-    elif isinstance(var, str):
-        if var == "rand":
-            var = model.var_rand
-        elif var == "det":
-            var = model.var_det
-        else:
-            raise ValueError("var flag not recognized; use 'rand' or 'det'")
-    else:
-        if not set(var).issubset(set(model.var)):
-            raise ValueError("var must be subset of model.var")
-    var_fix = list(set(model.var).difference(set(var)))
-
-    ## TODO
-    if skip == True:
-        raise NotImplementedError("skip not implemented")
-
-    ## Build stencil
-    n_var = len(var)
-    stencil = eye(n_var) * h
-    stepscale = tile(atleast_2d(0.5 / h).T, (1, model.n_out))
-
-    outputs = model.out
-    nested_labels = [
-        list(map(lambda s_out: "D" + s_out + "_D" + s_var, outputs)) for s_var in var
-    ]
-    grad_labels = list(itertools.chain.from_iterable(nested_labels))
-
-    ## Loop over df_base
-    results = []  # TODO: Preallocate?
-    for row_i in range(df_base.shape[0]):
-        ## Evaluate
-        df_left = eval_df(
-            model,
-            tran_outer(
-                DataFrame(
-                    columns=var, data=-stencil + df_base[var].iloc[[row_i]].values
-                ),
-                df_base[var_fix].iloc[[row_i]],
-            ),
-            append=False,
-        )
-
-        df_right = eval_df(
-            model,
-            tran_outer(
-                DataFrame(
-                    columns=var, data=+stencil + df_base[var].iloc[[row_i]].values
-                ),
-                df_base[var_fix].iloc[[row_i]],
-            ),
-            append=False,
-        )
+    ## Compute subspace angles
+    A1 = df.values
+    A2 = df2.values
 
-        ## Compute differences
-        res = (stepscale * (df_right[outputs] - df_left[outputs]).values).flatten()
-        df_grad = DataFrame(columns=grad_labels, data=[res])
+    return subspace_angles(A1, A2)
 
-        results.append(df_grad)
 
-    return concat(results).reset_index(drop=True)
+tf_angles = add_pipe(tran_angles)
 
 
-ev_grad_fd = add_pipe(eval_grad_fd)
-
-## Conservative quantile evaluation
+## Compute Gaussian copula correlations from data
 # --------------------------------------------------
-@curry
-def eval_conservative(model, quantiles=None, df_det=None, append=True, skip=False):
-    r"""Evaluates a given model at conservative input quantiles
+def tran_copula_corr(df, model=None, density=None):
+    r"""Compute Gaussian copula correlations from data
+
+    Convenience function to fit a Gaussian copula (correlations) based on data and pre-fitted marginals. Intended for use with ``gr.comp_copula_gaussian()``. Must provide either `model` or `density`.
 
-    Uses model specifications to determine the "conservative" direction
-    for each input, and evaluates the model at the desired quantile.
-    Provided primarily for comparing UQ against pseudo-deterministic
-    design criteria.
-
-    Note that if there is no conservative direction for the given input,
-    the given quantile will be ignored and the median will automatically
-    be selected.
+    Note: This is called automatically when you provide a dataset to ``gr.comp_copula_gaussian()``.
 
     Args:
-        model (gr.Model): Model to evaluate
-        quantiles (numeric): lower quantile value(s) for conservative
-            evaluation; can be single value for all inputs, array
-            of values for each random variable, or None for default 0.01.
-            values in [0, 0.5]
-        df_det (DataFrame): Deterministic levels for evaluation; use "nom"
-            for nominal deterministic levels.
-        append (bool): Append results to conservative inputs?
-        skip (bool): Skip evaluation of the functions?
+        df (DataFrame): Matrix of data for correlation estimation
+        model (gr.Model): Model with defined marginals
+        density (gr.Density): Density with defined marginals
 
     Returns:
-        DataFrame: Conservative evaluation or unevaluated design
+        DataFrame: Correlation data ready for use with ``gr.comp_copula_gaussian()``
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.models import make_plate_buckle
-        >>> md = make_plate_buckle()
-        >>> md >> gr.ev_conservative(df_det="nom")
+        import grama as gr
+        from grama.data import df_stang
+        ## Verbose, manual approach
+        md = (
+            gr.Model()
+            >> gr.cp_marginals(
+                E=gr.marg_named(df_stang.E, "norm"),
+                mu=gr.marg_named(df_stang.mu, "beta"),
+                thick=gr.marg_named(df_stang.thick, "norm"),
+            )
+        )
+        df_corr = gr.tran_copula_corr(df_stang, model=md)
+        md = gr.comp_copula_gaussian(md, df_corr=df_corr)
+
+        ## Automatic approach
+        md = (
+            gr.Model()
+            >> gr.cp_marginals(
+                E=gr.marg_named(df_stang.E, "norm"),
+                mu=gr.marg_named(df_stang.mu, "beta"),
+                thick=gr.marg_named(df_stang.thick, "norm"),
+            )
+            >> gr.cp_copula_gaussian(df_data=df_stang)
+        )
 
     """
-    ## Default behavior
-    if quantiles is None:
-        print("eval_conservative() using quantile default 0.01;")
-        print("provide `quantiles` keyword for non-default behavior.")
-        quantiles = [0.01] * model.n_var_rand
-
-    ## Handle scalar vs vector quantiles
-    try:
-        len(quantiles)
-    except TypeError:
-        quantiles = [quantiles] * model.n_var_rand
-
-    ## Modify quantiles for conservative directions
-    quantiles = [
-        0.5 + (0.5 - quantiles[i]) * model.density.marginals[model.var_rand[i]].sign
-        for i in range(model.n_var_rand)
-    ]
-    quantiles = atleast_2d(quantiles)
-
-    ## Draw samples
-    df_pr = DataFrame(data=quantiles, columns=model.var_rand)
-    ## Convert samples to desired marginals
-    df_rand = model.density.pr2sample(df_pr)
-    ## Construct outer-product DOE
-    df_samp = model.var_outer(df_rand, df_det=df_det)
-
-    if skip:
-        return df_samp
-    return eval_df(model, df=df_samp, append=append)
+    if density is None:
+        density = model.density
 
+    ## Check invariants
+    if not set(density.marginals.keys()).issubset(set(df.columns)):
+        raise ValueError("df must have columns for all var_rand")
 
-ev_conservative = add_pipe(eval_conservative)
+    ## Convert data
+    df_res = density.sample2pr(df)
+    df_norm = df_res.apply(norm.ppf)
 
-## Random sampling
+    ## Compute correlations
+    df_mat = df_norm.corr()
+    Ind = triu_indices(len(density.marginals), 1)
+
+    ## Arrange
+    var_rand = df_mat.columns
+    var1_all = []
+    var2_all = []
+    corr_all = []
+
+    for i, j in zip(Ind[0], Ind[1]):
+        var1_all.append(var_rand[i])
+        var2_all.append(var_rand[j])
+        corr_all.append(df_mat.iloc[i, j])
+
+    return DataFrame(dict(var1=var1_all, var2=var2_all, corr=corr_all))
+
+
+tf_copula_corr = add_pipe(tran_copula_corr)
+
+## Model as transform
 # --------------------------------------------------
 @curry
-def eval_sample(model, n=None, df_det=None, seed=None, append=True, skip=False):
-    r"""Draw a random sample
+def tran_md(df, md=None, append=True):
+    r"""Model as transform
 
-    Evaluates a model with a random sample of the random model inputs. Generates outer product with deterministic samples.
-
-    For more expensive models, it can be helpful to tune n to achieve a reasonable runtime. An even more effective approach is to use skip evaluation along with tran_sp() to evaluate a small, representative sample. (See examples below.)
+    Use a model to transform data; useful when pre-processing data to evaluate a model.
 
     Args:
-        model (gr.Model): Model to evaluate
-        n (numeric): number of observations to draw
-        df_det (DataFrame): Deterministic levels for evaluation; use "nom"
-            for nominal deterministic levels.
-        seed (int): random seed to use
-        append (bool): Append results to input values?
-        skip (bool): Skip evaluation of the functions?
+        df (DataFrame): Data to merge
+        md (gr.Model): Model to use as transform
 
     Returns:
-        DataFrame: Results of evaluation or unevaluated design
-
-    Examples:
+        DataFrame: Output of evaluated model
 
-        >>> import grama as gr
-        >>> from grama.models import make_test
-        >>> DF = gr.Intention()
-        >>>
-        >>> # Simple random sample evaluation
-        >>> md = make_test()
-        >>> df = md >> gr.ev_sample(n=1e2, df_det="nom")
-        >>> df.describe()
-        >>>
-        >>> ## Use autoplot to visualize results
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sample(n=1e2, df_det="nom")
-        >>>     >> gr.pt_auto()
-        >>> )
-        >>>
-        >>> ## Cantilever beam examples
-        >>> from grama.models import make_cantilever_beam
-        >>> md_beam = make_cantilever_beam()
-        >>>
-        >>> ## Use iocorr to generate input/output correlation tile plot
-        >>> (
-        >>>     md_beam
-        >>>     >> gr.ev_sample(n=1e3, df_det="nom", skip=True)
-        >>>     # Generate input/output correlation summary
-        >>>     >> gr.tf_iocorr()
-        >>>     # Visualize
-        >>>     >> gr.pt_auto()
-        >>> )
-        >>>
-        >>> ## Use support points to reduce model runtime
-        >>> (
-        >>>     md_beam
-        >>>     # Generate large input sample but don't evaluate outputs
-        >>>     >> gr.ev_sample(n=1e5, df_det="nom", skip=True)
-        >>>     # Reduce to a smaller---but representative---sample
-        >>>     >> gr.tf_sp(n=50)
-        >>>     # Evaluate the outputs
-        >>>     >> gr.tf_md(md_beam)
-        >>> )
-        >>>
-        >>> ## Estimate probabilities
-        >>> (
-        >>>     md_beam
-        >>>     # Generate large
-        >>>     >> gr.ev_sample(n=1e5, df_det="nom")
-        >>>     # Estimate probabilities of failure
-        >>>     >> gr.tf_summarize(
-        >>>         pof_stress=gr.mean(DF.g_stress <= 0),
-        >>>         pof_disp=gr.mean(DF.g_disp <= 0),
-        >>>     )
-        >>> )
+    Examples::
 
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        ## Use support points to generate a smaller---but representative---sample
+        df_res = (
+            md_beam
+            >> gr.ev_sample(n=1e3, df_det="nom", skip=True, seed=101)
+            >> gr.tf_sp(n=100)
+            >> gr.tf_md(md=md_beam)
+        )
 
     """
-    ## Check invariants
-    if n is None:
-        raise ValueError("Must provide a valid n value.")
-
-    ## Set seed only if given
-    if seed is not None:
-        set_seed(seed)
+    if md is None:
+        raise ValueError("No input md given")
+    if len(md.functions) == 0:
+        raise ValueError("Given model has no functions")
+    out_intersect = set(df.columns).intersection(md.out)
+    if len(out_intersect) > 0:
+        print(
+            "... provided columns intersect model output.\n"
+            + "tran_md() is dropping {}".format(out_intersect)
+        )
 
-    ## Ensure sample count is int
-    if not isinstance(n, Integral):
-        print("eval_sample() is rounding n...")
-        n = int(n)
-
-    ## Draw samples
-    df_rand = model.density.sample(n=n, seed=seed)
-    ## Construct outer-product DOE
-    df_samp = model.var_outer(df_rand, df_det=df_det)
-
-    if skip:
-        ## Evaluation estimate
-        runtime_est = model.runtime(df_samp.shape[0])
-        if runtime_est > 0:
-            print(
-                "Estimated runtime for design with model ({0:1}):\n  {1:4.3} sec".format(
-                    model.name, runtime_est
-                )
-            )
-        else:
-            print("Design runtime estimates unavailable; model has no timing data.")
+    df_res = md.evaluate_df(df)
 
-        ## Attach metadata
-        with catch_warnings():
-            simplefilter("ignore")
-            df_samp._plot_info = {
-                "type": "sample_inputs",
-                "var": model.var_rand,
-            }
-
-        return df_samp
-
-    df_res = eval_df(model, df=df_samp, append=append)
-    ## Attach metadata
-    with catch_warnings():
-        simplefilter("ignore")
-        df_res._plot_info = {
-            "type": "sample_outputs",
-            "var": model.var,
-            "out": model.out,
-        }
+    if append:
+        df_res = concat(
+            [df.reset_index(drop=True).drop(md.out, axis=1, errors="ignore"), df_res,],
+            axis=1,
+        )
 
     return df_res
 
 
-ev_sample = add_pipe(eval_sample)
+tf_md = add_pipe(tran_md)
```

### Comparing `py_grama-0.3.4/grama/eval_opt.py` & `py_grama-0.3.5/grama/eval_opt.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "eval_min",
     "ev_min",
 ]
 
 from grama import add_pipe, pipe, custom_formatwarning, df_make, \
     eval_df, eval_nominal, eval_sample, comp_marginals, \
     comp_copula_independence, tran_outer
+from grama.eval_defaults import invariants_eval_model, invariants_eval_df
 from numpy import Inf, isfinite
 from numpy.random import seed as setseed
 from pandas import DataFrame, concat
 from scipy.optimize import minimize
 from toolz import curry
 
 
@@ -45,41 +46,48 @@
             variables may have semi-infinite bounds.
         df_data (DataFrame): Data for estimating parameters. Variables not
             found in df_data optimized in fitting.
         out (list or None): Output contributions to consider in computing MSE.
             Assumed to be model.out if left as None.
         var_fix (list or None): Variables to fix to nominal levels. Note that
             variables with domain width zero will automatically be fixed.
-        df_init (DataFrame): Initial guesses for parameters; overrides n_restart
+        df_init (DataFrame or None): Initial guesses for parameters; overrides 
+        n_restart
         append (bool): Append metadata? (Initial guess, MSE, optimizer status)
         tol (float): Optimizer convergence tolerance
         n_maxiter (int): Optimizer maximum iterations
         n_restart (int): Number of restarts; beyond n_restart=1 random
             restarts are used.
         seed (int OR None): Random seed for restarts
         verbose (bool): Print messages to console?
 
     Returns:
         DataFrame: Results of estimation
 
-    Examples:
-        >>> import grama as gr
-        >>> from grama.data import df_trajectory_full
-        >>> from grama.models import make_trajectory_linear
-        >>>
-        >>> md_trajectory = make_trajectory_linear()
-        >>>
-        >>> df_fit = (
-        >>>     md_trajectory
-        >>>     >> gr.ev_nls(df_data=df_trajectory_full)
-        >>> )
-        >>>
-        >>> print(df_fit)
+    Examples::
+
+        import grama as gr
+        from grama.data import df_trajectory_full
+        from grama.models import make_trajectory_linear
+
+        md_trajectory = make_trajectory_linear()
+
+        df_fit = (
+            md_trajectory
+            >> gr.ev_nls(df_data=df_trajectory_full)
+        )
+
+        print(df_fit)
 
     """
+    ## Common invariant checks
+    invariants_eval_model(model)
+    invariants_eval_df(df_data, arg_name="df_data")
+    invariants_eval_df(df_init, arg_name="df_init", acc_none=True)
+
     ## Check `out` invariants
     if out is None:
         out = model.out
         if verbose:
             print("... eval_nls setting out = {}".format(out))
     set_diff = set(out).difference(set(df_data.columns))
     if len(set_diff) > 0:
@@ -279,44 +287,52 @@
             restarts are used.
         df_start (None or DataFrame): Specific starting values to use; overrides
             n_restart if non None provided.
 
     Returns:
         DataFrame: Results of optimization
 
-    Examples:
-        >>> import grama as gr
-        >>> md = (
-        >>>     gr.Model("Constrained Rosenbrock")
-        >>>     >> gr.cp_function(
-        >>>         fun=lambda x: (1 - x[0])**2 + 100*(x[1] - x[0]**2)**2,
-        >>>         var=["x", "y"],
-        >>>         out=["c"],
-        >>>     )
-        >>>     >> gr.cp_function(
-        >>>         fun=lambda x: (x[0] - 1)**3 - x[1] + 1,
-        >>>         var=["x", "y"],
-        >>>         out=["g1"],
-        >>>     )
-        >>>     >> gr.cp_function(
-        >>>         fun=lambda x: x[0] + x[1] - 2,
-        >>>         var=["x", "y"],
-        >>>         out=["g2"],
-        >>>     )
-        >>>     >> gr.cp_bounds(
-        >>>         x=(-1.5, +1.5),
-        >>>         y=(-0.5, +2.5),
-        >>>     )
-        >>> )
-        >>> md >> gr.ev_min(
-        >>>     out_min="c",
-        >>>     out_leq=["g1", "g2"]
-        >>> )
+    Examples::
+
+        import grama as gr
+        ## Define a model with objective and constraints
+        md = (
+            gr.Model("Constrained Rosenbrock")
+            >> gr.cp_function(
+                fun=lambda x: (1 - x[0])**2 + 100*(x[1] - x[0]**2)**2,
+                var=["x", "y"],
+                out=["c"],
+            )
+            >> gr.cp_function(
+                fun=lambda x: (x[0] - 1)**3 - x[1] + 1,
+                var=["x", "y"],
+                out=["g1"],
+            )
+            >> gr.cp_function(
+                fun=lambda x: x[0] + x[1] - 2,
+                var=["x", "y"],
+                out=["g2"],
+            )
+            >> gr.cp_bounds(
+                x=(-1.5, +1.5),
+                y=(-0.5, +2.5),
+            )
+        )
+
+        ## Run the optimizer
+        md >> gr.ev_min(
+            out_min="c",
+            out_leq=["g1", "g2"]
+        )
 
     """
+    ## Common invariant checks
+    invariants_eval_model(model)
+    invariants_eval_df(df_start, arg_name="df_start", acc_none=True)
+
     ## Check that model has only deterministic variables
     if model.n_var_rand > 0:
         raise ValueError("model must have no random variables")
     ## Check that objective is in model
     if not (out_min in model.out):
         raise ValueError("model must contain out_min")
     ## Check that constraints are in model
```

### Comparing `py_grama-0.3.4/grama/eval_pnd.py` & `py_grama-0.3.5/grama/eval_pnd.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     "make_proposal_sigma",
     "rprop",
     "dprop",
     "approx_pnd"
 ]
 
 from grama import add_pipe, Model, tf_md
+from grama.eval_defaults import invariants_eval_df, invariants_eval_model
 
 from numpy import array, diag, dot, ones, mean, zeros
 from numpy import any as npany
 from numpy import all as npall
 from numpy import min as npmin
 from numpy import max as npmax
 from numpy import sum as npsum
@@ -24,18 +25,17 @@
 from scipy.stats import multivariate_normal as mvnorm
 from toolz import curry
 
 
 @curry
 def eval_pnd(model, df_train, df_test, signs, n=int(1e4), seed=None, append=True, \
     mean_prefix="_mean", sd_prefix="_sd"):
-    """ Evaluate a Model using a predictive model
+    """Approximate the probability non-dominated (PND)
 
-    Evaluates a given model against a PND algorithm to determine
-    "optimal points".
+    Approximates the probability non-dominated (PND) for a set of training points given a fitted probabilistic model. Used to rank a set of candidates in the context of multiobjective optimization.
 
     Args:
         model (gr.model): predictive model to evaluate
         df_train (DataFrame): dataframe with training data
         df_test (DataFrame): dataframe with test data
         signs (dict): dict with the variables you would like to use and
             minimization or maximization parameter for each
@@ -45,74 +45,71 @@
         n (int): Number of draws for importance sampler
         seed (int): declarble seed value for reproducibility
 
     Returns:
         DataFrame: Results of predictive model going through a PND algorithm.
         Conatians both values and their scores.
 
-    Example:
-    >>> import grama as gr
-    >>>
-    >>> md_true = gr.make_pareto_random()
-    >>>
-    >>> df_data = (
-    >>>     md_true
-    >>>     >> gr.ev_sample(n=2e3, seed=101, df_det="nom")
-    >>> )
-    >>>
-    >>> df_train = (
-    >>>     df_data
-    >>>     >> gr.tf_sample(n=10))
-    >>> )
-    >>>
-    >>> df_test = (
-    >>>     df_data
-    >>>     >> gr.anti_join(
-    >>>         df_train,
-    >>>         by = ["x1","x2"]
-    >>>     )
-    >>>     >> gr.tf_sample(n=200)
-    >>> )
-    >>>
-    >>> md_fit = (
-    >>>     df_train
-    >>>     >> gr.ft_gp(
-    >>>         var=["x1","x2"]
-    >>>         out=["y1","y2"]
-    >>>     )
-    >>> )
-    >>>
-    >>> df_pnd = (
+    References:
+        del Rosario, Zachary, et al. "Assessing the frontier: Active learning, model accuracy, and multi-objective candidate discovery and optimization." The Journal of Chemical Physics 153.2 (2020): 024112.
+
+    Examples::
+
+        import grama as gr
+
+        ## Define a ground-truth model
+        md_true = gr.make_pareto_random()
+        df_data = (
+            md_true
+            >> gr.ev_sample(n=2e3, seed=101, df_det="nom")
+        )
+        ## Generate test/train data
+        df_train = (
+            df_data
+            >> gr.tf_sample(n=10)
+        )
+
+        df_test = (
+            df_data
+            >> gr.anti_join(
+                df_train,
+                by = ["x1","x2"]
+            )
+            >> gr.tf_sample(n=200)
+        )
+        ## Fit a model to training data
+        md_fit = (
+            df_train
+            >> gr.ft_gp(
+                var=["x1","x2"]
+                out=["y1","y2"]
+            )
+        )
+        ## Rank training points by PND algorithm
+        df_pnd = (
             md_fit
             >> gr.ev_pnd(
                 df_train,
                 df_test,
                 signs = {"y1":1, "y2":1},
                 seed = 101
             )
             >> gr.tf_arrange(gr.desc(DF.pr_scores))
         )
+
     """
-    # # Check for correct types
-    # if not isinstance(model, Model):
-    #     raise TypeError('model must be a Model')
-
-    # if not isinstance(df_train, DataFrame):
-    #     raise TypeError('df_train must be a DataFrame')
-    #
-    # if not isinstance(df_test, DataFrame):
-    #     raise TypeError('df_test must be a DataFrame')
+    invariants_eval_model(model)
+    invariants_eval_df(df_train, arg_name="df_train")
+    invariants_eval_df(df_test, arg_name="df_test")
+
 
     # Check content
     if len(model.out)/2 < 2:
         raise ValueError('Given Model needs multiple outputs')
 
-    if len(model.functions) == 0:
-        raise ValueError("Given model has no functions")
-
     if not set(model.var).issubset(set(df_train.columns)):
         raise ValueError("model.var must be subset of df_train.columns")
 
     if not set(model.var).issubset(set(df_test.columns)):
         raise ValueError("model.var must be subset of df_test.columns")
 
     for key in signs.keys():
```

### Comparing `py_grama-0.3.4/grama/eval_random.py` & `py_grama-0.3.5/grama/eval_random.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     "ev_sinews",
     "eval_hybrid",
     "ev_hybrid",
 ]
 
 from grama import add_pipe, CopulaIndependence, custom_formatwarning
 from grama import comp_marginals, eval_df
+from grama.eval_defaults import invariants_eval_model, invariants_eval_df
 from numbers import Integral
 from numpy import tile, linspace, zeros, isfinite
 from numpy.linalg import cholesky, inv
 from numpy.random import random
 from numpy.random import seed as set_seed
 from pandas import DataFrame
 from scipy.stats import norm, lognorm
@@ -54,26 +55,29 @@
         indname (str): Column name to give for sweep index; default="sweep_ind"
         append (bool): Append results to conservative inputs?
         skip (bool): Skip evaluation of the functions?
 
     Returns:
         DataFrame: Results of evaluation or unevaluated design
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> md = gr.make_cantilever_beam()
-        >>> # Skip evaluation, vis. design
-        >>> df_design = md >> gr.ev_sinews(df_det="nom", skip=True)
-        >>> df_design >> gr.pt_auto()
-        >>> # Vis results
-        >>> df_sinew = md >> gr.ev_sinews(df_det="nom")
-        >>> df_sinew >> gr.pt_auto()
+        import grama as gr
+        md = gr.make_cantilever_beam()
+        # Skip evaluation, used to visualize the design (input points)
+        df_design = md >> gr.ev_sinews(df_det="nom", skip=True)
+        df_design >> gr.pt_auto()
+        # Visualize the input-to-output relationships of the model
+        df_sinew = md >> gr.ev_sinews(df_det="nom")
+        df_sinew >> gr.pt_auto()
 
     """
+    ## Common invariant checks
+    invariants_eval_model(model, skip)
+    invariants_eval_df(df_det, arg_name="df_det", valid_str=["nom", "swp"])
     ## Override model if deterministic sweeps desired
     if df_det == "swp":
         ## Collect sweep-able deterministic variables
         var_sweep = list(
             filter(
                 lambda v: isfinite(model.domain.get_width(v))
                 & (model.domain.get_width(v) > 0),
@@ -136,23 +140,16 @@
     df_rand[varname] = C_var
     df_rand[indname] = C_ind
     ## Construct outer-product DOE
     df_samp = model.var_outer(df_rand, df_det=df_det)
 
     if skip:
         ## Evaluation estimate
-        runtime_est = model.runtime(df_samp.shape[0])
-        if runtime_est > 0:
-            print(
-                "Estimated runtime for design with model ({0:1}):\n  {1:4.3} sec".format(
-                    model.name, runtime_est
-                )
-            )
-        else:
-            print("Design runtime estimates unavailable; model has no timing data.")
+        runtime_msg = model.runtime_message(df_samp)
+        print(runtime_msg)
 
         ## For autoplot
         with catch_warnings():
             simplefilter("ignore")
             df_samp._plot_info = {"type": "sinew_inputs", "var": model.var_rand}
 
         ## Pass-through
@@ -204,29 +201,31 @@
         append (bool): Append results to conservative inputs?
         skip (bool): Skip evaluation of the functions?
 
     Returns:
         DataFrame: Results of evaluation or unevaluated design
 
     References:
-        I.M. Sobol', "Sensitivity Estimates for Nonlinear Mathematical Models"
-        (1999) MMCE, Vol 1.
+        I.M. Sobol', "Sensitivity Estimates for Nonlinear Mathematical Models" (1999) MMCE, Vol 1.
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> md = gr.make_cantilever_beam()
-        >>> df_first = md >> gr.ev_hybrid(df_det="nom", plan="first")
-        >>> df_first >> gr.tf_sobol()
-        >>>
-        >>> df_total = md >> gr.ev_hybrid(df_det="nom", plan="total")
-        >>> df_total >> gr.tf_sobol()
+        import grama as gr
+        md = gr.make_cantilever_beam()
+        ## Compute the first-order indices
+        df_first = md >> gr.ev_hybrid(df_det="nom", plan="first")
+        df_first >> gr.tf_sobol()
+        ## Compute the total-order indices
+        df_total = md >> gr.ev_hybrid(df_det="nom", plan="total")
+        df_total >> gr.tf_sobol()
 
     """
     ## Check invariants
+    invariants_eval_model(model, skip)
+    invariants_eval_df(df_det, arg_name="df_det", valid_str=["nom"])
     if not isinstance(model.density.copula, CopulaIndependence):
         raise ValueError(
             "model must have CopulaIndependence structure;\n"
             + "Sobol' indices only defined for independent variables"
         )
 
     ## Set seed only if given
@@ -267,14 +266,19 @@
     ## Convert samples to desired marginals
     df_rand = model.density.pr2sample(df_pr)
     df_rand[varname] = C_var
     ## Construct outer-product DOE
     df_samp = model.var_outer(df_rand, df_det=df_det)
 
     if skip:
+        ## Evaluation estimate
+        runtime_msg = model.runtime_message(df_samp)
+        print(runtime_msg)
+
+        # Generate design
         with catch_warnings():
             simplefilter("ignore")
             df_samp._meta = dict(
                 type="eval_hybrid",
                 varname=varname,
                 plan=plan,
                 var_rand=model.var_rand,
```

### Comparing `py_grama-0.3.4/grama/eval_tail.py` & `py_grama-0.3.5/grama/fit/fit_scikitlearn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,369 +1,544 @@
 __all__ = [
-    "eval_form_pma",
-    "ev_form_pma",
-    "eval_form_ria",
-    "ev_form_ria",
+    "fit_gp",
+    "ft_gp",
+    "fit_lm",
+    "ft_lm",
+    "fit_rf",
+    "ft_rf",
+    "fit_kmeans",
+    "ft_kmeans",
 ]
 
-from grama import add_pipe, pipe, custom_formatwarning
-from .eval_defaults import eval_df
-from numpy import array, argmin, ones, eye, zeros, sqrt, NaN, max
-from numpy.linalg import norm as length
-from numpy.random import multivariate_normal
-from pandas import DataFrame, concat
-from scipy.optimize import minimize
+## Fitting via sklearn package
+try:
+    from sklearn.linear_model import LinearRegression
+    from sklearn.gaussian_process import GaussianProcessRegressor
+    from sklearn.gaussian_process.kernels import Kernel, RBF, ConstantKernel as Con
+    from sklearn.cluster import KMeans
+    from sklearn.ensemble import RandomForestRegressor
+
+except ModuleNotFoundError:
+    pass
+
+from copy import deepcopy
+from grama import add_pipe, cp_vec_function, Function, Model, pipe
+from pandas import concat, DataFrame, Series
 from toolz import curry
+from warnings import filterwarnings
 
 
-## Utility Functions
+## Helper functions and classes
 # --------------------------------------------------
-def make_T(model, df_corr):
-    """Make covariance matrix from list
+def standardize_cols(df, ser_min, ser_max, var):
+    """
+    @pre set(ser_min.index) == set(ser_max.index)
+    """
+
+    df_std = df.copy()
+    for v in var:
+        den = ser_max[v] - ser_min[v]
+        if den < 1e-16:
+            den = 1
+        df_std[v] = (df_std[v] - ser_min[v]) / den
+    return df_std
 
-    Construct a covariance matrix from given entries. Check for correctness
-    against a model.
 
+def restore_cols(df, ser_min, ser_max, var):
     """
-    ## TODO
-    raise NotImplementedError
+    @pre set(ser_min.index) == set(ser_max.index)
+    """
+    df_res = df.copy()
+    for v in var:
+        den = ser_max[v] - ser_min[v]
+        if den < 1e-16:
+            den = 1
+        df_res[v] = den * df[v] + ser_min[v]
+    return df_res
+
+
+class FunctionGPR(Function):
+    def __init__(self, gpr, var, out, name, runtime, var_min, var_max):
+        self.gpr = gpr
+        # self.df_train = df_train
+        self.var = var
+        ## "Natural" outputs; what we're modeling
+        self.out_nat = out
+        ## Predicted outputs; mean and std
+        self.out_mean = list(map(lambda s: s + "_mean", out))
+        self.out_sd = list(map(lambda s: s + "_sd", out))
+        self.out = self.out_mean + self.out_sd
+
+        self.name = name
+        self.runtime = runtime
+
+        self.var_min = var_min
+        self.var_max = var_max
+
+    def eval(self, df):
+        ## Check invariant; model inputs must be subset of df columns
+        if not set(self.var).issubset(set(df.columns)):
+            raise ValueError(
+                "Model function `{}` var not a subset of given columns".format(
+                    self.name
+                )
+            )
+        df_sd = standardize_cols(df, self.var_min, self.var_max, self.var)
+        y, y_sd = self.gpr.predict(df_sd[self.var], return_std=True)
+
+        return concat(
+            (
+                DataFrame(data=y, columns=self.out_mean),
+                DataFrame(data=y_sd, columns=self.out_sd),
+            ),
+            axis=1,
+        )
+
+    def copy(self):
+        func_new = FunctionGPR(
+            self.gpr,
+            self.df_train.copy(),
+            self.var,
+            self.out_nat,
+            self.name,
+            self.runtime,
+        )
+
+        return func_new
+
+
+class FunctionRegressor(Function):
+    def __init__(self, regressor, var, out, name, runtime):
+        """
+
+        Args:
+            regressor (scikit Regressor):
+        """
+        self.regressor = regressor
+        self.var = var
+        self.out = list(map(lambda s: s + "_mean", out))
+        self.name = name
+        self.runtime = runtime
+
+    def eval(self, df):
+        ## Check invariant; model inputs must be subset of df columns
+
+        if not set(self.var).issubset(set(df.columns)):
+            raise ValueError(
+                "Model function `{}` var not a subset of given columns".format(
+                    self.name
+                )
+            )
+
+        ## Predict
+        y = self.regressor.predict(df[self.var])
+        return DataFrame(data=y, columns=self.out)
 
 
-## FORM
+## Fit GP model with sklearn
 # --------------------------------------------------
 @curry
-def eval_form_pma(
-    model,
-    betas=None,
-    cons=None,
-    df_corr=None,
-    df_det=None,
-    append=True,
-    tol=1e-3,
-    n_maxiter=25,
-    n_restart=1,
-    verbose=False,
+def fit_gp(
+    df,
+    md=None,
+    var=None,
+    out=None,
+    domain=None,
+    density=None,
+    kernels=None,
+    seed=None,
+    suppress_warnings=True,
+    n_restart=5,
+    alpha=1e-10,
 ):
-    r"""Tail quantile via FORM PMA
+    r"""Fit a gaussian process
 
-    Approximate the desired tail quantiles using the performance measure
-    approach (PMA) of the first-order reliability method (FORM) [1]. Select
-    limit states to minimize at desired quantile with `betas`. Provide
-    confidence levels `cons` and estimator covariance `df_corr` to compute with
-    margin in beta [2].
+    Fit a gaussian process to given data. Specify var and out, or inherit from
+    an existing model.
+
+    Note that the new model will have two outputs `y_mean, y_sd` for each
+    original output `y`. The quantity `y_mean` is the best-fit value, while
+    `y_sd` is a measure of predictive uncertainty.
 
     Args:
-        model (gr.Model): Model to analyze
-        betas (dict): Target reliability indices;
-            key   = limit state name; must be in model.out
-            value = reliability index; beta = Phi^{-1}(reliability)
-        cons (dict or None): Target confidence levels;
-            key   = limit state name; must be in model.out
-            value = confidence level, \in (0, 1)
-        df_corr (DataFrame or None): Sampling distribution covariance entries;
-            parameters with no information assumed to be known exactly.
-        df_det (DataFrame): Deterministic levels for evaluation; use "nom"
-            for nominal deterministic levels.
-        n_maxiter (int): Maximum iterations for each optimization run
-        n_restart (int): Number of restarts (== number of optimization runs)
-        append (bool): Append MPP results for random values?
-        verbose (bool): Print optimization results?
+        df (DataFrame): Data for function fitting
+        md (gr.Model): Model from which to inherit metadata
+        var (list(str) or None): List of features or None for all except outputs
+        out (list(str)): List of outputs to fit
+        domain (gr.Domain): Domain for new model
+        density (gr.Density): Density for new model
+        seed (int or None): Random seed for fitting process
+        kernels (sklearn.gaussian_process.kernels.Kernel or dict or None): Kernel for GP
+        n_restart (int): Restarts for optimization
+        alpha (float or iterable): Value added to diagonal of kernel matrix
+        suppress_warnings (bool): Suppress warnings when fitting?
 
     Returns:
-        DataFrame: Results of MPP search
+        gr.Model: A grama model with fitted function(s)
 
     Notes:
-        - Since FORM PMA relies on optimization over the limit state, it is
-          often beneficial to scale your limit state to keep values near unity.
-
-    References:
-        - [1] Tu, Choi, and Park, "A new study on reliability-based design optimization," Journal of Mechanical Design, 1999
-        - [2] del Rosario, Fenrich, and Iaccarino, "Fast precision margin with the first-order reliability method," AIAA Journal, 2019
+        - Wrapper for sklearn.gaussian_process.GaussianProcessRegressor
 
     """
+    if suppress_warnings:
+        filterwarnings("ignore")
+
+    n_obs, n_in = df.shape
+
+    ## Infer fitting metadata, if available
+    if not (md is None):
+        domain = md.domain
+        density = md.density
+        out = md.out
+
     ## Check invariants
-    if betas is None:
+    if not set(out).issubset(set(df.columns)):
+        raise ValueError("out must be subset of df.columns")
+    ## Default input value
+    if var is None:
+        var = list(set(df.columns).difference(set(out)))
+    ## Check more invariants
+    set_inter = set(out).intersection(set(var))
+    if len(set_inter) > 0:
         raise ValueError(
-            "Must provide `betas` keyword argument to define reliability targets"
+            "out and var must be disjoint; intersect = {}".format(set_inter)
         )
-    if not set(betas.keys()).issubset(set(model.out)):
-        raise ValueError("betas.keys() must be subset of model.out")
-    if not cons is None:
-        if not (set(cons.keys()) == set(betas.keys())):
-            raise ValueError("cons.keys() must be same as betas.keys()")
-        else:
-            if df_corr is None:
-                raise ValueError("Must provide df_corr is using cons")
-        raise NotImplementedError
-
-    df_det = model.var_outer(
-        DataFrame(data=zeros((1, model.n_var_rand)), columns=model.var_rand),
-        df_det=df_det,
-    )
-    df_det = df_det[model.var_det]
-
-    df_return = DataFrame()
-    for ind in range(df_det.shape[0]):
-        ## Loop over objectives
-        for key in betas.keys():
-            ## Temp dataframe
-            df_inner = df_det.iloc[[ind]].reset_index(drop=True)
-
-            ## Construct lambdas
-            def objective(z):
-                ## Transform: standard normal-to-random variable
-                df_norm = DataFrame(data=[z], columns=model.var_rand)
-                df_rand = model.norm2rand(df_norm)
-                df = model.var_outer(df_rand, df_det=df_inner)
-
-                df_res = eval_df(model, df=df)
-                g = df_res[key].iloc[0]
-
-                # return (g, jac)
-                return g
-
-            def con_beta(z):
-                return z.dot(z) - (betas[key]) ** 2
-
-            ## Use conservative direction for initial guess
-            signs = array([model.density.marginals[k].sign for k in model.var_rand])
-            if length(signs) > 0:
-                z0 = betas[key] * signs / length(signs)
-            else:
-                z0 = betas[key] * ones(model.n_var_rand) / sqrt(model.n_var_rand)
-
-            ## Minimize
-            res_all = []
-            for jnd in range(n_restart):
-                res = minimize(
-                    objective,
-                    z0,
-                    args=(),
-                    method="SLSQP",
-                    jac=False,
-                    tol=tol,
-                    options={"maxiter": n_maxiter, "disp": False},
-                    constraints=[{"type": "eq", "fun": con_beta}],
-                )
-                # Append only a successful result
-                if res["status"] == 0:
-                    res_all.append(res)
-                # Set a random start; repeat
-                z0 = multivariate_normal([0] * model.n_var_rand, eye(model.n_var_rand))
-                z0 = z0 / length(z0) * betas[key]
-
-            # Choose value among restarts
-            n_iter_total = sum([res_all[i].nit for i in range(len(res_all))])
-            if len(res_all) > 0:
-                i_star = argmin([res.fun for res in res_all])
-                x_star = res_all[i_star].x
-                fun_star = res_all[i_star].fun
-                if verbose:
-                    print("out = {}: Optimization successful".format(key))
-                    print("n_iter = {}".format(res_all[i_star].nit))
-                    print("n_iter_total = {}".format(n_iter_total))
-            else:
-                ## WARNING
-                x_star = [NaN] * model.n_var_rand
-                fun_star = NaN
-                if verbose:
-                    print("out = {}: Optimization unsuccessful".format(key))
-                    print("n_iter = {}".format(res_all[i_star].nit))
-                    print("n_iter_total = {}".format(n_iter_total))
-
-            ## Extract results
-            if append:
-                df_inner = concat(
-                    (
-                        df_inner,
-                        model.norm2rand(
-                            DataFrame(data=[x_star], columns=model.var_rand)
-                        ),
-                    ),
-                    axis=1,
-                    sort=False,
-                )
-            df_inner[key] = [fun_star]
-            df_return = concat((df_return, df_inner), axis=0, sort=False)
+    if not set(var).issubset(set(df.columns)):
+        raise ValueError("var must be subset of df.columns")
 
-    if not append:
-        df_return = (
-            df_return.groupby(model.var_det)
-            .agg({s: max for s in betas.keys()})
-            .reset_index()
+    ## Pre-process kernel selection
+    try:
+        if kernels is None:
+            # Vectorize
+            kernels = {o: None for o in out}
+        elif isinstance(kernels, Kernel):
+            kernels = {o: kernels for o in out}
+
+    except NameError as e:
+        error_string = str(e)
+        raise NameError(
+            error_string +
+            "\n\nThis function requires the `sklearn` package. " +
+            "Try running the following to install the package:\n"
+            "    pip install scikit-learn"
         )
 
-    return df_return
+    ## Pre-process data
+    var_min = df[var].min()
+    var_max = df[var].max()
+    df_sd = standardize_cols(df, var_min, var_max, var)
+
+    ## Construct gaussian process for each output
+    functions = []
+
+    try:
+        for output in out:
+            # Define and fit model
+            gpr = GaussianProcessRegressor(
+                kernel=deepcopy(kernels[output]),
+                random_state=seed,
+                normalize_y=True,
+                copy_X_train=True,
+                n_restarts_optimizer=n_restart,
+                alpha=alpha,
+            )
+            gpr.fit(df_sd[var], df_sd[output])
+            name = "GP ({})".format(str(gpr.kernel_))
+
+            fun = FunctionGPR(gpr, var, [output], name, 0, var_min, var_max)
+            functions.append(fun)
+
+    except NameError as e:
+        error_string = str(e)
+        raise NameError(
+            error_string +
+            "\n\nThis function requires the `sklearn` package. " +
+            "Try running the following to install the package:\n"
+            "    pip install scikit-learn"
+        )
 
+    ## Construct model
+    return Model(functions=functions, domain=domain, density=density)
 
-ev_form_pma = add_pipe(eval_form_pma)
 
+ft_gp = add_pipe(fit_gp)
 
+## Fit random forest model with sklearn
+# --------------------------------------------------
 @curry
-def eval_form_ria(
-    model,
-    limits=None,
-    cons=None,
-    df_corr=None,
-    df_det=None,
-    append=True,
-    tol=1e-3,
-    n_maxiter=25,
-    n_restart=1,
-    verbose=False,
+def fit_rf(
+    df,
+    md=None,
+    var=None,
+    out=None,
+    domain=None,
+    density=None,
+    seed=None,
+    suppress_warnings=True,
+    **kwargs
 ):
-    r"""Tail reliability via FORM RIA
+    r"""Fit a random forest
 
-    Approximate the desired tail probability using the reliability index
-    approach (RIA) of the first-order reliability method (FORM) [1]. Select
-    limit states to analyze with list input `limits`. Provide confidence levels
-    `cons` and estimator covariance `df_corr` to compute with margin in beta
-    [2].
+    Fit a random forest to given data. Specify inputs and outputs, or inherit
+    from an existing model.
 
     Args:
-        model (gr.Model): Model to analyze
-        limits (list): Target limit states; must be in model.out; limit state
-            assumed to be critical at g == 0
-        cons (dict or None): Target confidence levels;
-            key   = limit state name; must be in model.out
-            value = confidence level, \in (0, 1)
-        df_corr (DataFrame or None): Sampling distribution covariance entries;
-            parameters with no information assumed to be known exactly.
-        df_det (DataFrame): Deterministic levels for evaluation; use "nom"
-            for nominal deterministic levels.
-        n_maxiter (int): Maximum iterations for each optimization run
-        n_restart (int): Number of restarts (== number of optimization runs)
-        append (bool): Append MPP results for random values?
-        verbose (bool): Print optimization results?
+        df (DataFrame): Data for function fitting
+        md (gr.Model): Model from which to inherit metadata
+        var (list(str) or None): List of features or None for all except outputs
+        out (list(str)): List of outputs to fit
+        domain (gr.Domain): Domain for new model
+        density (gr.Density): Density for new model
+        seed (int or None): Random seed for fitting process
+        suppress_warnings (bool): Suppress warnings when fitting?
+
+    Keyword Arguments:
+        n_estimators (int):
+        criterion (int):
+        max_depth (int or None):
+        min_samples_split (int, float):
+        min_samples_leaf (int, float):
+        min_weight_fraction_leaf (float):
+        max_features (int, float, string):
+        max_leaf_nodes (int or None):
+        min_impurity_decrease (float):
+        min_impurity_split (float):
+        bootstrap (bool):
+        oob_score (bool):
+        n_jobs (int or None):
+        random_state (int):
 
     Returns:
-        DataFrame: Results of MPP search
+        gr.Model: A grama model with fitted function(s)
 
     Notes:
-        - Since FORM RIA relies on optimization over the limit state, it is
-          often beneficial to scale your limit state to keep values near unity.
+        - Wrapper for sklearn.ensemble.RandomForestRegressor
 
-    References:
-        - [1] Tu, Choi, and Park, "A new study on reliability-based design optimization," Journal of Mechanical Design, 1999
-        - [2] del Rosario, Fenrich, and Iaccarino, "Fast precision margin with the first-order reliability method," AIAA Journal, 2019
+    """
+    if suppress_warnings:
+        filterwarnings("ignore")
+
+    n_obs, n_in = df.shape
+
+    ## Infer fitting metadata, if available
+    if not (md is None):
+        domain = md.domain
+        density = md.density
+        out = md.out
+
+    ## Check invariants
+    if not set(out).issubset(set(df.columns)):
+        raise ValueError("out must be subset of df.columns")
+    ## Default input value
+    if var is None:
+        var = list(set(df.columns).difference(set(out)))
+    ## Check more invariants
+    set_inter = set(out).intersection(set(var))
+    if len(set_inter) > 0:
+        raise ValueError(
+            "outputs and inputs must be disjoint; intersect = {}".format(set_inter)
+        )
+    if not set(var).issubset(set(df.columns)):
+        raise ValueError("var must be subset of df.columns")
+
+    ## Construct gaussian process for each output
+    functions = []
+
+    try:
+        for output in out:
+            rf = RandomForestRegressor(random_state=seed, **kwargs)
+            rf.fit(df[var], df[output])
+            name = "RF"
+
+            fun = FunctionRegressor(rf, var, [output], name, 0)
+            functions.append(fun)
+
+    except NameError as e:
+        error_string = str(e)
+        raise NameError(
+            error_string +
+            "\n\nThis function requires the `sklearn` package. " +
+            "Try running the following to install the package:\n"
+            "    pip install scikit-learn"
+        )
+
+    ## Construct model
+    return Model(functions=functions, domain=domain, density=density)
+
+
+ft_rf = add_pipe(fit_rf)
+
+## Fit linear model with sklearn
+# --------------------------------------------------
+@curry
+def fit_lm(
+    df,
+    md=None,
+    var=None,
+    out=None,
+    domain=None,
+    density=None,
+    seed=None,
+    suppress_warnings=True,
+    **kwargs
+):
+    r"""Fit a linear model
+
+    Fit a linear model to given data. Specify inputs and outputs, or inherit
+    from an existing model.
+
+    Args:
+        df (DataFrame): Data for function fitting
+        md (gr.Model): Model from which to inherit metadata
+        var (list(str) or None): List of features or None for all except outputs
+        out (list(str)): List of outputs to fit
+        domain (gr.Domain): Domain for new model
+        density (gr.Density): Density for new model
+        seed (int or None): Random seed for fitting process
+        suppress_warnings (bool): Suppress warnings when fitting?
+
+    Returns:
+        gr.Model: A grama model with fitted function(s)
+
+    Notes:
+        - Wrapper for sklearn.ensemble.RandomForestRegressor
 
     """
+    if suppress_warnings:
+        filterwarnings("ignore")
+
+    n_obs, n_in = df.shape
+
+    ## Infer fitting metadata, if available
+    if not (md is None):
+        domain = md.domain
+        density = md.density
+        out = md.out
+
     ## Check invariants
-    if limits is None:
+    if not set(out).issubset(set(df.columns)):
+        raise ValueError("out must be subset of df.columns")
+    ## Default input value
+    if var is None:
+        var = list(set(df.columns).difference(set(out)))
+    ## Check more invariants
+    set_inter = set(out).intersection(set(var))
+    if len(set_inter) > 0:
         raise ValueError(
-            "Must provide `limits` keyword argument to define reliability targets"
+            "outputs and inputs must be disjoint; intersect = {}".format(set_inter)
         )
-    if not set(limits).issubset(set(model.out)):
-        raise ValueError("`limits` must be subset of model.out")
-    if not cons is None:
-        if not (set(cons.keys()) == set(limits)):
-            raise ValueError("cons.keys() must be same as limits")
-        else:
-            if df_corr is None:
-                raise ValueError("Must provide df_corr is using cons")
-        raise NotImplementedError
-
-    df_det = model.var_outer(
-        DataFrame(data=zeros((1, model.n_var_rand)), columns=model.var_rand),
-        df_det=df_det,
-    )
-    df_det = df_det[model.var_det]
-
-    # df_return = DataFrame(columns=model.var_rand + model.var_det + limits)
-    df_return = DataFrame()
-    for ind in range(df_det.shape[0]):
-        ## Loop over objectives
-        for key in limits:
-            ## Temp dataframe
-            df_inner = df_det.iloc[[ind]].reset_index(drop=True)
-
-            ## Construct lambdas
-            def fun_jac(z):
-                ## Squared reliability index
-                fun = z.dot(z)
-                jac = 2 * z * length(z)
-
-                return (fun, jac)
-
-            def con_limit(z):
-                ## Transform: standard normal-to-random variable
-                df_norm = DataFrame(data=[z], columns=model.var_rand)
-                df_rand = model.norm2rand(df_norm)
-                df = model.var_outer(df_rand, df_det=df_inner)
-
-                ## Eval limit state
-                df_res = eval_df(model, df=df)
-                g = df_res[key].iloc[0]
-
-                return g
-
-            ## Use conservative direction for initial guess
-            signs = array([model.density.marginals[k].sign for k in model.var_rand])
-            if length(signs) > 0:
-                z0 = signs / length(signs)
-            else:
-                z0 = ones(model.n_var_rand) / sqrt(model.n_var_rand)
-
-            ## Minimize
-            res_all = []
-            for jnd in range(n_restart):
-                res = minimize(
-                    fun_jac,
-                    z0,
-                    args=(),
-                    method="SLSQP",
-                    jac=True,
-                    tol=tol,
-                    options={"maxiter": n_maxiter, "disp": False},
-                    constraints=[{"type": "eq", "fun": con_limit}],
-                )
-                # Append only a successful result
-                if res["status"] == 0:
-                    res_all.append(res)
-                # Set a random start; repeat
-                z0 = multivariate_normal([0] * model.n_var_rand, eye(model.n_var_rand))
-                z0 = z0 / length(z0)
-
-            # Choose value among restarts
-            n_iter_total = sum([res_all[i].nit for i in range(len(res_all))])
-            if len(res_all) > 0:
-                i_star = argmin([res.fun for res in res_all])
-                x_star = res_all[i_star].x
-                fun_star = sqrt(res_all[i_star].fun)
-                if verbose:
-                    print("out = {}: Optimization successful".format(key))
-                    print("n_iter = {}".format(res_all[i_star].nit))
-                    print("n_iter_total = {}".format(n_iter_total))
-            else:
-                ## WARNING
-                x_star = [NaN] * model.n_var_rand
-                fun_star = NaN
-                if verbose:
-                    print("out = {}: Optimization unsuccessful".format(key))
-                    print("n_iter = {}".format(res_all[i_star].nit))
-                    print("n_iter_total = {}".format(n_iter_total))
-
-            ## Extract results
-            if append:
-                df_inner = concat(
-                    (
-                        df_inner,
-                        model.norm2rand(
-                            DataFrame(data=[x_star], columns=model.var_rand)
-                        ),
-                    ),
-                    axis=1,
-                    sort=False,
-                )
-            df_inner["beta_" + key] = [fun_star]
-            df_return = concat((df_return, df_inner), axis=0, sort=False)
+    if not set(var).issubset(set(df.columns)):
+        raise ValueError("var must be subset of df.columns")
+
+    ## Construct gaussian process for each output
+    functions = []
+
+    try:
+        for output in out:
+            lm = LinearRegression(**kwargs)
+            lm.fit(df[var], df[output])
+            name = "LM"
+
+            fun = FunctionRegressor(lm, var, [output], name, 0)
+            functions.append(fun)
+
+    except NameError as e:
+        error_string = str(e)
+        raise NameError(
+            error_string +
+            "\n\nThis function requires the `sklearn` package. " +
+            "Try running the following to install the package:\n"
+            "    pip install scikit-learn"
+        )
+
+    ## Construct model
+    return Model(functions=functions, domain=domain, density=density)
+
+
+ft_lm = add_pipe(fit_lm)
+
 
-    if not append:
-        df_return = (
-            df_return.groupby(model.var_det) \
-                     .agg({"beta_" + s: max for s in limits}).reset_index()
+## Fit kmeans clustering model
+# --------------------------------------------------
+@curry
+def fit_kmeans(df, var=None, colname="cluster_id", seed=None, **kwargs):
+    r"""K-means cluster a dataset
+
+    Create a cluster-labeling model on a dataset using the K-means algorithm.
+
+    Args:
+        df (DataFrame): Hybrid point results from gr.eval_hybrid()
+        var (list or None): Variables in df on which to cluster. Use None to
+            cluster on all variables.
+        colname (string): Name of cluster id; will be output in cluster model.
+        seed (int): Random seed for kmeans clustering
+
+    Kwargs:
+        n_clusters (int): Number of clusters to fit
+        random_state (int or None):
+
+    Returns:
+        gr.Model: Model that labels input data
+
+    Notes:
+        - A wrapper for sklearn.cluster.KMeans
+
+    References:
+        Scikit-learn: Machine Learning in Python, Pedregosa et al. JMLR 12, pp. 2825-2830, 2011.
+
+    Examples::
+
+        import grama as gr
+        from grama.data import df_stang
+        from grama.fit import ft_kmeans
+        DF = gr.Intention()
+        md_cluster = (
+            df_stang
+            >> ft_kmeans(var=["E", "mu"], n_clusters=2)
+        )
+        (
+            md_cluster
+            >> gr.ev_df(df_stang)
+            >> gr.tf_group_by(DF.cluster_id)
+            >> gr.tf_summarize(
+                thick_mean=gr.mean(DF.thick),
+                thick_sd=gr.sd(DF.thick),
+                n=gr.n(),
+            )
+        )
+
+    """
+    ## Check invariants
+    if var is None:
+        var = list(df.columns).copy()
+    else:
+        var = list(var).copy()
+        diff = set(var).difference(set(df.columns))
+        if len(diff) > 0:
+            raise ValueError(
+                "`var` must be subset of `df.columns`\n" "diff = {}".format(diff)
+            )
+
+    ## Generate clustering
+    try:
+        kmeans = KMeans(random_state=seed, **kwargs).fit(df[var].values)
+
+    except NameError as e:
+        error_string = str(e)
+        raise NameError(
+            error_string +
+            "\n\nThis function requires the `sklearn` package. " +
+            "Try running the following to install the package:\n"
+            "    pip install scikit-learn"
         )
 
-    return df_return
+    ## Build grama model
+    def fun_cluster(df):
+        res = kmeans.predict(df[var].values)
+        return DataFrame(data={colname: res})
+
+    md = Model() >> cp_vec_function(fun=fun_cluster, var=var, out=[colname])
+
+    return md
 
 
-ev_form_ria = add_pipe(eval_form_ria)
+ft_kmeans = add_pipe(fit_kmeans)
```

### Comparing `py_grama-0.3.4/grama/fit/fit_lolo.py` & `py_grama-0.3.5/grama/fit/fit_lolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         self.rf = rf
         self.var = var
         self.name = name
         self.runtime = runtime
 
         self.return_std = return_std
         if return_std:
-            self.out = list(map(lambda s: s + "_mean", out)) + list(map(lambda s: s + "_sd", out))
+            self.out = list(map(lambda s: s + "_mean", out)) + list(
+                map(lambda s: s + "_sd", out)
+            )
         else:
             self.out = list(map(lambda s: s + "_mean", out))
 
     def eval(self, df):
         ## Check invariant; model inputs must be subset of df columns
         if not set(self.var).issubset(set(df.columns)):
             raise ValueError(
@@ -69,14 +71,16 @@
     seed=None,
     return_std=True,
     suppress_warnings=True,
     **kwargs
 ):
     r"""Fit a random forest
 
+    DEPRECATED DO NOT USE
+
     Fit a random forest to given data. Specify inputs and outputs, or inherit
     from an existing model.
 
     Args:
         df (DataFrame): Data for function fitting
         md (gr.Model): Model from which to inherit metadata
         var (list(str) or None): List of features or None for all except outputs
@@ -149,17 +153,17 @@
 
             fun = FunctionRFR(rf, var, [output], name, 0, return_std)
             functions.append(fun)
 
     except NameError as e:
         error_string = str(e)
         raise NameError(
-            error_string +
-            "\n\nThis function requires the `lolopy` package. " +
-            "Try running the following to install the package:\n"
+            error_string
+            + "\n\nThis function requires the `lolopy` package. "
+            + "Try running the following to install the package:\n"
             "    pip install lolopy"
         )
 
     ## Construct model
     return Model(functions=functions, domain=domain, density=density)
```

### Comparing `py_grama-0.3.4/grama/fit/fit_statsmodels.py` & `py_grama-0.3.5/grama/fit/fit_statsmodels.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/fit_synonyms.py` & `py_grama-0.3.5/grama/fit_synonyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,29 +45,26 @@
         md (gr.Model): Model to analyze. All model variables
             selected for fitting must be bounded or random. Deterministic
             variables may have semi-infinite bounds.
 
         var_fix (list or None): Variables to fix to nominal levels. Note that
             variables with domain width zero will automatically be fixed.
         df_init (DataFrame): Initial guesses for parameters; overrides n_restart
-        n_restart (int): Number of restarts to try; the first try is at
-            the nominal conditions of the model. Returned model will use
-            the least-error parameter set among restarts tested.
+        n_restart (int): Number of restarts to try; the first try is at the nominal conditions of the model. Returned model will use the least-error parameter set among restarts tested.
         n_maxiter (int): Optimizer maximum iterations
         verbose (bool): Print best-fit parameters to console?
-        uq_method (str OR None): If string, select method to quantify parameter
-            uncertainties. If None, provide best-fit values only. Methods:
-            uq_method = "linpool": assume normal errors; linearly approximate
-                parameter effects; equally pool variance matrices for each output
+        uq_method (str OR None): If string, select method to quantify parameter uncertainties. If None, provide best-fit values only. Methods:
+            uq_method = "linpool": assume normal errors; linearly approximate parameter effects; equally pool variance matrices for each output
 
     Returns:
         gr.Model: Model for evaluation with best-fit variables frozen to
             optimized levels.
 
-    Examples:
+    Examples::
+
         import grama as gr
         from grama.data import df_trajectory_windowed
         from grama.models import make_trajectory_linear
         DF = gr.Intention()
 
         md_trajectory = make_trajectory_linear()
 
@@ -111,18 +108,20 @@
         var_fix = set()
     else:
         var_fix = set(var_fix)
     for var in md.var_det:
         wid = md.domain.get_width(var)
         if wid == 0:
             var_fix.add(var)
+    var_fix = list(var_fix)
 
     ## Run eval_nls to fit model parameter values
     df_fit = eval_nls(
         md,
+        out=out,
         df_data=df_data,
         var_fix=var_fix,
         df_init=df_init,
         append=True,
         verbose=verbose,
         **kwargs,
     )
@@ -204,15 +203,15 @@
 
         ## Construct model with Gaussian copula
         if len(var_fix) > 0:
             md_res = (
                 Model(name)
                 >> cp_function(
                     lambda x: df_nom[var_fix].values,
-                    var=set(var_remain).difference(var_fix),
+                    var=list(set(var_remain).difference(var_fix)),
                     out=var_fix,
                     name="Fix variable levels",
                 )
                 >> cp_md_det(md=md)
                 >> cp_marginals(**marginals)
                 >> cp_copula_gaussian(df_corr=df_corr)
             )
```

### Comparing `py_grama-0.3.4/grama/marginals.py` & `py_grama-0.3.5/grama/marginals.py`

 * *Files 6% similar despite different names*

```diff
@@ -445,21 +445,17 @@
         kurt_excess=None,
         floc=None,
         sign=0,
         dict_x0=None,
 ):
     r"""Fit scipy.stats continuous distribution via moments
 
-    Fit a continuous distribution using the method of moments. Select a
-    distribution shape and provide numerical values for a convenient set of
-    common moments.
-
-    This routine uses a vector-output root finding routine to match the moments.
-    You may set an optional initial guess for the distribution parameters using
-    the dict_x0 argument.
+    Fit a continuous distribution using the method of moments. Select a distribution shape and provide numerical values for a convenient set of common moments.
+
+    This routine uses a vector-output root finding routine to match the moments. You may set an optional initial guess for the distribution parameters using the dict_x0 argument.
 
     Args:
         dist (str): Name of distribution to fit
 
     Kwargs:
         mean (float): Mean of distribution
         sd (float): Standard deviation of distribution
@@ -476,30 +472,31 @@
 
         sign (-1, 0, +1): Sign
         dict_x0 (dict): Dictionary of initial parameter guesses
 
     Returns:
         gr.MarginalNamed: Distribution
 
-    Examples:
-        >>> import grama as gr
-        >>> ## Fit a normal distribution
-        >>> mg_norm = gr.marg_mom("norm", mean=0, sd=1)
-        >>> ## Fit a (3-parameter) lognormal distribution
-        >>> mg_lognorm = gr.marg_mom("lognorm", mean=1, sd=1, skew=1)
-        >>> ## Fit a lognormal, controlling kurtosis instead
-        >>> mg_lognorm = gr.marg_mom("lognorm", mean=1, sd=1, kurt=1)
-        >>> ## Fit a 2-parameter lognormal; no skewness or kurtosis needed
-        >>> mg_lognorm = gr.marg_mom("lognorm", mean=1, sd=1, floc=0)
-        >>>
-        >>> ## Not all moment combinations are feasible; this will fail
-        >>> gr.marg_mom("beta", mean=1, sd=1, skew=0, kurt=4)
-        >>> ## Skewness and kurtosis are related for the beta distribution;
-        >>> ## a different combination is feasible
-        >>> gr.marg_mom("beta", mean=1, sd=1, skew=0, kurt=2)
+    Examples::
+
+        import grama as gr
+        ## Fit a normal distribution
+        mg_norm = gr.marg_mom("norm", mean=0, sd=1)
+        ## Fit a (3-parameter) lognormal distribution
+        mg_lognorm = gr.marg_mom("lognorm", mean=1, sd=1, skew=1)
+        ## Fit a lognormal, controlling kurtosis instead
+        mg_lognorm = gr.marg_mom("lognorm", mean=1, sd=1, kurt=1)
+        ## Fit a 2-parameter lognormal; no skewness or kurtosis needed
+        mg_lognorm = gr.marg_mom("lognorm", mean=1, sd=1, floc=0)
+
+        ## Not all moment combinations are feasible; this will fail
+        gr.marg_mom("beta", mean=1, sd=1, skew=0, kurt=4)
+        ## Skewness and kurtosis are related for the beta distribution;
+        ## a different combination is feasible
+        gr.marg_mom("beta", mean=1, sd=1, skew=0, kurt=2)
 
     """
     ## Number of distribution parameters
     n_param = len(param_dist[dist])
     if n_param > 4:
         raise NotImplementedError(
             "marg_nom does not yet handle distributions with more than 4 parameters"
@@ -625,16 +622,15 @@
         param["loc"] = floc
     return MarginalNamed(sign=sign, d_name=dist, d_param=param)
 
 ## Fit a named scipy.stats distribution
 def marg_fit(dist, data, name=True, sign=None, **kwargs):
     r"""Fit scipy.stats continuous distirbution
 
-    Fits a scipy.stats continuous distribution. Intended to be used to define a
-    marginal distribution from data.
+    Fits a scipy.stats continuous distribution. Intended to be used to define a marginal distribution from data.
 
     Arguments:
         dist (str): Distribution to fit
         data (iterable): Data for fit
         name (bool): Include distribution name?
         sign (bool): Include sign? (Optional)
 
@@ -647,56 +643,56 @@
         fscale (float): Value to fix the location `scale` parameter (Optional)
         f* (float): Value to fix the specified shape parameter (Optional)
             e.g. give fc to fix the `c` parameter
 
     Returns:
         gr.MarginalNamed: Distribution
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.data import df_shewhart
-        >>> # Fit normal distribution
-        >>> mg_normal = gr.marg_named(
-        >>>     "norm",
-        >>>     df_shewhart.tensile_strength,
-        >>> )
-        >>> # Fit two-parameter Weibull distribution
-        >>> mg_weibull2 = gr.marg_named(
-        >>>     "weibull_min",
-        >>>     df_shewhart.tensile_strength,
-        >>>     floc=0,        # 2-parameter has frozen loc == 0
-        >>> )
-        >>> # Fit three-parameter Weibull distribution
-        >>> mg_weibull3 = gr.marg_named(
-        >>>     "weibull_min",
-        >>>     df_shewhart.tensile_strength,
-        >>>     loc=0,        # 3-parameter fit tends to be unstable;
-        >>>                   # an inital guess helps stabilize fit
-        >>> )
-        >>> # Inspect fits with QQ plot
-        >>> (
-        >>>     df_shewhart
-        >>>     >> gr.tf_mutate(
-        >>>         q_normal=gr.qqvals(DF.tensile_strength, marg=mg_normal),
-        >>>         q_weibull2=gr.qqvals(DF.tensile_strength, marg=mg_weibull2),
-        >>>     )
-        >>>     >> gr.tf_pivot_longer(
-        >>>         columns=[
-        >>>             "q_normal",
-        >>>             "q_weibull2",
-        >>>         ],
-        >>>         names_to=[".value", "Distribution"],
-        >>>         names_sep="_"
-        >>>     )
-        >>>
-        >>>     >> gr.ggplot(gr.aes("q", "tensile_strength"))
-        >>>     + gr.geom_abline(intercept=0, slope=1, linetype="dashed")
-        >>>     + gr.geom_point(gr.aes(color="Distribution"))
-        >>> )
+        import grama as gr
+        from grama.data import df_shewhart
+        # Fit normal distribution
+        mg_normal = gr.marg_named(
+            "norm",
+            df_shewhart.tensile_strength,
+        )
+        # Fit two-parameter Weibull distribution
+        mg_weibull2 = gr.marg_named(
+            "weibull_min",
+            df_shewhart.tensile_strength,
+            floc=0,        # 2-parameter has frozen loc == 0
+        )
+        # Fit three-parameter Weibull distribution
+        mg_weibull3 = gr.marg_named(
+            "weibull_min",
+            df_shewhart.tensile_strength,
+            loc=0,        # 3-parameter fit tends to be unstable;
+                          # an inital guess helps stabilize fit
+        )
+        # Inspect fits with QQ plot
+        (
+            df_shewhart
+            >> gr.tf_mutate(
+                q_normal=gr.qqvals(DF.tensile_strength, marg=mg_normal),
+                q_weibull2=gr.qqvals(DF.tensile_strength, marg=mg_weibull2),
+            )
+            >> gr.tf_pivot_longer(
+                columns=[
+                    "q_normal",
+                    "q_weibull2",
+                ],
+                names_to=[".value", "Distribution"],
+                names_sep="_"
+            )
+
+            >> gr.ggplot(gr.aes("q", "tensile_strength"))
+            + gr.geom_abline(intercept=0, slope=1, linetype="dashed")
+            + gr.geom_point(gr.aes(color="Distribution"))
+        )
 
     """
     ## Catch case where user provides entire DataFrame
     if isinstance(data, DataFrame):
         raise ValueError("`data` argument must be a single column; try data.var")
 
     ## Fit the distribution
@@ -724,24 +720,26 @@
     Args:
         data (iterable): Data for fit
         sign (bool): Include sign? (Optional)
 
     Returns:
         gr.MarginalGKDE: Marginal distribution
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.data import df_stang
-        >>> md = gr.Model("Marginal Example") >> \
-        >>>     gr.cp_marginals(
-        >>>         E=gr.marg_gkde(df_stang.E),
-        >>>         mu=gr.marg_gkde(df_stang.mu)
-        >>>     )
-        >>> md.printpretty()
+        import grama as gr
+        from grama.data import df_stang
+        md = (
+            gr.Model("Marginal Example")
+            >> gr.cp_marginals(
+                E=gr.marg_gkde(df_stang.E),
+                mu=gr.marg_gkde(df_stang.mu),
+            )
+        )
+        md
 
     """
     ## Catch case where user provides entire DataFrame
     if isinstance(data, DataFrame):
         raise ValueError("`data` argument must be a single column; try data.var")
 
     kde = gaussian_kde(data)
```

### Comparing `py_grama-0.3.4/grama/models/cantilever_beam.py` & `py_grama-0.3.5/grama/models/cantilever_beam.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/models/channel1d.py` & `py_grama-0.3.5/grama/models/channel1d.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/models/circuit_RLC.py` & `py_grama-0.3.5/grama/models/circuit_RLC.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     md_RLC_det = (
         Model("RLC Circuit")
         >> cp_vec_function(
             fun=lambda df: df_make(omega0=sqrt(1 / df.L / df.C)),
             var=["L", "C"],
             out=["omega0"],
         )
-        >> cp_function(
+        >> cp_vec_function(
             fun=lambda df: df_make(Q=df.omega0 * df.R * df.C),
             name="parallel RLC",
             var=["omega0", "R", "C"],
             out=["Q"]
         )
         >> cp_bounds(
             R=(1e-3, 1e0),
```

### Comparing `py_grama-0.3.4/grama/models/ishigami.py` & `py_grama-0.3.5/grama/models/ishigami.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 __all__ = ["make_ishigami"]
 
 from grama import cp_bounds, cp_function, cp_copula_independence, cp_marginals, \
     Model
 from numpy import sin, pi
 
 
-def fun(x):
-    a, b, x1, x2, x3 = x
+def fun(a, b, x1, x2, x3):
     return sin(x1) + a * sin(x2)**2 + b * x3**4 * sin(x1)
 
 def make_ishigami():
     """Ishigami function
 
     The Ishigami function is commonly used as a test case for estimating Sobol'
     indices.
```

### Comparing `py_grama-0.3.4/grama/models/linear_normal.py` & `py_grama-0.3.5/grama/models/linear_normal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 __all__ = ["make_linear_normal"]
 
 from grama import cp_copula_independence, cp_function, cp_marginals, Model
 
 
-def limit_state(x):
-    x1, x2 = x
-
+def limit_state(x1, x2):
     return 1 - x1 - x2
 
 def make_linear_normal():
     md = Model("Linear-Normal Reliability Problem") >> \
          cp_function(
              fun=limit_state,
              var=2,
```

### Comparing `py_grama-0.3.4/grama/models/pareto_random.py` & `py_grama-0.3.5/grama/models/pareto_random.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/models/plane_laminate.py` & `py_grama-0.3.5/grama/models/plane_laminate.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,15 +409,15 @@
         deg_str = map(mapSign, deg_int)
         name =  "Composite Plate in Tension " + "-".join(deg_str)
 
         super().__init__(
             name=name,
             functions=[
                 Function(
-                    lambda X: uniaxial_stress_limit(X),
+                    lambda *X: uniaxial_stress_limit(X),
                     make_names(Theta_nom),
                     list(itertools.chain.from_iterable([
                         ["g_11_tension_{}".format(i),
                          "g_22_tension_{}".format(i),
                          "g_11_compression_{}".format(i),
                          "g_22_compression_{}".format(i),
                          "g_12_shear_{}".format(i)] for i in range(k)
```

### Comparing `py_grama-0.3.4/grama/models/plate_buckling.py` & `py_grama-0.3.5/grama/models/plate_buckling.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/models/poly.py` & `py_grama-0.3.5/grama/models/poly.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/models/test.py` & `py_grama-0.3.5/grama/models/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from pandas import DataFrame
 
 
 ## Define a test dataset
 df_test_input = DataFrame(data={"x0": [0], "x1": [0], "x2": [0]})
 
 ## Define a test model
-def fun(x):
-    x1, x2, x3 = x
+def fun(x1, x2, x3):
     return x1 + x2 + x3
 
 def make_test():
     md = Model() >> \
          cp_function(fun=fun, var=3, out=1) >> \
          cp_bounds(x0=(-1,+1), x1=(-1,+1), x2=(-1,+1)) >> \
          cp_marginals(
```

### Comparing `py_grama-0.3.4/grama/models/trajectory_linear_drag.py` & `py_grama-0.3.5/grama/models/trajectory_linear_drag.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/mutate_helpers.py` & `py_grama-0.3.5/grama/mutate_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -164,14 +164,19 @@
     """
     return x.astype(str)
 
 
 @make_symbolic
 def as_factor(x, categories=None, ordered=True, dtype=None):
     r"""Cast to factor
+
+    Args:
+        x (pd.Series): Column to convert
+        categories (list): Categories (levels) of factor (Optional)
+        ordered (boolean): Order the factor?
     """
     return Categorical(x, categories=categories, ordered=ordered, dtype=dtype)
 
 
 @make_symbolic
 def as_numeric(x):
     r"""Cast to numeric
@@ -211,14 +216,15 @@
     Find the Pareto-efficient points that minimize the provided features.
 
     Args:
         xi (iterable OR gr.Intention()): Feature to minimize; use -X to maximize
 
     Returns:
         np.array of boolean: Indicates if observation is Pareto-efficient
+
     """
     # Check invariants
     lengths = map(len, args)
     if len(set(lengths)) > 1:
         raise ValueError("All arguments to pareto_min must be of equal length")
 
     # Compute pareto points
@@ -237,16 +243,15 @@
 def stratum_min(*args, max_depth=10):
     r"""Compute Pareto stratum number
 
     Compute the Pareto stratum number for a given dataset.
 
     Args:
         xi (iterable OR gr.Intention()): Feature to minimize; use -X to maximize
-        max_depth (int): Maximum depth for recursive computation; stratum numbers exceeding
-            this value will not be computed and will be flagged as NaN.
+        max_depth (int): Maximum depth for recursive computation; stratum numbers exceeding this value will not be computed and will be flagged as NaN.
 
     Returns:
         np.array of floats: Pareto stratum number
 
     References:
         del Rosario, Rupp, Kim, Antono, and Ling "Assessing the frontier: Active learning, model accuracy, and multi-objective candidate discovery and optimization" (2020) J. Chem. Phys.
     """
@@ -287,15 +292,16 @@
         f (iterable OR DataFrame column): factor to reorder
         x (iterable OR DataFrame column): variable on which to reorder; specify aggregation method with fun
         fun (function): aggregation function for reordering, default=median
 
     Returns:
         Categorical: Iterable with levels sorted according to x
 
-    Examples:
+    Examples::
+
         import grama as gr
         from grama.data import df_diamonds
         DF = gr.Intention()
         (
             df_diamonds
             >> gr.tf_mutate(cut=gr.fct_reorder(DF.cut, DF.price))
             >> gr.tf_group_by(DF.cut)
@@ -318,65 +324,75 @@
 # -------------------------
 @make_symbolic
 def fillna(*args, **kwargs):
     r"""Wrapper for pandas Series.fillna
 
     (See below for Pandas documentation)
 
-    Examples:
-        >>> import grama as gr
-        >>> X = gr.Intention()
-        >>> df = gr.df_make(x=[1, gr.NaN], y=[2, 3])
-        >>> df_filled = (
-        >>>     df
-        >>>     >> gr.tf_mutate(x=gr.fillna(X.x, 0))
-        >>> )
+    Examples::
+
+        import grama as gr
+        X = gr.Intention()
+        df = gr.df_make(x=[1, gr.NaN], y=[2, 3])
+        df_filled = (
+            df
+            >> gr.tf_mutate(x=gr.fillna(X.x, 0))
+        )
     """
     return Series.fillna(*args, **kwargs)
 
 
 fillna.__doc__ = fillna.__doc__ + Series.fillna.__doc__
 
 # Q-Q Plot Helper
 # -------------------------
 @make_symbolic
 def qqvals(x, dist=None, marg=None):
     r"""Generate theoretical quantiles
 
-    Generate theoretical quantiles for a Q-Q plot. Can provide either a
-    pre-defined Marginal object or the name of a distribution to fit.
+    Generate theoretical quantiles for a Q-Q plot. Can provide either a pre-defined Marginal object or the name of a distribution to fit.
 
     Arguments:
         x (array-like or gr.Intention()): Target observations
 
     Keyword Arguments:
+        dist (str or None): Name of scipy distribution to fit; see gr.valid_dist for list of valid distributions
         marg (gr.Marginal() or None): Pre-fitted marginal
-        dist (str or None): Name of scipy distribution to fit; see
-            gr.valid_dist for list of valid distributions
 
     Returns:
         Series: Theoretical quantiles, matched in order with target observations
 
     References:
-        Filliben, J. J., "The Probability Plot Correlation Coefficient Test
-        for Normality" (1975) Technometrics. DOI: 10.1080/00401706.1975.10489279
+        Filliben, J. J., "The Probability Plot Correlation Coefficient Test for Normality" (1975) Technometrics. DOI: 10.1080/00401706.1975.10489279
+
+    Examples::
+
+        import grama as gr
+        from grama.data import df_shewhart
+        DF = gr.Intention()
+
+        ## Make a Q-Q plot
+        (
+            df_shewhart
+            >> gr.tf_mutate(q=gr.qqvals(DF.tensile_strength, dist="norm"))
+            >> gr.ggplot(gr.aes("q", "tensile_strength"))
+            + gr.geom_abline(intercept=0, slope=1, linetype="dashed")
+            + gr.geom_point()
+        )
 
-    Examples:
-        >>> import grama as gr
-        >>> from grama.data import df_shewhart
-        >>> DF = gr.Intention()
-        >>>
-        >>> (
-        >>>     ## Make a Q-Q plot
-        >>>     df_shewhart
-        >>>     >> gr.tf_mutate(q=gr.qqvals(DF.tensile_strength, dist="norm"))
-        >>>     >> gr.ggplot(gr.aes("q", "tensile_strength"))
-        >>>     + gr.geom_abline(intercept=0, slope=1, linetype="dashed")
-        >>>     + gr.geom_point()
-        >>> )
+        ## Fit a marginal, use in Q-Q plot
+        mg_tys = gr.marg_fit("lognorm", df_shewhart.tensile_strength, floc=0)
+        # Plot to assess the fit
+        (
+            df_shewhart
+            >> gr.tf_mutate(q=gr.qqvals(DF.tensile_strength, marg=mg_tys))
+            >> gr.ggplot(gr.aes("q", "tensile_strength"))
+            + gr.geom_abline(intercept=0, slope=1, linetype="dashed")
+            + gr.geom_point()
+        )
 
     """
     # Check invariants
     if (marg is None) and (dist is None):
         raise ValueError(
             "Must provide one of marg or dist (exclusively)."
         )
@@ -399,70 +415,70 @@
 
     return marg.q(p)
 
 
 # Array constructors
 # -------------------------
 @make_symbolic
-def linspace(a, b, n, **kwargs):
+def linspace(a, b, n=100, **kwargs):
     r"""Linearly-spaced values
 
-    Create an array of linearly-spaced values. Accepts keyword arguments for
-    numpy.linspace.
+    Create an array of linearly-spaced values. Accepts keyword arguments for numpy.linspace.
 
     Arguments:
         a (numeric): Smallest value
         b (numeric): Largest value
         n (int): Number of points
 
     Returns:
         numpy array: Array of requested values
 
     Notes:
-        This is a symbolic alias for np.linspace(); you can use this in
-        pipe-enabled functions.
+        This is a symbolic alias for np.linspace(); you can use this in pipe-enabled functions.
+
+    Examples::
+
+        import grama as gr
+        from grama.data import df_stang
+        DF = gr.Intention()
+        (
+            df_stang
+            >> gr.tf_mutate(c=gr.linspace(0, 1, gr.n(DF.index)))
+        )
 
-    Examples:
-        >>> import grama as gr
-        >>> from grama.data import df_stang
-        >>> DF = gr.Intention()
-        >>> (
-        >>>     df_stang
-        >>>     >> gr.tf_mutate(c=gr.linspace(0, 1, gr.n(DF.index)))
-        >>> )
     """
     return nplinspace(a, b, num=n, **kwargs)
 
 @make_symbolic
-def logspace(a, b, n, **kwargs):
+def logspace(a, b, n=100, **kwargs):
     r"""Logarithmically-spaced values
 
-    Create an array of logarithmically-spaced values. Accepts keyword arguments for
-    numpy.logspace.
+    Create an array of logarithmically-spaced values. Accepts keyword arguments for numpy.logspace.
 
     Arguments:
         a (numeric): Smallest value
         b (numeric): Largest value
         n (int): Number of points
 
     Returns:
         numpy array: Array of requested values
 
     Notes:
-        This is a symbolic alias for np.logspace(); you can use this in
-        pipe-enabled functions.
+        This is a symbolic alias for np.logspace(); you can use this in pipe-enabled functions.
+
+    Examples::
+
+        import grama as gr
+        from grama.data import df_stang
+        DF = gr.Intention()
+        (
+            df_stang
+            >> gr.tf_mutate(c=gr.logspace(0, 1, gr.n(DF.index)))
+        )
 
-    Examples:
-        >>> import grama as gr
-        >>> from grama.data import df_stang
-        >>> DF = gr.Intention()
-        >>> (
-        >>>     df_stang
-        >>>     >> gr.tf_mutate(c=gr.logspace(0, 1, gr.n(DF.index)))
-        >>> )
     """
     return nplogspace(a, b, num=n, **kwargs)
 
 
 @make_symbolic
 def consec(series, i=3):
     r"""Flag consecutive runs of True values
```

### Comparing `py_grama-0.3.4/grama/plot_auto.py` & `py_grama-0.3.5/grama/plot_auto.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,23 +12,25 @@
     "plot_sinew_outputs",
     "pt_sinew_outputs",
     "plot_auto",
     "pt_auto",
     "plot_list",
 ]
 
-from grama import add_pipe, pipe, tf_pivot_longer, tf_outer, tf_select, tf_rename, tf_filter
+from grama import add_pipe, pipe, tf_pivot_longer, tf_outer, tf_select, tf_rename, tf_filter, tf_mutate
+from grama import case_when
 from grama import Intention
+from .string_helpers import str_replace
 from pandas import melt
 
 from plotnine import aes, annotate, ggplot, facet_grid, facet_wrap, labs, guides
 from plotnine import theme, theme_void, theme_minimal
 from plotnine import element_text, element_rect
-from plotnine import scale_x_continuous, scale_y_continuous, scale_fill_gradient2
-from plotnine import geom_point, geom_density, geom_histogram, geom_line, geom_tile
+from plotnine import scale_x_continuous, scale_y_continuous, scale_fill_gradient, scale_fill_gradient2, scale_fill_gradientn
+from plotnine import geom_point, geom_density, geom_histogram, geom_line, geom_tile, geom_text
 from plotnine import geom_segment, geom_blank
 from matplotlib import gridspec
 
 from toolz import curry
 
 ## Helper functions
 ##################################################
@@ -41,115 +43,216 @@
         ["\n{0:1.1e}".format(v[-1])]
     )
 
 ## Function-specific plot functions
 ##################################################
 ## eval_contour
 @curry
-def plot_contour(df, var=None, out="out", level="level", aux=False):
+def plot_contour(df, var=None, out="out", level="level", aux=False, color="full"):
     r"""Plot 2d contours
 
-    Plot contours.
-
-    Usually called as a dispatch from plot_auto().
+    Plot contours. Usually called as a dispatch from plot_auto().
 
     Args:
         var (array of str): Variables for plot axes
         out (str): Name of output identifier column
         level (str): Name of level identifier column
         aux (bool): Auxillary variables present?
+        color (str): Color mode; options: "full", "bw"
 
     Returns:
         ggplot: Contour image
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.models import make_cantilever_beam
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        (
+            md_beam
+            >> gr.ev_contour(
+                var=["w", "t"],
+                out=["g_stress"],
+                # Set auxilliary inputs to nominal levels
+                df=gr.eval_nominal(md_beam, df_det="nom"),
+            )
+            >> gr.pt_auto()
+        )
 
     """
     # Check invariants
     if var is None:
         raise ValueError("Must provide input columns list as keyword var")
     if aux:
         raise ValueError(
             "Autoplot plot_contour not designed to handle auxiliary variables. " +
             "Regenerate contour data with fixed auxilary variables, " +
             "or try creating a manual plot."
         )
 
-    return (
-        df
-        >> ggplot()
-        + geom_segment(
-            aes(
-                var[0],
-                var[1],
-                xend=var[0]+"_end",
-                yend=var[1]+"_end",
-                linetype=out,
-                color=level,
+    if color == "full":
+        return (
+            df
+            >> ggplot()
+            + geom_segment(
+                aes(
+                    var[0],
+                    var[1],
+                    xend=var[0]+"_end",
+                    yend=var[1]+"_end",
+                    linetype=out,
+                    color=level,
+                )
             )
         )
-    )
+    elif color == "bw":
+        return (
+            df
+            >> ggplot()
+            + geom_segment(
+                aes(
+                    var[0],
+                    var[1],
+                    xend=var[0]+"_end",
+                    yend=var[1]+"_end",
+                    linetype=out,
+                    group=level,
+                )
+            )
+        )
+    else:
+        raise ValueError("Color mode {} not recognized.".format(color))
 
 
 pt_contour = add_pipe(plot_contour)
 
 ## tran_iocorr
 # --------------------------------------------------
 @curry
-def plot_corrtile(df, var=None, out=None, corr=None):
+def plot_corrtile(df, var=None, out=None, corr=None, color="full"):
     r"""
     """
-    return (
+    if color == "full":
+        return (
+            df
+            >> ggplot(aes(var, out))
+            + geom_tile(aes(fill=corr))
+            + scale_fill_gradient2(name="Corr", midpoint=0)
+            + theme_minimal()
+            + theme(axis_text_x=element_text(angle=270))
+        )
+    elif color == "bw":
+        DF = Intention()
+        return (
+            df
+            >> tf_mutate(
+                sign=case_when(
+                    [DF[corr] > 0, "+"],
+                    [DF[corr] < 0, "-"],
+                    [True, None],
+                )
+            )
+            >> ggplot(aes(var, out))
+            + geom_tile(aes(fill=corr))
+            + geom_text(aes(label="sign"), size=12, color="white")
+            + scale_fill_gradientn(
+                name="Corr",
+                colors=("black", "white", "black"),
+                values=(0, 0.5, 1),
+            )
+            + theme_minimal()
+            + theme(axis_text_x=element_text(angle=270))
+        )
+    else:
+        raise ValueError("Color mode {} not recognized.".format(color))
+
+pt_corrtile = add_pipe(plot_corrtile)
+
+## tran_sobol
+# --------------------------------------------------
+@curry
+def plot_sobol_outputs(df, idx=None, color="full"):
+    r"""
+    """
+    df_data = (
         df
-        >> ggplot(aes(var, out))
-        + geom_tile(aes(fill=corr))
-        + scale_fill_gradient2(name="Corr", midpoint=0)
-        + theme(axis_text_x=element_text(angle=270))
+        >> tf_pivot_longer(
+            columns=df.drop(idx, axis=1).columns,
+            names_to="out",
+            values_to="S"
+        )
     )
+    df_data[idx] = str_replace(df_data[idx], "^S_", "")
+
+    if color == "full":
+        return (
+            df_data
+            >> ggplot(aes(idx, "out"))
+            + geom_tile(aes(fill="S"))
+            + scale_fill_gradient(name="Sobol' Index", breaks=(0, 0.5, 1), limits=(0, 1))
+            + theme_minimal()
+            + theme(axis_text_x=element_text(angle=270))
+            + labs(
+                x="var",
+                y="out",
+            )
+        )
+    elif color == "bw":
+        return (
+            df_data
+            >> ggplot(aes(idx, "out"))
+            + geom_tile(aes(fill="S"))
+            + scale_fill_gradient(name="Sobol' Index", low="white", high="black", breaks=(0, 0.5, 1), limits=(0, 1))
+            + theme_minimal()
+            + theme(axis_text_x=element_text(angle=270))
+            + labs(
+                x="var",
+                y="out",
+            )
+        )
+    else:
+        raise ValueError("Color mode {} not recognized.".format(color))
 
 pt_corrtile = add_pipe(plot_corrtile)
 
 ## Sample
 # --------------------------------------------------
 @curry
-def plot_scattermat(df, var=None):
+def plot_scattermat(df, var=None, color="full"):
     r"""Create a scatterplot matrix
 
     Create a scatterplot matrix. Often used to visualize a design (set of inputs
     points) before evaluating the functions.
 
     Usually called as a dispatch from plot_auto().
 
     Args:
         var (list of strings): Variables to plot
+        color (str): Color mode; value ignored as default vis is black & white
 
     Returns:
         ggplot: Scatterplot matrix
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> import matplotlib.pyplot as plt
-        >>> from grama.models import make_cantilever_beam
-        >>> md = make_cantilever_beam()
-        >>> ## Dispatch from autoplotter
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sample(n=100, df_det="nom", skip=True)
-        >>>     >> gr.pt_auto()
-        >>> )
-        >>> ## Re-create plot without metadata
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sample(n=100, df_det="nom")
-        >>>     >> gr.pt_scattermat(var=md.var)
-        >>> )
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        ## Dispatch from autoplotter
+        (
+            md_beam
+            >> gr.ev_sample(n=100, df_det="nom", skip=True)
+            >> gr.pt_auto()
+        )
+        ## Re-create plot without metadata
+        (
+            md_beam
+            >> gr.ev_sample(n=100, df_det="nom")
+            >> gr.pt_scattermat(var=md.var)
+        )
 
     """
     if var is None:
         raise ValueError("Must provide input columns list as keyword var")
 
     ## Define helpers
     labels_blank = lambda v: [""] * len(v)
@@ -234,46 +337,46 @@
     fig.show()
 
 
 pt_scattermat = add_pipe(plot_scattermat)
 
 
 @curry
-def plot_hists(df, out=None, **kwargs):
+def plot_hists(df, out=None, color="full", **kwargs):
     r"""Construct histograms
 
     Create a set of histograms. Often used to visualize the results of random
     sampling for multiple outputs.
 
     Usually called as a dispatch from plot_auto().
 
     Args:
         out (list of strings): Variables to plot
+        color (str): Color mode; value ignored as default vis is black & white
 
     Returns:
         Seaborn histogram plot
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> import matplotlib.pyplot as plt
-        >>> from grama.models import make_cantilever_beam
-        >>> md = make_cantilever_beam()
-        >>> ## Dispatch from autoplotter
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sample(n=100, df_det="nom")
-        >>>     >> gr.pt_auto()
-        >>> )
-        >>> ## Re-create without metadata
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sample(n=100, df_det="nom")
-        >>>     >> gr.pt_hists(out=md.out)
-        >>> )
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        ## Dispatch from autoplotter
+        (
+            md_beam
+            >> gr.ev_sample(n=100, df_det="nom")
+            >> gr.pt_auto()
+        )
+        ## Re-create without metadata
+        (
+            md_beam
+            >> gr.ev_sample(n=100, df_det="nom")
+            >> gr.pt_hists(out=md.out)
+        )
 
     """
     if out is None:
         raise ValueError("Must provide input columns list as keyword out")
 
     return (
         df
@@ -294,52 +397,54 @@
 
 
 pt_hists = add_pipe(plot_hists)
 
 ## Sinew plots
 # --------------------------------------------------
 @curry
-def plot_sinew_inputs(df, var=None, sweep_ind="sweep_ind"):
+def plot_sinew_inputs(df, var=None, color="full", sweep_ind="sweep_ind"):
     r"""Inspect a sinew design
 
     Create a scatterplot matrix with hues. Often used to visualize a sinew
     design before evaluating the model functions.
 
     Usually called as a dispatch from plot_auto().
 
     Args:
         df (Pandas DataFrame): Input design data
         var (list of strings): Variables to plot
         sweep_ind (string): Sweep index column in df
+        color (str): Color mode; options: "full", "bw"
 
     Returns:
         Seaborn scatterplot matrix
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> import matplotlib.pyplot as plt
-        >>> from grama.models import make_cantilever_beam
-        >>> md = make_cantilever_beam()
-        >>> ## Dispatch from autoplotter
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sinews(df_det="swp", skip=True)
-        >>>     >> gr.pt_auto()
-        >>> )
-        >>> ## Re-create without metadata
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sinews(df_det="swp")
-        >>>     >> gr.pt_sinew_inputs(var=md.var)
-        >>> )
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        ## Dispatch from autoplotter
+        (
+            md_beam
+            >> gr.ev_sinews(df_det="swp", skip=True)
+            >> gr.pt_auto()
+        )
+        ## Re-create without metadata
+        (
+            md_beam
+            >> gr.ev_sinews(df_det="swp")
+            >> gr.pt_sinew_inputs(var=md.var)
+        )
 
     """
     if var is None:
         raise ValueError("Must provide input columns list as keyword var")
+    if not (color in ("full", "bw")):
+        raise ValueError("Color mode {} not recognized.".format(color))
 
     ## Define helpers
     labels_blank = lambda v: [""] * len(v)
     breaks_min = lambda lims: (lims[0], 0.5 * (lims[0] + lims[1]), lims[1])
 
     ## Make blank figure
     fig = (
@@ -371,88 +476,108 @@
                     + annotate(
                         "label",
                         x=0,
                         y=0,
                         label=v1,
                     )
                     + theme_void()
-                    + guides(color=None)
+                    + guides(color=None, linetype=None)
                 )
 
             ## Scatterplot
             else:
-                p = (
-                    df
-                    >> ggplot(aes(v2, v1, color="factor("+sweep_ind+")"))
-                    + geom_point(size=0.1)
-                    + scale_x_continuous(
-                        breaks=breaks_min,
-                        labels=labels_x,
-                    )
-                    + scale_y_continuous(
-                        breaks=breaks_min,
-                        labels=labels_y,
+                if color == "full":
+                    p = (
+                        df
+                        >> ggplot(aes(v2, v1, color="factor("+sweep_ind+")"))
+                        + geom_point(size=0.1)
+                        + scale_x_continuous(
+                            breaks=breaks_min,
+                            labels=labels_x,
+                        )
+                        + scale_y_continuous(
+                            breaks=breaks_min,
+                            labels=labels_y,
+                        )
+                        + guides(color=None)
+                        + theme_minimal()
+                        + theme(
+                            axis_title=element_text(va="top", size=12),
+                        )
                     )
-                    + guides(color=None)
-                    + theme_minimal()
-                    + theme(
-                        axis_title=element_text(va="top", size=12),
+                elif color == "bw":
+                    p = (
+                        df
+                        >> ggplot(aes(v2, v1))
+                        + geom_point(size=0.1)
+                        + scale_x_continuous(
+                            breaks=breaks_min,
+                            labels=labels_x,
+                        )
+                        + scale_y_continuous(
+                            breaks=breaks_min,
+                            labels=labels_y,
+                        )
+                        + guides(color=None)
+                        + theme_minimal()
+                        + theme(
+                            axis_title=element_text(va="top", size=12),
+                        )
                     )
-                )
 
             _ = p._draw_using_figure(fig, [ax])
 
 
     ## Plot
     # NB Returning the figure causes a "double plot" in Jupyter....
     fig.show()
 
 
 pt_sinew_inputs = add_pipe(plot_sinew_inputs)
 
 
 @curry
 def plot_sinew_outputs(
-    df, var=None, out=None, sweep_ind="sweep_ind", sweep_var="sweep_var"
+    df, var=None, out=None, sweep_ind="sweep_ind", sweep_var="sweep_var", color="full",
 ):
     r"""Construct sinew plot
 
     Create a relational lineplot with hues for each sweep. Often used to
     visualize the outputs of a sinew design.
 
     Usually called as a dispatch from plot_auto().
 
     Args:
         df (Pandas DataFrame): Input design data with output results
         var (list of strings): Variables to plot
         out (list of strings): Outputs to plot
         sweep_ind (string): Sweep index column in df
         sweep_var (string): Swept variable column in df
+        color (str): Color mode; options: "full", "bw"
 
     Returns:
-        Seaborn relational lineplot
+        Relational lineplot
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> import matplotlib.pyplot as plt
-        >>> from grama.models import make_cantilever_beam
-        >>> md = make_cantilever_beam()
-        >>> ## Dispatch from autoplotter
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sinews(df_det="swp")
-        >>>     >> gr.pt_auto()
-        >>> )
-        >>> ## Re-create without metadata
-        >>> (
-        >>>     md
-        >>>     >> gr.ev_sinews(df_det="swp")
-        >>>     >> gr.pt_sinew_inputs(var=md.var, out=md.out)
-        >>> )
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        ## Dispatch from autoplotter
+        (
+            md_beam
+            >> gr.ev_sinews(df_det="swp")
+            >> gr.pt_auto()
+        )
+        ## Re-create without metadata
+        (
+            md_beam
+            >> gr.ev_sinews(df_det="swp")
+            >> gr.pt_sinew_inputs(var=md.var, out=md.out)
+        )
 
     """
     if var is None:
         raise ValueError("Must provide input columns list as keyword arg var")
     if out is None:
         raise ValueError("Must provide output columns list as keyword arg out")
 
@@ -465,71 +590,104 @@
     id_vars = [col for col in df_tmp.columns if col not in out]
     df_plot = melt(df_tmp, id_vars, out, "_out", "_y")
 
     # Filter off-sweep values
     df_plot = df_plot[df_plot[sweep_var] == df_plot["_var"]]
 
     breaks_min = lambda lims: (lims[0], 0.5 * (lims[0] + lims[1]), lims[1])
-    return (
-        df_plot
-        >> ggplot(aes(
-            "_x",
-            "_y",
-            color="factor(" + sweep_ind + ")",
-            group="factor(" + sweep_ind + ")",
-        ))
-        + geom_line()
-        + facet_grid("_out~_var", scales="free")
-
-        + scale_x_continuous(
-            breaks=breaks_min,
-            labels=_sci_format,
-        )
-        + scale_y_continuous(
-            breaks=breaks_min,
-            labels=_sci_format,
-        )
-        + guides(color=None)
-        + theme_minimal()
-        + theme(
-            strip_text_y=element_text(angle=0),
-            panel_border=element_rect(color="black", size=0.5),
+    if color == "full":
+        return (
+            df_plot
+            >> ggplot(aes(
+                "_x",
+                "_y",
+                color="factor(" + sweep_ind + ")",
+                group="factor(" + sweep_ind + ")",
+            ))
+            + geom_line()
+            + facet_grid("_out~_var", scales="free")
+
+            + scale_x_continuous(
+                breaks=breaks_min,
+                labels=_sci_format,
+            )
+            + scale_y_continuous(
+                breaks=breaks_min,
+                labels=_sci_format,
+            )
+            + guides(color=None)
+            + theme_minimal()
+            + theme(
+                strip_text_y=element_text(angle=0),
+                panel_border=element_rect(color="black", size=0.5),
+            )
+            + labs(
+                x="Input Value",
+                y="Output Value",
+            )
         )
-        + labs(
-            x="Input Value",
-            y="Output Value",
+    elif color == "bw":
+        return (
+            df_plot
+            >> ggplot(aes(
+                "_x",
+                "_y",
+                linetype="factor(" + sweep_ind + ")",
+                group="factor(" + sweep_ind + ")",
+            ))
+            + geom_line()
+            + facet_grid("_out~_var", scales="free")
+
+            + scale_x_continuous(
+                breaks=breaks_min,
+                labels=_sci_format,
+            )
+            + scale_y_continuous(
+                breaks=breaks_min,
+                labels=_sci_format,
+            )
+            + guides(linetype=None)
+            + theme_minimal()
+            + theme(
+                strip_text_y=element_text(angle=0),
+                panel_border=element_rect(color="black", size=0.5),
+            )
+            + labs(
+                x="Input Value",
+                y="Output Value",
+            )
         )
-    )
+    else:
+        raise ValueError("Color mode {} not recognized.".format(color))
 
 
 pt_sinew_outputs = add_pipe(plot_sinew_outputs)
 
 ## Autoplot dispatcher
 ## ##################################################
 plot_list = {
     "contour": plot_contour,
     "sinew_inputs": plot_sinew_inputs,
     "sinew_outputs": plot_sinew_outputs,
     "sample_inputs": plot_scattermat,
     "sample_outputs": plot_hists,
     "iocorr": plot_corrtile,
+    "sobol_outputs": plot_sobol_outputs,
 }
 
 
 @curry
-def plot_auto(df):
+def plot_auto(df, color="full"):
     r"""Automagic plotting
 
-    Convenience tool for various grama outputs. Prints delegated plotting
-    function, which can be called manually with different arguments for
-    more tailored plotting.
+    Convenience tool for various grama outputs. Prints delegated plotting function, which can be called manually with different arguments for more tailored plotting.
 
     Args:
-        df (DataFrame): Data output from appropriate grama routine. See
-            gr.plot_list.keys() for list of supported methods.
+        df (DataFrame): Data output from appropriate grama routine. See gr.plot_list.keys() for list of supported methods.
+        color (str): Color mode; options: "full", "bw"
 
     Returns:
         Plot results
 
     """
     try:
         d = df._plot_info
@@ -544,11 +702,11 @@
         plot_fcn = plot_list[d["type"]]
     except KeyError:
         raise KeyError("'{}' Plot type not implemented.".format(d["type"]))
     plt_kwargs = {key: value for key, value in d.items() if key != "type"}
 
     print("Calling {0:}....".format(plot_fcn.__name__))
 
-    return plot_fcn(df, **plt_kwargs)
+    return plot_fcn(df, color=color, **plt_kwargs)
 
 
 pt_auto = add_pipe(plot_auto)
```

### Comparing `py_grama-0.3.4/grama/psdr/basis.py` & `py_grama-0.3.5/grama/psdr/basis.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/domains/box.py` & `py_grama-0.3.5/grama/psdr/domains/box.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/domains/domain.py` & `py_grama-0.3.5/grama/psdr/domains/domain.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/domains/euclidean.py` & `py_grama-0.3.5/grama/psdr/domains/euclidean.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/domains/linineq.py` & `py_grama-0.3.5/grama/psdr/domains/linineq.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/domains/linquad.py` & `py_grama-0.3.5/grama/psdr/domains/linquad.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/domains/tensor.py` & `py_grama-0.3.5/grama/psdr/domains/tensor.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/function.py` & `py_grama-0.3.5/grama/psdr/function.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/geometry/fill.py` & `py_grama-0.3.5/grama/psdr/geometry/fill.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/geometry/geometry.py` & `py_grama-0.3.5/grama/psdr/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/geometry/miniball.py` & `py_grama-0.3.5/grama/psdr/geometry/miniball.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/geometry/vertex.py` & `py_grama-0.3.5/grama/psdr/geometry/vertex.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/gn.py` & `py_grama-0.3.5/grama/psdr/gn.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/initialization.py` & `py_grama-0.3.5/grama/psdr/initialization.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/local_linear.py` & `py_grama-0.3.5/grama/psdr/local_linear.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/misc.py` & `py_grama-0.3.5/grama/psdr/misc.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/pgf.py` & `py_grama-0.3.5/grama/psdr/pgf.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/poly.py` & `py_grama-0.3.5/grama/psdr/poly.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/polyridge.py` & `py_grama-0.3.5/grama/psdr/polyridge.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/psdr_tools.py` & `py_grama-0.3.5/grama/psdr/psdr_tools.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/quadrature.py` & `py_grama-0.3.5/grama/psdr/quadrature.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/ridge.py` & `py_grama-0.3.5/grama/psdr/ridge.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/seqlp.py` & `py_grama-0.3.5/grama/psdr/seqlp.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/psdr/subspace.py` & `py_grama-0.3.5/grama/psdr/subspace.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/spc.py` & `py_grama-0.3.5/grama/spc.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,25 @@
 
 from scipy.special import gamma
 from grama import add_pipe, Intention
 from grama import tf_group_by, tf_summarize, tf_mutate, tf_ungroup, tf_filter
 from grama import tf_pivot_longer, tf_left_join
 from grama import mean, sd, lead, lag, consec, case_when
 from grama import n as nfcn
-from plotnine import ggplot, aes, geom_line, geom_hline, geom_point, facet_grid, theme, guides
+from plotnine import ggplot, aes, geom_line, geom_hline, geom_point, facet_grid, theme, theme_minimal, guides
 from plotnine import scale_linetype_manual, scale_shape_manual, scale_color_manual
 from plotnine import labs, labeller
 from numpy import sqrt
 
 ## Helper functions
 # --------------------------------------------------
 def c_sd(n):
     r"""Anti-biasing constant for aggregate standard deviation
 
-    Returns the anti-biasing constant for aggregated standard deviation
-    estimates. If the average of $k$ samples each size $n$ are averaged to
-    produce $\overline{S} = (1/k) \sum_{i=1}^k S_i$, then the de-biased standard
-    deviation is:
+    Returns the anti-biasing constant for aggregated standard deviation estimates. If the average of $k$ samples each size $n$ are averaged to produce $\overline{S} = (1/k) \sum_{i=1}^k S_i$, then the de-biased standard deviation is:
 
         $$\hat{\sigma} = \overline{S} / c(n)$$
 
     Arguments:
         n (int): Sample (batch) size
 
     Returns:
@@ -87,33 +84,34 @@
 
     """
     return 1 + 3 / c_sd(n) * sqrt(1 - c_sd(n)**2)
 
 
 ## Control Chart constructors
 # --------------------------------------------------
-def plot_xbs(df, group, var, n_side=9, n_delta=6):
+def plot_xbs(df, group, var, n_side=9, n_delta=6, color="full"):
     r"""Construct Xbar and S chart
 
     Construct an Xbar and S chart to assess the state of statistical control of
     a dataset.
 
     Args:
         df (DataFrame): Data to analyze
         group (str): Variable for grouping
         var (str): Variable to study
 
     Keyword args:
         n_side (int): Number of consecutive runs above/below centerline to flag
         n_delta (int): Number of consecutive runs increasing/decreasing to flag
+        color (str): Color mode; "full" for full color, "bw" for greyscale
 
     Returns:
         plotnine object: Xbar and S chart
 
-    Examples:
+    Examples::
 
         import grama as gr
         DF = gr.Intention()
 
         from grama.data import df_shewhart
         (
             df_shewhart
@@ -211,53 +209,106 @@
                 [True, "None"],
             )
         )
         >> tf_ungroup()
     )
 
     ## Visualize
-    return (
-        df_batched_long
-        >> ggplot(aes(x=group))
-        + geom_hline(
-            data=df_stats_long,
-            mapping=aes(yintercept="_value", linetype="_stat"),
-        )
-        + geom_line(aes(y="_value", group="_var"), size=0.2)
-        + geom_point(
-            aes(y="_value", color="sign", shape="glyph"),
-            size=3,
-        )
-
-        + scale_color_manual(
-            values={"-2": "blue", "-1": "darkturquoise", "0": "black", "+1": "salmon", "+2": "red"},
-        )
-        + scale_shape_manual(
-            name="Patterns",
-            values={
-                "Below Limit": "s",
-                "Above Limit": "s",
-                "Low Run": "X",
-                "High Run": "X",
-                "Increasing Run": "^",
-                "Decreasing Run": "v",
-                "None": "."
-            },
-        )
-        + scale_linetype_manual(
-            name="Guideline",
-            values=dict(LCL="dashed", UCL="dashed", center="solid"),
-        )
-        + guides(color=None)
-        + facet_grid(
-            "_var~.",
-            scales="free_y",
-            labeller=labeller(dict(X="Mean", S="Variability")),
-        )
-        + labs(
-            x="Group variable ({})".format(group),
-            y="Value ({})".format(var),
+    if color == "full":
+        return (
+            df_batched_long
+            >> ggplot(aes(x=group))
+            + geom_hline(
+                data=df_stats_long,
+                mapping=aes(yintercept="_value", linetype="_stat"),
+            )
+            + geom_line(aes(y="_value", group="_var"), size=0.2)
+            + geom_point(
+                aes(y="_value", color="sign", shape="glyph"),
+                size=3,
+            )
+
+            + scale_color_manual(
+                values={"-2": "blue", "-1": "darkturquoise", "0": "black", "+1": "salmon", "+2": "red"},
+            )
+            + scale_shape_manual(
+                name="Patterns",
+                values={
+                    "Below Limit": "X",
+                    "Above Limit": "X",
+                    "Low Run": "s",
+                    "High Run": "s",
+                    "Increasing Run": "^",
+                    "Decreasing Run": "v",
+                    "None": "."
+                },
+            )
+            + scale_linetype_manual(
+                name="Guideline",
+                values=dict(LCL="dashed", UCL="dashed", center="solid"),
+            )
+            + theme_minimal()
+            + guides(color=None)
+            + facet_grid(
+                "_var~.",
+                scales="free_y",
+                labeller=labeller(dict(X="Mean", S="Variability")),
+            )
+            + labs(
+                x="Group variable ({})".format(group),
+                y="Value ({})".format(var),
+            )
+        )
+    elif color == "bw":
+        return (
+            df_batched_long
+            >> ggplot(aes(x=group))
+            + geom_hline(
+                data=df_stats_long,
+                mapping=aes(yintercept="_value", linetype="_stat"),
+            )
+            + geom_line(aes(y="_value", group="_var"), size=0.2)
+            + geom_point(
+                aes(y="_value", color="sign", shape="glyph"),
+                size=3,
+            )
+
+            + scale_color_manual(
+                values={
+                    "-2": "grey",
+                    "-1": "grey",
+                    "0": "black",
+                    "+1": "grey",
+                    "+2": "grey"
+                },
+            )
+            + scale_shape_manual(
+                name="Patterns",
+                values={
+                    "Below Limit": "X",
+                    "Above Limit": "X",
+                    "Low Run": "s",
+                    "High Run": "s",
+                    "Increasing Run": "^",
+                    "Decreasing Run": "v",
+                    "None": "."
+                },
+            )
+            + scale_linetype_manual(
+                name="Guideline",
+                values=dict(LCL="dashed", UCL="dashed", center="solid"),
+            )
+            + theme_minimal()
+            + guides(color=None)
+            + facet_grid(
+                "_var~.",
+                scales="free_y",
+                labeller=labeller(dict(X="Mean", S="Variability")),
+            )
+            + labs(
+                x="Group variable ({})".format(group),
+                y="Value ({})".format(var),
+            )
         )
-    )
 
 
 pt_xbs = add_pipe(plot_xbs)
```

### Comparing `py_grama-0.3.4/grama/string_helpers.py` & `py_grama-0.3.5/grama/string_helpers.py`

 * *Files identical despite different names*

### Comparing `py_grama-0.3.4/grama/support.py` & `py_grama-0.3.5/grama/support.py`

 * *Files 13% similar despite different names*

```diff
@@ -146,32 +146,33 @@
 
     Returns:
         DataFrame: dataset compacted with support points
 
     References:
         Mak and Joseph, "Support Points" (2018) *The Annals of Statistics*
 
-    Examples:
-        >>> import grama as gr
-        >>> # Compact an existing dataset
-        >>> from grama.data import df_diamonds
-        >>> df_sp = gr.tran_sp(df_diamonds, n=50, var=["price", "carat"])
-        >>>
-        >>> # Use support points to reduce model runtime
-        >>> from grama.models import make_cantilever_beam
-        >>> md_beam = make_cantilever_beam()
-        >>> (
-        >>>     md_beam
-        >>>     ## Generate input sample but don't evaluate outputs
-        >>>     >> gr.ev_sample(n=1e4, df_det="nom", skip=True)
-        >>>     ## Reduce to a smaller---but representative---sample
-        >>>     >> gr.tf_sp(n=50)
-        >>>     ## Evaluate the outputs
-        >>>     >> gr.tf_md(md_beam)
-        >>> )
+    Examples::
+
+        import grama as gr
+        # Compact an existing dataset
+        from grama.data import df_diamonds
+        df_sp = gr.tran_sp(df_diamonds, n=50, var=["price", "carat"])
+
+        # Use support points to reduce model runtime
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        (
+            md_beam
+            ## Generate input sample but don't evaluate outputs
+            >> gr.ev_sample(n=1e4, df_det="nom", skip=True)
+            ## Reduce to a smaller---but representative---sample
+            >> gr.tf_sp(n=50)
+            ## Evaluate the outputs
+            >> gr.tf_md(md_beam)
+        )
 
     """
     ## Setup
     setseed(seed)
     # Handle input variables
     if var is None:
         # Select numeric columns only
```

### Comparing `py_grama-0.3.4/grama/tools.py` & `py_grama-0.3.5/grama/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 __all__ = [
     "add_pipe",
     "copy_meta",
     "custom_formatwarning",
     "lookup",
+    "hide_traceback",
     "param_dist",
     "pipe",
     "valid_dist",
     "tran_outer",
     "tf_outer",
 ]
 
 import warnings
+import sys
 from functools import wraps
 from inspect import signature
 from numbers import Integral
 from numpy import empty
 from pandas import DataFrame, concat
 from pandas.core.dtypes.common import is_object_dtype
 from pandas._libs import (
@@ -336,26 +338,27 @@
     Args:
         df (DataFrame): Data to merge
         df_outer (DataFrame): Data to merge; outer
 
     Returns:
         DataFrame: Merged data
 
-    Examples:
-        >>> import grama as gr
-        >>> import pandas as pd
-        >>> df = pd.DataFrame(dict(x=[1,2]))
-        >>> df_outer = pd.DataFrame(dict(y=[3,4]))
-        >>> df_res = gr.tran_outer(df, df_outer)
-        >>> df_res
-        >>>    x  y
-        >>> 0  1  3
-        >>> 1  2  3
-        >>> 2  1  4
-        >>> 3  2  4
+    Examples::
+
+        import grama as gr
+        import pandas as pd
+        df = pd.DataFrame(dict(x=[1,2]))
+        df_outer = pd.DataFrame(dict(y=[3,4]))
+        df_res = gr.tran_outer(df, df_outer)
+        df_res
+             x  y
+          0  1  3
+          1  2  3
+          2  1  4
+          3  2  4
 
     """
     # Check invariants
     if (df.shape[0] == 0) and (df_outer.shape[0] == 0):
         raise ValueError("At least one of df and df_outer must be non-empty")
     # Handle single-empty cases
     if (df.shape[0] == 0):
@@ -411,7 +414,22 @@
             print(r,c)
             result[i] = df._get_value(r, c)
 
     if is_object_dtype(result):
         result = lib.maybe_convert_objects(result)
 
     return result
+
+
+# Suppress traceback
+def hide_traceback():
+    r"""Configure Jupyter to hide error traceback
+    """
+    ipython = get_ipython()
+
+    def _hide_traceback(exc_tuple=None, filename=None, tb_offset=None,
+                        exception_only=False, running_compiled_code=False):
+        etype, value, tb = sys.exc_info()
+        value.__cause__ = None  # suppress chained exceptions
+        return ipython._showtraceback(etype, value, ipython.InteractiveTB.get_exception_only(etype, value))
+
+    ipython.showtraceback = _hide_traceback
```

### Comparing `py_grama-0.3.4/grama/tran/tran_matminer.py` & `py_grama-0.3.5/grama/tran/tran_matminer.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,21 +44,22 @@
 
     Notes:
         - A pre-processor and wrapper for matminer.featurizers.composition
 
     References:
         Ward, L., Dunn, A., Faghaninia, A., Zimmermann, N. E. R., Bajaj, S., Wang, Q., Montoya, J. H., Chen, J., Bystrom, K., Dylla, M., Chard, K., Asta, M., Persson, K., Snyder, G. J., Foster, I., Jain, A., Matminer: An open source toolkit for materials data mining. Comput. Mater. Sci. 152, 60-69 (2018).
 
-    Examples:
-        >>> import grama as gr
-        >>> from grama.tran import tf_feat_composition
-        >>> (
-        >>>     gr.df_make(FORMULA=["C6H12O6"])
-        >>>     >> gr.tf_feat_composition()
-        >>> )
+    Examples::
+
+        import grama as gr
+        from grama.tran import tf_feat_composition
+        (
+            gr.df_make(FORMULA=["C6H12O6"])
+            >> gr.tf_feat_composition()
+        )
 
     """
     ## Check invariants
 
     ## Featurize
     try:
         featurizer = ElementProperty.from_preset(preset_name=preset_name)
```

### Comparing `py_grama-0.3.4/grama/tran/tran_scikitlearn.py` & `py_grama-0.3.5/grama/tran/tran_scikitlearn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 __all__ = [
     "tran_tsne",
     "tf_tsne",
-    "tran_poly",
-    "tf_poly",
+    # "tran_poly",
+    # "tf_poly",
 ]
 
 ## Transforms via sklearn package
 try:
     from sklearn.manifold import TSNE
-    from sklearn.preprocessing import PolynomialFeatures
+    # from sklearn.preprocessing import PolynomialFeatures
 
 except ModuleNotFoundError:
     pass
 
 from grama import add_pipe
 from pandas import concat, DataFrame
 from toolz import curry
@@ -99,71 +99,71 @@
 
     return df_res
 
 
 tf_tsne = add_pipe(tran_tsne)
 
 # --------------------------------------------------
-@curry
-def tran_poly(df, degree=None, var=None, keep=True, **kwargs):
-    r"""Compute polynomial features of a dataset
-
-    Compute polynomial features of a dataset.
-
-    Args:
-        df (DataFrame): Hybrid point results from gr.eval_hybrid()
-
-    Kwargs:
-        degree (int): Maximum degree of polynomial features
-        var (list or None): Variables in df on which to perform dimension reduction.
-            Use None to compute with all variables.
-        keep (bool): Keep unused columns (outside `var`) in new DataFrame?
-        interaction_only (bool): If true, only produce interaction features
-        include_bias (bool): If true, include a constant feature term (bias)
-
-    Notes:
-        - A wrapper for sklearn.preprocessing.PolynomialFeatures
-
-    References:
-        Scikit-learn: Machine Learning in Python, Pedregosa et al. JMLR 12, pp. 2825-2830, 2011.
-
-    Examples:
-
-    """
-    ## Check invariants
-    if var is None:
-        var = list(df.columns).copy()
-    else:
-        var = list(var).copy()
-        diff = set(var).difference(set(df.columns))
-        if len(diff) > 0:
-            raise ValueError(
-                "`var` must be subset of `df.columns`\n" "diff = {}".format(diff)
-            )
-    var_leftover = list(set(df.columns).difference(set(var)))
-
-    ## Compute the features
-    try:
-        fit = PolynomialFeatures(degree)
-
-    except NameError as e:
-        error_string = str(e)
-        raise NameError(
-            error_string +
-            "\n\nThis function requires the `sklearn` package. " +
-            "Try running the following to install the package:\n"
-            "    pip install scikit-learn"
-        )
-
-    X_feat = fit.fit_transform(df[var].values)
-    var_feat = fit.get_feature_names(var)
+# @curry
+# def tran_poly(df, degree=None, var=None, keep=True, **kwargs):
+#     r"""Compute polynomial features of a dataset
+
+#     Compute polynomial features of a dataset.
+
+#     Args:
+#         df (DataFrame): Hybrid point results from gr.eval_hybrid()
+
+#     Kwargs:
+#         degree (int): Maximum degree of polynomial features
+#         var (list or None): Variables in df on which to perform dimension reduction.
+#             Use None to compute with all variables.
+#         keep (bool): Keep unused columns (outside `var`) in new DataFrame?
+#         interaction_only (bool): If true, only produce interaction features
+#         include_bias (bool): If true, include a constant feature term (bias)
+
+#     Notes:
+#         - A wrapper for sklearn.preprocessing.PolynomialFeatures
+
+#     References:
+#         Scikit-learn: Machine Learning in Python, Pedregosa et al. JMLR 12, pp. 2825-2830, 2011.
+
+#     Examples:
+
+#     """
+#     ## Check invariants
+#     if var is None:
+#         var = list(df.columns).copy()
+#     else:
+#         var = list(var).copy()
+#         diff = set(var).difference(set(df.columns))
+#         if len(diff) > 0:
+#             raise ValueError(
+#                 "`var` must be subset of `df.columns`\n" "diff = {}".format(diff)
+#             )
+#     var_leftover = list(set(df.columns).difference(set(var)))
+
+#     ## Compute the features
+#     try:
+#         fit = PolynomialFeatures(degree)
+
+#     except NameError as e:
+#         error_string = str(e)
+#         raise NameError(
+#             error_string +
+#             "\n\nThis function requires the `sklearn` package. " +
+#             "Try running the following to install the package:\n"
+#             "    pip install scikit-learn"
+#         )
+
+#     X_feat = fit.fit_transform(df[var].values)
+#     var_feat = ["poly{}".format(i) for i in range(X_feat.shape[1])]
+
+#     ## Package results
+#     df_feat = DataFrame(data=X_feat, columns=var_feat)
 
-    ## Package results
-    df_feat = DataFrame(data=X_feat, columns=var_feat)
-
-    if keep:
-        return concat((df_feat, df[var_leftover].reset_index(drop=True)), axis=1)
+#     if keep:
+#         return concat((df_feat, df[var_leftover].reset_index(drop=True)), axis=1)
 
-    return df_feat
+#     return df_feat
 
 
-tf_poly = add_pipe(tran_poly)
+# tf_poly = add_pipe(tran_poly)
```

### Comparing `py_grama-0.3.4/grama/tran/tran_umap.py` & `py_grama-0.3.5/grama/tran/tran_umap.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,32 @@
 
     Kwargs:
         n_neighbors (int): A smaller value emphasizes local structure, larger value emphasizes global structure. Assumed number of nearest-neighbors in clusters. Coenen and Pearce claim this is the most important hyperparameter for UMAP. default=15
         min_dist (float): Minimum distance between mapped points. default=0.1
         metric (str or function): Metric used for distance computations. See url: https://umap-learn.readthedocs.io/en/latest/parameters.html#metric
 
     Notes:
-        - A wrapper for umap.UMAP
+        A wrapper for umap.UMAP
 
     References:
-        - McInnes, L, Healy, J, UMAP: Uniform Manifold Approximation and Projection for Dimension Reduction, ArXiv e-prints 1802.03426, 2018
-        - Andy Coenen, Adam Pearce "Understanding UMAP" url: https://pair-code.github.io/understanding-umap/
+        McInnes, L, Healy, J, UMAP: Uniform Manifold Approximation and Projection for Dimension Reduction, ArXiv e-prints 1802.03426, 2018
+        Andy Coenen, Adam Pearce "Understanding UMAP" url: https://pair-code.github.io/understanding-umap/
 
     Examples:
 
+        import grama as gr
+        from grama.data import df_diamonds
+        (
+            df_diamonds
+            >> gr.tf_sample(1000) # For speed
+            >> gr.tf_umap(var=["x", "y", "z", "carat"])
+            >> gr.ggplot(gr.aes("xi0", "xi1"))
+            + gr.geom_point()
+        )
+
     """
     ## Check invariants
     if var is None:
         var = list(df.columns).copy()
     else:
         var = list(var).copy()
         diff = set(var).difference(set(df.columns))
```

### Comparing `py_grama-0.3.4/grama/tran_is.py` & `py_grama-0.3.5/grama/tran_is.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,27 +15,19 @@
         md_base,
         md_new,
         var_weight="weight",
         append=True,
 ):
     r"""Reweight a sample using likelihood ratio
 
-    Reweight is a tool to facilitate "What If?" Monte Carlo simulation;
-    specifically, to make testing a models with the same function(s) but
-    different distributions more computationally efficient.
-
-    This tool automates calulation of the *likelihood ratio* between the
-    distributions of two given models. Using the resulting weights to scale
-    (elementwise multiply) output values and compute summaries is called
-    *importance sampling*, enabling "What If?" testing. Use of this tool enables
-    one to generate a single Monte Carlo sample, rather than multiple samples
-    for each "What If?" scenario (avoiding extraneous function evaluations).
+    Reweight is a tool to facilitate "What If?" Monte Carlo simulation; specifically, to make testing a models with the same function(s) but different distributions more computationally efficient.
 
-    Let `y` be a generic output of the scenario. The importance sampling
-    procedure is as follows:
+    This tool automates calulation of the *likelihood ratio* between the distributions of two given models. Using the resulting weights to scale (elementwise multiply) output values and compute summaries is called *importance sampling*, enabling "What If?" testing. Use of this tool enables one to generate a single Monte Carlo sample, rather than multiple samples for each "What If?" scenario (avoiding extraneous function evaluations).
+
+    Let `y` be a generic output of the scenario. The importance sampling procedure is as follows:
 
     1. Create a base scenario represented by `md_base`, and a desired number
        of alternative "What If?" scenarios represented my other models.
     2. Use `gr.eval_monte_carlo` to generate a single sample `df_base` of size `n`
        using the base scenario `md_base`. Compute statistics of interest on
        the output `y` for this base scenario.
     3. For each alternative scenario `md_new`, use `gr.tran_reweight` to
@@ -60,68 +52,67 @@
         - The base scenario `md_base` should have fatter tails than any of
           the scenarios considered as `df_new`. See Owen (2013) Chapter 9
           for more details.
 
     References:
         A.B. Owen, "Monte Carlo theory, methods and examples" (2013)
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.models import make_cantilever_beam
-        >>> DF = gr.Intention()
-        >>>
-        >>> md_base = make_cantilever_beam()
-        >>> md_new = (
-        >>>     md_base
-        >>>     >> gr.cp_marginals(
-        >>>         H=dict(dist="norm", loc=500.0, scale=50.0),
-        >>>     )
-        >>> )
-        >>>
-        >>> ## Assess safety via simple Monte Carlo
-        >>> df_base = gr.eval_monte_carlo(md_base, df_det="nom", n=1e3)
-        >>> print(
-        >>>     df_base
-        >>>     >> gr.tf_summarize(
-        >>>         pof_stress=gr.mean(DF.g_stress <= 0),
-        >>>         pof_disp=gr.mean(DF.g_disp <= 0),
-        >>>     )
-        >>> )
-        >>>
-        >>> ## Re-use samples to test another scenario
-        >>> print(
-        >>>     df_base
-        >>>     >> gr.tf_reweight(md_base=md_base, md_new=md_new)
-        >>>     >> gr.tf_summarize(
-        >>>         pof_stress=gr.mean((DF.g_stress <= 0) * DF.weight),
-        >>>         pof_disp=gr.mean((DF.g_disp <= 0) * DF.weight),
-        >>>         n_eff=gr.neff_is(DF.weight),
-        >>>     )
-        >>> )
-        >>>
-        >>> ## It is unsafe to study new scenarios with wider uncertainty than the base
-        >>> ## scenario
-        >>> md_poor = (
-        >>>     md_base
-        >>>     >> gr.cp_marginals(
-        >>>         H=dict(dist="norm", loc=500.0, scale=400.0),
-        >>>     )
-        >>> )
-        >>> ## Note the tiny effective size in this case
-        >>> print(
-        >>>     md_base
-        >>>     >> gr.ev_monte_carlo(n=1e3, df_det="nom")
-        >>>     >> gr.tf_reweight(md_base=md_base, md_new=md_poor)
-        >>>     >> gr.tf_summarize(
-        >>>         pof_stress=gr.mean((DF.g_stress <= 0) * DF.weight),
-        >>>         pof_disp=gr.mean((DF.g_disp <= 0) * DF.weight),
-        >>>         n_eff=gr.neff_is(DF.weight),
-        >>>     )
-        >>> )
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        DF = gr.Intention()
+
+        md_base = make_cantilever_beam()
+        md_new = (
+            md_base
+            >> gr.cp_marginals(
+                H=dict(dist="norm", loc=500.0, scale=50.0),
+            )
+        )
+
+        ## Assess safety via simple Monte Carlo
+        df_base = gr.eval_monte_carlo(md_base, df_det="nom", n=1e3)
+        print(
+            df_base
+            >> gr.tf_summarize(
+                pof_stress=gr.mean(DF.g_stress <= 0),
+                pof_disp=gr.mean(DF.g_disp <= 0),
+            )
+        )
+
+        ## Re-use samples to test another scenario
+        print(
+            df_base
+            >> gr.tf_reweight(md_base=md_base, md_new=md_new)
+            >> gr.tf_summarize(
+                pof_stress=gr.mean((DF.g_stress <= 0) * DF.weight),
+                pof_disp=gr.mean((DF.g_disp <= 0) * DF.weight),
+                n_eff=gr.neff_is(DF.weight),
+            )
+        )
+
+        ## It is unsafe to study new scenarios with wider uncertainty than the base scenario
+        md_poor = (
+            md_base
+            >> gr.cp_marginals(
+                H=dict(dist="norm", loc=500.0, scale=400.0),
+            )
+        )
+        ## Note the tiny effective sample size in this case
+        print(
+            md_base
+            >> gr.ev_monte_carlo(n=1e3, df_det="nom")
+            >> gr.tf_reweight(md_base=md_base, md_new=md_poor)
+            >> gr.tf_summarize(
+                pof_stress=gr.mean((DF.g_stress <= 0) * DF.weight),
+                pof_disp=gr.mean((DF.g_disp <= 0) * DF.weight),
+                n_eff=gr.neff_is(DF.weight),
+            )
+        )
 
     """
     ## Check invariants
     # Check that random inputs to md_base available in df_base
     var_diff = set(md_base.var_rand).difference(set(df_base.columns))
     if not (len(var_diff) == 0):
         raise ValueError(
```

### Comparing `py_grama-0.3.4/grama/tran_pivot.py` & `py_grama-0.3.5/grama/tran_pivot.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,54 +28,85 @@
     #names_transform = list(),
     #names_repair,
     values_to = None,
     #values_drop_na = False,
     #values_ptypes = list(),
     #values_transform = list(),
 ):
-    """
+    """Lengthen a dataset
 
     "Lengthens" data by increasing the number of rows and decreasing the
     number of columns.
 
     Args:
         df (DataFrame): DataFrame passed through
         columns (str): Label of column(s) to pivot into longer format
-        index_to(str): str name to create a new representation index of
-                        observations
+        index_to(str): str name to create a new representation index of observations; Optional.
         names_to (str): name to use for the 'variable' column, if None frame.columns.name
                         is used or ‘variable’
                           • .value indicates that component of the name defines
                             the name of the column containing the cell values,
                             overriding values_to
-        names_sep (str): delimter to seperate the values of the argument(s) from
+        names_sep (str OR list of int): delimter to seperate the values of the argument(s) from
                         the 'columns' parameter into 2 new columns with those
                         values split by that delimeter
                           • Regex expression is a valid input for names_sep
-        values_to (str): name to use for the 'value' column
+        names_pattern (str): Regular expression with capture groups to define targets for names_to.
+        values_to (str): name to use for the 'value' column; overridden if ".value" is provided in names_to argument.
+
+    Notes:
+        Only one of names_sep OR names_pattern may be given.
 
     Returns:
         DataFrame: result of being pivoted into a longer format
 
-    Examples:
+    Examples::
+
+        import grama as gr
+        ## Simple example
+        (
+            gr.df_make(
+                A=[1, 2, 3],
+                B=[4, 5, 6],
+                C=[7, 8, 9],
+            )
+            >> gr.tf_pivot_longer(
+                columns=["A", "B", "C"],
+                names_to="variable",
+                values_to="value",
+            )
+        )
+
+        ## Matching columns on patterns
+        (
+            gr.df_make(
+                x1=[1, 2, 3],
+                x2=[4, 5, 6],
+                x3=[7, 8, 9],
+            )
+            >> gr.tf_pivot_longer(
+                columns=gr.matches("\\d+"),
+                names_to="variable",
+                values_to="value",
+            )
+        )
 
-        >>> import grama as gr
-        >>> from pandas import DataFrame
-        >>> wide = DataFrame(
-                {
-                    "One": {"A": 1.0, "B": 2.0, "C": 3.0},
-                    "Two": {"A": 1.0, "B": 2.0, "C": 3.0},
-                }
-            )
-        >>> long = gr.tran_pivot_longer(
-                    wide,
-                    columns=("One","Two"),
-                    index_to="index",
-                    names_to="columns",
-                    values_to="values")
+        ## Separating column names and data on a names_pattern
+        (
+            gr.df_make(
+                E00=[1, 2, 3],
+                E45=[4, 5, 6],
+                E90=[7, 8, 9],
+            )
+            >> gr.tf_pivot_longer(
+                columns=gr.matches("\\d+"),
+                names_to=[".value", "angle"],
+                names_pattern="(E)(\\d+)",
+            )
+        )
 
     """
 
 
     ########### Pre-Check List #############
     ### Check if tran_select was used
     if isinstance(columns, DataFrame):
@@ -319,45 +350,40 @@
      #names_glue = None,
      #names_sort = False,
      #names_glue,
      values_from = None,
      #values_fill = None,
      #values_fn = None
  ):
-    """
+    """Widen a dataset
 
      "Widens" data by increasing the number of columns and decreasing the
      number of rows.
 
      Args:
          df (DataFrame): DataFrame passed through
          names_from (str): Column(s) name(s) to use to make new columns
          indexes_from (str): Column(s) to use to make new index, if None will
                              preserve and use unspecified columns as index
          values_from (str): Column(s) to use as new values column(s)
 
      Returns:
         DataFrame: result of being pivoted wider
 
-     Example:
-        >>> import grama as gr
-        >>> from pandas import DataFrame
-        >>> long = DataFrame(
-                {
-                    "index": ["A", "B", "C", "A", "B", "C"],
-                    "columns": ["One", "One", "One", "Two", "Two", "Two"],
-                    "values": [1.0, 2.0, 3.0, 1.0, 2.0, 3.0],
-                }
-            )
-        >>> wide = gr.tran_pivot_wider(
-                long,
-                indexes_from="index",
-                names_from="columns",
-                values_from="values"
+     Examples::
+
+        import grama as gr
+        ## Simple example
+        (
+            gr.df_make(var=["x", "x", "y", "y"], value=[0, 1, 2, 3])
+            >> gr.tf_pivot_wider(
+                names_from="var",
+                values_from="value",
             )
+        (
 
     """
 
     if indexes_from is None:
         ### Clean columns list to find unused columns and preserve them
         data_columns = df.columns
         data_values_used = values_from
@@ -497,17 +523,17 @@
 
     # rename columns
     for i,v in enumerate(names_to):
         longer.rename(columns={i: v},inplace=True)
 
     # if any values are None make them NaN
     for i,v in enumerate(names_to):
-        for j, w in enumerate(longer[names_to[i]]):
+        for j, w in enumerate(longer[names_to[i]].values):
             if w is None:
-                longer[names_to[i]][j] = NaN
+                longer[names_to[i]].values[j] = NaN
 
     # reorder values column to the end
     longer = longer[[c for c in longer if c not in values_to] + [values_to]]
 
     return longer
 
 
@@ -536,16 +562,16 @@
                 value=df[data_index[i]]
             )
 
     ### repair NaN values from transformation
     for index in data_index:
         length = len(df[index])
         for i, v in enumerate(longer[index]):
-            if isnull(longer[index][i]):
-                longer[index][i] = longer[index][i%length]
+            if isnull(longer[index].values[i]):
+                longer[index].values[i] = longer[index].values[i%length]
 
     return longer
 
 
 @group_delegation
 @symbolic_evaluation(eval_as_selector=True)
 def pivot_select(df, columns):
```

### Comparing `py_grama-0.3.4/grama/tran_shapley.py` & `py_grama-0.3.5/grama/tran_shapley.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,63 +19,56 @@
 
 
 ## Cohort Shapley
 @curry
 def tran_shapley_cohort(df, var=None, out=None, bins=20, inds=None):
     """Compute cohort shapley values
 
-    Assess the impact of each variable on selected observations via cohort
-    shapley [1]. Shapley values are a game-theoretic way to assess the
-    importance of input variables (var) on each of a set of outputs (out). Since
-    values are computed on each observation, cohort shapley can distinguish
-    cases where a variable has a positive impact on one observation, and a
-    negative impact on a different observation.
-
-    Note that cohort shapley is combinatorialy expensive in the number of
-    variables, and this expense is multiplied by the number of observations. Use
-    with caution in cases of high dimensionality. Consider using the `inds`
-    argument to analyze a small subset of your observations.
+    Assess the impact of each variable on selected observations via cohort shapley [1]. Shapley values are a game-theoretic way to assess the importance of input variables (var) on each of a set of outputs (out). Since values are computed on each observation, cohort shapley can distinguish cases where a variable has a positive impact on one observation, and a negative impact on a different observation.
+
+    Note that cohort shapley is combinatorialy expensive in the number of variables, and this expense is multiplied by the number of observations. Use with caution in cases of high dimensionality. Consider using the `inds` argument to analyze a small subset of your observations.
 
     Args:
         df (DataFrame): Variable and output data to analyze
         var (list of strings): Input variables
         out (list of strings): Outputs variables
         bins (integer): Number of "bins" to define coordinate refinement distance
         inds (iterable of indices or None): Indices of rows to analyze
 
     References:
-        - [1] Mase, Owen, and Seiler, "Explaining black box decisions by Shapley cohort refinement" (2019) Arxiv
+        [1] Mase, Owen, and Seiler, "Explaining black box decisions by Shapley cohort refinement" (2019) Arxiv
+
+    Examples::
 
-    Examples:
-        >>> import grama as gr
-        >>> from grama.data import df_stang
-        >>> X = gr.Intention()
-        >>> # Analyze all observations
-        >>> (
-        >>>     gr.tran_shapley_cohort(
-        >>>         df_stang,
-        >>>         var=["thick", "ang"],
-        >>>         out=["E"],
-        >>>     )
-        >>>     >> gr.tf_bind_cols(df_stang)
-        >>>     >> gr.tf_filter(X.E_thick < 0)
-        >>> )
-        >>> # Compute subset of values
-        >>> (
-        >>>     gr.tran_shapley_cohort(
-        >>>         df_stang,
-        >>>         var=["thick", "ang"],
-        >>>         out=["E"],
-        >>>         inds=(
-        >>>             df_stang
-        >>>             >> gr.tf_filter(X.thick > 0.08)
-        >>>         ).index
-        >>>     )
-        >>>     >> gr.tf_bind_cols(df_stang)
-        >>> )
+        import grama as gr
+        from grama.data import df_stang
+        DF = gr.Intention()
+        # Analyze all observations
+        (
+            gr.tran_shapley_cohort(
+                df_stang,
+                var=["thick", "ang"],
+                out=["E"],
+            )
+            >> gr.tf_bind_cols(df_stang)
+            >> gr.tf_filter(DF.E_thick < 0)
+        )
+        # Compute subset of values
+        (
+            gr.tran_shapley_cohort(
+                df_stang,
+                var=["thick", "ang"],
+                out=["E"],
+                inds=(
+                    df_stang
+                    >> gr.tf_filter(DF.thick > 0.08)
+                ).index
+            )
+            >> gr.tf_bind_cols(df_stang)
+        )
 
     """
     ## Check invariants
     if not set(var).issubset(set(df.columns)):
         raise ValueError("var must be subset of df.columns")
     if not set(out).issubset(set(df.columns)):
         raise ValueError("out must be subset of df.columns")
```

### Comparing `py_grama-0.3.4/grama/tran_summaries.py` & `py_grama-0.3.5/grama/tran_summaries.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,24 +51,24 @@
           T: Un-normalized index
           var: Total variance
 
     References:
         I.M. Sobol', "Sensitivity Estimates for Nonlinear Mathematical Models"
         (1999) MMCE, Vol 1.
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.models import make_cantilever_beam
-        >>> md = make_cantilever_beam()
-        >>> df_first = md >> gr.ev_hybrid(df_det="nom", plan="first")
-        >>> df_first >> gr.tf_sobol()
-        >>>
-        >>> df_total = md >> gr.ev_hybrid(df_det="nom", plan="total")
-        >>> df_total >> gr.tf_sobol()
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md = make_cantilever_beam()
+        df_first = md >> gr.ev_hybrid(df_det="nom", plan="first")
+        df_first >> gr.tf_sobol()
+
+        df_total = md >> gr.ev_hybrid(df_det="nom", plan="total")
+        df_total >> gr.tf_sobol()
 
     """
     ## Determine plan from dataframe metadata
     metadata = df._meta
     if metadata["type"] == "eval_hybrid":
         plan = metadata["plan"]
         varname = metadata["varname"]
@@ -148,14 +148,22 @@
     if not full:
         I_normalized = list(map(lambda s: s[0] == "S", df_res[typename]))
         df_res = df_res[I_normalized]
 
     ## Fill NaN's
     df_res.fillna(value=0, inplace=True)
 
+    ## Append metadata for autoplot dispatch
+    with catch_warnings():
+        simplefilter("ignore")
+        df_res._plot_info = {
+            "type": "sobol_outputs",
+            "idx": typename,
+        }
+
     return df_res
 
 
 tf_sobol = add_pipe(tran_sobol)
 
 ## Linear algebra tools
 ##################################################
@@ -175,19 +183,19 @@
 
     Returns:
         DataFrame: principal directions and eigenvalues
 
     References:
         TODO
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.data import df_stang
-        >>> df_pca = df_stang >> gr.tf_pca()
+        import grama as gr
+        from grama.data import df_stang
+        df_pca = df_stang >> gr.tf_pca()
 
     """
     ## Handle variable selection
     columns_numeric = list(df.select_dtypes("number").columns)
     if var is None:
         var = columns_numeric
     else:
@@ -210,37 +218,38 @@
 tf_pca = add_pipe(tran_pca)
 
 ## Gradient principal directions (AS)
 @curry
 def tran_asub(df, prefix="D", outvar="out", lamvar="lam"):
     r"""Active subspace estimator
 
-    Compute principal directions and eigenvalues for all outputs based on output
-    of ev_grad_fd() to estimate the /active subspace/ (Constantine, 2015).
+    Compute principal directions and eigenvalues for all outputs based on output of ev_grad_fd() to estimate the /active subspace/ (Constantine, 2015).
+
+    See also ``gr.tran_polyridge()`` for a gradient-free approach to approximating the active subspace.
 
     Args:
         df (DataFrame): Gradient evaluations
         prefix (str): Column name prefix; default="D"
         outvar (str): Name to give output id column; default="output"
         lambvar (str): Name to give eigenvalue column; default="lam"
 
     Returns:
         DataFrame: Active subspace directions and eigenvalues
 
     References:
         Constantine, "Active Subspaces" (2015) SIAM
 
-    Examples:
+    Examples::
 
-        >>> import grama as gr
-        >>> from grama.models import make_cantilever_beam
-        >>> md = make_cantilever_beam()
-        >>> df_base = md >> gr.ev_monte_carlo(n=1e2, df_det="nom", skip=True)
-        >>> df_grad = md >> gr.ev_grad_fd(df_base=df_base)
-        >>> df_as = df_grad >> gr.tf_asub()
+        import grama as gr
+        from grama.models import make_cantilever_beam
+        md = make_cantilever_beam()
+        df_base = md >> gr.ev_sample(n=1e2, df_det="nom", skip=True)
+        df_grad = md >> gr.ev_grad_fd(df_base=df_base)
+        df_as = df_grad >> gr.tf_asub()
 
     """
     ## Setup
     res = list(map(lambda s: s.split("_" + prefix, 1), df.columns))
     all_outputs = list(map(lambda r: re.sub("^" + prefix, "", r[0]), res))
     all_inputs = list(map(lambda r: r[1], res))
     outputs = list(set(all_outputs))
@@ -279,45 +288,55 @@
             default="dot"
         name (str): Name of identity column in df_weights or None
         append (bool): Append new data to original DataFrame?
 
     Returns:
         DataFrame: Results of inner products
 
-    Examples:
+    Examples::
+
+        ## Setup
+        import grama as gr
+        DF = gr.Intention()
+
+        ## PCA example
+        from grama.data import df_diamonds
+        # Compute PCA weights
+        df_weights = gr.tran_pca(
+            df_diamonds
+            >> gr.tf_sample(1000),
+            var=["x", "y", "z", "carat"],
+        )
+        # Visualize
+        (
+            df_diamonds
+            >> gr.tf_inner(df_weights=df_weights)
+            >> gr.ggplot(gr.aes("dot0", "dot1"))
+            + gr.geom_point()
+        )
 
-        >>> ## Setup
-        >>> from dfply import *
-        >>> import grama as gr
-        >>> from grama.models import make_cantilever_beam
-        >>> import seaborn as sns
-        >>> import matplotlib.pyplot as plt
-        >>> md = make_cantilever_beam()
-        >>> # Generate active subspace results
-        >>> df_base = md >> gr.ev_monte_carlo(n=1e2, df_det="nom")
-        >>> df_grad = md >> gr.ev_grad_fd(df_base=df_base)
-        >>> df_as = df_grad >> \
-        >>>     gr.tf_asub() >> \
-        >>>     group_by(X.out) >> \
-        >>>     mask(min_rank(-X.lam) == 1) >> \
-        >>>     ungroup()
-        >>> # Post-process
-        >>> df_reduce = gr.tran_inner(df_base, df_as, name="out")
-        >>> sns.scatterplot(
-        >>>     data=df_reduce,
-        >>>     x="dot_g_stress",
-        >>>     y="g_stress"
-        >>> )
-        >>> plt.show()
-        >>> sns.scatterplot(
-        >>>     data=df_reduce,
-        >>>     x="dot_g_disp",
-        >>>     y="g_disp"
-        >>> )
-        >>> plt.show()
+        ## Active subspace example
+        from grama.models import make_cantilever_beam
+        md_beam = make_cantilever_beam()
+        # Approximate the active subspace
+        df_data = gr.ev_sample(md_beam, n=1e2, df_det="nom")
+        df_weights = gr.tran_polyridge(
+            df_data,
+            var=md_beam.var_rand, # Use meaningful predictors only
+            out="g_disp",         # Target g_disp for reduction
+            n_degree=2,
+            n_degree=1,
+        )
+        # Construct shadow plot; use tran_inner to calculate active variable
+        (
+            df_data
+            >> gr.tf_inner(df_weights=df_weights)
+            >> gr.ggplot(gr.aes("dot", "g_disp"))
+            + gr.geom_point()
+        )
 
     """
     ## Check invariants
     if df_weights.shape[0] == 0:
         raise ValueError("df_weights cannot be empty")
     if isinstance(name, str):
         if not (name in df_weights.columns):
```

### Comparing `py_grama-0.3.4/py_grama.egg-info/PKG-INFO` & `py_grama-0.3.5/py_grama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grama
-Version: 0.3.4
+Version: 0.3.5
 Summary: A grammar of model analysis
 Home-page: https://github.com/zdelrosario/py_grama
 Author: Zachary del Rosario
 Author-email: zdelrosario@outlook.com
 License: MIT
 Description: # py_grama
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.02462/status.svg)](https://doi.org/10.21105/joss.02462) [![PyPI version](https://badge.fury.io/py/py-grama.svg)](https://badge.fury.io/py/py-grama) [![Documentation Status](https://readthedocs.org/projects/py_grama/badge/?version=latest)](https://py_grama.readthedocs.io/en/latest/?badge=latest) ![Python package test](https://github.com/zdelrosario/py_grama/workflows/Python%20package%20test/badge.svg) [![codecov](https://codecov.io/gh/zdelrosario/py_grama/branch/master/graph/badge.svg)](https://codecov.io/gh/zdelrosario/py_grama) [![CodeFactor](https://www.codefactor.io/repository/github/zdelrosario/py_grama/badge/master)](https://www.codefactor.io/repository/github/zdelrosario/py_grama/overview/master) 
@@ -76,16 +76,15 @@
         }
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8, <3.10
 Description-Content-Type: text/markdown
-Provides-Extra: lolo
 Provides-Extra: matminer
 Provides-Extra: sklearn
 Provides-Extra: statsmodels
 Provides-Extra: pyDOE
 Provides-Extra: umap
 Provides-Extra: dev
```

### Comparing `py_grama-0.3.4/setup.py` & `py_grama-0.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="py_grama",
     author="Zachary del Rosario",
     author_email="zdelrosario@outlook.com",
-    version="0.3.4",
+    version="0.3.5",
     packages=[
         "grama",
         "grama.data",
         "grama.dfply",
         "grama.eval",
         "grama.fit",
         "grama.models",
@@ -24,33 +24,31 @@
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8, <3.10",
     install_requires=[
         "matplotlib",
         "numpy>=1.15",
-        "pandas",
+        "pandas<=1.5.3",
         "plotnine>=0.8.0",
         "scipy",
         "toolz",
         "networkx",
     ],
     extras_require={
-        "lolo": ["lolopy"],
         "matminer": ["pymatgen==2021.2.8.1", "matminer"],
         "sklearn": ["scikit-learn"],
         "statsmodels": ["statsmodels"],
         "pyDOE": ["pyDOE"],
         "umap": ["umap-learn"],
         "dev": [
-            "lolopy",
             "pymatgen==2021.2.8.1",
             "matminer",
             "scikit-learn",
             "statsmodels",
             "pyDOE",
             "umap-learn",
         ],
```

