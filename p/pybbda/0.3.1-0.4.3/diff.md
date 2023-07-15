# Comparing `tmp/pybbda-0.3.1.tar.gz` & `tmp/pybbda-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybbda-0.3.1.tar", last modified: Sat Feb  6 17:37:55 2021, max compression
+gzip compressed data, was "pybbda-0.4.3.tar", last modified: Sat Jul 15 19:14:58 2023, max compression
```

## Comparing `pybbda-0.3.1.tar` & `pybbda-0.4.3.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (116)    18092 2021-02-06 17:37:47.000000 pybbda-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      182 2021-02-06 17:37:47.000000 pybbda-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     9432 2021-02-06 17:37:55.545724 pybbda-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7148 2021-02-06 17:37:47.000000 pybbda-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda/
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda/analysis/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda/analysis/projections/
--rw-r--r--   0 runner    (1001) docker     (116)      195 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/projections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda/analysis/projections/marcels/
--rw-r--r--   0 runner    (1001) docker     (116)      179 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/projections/marcels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      344 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/projections/marcels/age_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (116)    10181 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/projections/marcels/marcels_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1644 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/projections/marcels/marcels_batting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1986 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/projections/marcels/marcels_pitching.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda/analysis/run_expectancy/
--rw-r--r--   0 runner    (1001) docker     (116)      238 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/run_expectancy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda/analysis/run_expectancy/markov/
--rw-r--r--   0 runner    (1001) docker     (116)      155 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/run_expectancy/markov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4507 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/run_expectancy/markov/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    17372 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/run_expectancy/markov/markov.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda/analysis/simulations/
--rw-r--r--   0 runner    (1001) docker     (116)      810 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.541725 pybbda-0.3.1/pybbda/analysis/simulations/components/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4287 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/components/event.py
--rw-r--r--   0 runner    (1001) docker     (116)      984 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/components/lineup.py
--rw-r--r--   0 runner    (1001) docker     (116)     1425 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/components/player.py
--rw-r--r--   0 runner    (1001) docker     (116)     2469 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/components/player_registry.py
--rw-r--r--   0 runner    (1001) docker     (116)    14652 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/components/state.py
--rw-r--r--   0 runner    (1001) docker     (116)      123 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/simulations/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.541725 pybbda-0.3.1/pybbda/analysis/trajectories/
--rw-r--r--   0 runner    (1001) docker     (116)      334 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/trajectories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.541725 pybbda-0.3.1/pybbda/analysis/trajectories/batted_balls/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/trajectories/batted_balls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7689 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/trajectories/batted_balls/calculator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2489 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/trajectories/batted_balls/parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.541725 pybbda-0.3.1/pybbda/data/
--rw-r--r--   0 runner    (1001) docker     (116)      550 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.541725 pybbda-0.3.1/pybbda/data/sources/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.541725 pybbda-0.3.1/pybbda/data/sources/baseball_reference/
--rw-r--r--   0 runner    (1001) docker     (116)      214 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/baseball_reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1713 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/baseball_reference/_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     1461 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/baseball_reference/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.541725 pybbda-0.3.1/pybbda/data/sources/data_source/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1191 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/data_source/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/sources/fangraphs/
--rw-r--r--   0 runner    (1001) docker     (116)       45 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/fangraphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4880 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/fangraphs/_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     1251 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/fangraphs/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/fangraphs/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/sources/lahman/
--rw-r--r--   0 runner    (1001) docker     (116)      609 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/lahman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1519 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/lahman/_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     1668 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/lahman/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/sources/retrosheet/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/retrosheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3964 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/retrosheet/_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     3555 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/retrosheet/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/sources/statcast/
--rw-r--r--   0 runner    (1001) docker     (116)       44 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/statcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3869 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/statcast/_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     2100 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/statcast/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     4509 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/statcast/data.py
--rw-r--r--   0 runner    (1001) docker     (116)      732 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/sources/statcast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/tools/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/tools/fangraphs/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/fangraphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6857 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/fangraphs/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/tools/lahman/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/lahman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1405 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/lahman/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/data/tools/processing/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      107 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/processing/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (116)      426 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/processing/transform.py
--rw-r--r--   0 runner    (1001) docker     (116)     4565 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/data/tools/update.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.545724 pybbda-0.3.1/pybbda/utils/
--rw-r--r--   0 runner    (1001) docker     (116)       58 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      711 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/utils/html_table.py
--rw-r--r--   0 runner    (1001) docker     (116)      627 2021-02-06 17:37:47.000000 pybbda-0.3.1/pybbda/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 17:37:55.537724 pybbda-0.3.1/pybbda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9432 2021-02-06 17:37:55.000000 pybbda-0.3.1/pybbda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2715 2021-02-06 17:37:55.000000 pybbda-0.3.1/pybbda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-06 17:37:55.000000 pybbda-0.3.1/pybbda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      141 2021-02-06 17:37:55.000000 pybbda-0.3.1/pybbda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      100 2021-02-06 17:37:55.000000 pybbda-0.3.1/pybbda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-02-06 17:37:55.000000 pybbda-0.3.1/pybbda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      200 2021-02-06 17:37:47.000000 pybbda-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      190 2021-02-06 17:37:47.000000 pybbda-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-02-06 17:37:55.545724 pybbda-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1201 2021-02-06 17:37:47.000000 pybbda-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-15 19:14:47.000000 pybbda-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-15 19:14:47.000000 pybbda-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-15 19:14:58.889694 pybbda-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-07-15 19:14:47.000000 pybbda-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.881694 pybbda-0.4.3/pybbda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/projections/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/projections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/projections/marcels/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/projections/marcels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/projections/marcels/age_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/projections/marcels/marcels_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/projections/marcels/marcels_batting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/projections/marcels/marcels_pitching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/run_expectancy/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/run_expectancy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/run_expectancy/markov/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/run_expectancy/markov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/run_expectancy/markov/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/run_expectancy/markov/markov.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/simulations/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/components/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/components/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/components/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/components/player_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/components/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/simulations/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/trajectories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/analysis/trajectories/batted_balls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/trajectories/batted_balls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/trajectories/batted_balls/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/trajectories/batted_balls/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/data/sources/baseball_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/baseball_reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/baseball_reference/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/baseball_reference/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/data/sources/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/data_source/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/data/sources/fangraphs/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/fangraphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/fangraphs/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/fangraphs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/fangraphs/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/data/sources/lahman/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/lahman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/lahman/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/lahman/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.885694 pybbda-0.4.3/pybbda/data/sources/retrosheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/retrosheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/retrosheet/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/retrosheet/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/pybbda/data/sources/statcast/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/statcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/statcast/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/statcast/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/statcast/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/sources/statcast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/pybbda/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/pybbda/data/tools/fangraphs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/fangraphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/fangraphs/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/pybbda/data/tools/lahman/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/lahman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/lahman/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/pybbda/data/tools/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/processing/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/processing/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/data/tools/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/pybbda/graphics/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/graphics/graphical_standings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.889694 pybbda-0.4.3/pybbda/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/utils/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-15 19:14:47.000000 pybbda-0.4.3/pybbda/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:58.881694 pybbda-0.4.3/pybbda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-15 19:14:58.000000 pybbda-0.4.3/pybbda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-15 19:14:58.000000 pybbda-0.4.3/pybbda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 19:14:58.000000 pybbda-0.4.3/pybbda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-15 19:14:58.000000 pybbda-0.4.3/pybbda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-15 19:14:58.000000 pybbda-0.4.3/pybbda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 19:14:58.000000 pybbda-0.4.3/pybbda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-15 19:14:47.000000 pybbda-0.4.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-15 19:14:47.000000 pybbda-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-15 19:14:58.889694 pybbda-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-15 19:14:47.000000 pybbda-0.4.3/setup.py
```

### Comparing `pybbda-0.3.1/LICENSE` & `pybbda-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/README.md` & `pybbda-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/__init__.py` & `pybbda-0.4.3/pybbda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 import os
 import logging
 
 logging.basicConfig(format="%(levelname)s:%(name)s:%(module)s:%(message)s")
 logger = logging.getLogger("pybbda")
 
-_version = "0.3.1"
+_version = "0.4.3"
 
 PYBBDA_LOG_LEVEL_NAME = os.environ.get("PYBBDA_LOG_LEVEL", "")
 _PYBBDA_LOG_LEVEL_MAP = {
     "DEBUG": logging.DEBUG,
     "INFO": logging.INFO,
     "WARNING": logging.WARNING,
     "CRITICAL": logging.CRITICAL,
```

### Comparing `pybbda-0.3.1/pybbda/analysis/projections/marcels/marcels_base.py` & `pybbda-0.4.3/pybbda/analysis/projections/marcels/marcels_base.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/projections/marcels/marcels_batting.py` & `pybbda-0.4.3/pybbda/analysis/projections/marcels/marcels_batting.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/projections/marcels/marcels_pitching.py` & `pybbda-0.4.3/pybbda/analysis/projections/marcels/marcels_pitching.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/run_expectancy/markov/cli.py` & `pybbda-0.4.3/pybbda/analysis/run_expectancy/markov/cli.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/run_expectancy/markov/markov.py` & `pybbda-0.4.3/pybbda/analysis/run_expectancy/markov/markov.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/simulations/__init__.py` & `pybbda-0.4.3/pybbda/analysis/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/simulations/components/event.py` & `pybbda-0.4.3/pybbda/analysis/simulations/components/event.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/simulations/components/lineup.py` & `pybbda-0.4.3/pybbda/analysis/simulations/components/lineup.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/simulations/components/player.py` & `pybbda-0.4.3/pybbda/analysis/simulations/components/player.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/simulations/components/player_registry.py` & `pybbda-0.4.3/pybbda/analysis/simulations/components/player_registry.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/simulations/components/state.py` & `pybbda-0.4.3/pybbda/analysis/simulations/components/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,29 +30,27 @@
     def evolve(
         self,
         batting_event,
         first_base_running_event=FirstBaseRunningEvent.DEFAULT,
         second_base_running_event=SecondBaseRunningEvent.DEFAULT,
         third_base_running_event=ThirdBaseRunningEvent.DEFAULT,
     ):
-
         if batting_event == BattingEvent.OUT:
             base_state = attr.evolve(self)
 
         elif batting_event == BattingEvent.BASE_ON_BALLS:
             base_state = BaseState(
                 first_base=1,
                 second_base=1 if self.first_base == 1 else self.second_base,
                 third_base=1
                 if self.first_base == 1 and self.second_base == 1
                 else self.third_base,
             )
 
         elif batting_event == BattingEvent.SINGLE:
-
             running_events = get_running_events_cached(
                 batting_event,
                 first_base_running_event,
                 second_base_running_event,
                 third_base_running_event,
             )[0:2]
 
@@ -350,15 +348,14 @@
     def evolve(
         self,
         batting_event,
         first_base_running_event=FirstBaseRunningEvent.DEFAULT,
         second_base_running_event=SecondBaseRunningEvent.DEFAULT,
         third_base_running_event=ThirdBaseRunningEvent.DEFAULT,
     ):
-
         outs = self.outs
 
         if outs == self.max_outs:
             base_state = attr.evolve(self)
         elif batting_event == BattingEvent.OUT:
             outs = self.outs + 1
             if outs % INNING_OUTS == 0:
```

### Comparing `pybbda-0.3.1/pybbda/analysis/trajectories/batted_balls/calculator.py` & `pybbda-0.4.3/pybbda/analysis/trajectories/batted_balls/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         :param spin_angle: float
         :param launch_angle: float
         :param launch_direction_angle: float
         :return: numpy array
         """
         # trajectory_vars = x, y, z, vx, vy, vz
         _, _, _, vx, vy, vz = trajectory_vars
-        v = np.sqrt(vx ** 2 + vy ** 2 + vz ** 2)
+        v = np.sqrt(vx**2 + vy**2 + vz**2)
 
         sidespin = spin * sin_in_degrees(spin_angle)
         backspin = spin * cos_in_degrees(spin_angle)
 
         wb = backspin
         ws = sidespin
```

### Comparing `pybbda-0.3.1/pybbda/analysis/trajectories/batted_balls/parameters.py` & `pybbda-0.4.3/pybbda/analysis/trajectories/batted_balls/parameters.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/analysis/utils.py` & `pybbda-0.4.3/pybbda/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/__init__.py` & `pybbda-0.4.3/pybbda/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/sources/baseball_reference/_update.py` & `pybbda-0.4.3/pybbda/data/sources/baseball_reference/_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         logger.info("there was a download error code={}", response.status_code)
         raise FileNotFoundError
     it = response.iter_lines()
     return list(it)
 
 
 def _save(lines, file_name, output_path):
-
     output_file_path = os.path.join(output_path, file_name)
     output_payload = "\n".join(str(line, "utf-8") for line in lines)
     logger.info("saving file to {}".format(output_file_path))
     with gzip.open(output_file_path, "wb") as fh:
         fh.write(bytes(output_payload, encoding="utf-8"))
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/baseball_reference/data.py` & `pybbda-0.4.3/pybbda/data/sources/baseball_reference/data.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/sources/data_source/base.py` & `pybbda-0.4.3/pybbda/data/sources/data_source/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,16 +26,23 @@
             return full_path
         elif os.path.exists(full_path + ".gz"):
             return full_path + ".gz"
         else:
             raise FileNotFoundError(f"Cannot find file {full_path}")
 
     def _load(self, name):
-        file_full_path = self._locate_file(name)
-        return pd.read_csv(file_full_path)
+        if isinstance(name, str):
+            file_full_path = self._locate_file(name)
+            return pd.read_csv(file_full_path)
+        elif isinstance(name, list):
+            file_full_paths = [self._locate_file(n) for n in name]
+            dfs = [pd.read_csv(file_full_path) for file_full_path in file_full_paths]
+            return pd.concat(dfs, axis=0)
+        else:
+            raise TypeError
 
     def __getattr__(self, name):
         if name not in self.tables.keys():
             raise AttributeError
         try:
             self.__dict__[name] = self._load(name)
             return self.__dict__[name]
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/fangraphs/_update.py` & `pybbda-0.4.3/pybbda/data/sources/fangraphs/_update.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/sources/fangraphs/constants.py` & `pybbda-0.4.3/pybbda/data/sources/fangraphs/constants.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/sources/fangraphs/data.py` & `pybbda-0.4.3/pybbda/data/sources/fangraphs/data.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/sources/lahman/__init__.py` & `pybbda-0.4.3/pybbda/data/sources/lahman/__init__.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/sources/lahman/_update.py` & `pybbda-0.4.3/pybbda/data/sources/lahman/_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     archive.extractall(path=target)
     return target
 
 
 def _extract(target, output_root):
     output_path = os.path.join(output_root, "Lahman")
     os.makedirs(output_path, exist_ok=True)
-    extracted_files = glob.glob(os.path.join(target, "**", "*csv"), recursive=True)
+    extracted_files = glob.glob(
+        os.path.join(target, "baseballdatabank-master", "core", "*csv"), recursive=True
+    )
     for extracted_file in extracted_files:
         try:
             shutil.copy(extracted_file, output_path)
         except shutil.SameFileError:
             logger.warning(
                 "source and destination file (%s) are the same",
                 os.path.join(output_path, extracted_file),
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/lahman/data.py` & `pybbda-0.4.3/pybbda/data/sources/lahman/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import os
 import logging
+from pathlib import Path
 
 import pandas as pd
 
 from ..lahman import _LAHMAN_TABLES
 from pybbda import PYBBDA_DATA_ROOT
 from pybbda.utils.singleton import Singleton
 
@@ -17,15 +18,15 @@
     def __init__(self, data_path=None):
         """
 
         :param data_path:
         """
         if data_path is None:
             data_path = LAHMAN_DATA_PATH
-        self.data_path = data_path
+        self.data_path = Path(data_path)
         for file_name in _LAHMAN_TABLES:
             self.__setattr__(self._munge_attr_name(file_name), None)
 
     @staticmethod
     def _munge_attr_name(name):
         patts = [r"(^[a-z]{1})", r"_+([a-zA-Z]{1})"]
         for patt in patts:
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/retrosheet/_update.py` & `pybbda-0.4.3/pybbda/data/sources/retrosheet/_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 # TODO dry it up
 def _download_csv(url):
     logger.info("downloading file from {}".format(url))
     response = requests.get(url, stream=True)
     if response.status_code != 200:
-        logger.info("there was a download error code={}", response.status_code)
+        logger.info("there was a download error code=", response.status_code)
         raise FileNotFoundError
     it = response.iter_lines()
     return list(it)
 
 
 def _save(lines, file_name, output_path):
     output_file_path = os.path.join(output_path, file_name)
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/retrosheet/data.py` & `pybbda-0.4.3/pybbda/data/sources/retrosheet/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,27 @@
 
 from sqlalchemy import create_engine
 from pychadwick.chadwick import Chadwick
 from pybbda import PYBBDA_DATA_ROOT
 from pybbda.data.sources.data_source.base import DataSource
 
 RETROSHEET_DATA_PATH = PYBBDA_DATA_ROOT / "retrosheet"
-RETROSHEET_TABLES = {"people": "people.csv"}
-RETROSHEET_URLS = {
-    "people": "https://raw.githubusercontent.com/"
+RETROSHEET_TABLES = {"people": ["people{c}.csv" for c in "0123456789abcdef"]}
+
+RETROSHEET_URL_FMT = (
+    "https://raw.githubusercontent.com/"
     "chadwickbureau/"
     "register/"
     "master/"
     "data/"
-    "people.csv"
+    "people-{}.csv"
+)
+
+RETROSHEET_URLS = {
+    f"people{c}": RETROSHEET_URL_FMT.format(c) for c in "0123456789abcdef"
 }
 
 logger = logging.getLogger(__name__)
 
 
 class RetrosheetData(DataSource):
     _SOURCE_DATA_PATH = RETROSHEET_DATA_PATH
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/statcast/_update.py` & `pybbda-0.4.3/pybbda/data/sources/statcast/_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,14 @@
         overwrite=overwrite,
     )
 
 
 def _update(
     output_root=None, min_date=None, max_date=None, num_threads=2, overwrite=False
 ):
-
     today = datetime.date.today()
     min_date = min_date or (today - datetime.timedelta(1)).strftime("%Y-%m-%d")
     max_date = max_date or today.strftime("%Y-%m-%d")
 
     output_root = (
         output_root or pathlib.Path(__file__).absolute().parent.parent / "assets"
     )
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/statcast/constants.py` & `pybbda-0.4.3/pybbda/data/sources/statcast/constants.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/sources/statcast/data.py` & `pybbda-0.4.3/pybbda/data/sources/statcast/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 import datetime
+import io
+import requests
 
 import pandas as pd
 
 from .constants import (
     STATCAST_PBP_DAILY_URL_FORMAT,
     STATCAST_PBP_PLAYER_URL_FORMAT,
     STATCAST_PBP_DAILY_DF_DATA_TYPES,
@@ -63,15 +65,16 @@
                 "player_type": player_type,
                 "season": start_date[0:4],
                 "start_date": start_date,
                 "end_date": end_date,
             }
         )
 
-        daily_df = pd.read_csv(url)
+        file_handle = io.BytesIO(requests.get(url).content)
+        daily_df = pd.read_csv(file_handle)
         if len(daily_df) == STATCAST_QUERY_DATA_SIZE_LIMIT:
             logger.warning(
                 "Statcast query returned %d rows which probably "
                 "means you've exceeded the data limit. "
                 "You should try to break up the query.",
                 STATCAST_QUERY_DATA_SIZE_LIMIT,
             )
```

### Comparing `pybbda-0.3.1/pybbda/data/sources/statcast/utils.py` & `pybbda-0.4.3/pybbda/data/sources/statcast/utils.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/tools/fangraphs/data.py` & `pybbda-0.4.3/pybbda/data/tools/fangraphs/data.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/tools/lahman/data.py` & `pybbda-0.4.3/pybbda/data/tools/lahman/data.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/data/tools/update.py` & `pybbda-0.4.3/pybbda/data/tools/update.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/utils/html_table.py` & `pybbda-0.4.3/pybbda/utils/html_table.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda/utils/singleton.py` & `pybbda-0.4.3/pybbda/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `pybbda-0.3.1/pybbda.egg-info/SOURCES.txt` & `pybbda-0.4.3/pybbda.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,10 +63,12 @@
 pybbda/data/tools/fangraphs/__init__.py
 pybbda/data/tools/fangraphs/data.py
 pybbda/data/tools/lahman/__init__.py
 pybbda/data/tools/lahman/data.py
 pybbda/data/tools/processing/__init__.py
 pybbda/data/tools/processing/aggregate.py
 pybbda/data/tools/processing/transform.py
+pybbda/graphics/__init__.py
+pybbda/graphics/graphical_standings.py
 pybbda/utils/__init__.py
 pybbda/utils/html_table.py
 pybbda/utils/singleton.py
```

### Comparing `pybbda-0.3.1/setup.py` & `pybbda-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 with open("requirements.txt", "r") as fh:
     install_requires = [process_line(line) for line in fh.readlines() if len(line) > 1]
 
 setup(
     name="pybbda",
-    version="0.3.1",
+    version="0.4.3",
     author="Ben Dilday",
     author_email="ben.dilday.phd@gmail.com",
     description="Baseball data and analysis in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bdilday/pybbda",
     packages=find_packages(),
```

