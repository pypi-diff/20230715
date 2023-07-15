# Comparing `tmp/seismic-rna-0.1.3.tar.gz` & `tmp/seismic-rna-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-rna-0.1.3.tar", last modified: Fri Jul  7 23:32:23 2023, max compression
+gzip compressed data, was "seismic-rna-0.2.0.tar", last modified: Sat Jul 15 03:49:40 2023, max compression
```

## Comparing `seismic-rna-0.1.3.tar` & `seismic-rna-0.2.0.tar`

### file list

```diff
@@ -1,114 +1,117 @@
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.157153 seismic-rna-0.1.3/
--rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.1.3/LICENSE
--rw-r--r--   0 mfa        (503) staff       (20)     1882 2023-07-07 23:32:23.156853 seismic-rna-0.1.3/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     1319 2023-07-07 17:58:57.000000 seismic-rna-0.1.3/README.md
--rw-r--r--   0 mfa        (503) staff       (20)     1015 2023-07-07 19:47:31.000000 seismic-rna-0.1.3/pyproject.toml
--rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-07 23:32:23.157233 seismic-rna-0.1.3/setup.cfg
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.684454 seismic-rna-0.1.3/src/
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.807356 seismic-rna-0.1.3/src/seismic_rna.egg-info/
--rw-r--r--   0 mfa        (503) staff       (20)     1882 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     2954 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/SOURCES.txt
--rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/dependency_links.txt
--rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/entry_points.txt
--rw-r--r--   0 mfa        (503) staff       (20)      164 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/requires.txt
--rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/top_level.txt
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.699011 seismic-rna-0.1.3/src/seismicrna/
--rw-r--r--   0 mfa        (503) staff       (20)      171 2023-07-07 22:10:20.000000 seismic-rna-0.1.3/src/seismicrna/__init__.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.735159 seismic-rna-0.1.3/src/seismicrna/align/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.1.3/src/seismicrna/align/fq2bam.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/fqutil.py
--rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-06-29 21:22:27.000000 seismic-rna-0.1.3/src/seismicrna/align/main.py
--rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/strandedness.py
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/test.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.794325 seismic-rna-0.1.3/src/seismicrna/cluster/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     9128 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/compare.py
--rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/em.py
--rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/krun.py
--rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1874 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/main.py
--rw-r--r--   0 mfa        (503) staff       (20)      384 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/names.py
--rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.866107 seismic-rna-0.1.3/src/seismicrna/core/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.1.3/src/seismicrna/core/bitcall.py
--rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.1.3/src/seismicrna/core/bitvect.py
--rw-r--r--   0 mfa        (503) staff       (20)    23907 2023-07-07 02:41:42.000000 seismic-rna-0.1.3/src/seismicrna/core/cli.py
--rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.1.3/src/seismicrna/core/depend.py
--rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/docdef.py
--rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/docstring.py
--rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/dump.py
--rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/files.py
--rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.1.3/src/seismicrna/core/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.1.3/src/seismicrna/core/logs.py
--rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/mu.py
--rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.1.3/src/seismicrna/core/mu_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-06-29 19:37:32.000000 seismic-rna-0.1.3/src/seismicrna/core/parallel.py
--rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.1.3/src/seismicrna/core/path.py
--rw-r--r--   0 mfa        (503) staff       (20)    29386 2023-06-29 17:35:09.000000 seismic-rna-0.1.3/src/seismicrna/core/rel.py
--rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.1.3/src/seismicrna/core/rel_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    29608 2023-07-07 22:47:17.000000 seismic-rna-0.1.3/src/seismicrna/core/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/rna.py
--rw-r--r--   0 mfa        (503) staff       (20)    26188 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/sect.py
--rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.1.3/src/seismicrna/core/sect_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.1.3/src/seismicrna/core/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.1.3/src/seismicrna/core/seq_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.1.3/src/seismicrna/core/shell.py
--rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.1.3/src/seismicrna/core/sim.py
--rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.1.3/src/seismicrna/core/sim_test.py
--rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/types.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.1.3/src/seismicrna/core/xam.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.886709 seismic-rna-0.1.3/src/seismicrna/demult/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/demult/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    42588 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/demult/demultiplex.py
--rw-r--r--   0 mfa        (503) staff       (20)     2073 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/demult/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.938855 seismic-rna-0.1.3/src/seismicrna/draw/
--rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.1.3/src/seismicrna/draw/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/load_dataset.py
--rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/manipulator.py
--rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.1.3/src/seismicrna/draw/plotter.py
--rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/study.py
--rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/util.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.986300 seismic-rna-0.1.3/src/seismicrna/graph/
--rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     8667 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     3249 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/color.py
--rw-r--r--   0 mfa        (503) staff       (20)     2700 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/default.py
--rw-r--r--   0 mfa        (503) staff       (20)     7441 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/hist.py
--rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     8608 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     9491 2023-07-07 17:48:44.000000 seismic-rna-0.1.3/src/seismicrna/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.013069 seismic-rna-0.1.3/src/seismicrna/mask/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/mask/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     4068 2023-07-07 22:49:27.000000 seismic-rna-0.1.3/src/seismicrna/mask/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     4321 2023-07-06 23:44:35.000000 seismic-rna-0.1.3/src/seismicrna/mask/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/mask/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    14001 2023-07-06 23:57:39.000000 seismic-rna-0.1.3/src/seismicrna/mask/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.079074 seismic-rna-0.1.3/src/seismicrna/relate/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/export.py
--rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     3175 2023-06-30 04:06:44.000000 seismic-rna-0.1.3/src/seismicrna/relate/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/relate.py
--rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.1.3/src/seismicrna/relate/sam.py
--rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/seqpos.py
--rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/test.py
--rw-r--r--   0 mfa        (503) staff       (20)    15021 2023-06-30 04:03:22.000000 seismic-rna-0.1.3/src/seismicrna/relate/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.099741 seismic-rna-0.1.3/src/seismicrna/struct/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/struct/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3905 2023-06-29 20:47:08.000000 seismic-rna-0.1.3/src/seismicrna/struct/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1862 2023-06-29 20:23:36.000000 seismic-rna-0.1.3/src/seismicrna/struct/rnastructure.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.144297 seismic-rna-0.1.3/src/seismicrna/table/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     7405 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     5929 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1520 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    14642 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/tabulate.py
--rw-r--r--   0 mfa        (503) staff       (20)     4841 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.156415 seismic-rna-0.1.3/src/seismicrna/test/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/test/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.1.3/src/seismicrna/test/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.506955 seismic-rna-0.2.0/
+-rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.2.0/LICENSE
+-rw-r--r--   0 mfa        (503) staff       (20)     1930 2023-07-15 03:49:40.506597 seismic-rna-0.2.0/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     1367 2023-07-09 21:54:37.000000 seismic-rna-0.2.0/README.md
+-rw-r--r--   0 mfa        (503) staff       (20)     1034 2023-07-14 03:05:41.000000 seismic-rna-0.2.0/pyproject.toml
+-rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-15 03:49:40.507065 seismic-rna-0.2.0/setup.cfg
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.880285 seismic-rna-0.2.0/src/
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.893599 seismic-rna-0.2.0/src/seismic_rna.egg-info/
+-rw-r--r--   0 mfa        (503) staff       (20)     1930 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     3014 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/entry_points.txt
+-rw-r--r--   0 mfa        (503) staff       (20)      176 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/requires.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/top_level.txt
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.909350 seismic-rna-0.2.0/src/seismicrna/
+-rw-r--r--   0 mfa        (503) staff       (20)      171 2023-07-07 22:10:20.000000 seismic-rna-0.2.0/src/seismicrna/__init__.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.947381 seismic-rna-0.2.0/src/seismicrna/align/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/align/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.2.0/src/seismicrna/align/fq2bam.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/align/fqutil.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/align/main.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/align/strandedness.py
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/align/test.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.011993 seismic-rna-0.2.0/src/seismicrna/cluster/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    12885 2023-07-11 14:25:48.000000 seismic-rna-0.2.0/src/seismicrna/cluster/compare.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/em.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/krun.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2464 2023-07-12 20:23:19.000000 seismic-rna-0.2.0/src/seismicrna/cluster/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1264 2023-07-15 00:22:05.000000 seismic-rna-0.2.0/src/seismicrna/cluster/names.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.206074 seismic-rna-0.2.0/src/seismicrna/core/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.2.0/src/seismicrna/core/bitcall.py
+-rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.2.0/src/seismicrna/core/bitvect.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18246 2023-07-15 03:16:29.000000 seismic-rna-0.2.0/src/seismicrna/core/cli.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.2.0/src/seismicrna/core/depend.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/docdef.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/docstring.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/dump.py
+-rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/files.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.2.0/src/seismicrna/core/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.2.0/src/seismicrna/core/logs.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/mu.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.2.0/src/seismicrna/core/mu_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-07-12 20:28:15.000000 seismic-rna-0.2.0/src/seismicrna/core/parallel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.2.0/src/seismicrna/core/path.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29387 2023-07-14 20:09:45.000000 seismic-rna-0.2.0/src/seismicrna/core/rel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.2.0/src/seismicrna/core/rel_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29740 2023-07-12 04:26:52.000000 seismic-rna-0.2.0/src/seismicrna/core/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/rna.py
+-rw-r--r--   0 mfa        (503) staff       (20)    27329 2023-07-09 16:52:06.000000 seismic-rna-0.2.0/src/seismicrna/core/sect.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.2.0/src/seismicrna/core/sect_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.2.0/src/seismicrna/core/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.2.0/src/seismicrna/core/seq_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.2.0/src/seismicrna/core/shell.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.2.0/src/seismicrna/core/sim.py
+-rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.2.0/src/seismicrna/core/sim_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/types.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.2.0/src/seismicrna/core/xam.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.226177 seismic-rna-0.2.0/src/seismicrna/demult/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/demult/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    42624 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/demult/demultiplex.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2103 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/demult/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.276729 seismic-rna-0.2.0/src/seismicrna/draw/
+-rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.2.0/src/seismicrna/draw/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/load_dataset.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/manipulator.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.2.0/src/seismicrna/draw/plotter.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/study.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/util.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.319723 seismic-rna-0.2.0/src/seismicrna/graph/
+-rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/graph/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8731 2023-07-14 21:02:58.000000 seismic-rna-0.2.0/src/seismicrna/graph/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3539 2023-07-15 02:04:52.000000 seismic-rna-0.2.0/src/seismicrna/graph/color.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2701 2023-07-12 18:10:50.000000 seismic-rna-0.2.0/src/seismicrna/graph/default.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7483 2023-07-14 03:47:40.000000 seismic-rna-0.2.0/src/seismicrna/graph/hist.py
+-rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/graph/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    13371 2023-07-15 03:18:18.000000 seismic-rna-0.2.0/src/seismicrna/graph/seq.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.326149 seismic-rna-0.2.0/src/seismicrna/logo/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-07-09 20:01:37.000000 seismic-rna-0.2.0/src/seismicrna/logo/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3492 2023-07-12 02:42:12.000000 seismic-rna-0.2.0/src/seismicrna/logo/logo.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9517 2023-07-12 20:26:39.000000 seismic-rna-0.2.0/src/seismicrna/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.361295 seismic-rna-0.2.0/src/seismicrna/mask/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/mask/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4074 2023-07-08 00:07:16.000000 seismic-rna-0.2.0/src/seismicrna/mask/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4447 2023-07-09 18:20:20.000000 seismic-rna-0.2.0/src/seismicrna/mask/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/mask/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14001 2023-07-06 23:57:39.000000 seismic-rna-0.2.0/src/seismicrna/mask/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.430951 seismic-rna-0.2.0/src/seismicrna/relate/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/export.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3203 2023-07-09 18:21:57.000000 seismic-rna-0.2.0/src/seismicrna/relate/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/relate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.2.0/src/seismicrna/relate/sam.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/seqpos.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15085 2023-07-10 03:02:51.000000 seismic-rna-0.2.0/src/seismicrna/relate/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.450355 seismic-rna-0.2.0/src/seismicrna/struct/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/struct/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3937 2023-07-09 20:18:58.000000 seismic-rna-0.2.0/src/seismicrna/struct/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1850 2023-07-09 19:43:33.000000 seismic-rna-0.2.0/src/seismicrna/struct/rnastructure.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.492896 seismic-rna-0.2.0/src/seismicrna/table/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/table/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9414 2023-07-15 00:14:41.000000 seismic-rna-0.2.0/src/seismicrna/table/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7236 2023-07-15 00:22:19.000000 seismic-rna-0.2.0/src/seismicrna/table/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1724 2023-07-12 20:21:49.000000 seismic-rna-0.2.0/src/seismicrna/table/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    16181 2023-07-15 00:02:34.000000 seismic-rna-0.2.0/src/seismicrna/table/tabulate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4684 2023-07-15 00:02:34.000000 seismic-rna-0.2.0/src/seismicrna/table/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.506089 seismic-rna-0.2.0/src/seismicrna/test/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/test/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.2.0/src/seismicrna/test/main.py
```

### Comparing `seismic-rna-0.1.3/LICENSE` & `seismic-rna-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/PKG-INFO` & `seismic-rna-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.3
+Version: 0.2.0
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,16 @@
 
 
 # SEISMIC-RNA
 
 RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and
 Clustering
 
+![Logo of SEISMIC-RNA](logo.png "SEISMIC-RNA")
+
 
 ## About
 
 SEISMIC-RNA analyzes deep sequencing datasets from RNA mutational profiling
 experiments, such as [DMS-MaPseq](https://www.nature.com/articles/nmeth.4057)
 and [SHAPE-MaP](https://www.nature.com/articles/nmeth.3029).
 This software introduces an optimized implementation of the original algorithm
```

### Comparing `seismic-rna-0.1.3/README.md` & `seismic-rna-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 # SEISMIC-RNA
 
 RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and
 Clustering
 
+![Logo of SEISMIC-RNA](logo.png "SEISMIC-RNA")
+
 
 ## About
 
 SEISMIC-RNA analyzes deep sequencing datasets from RNA mutational profiling
 experiments, such as [DMS-MaPseq](https://www.nature.com/articles/nmeth.4057)
 and [SHAPE-MaP](https://www.nature.com/articles/nmeth.3029).
 This software introduces an optimized implementation of the original algorithm
```

### Comparing `seismic-rna-0.1.3/pyproject.toml` & `seismic-rna-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-rna"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
     {name="Matty Allan"},
     {name="Yves Martin"},
     {name="Scott Grote"},
     {name="Alberic de Lajarte"},
 ]
 description = "RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering"
@@ -16,14 +16,15 @@
 requires-python = ">=3.10"
 license = {text = "GPL-3.0-only"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "brotli>=1.0",
     "click>=8.1",
     "cutadapt>=4.4",
     "fastqsplitter>=1.2",
     "matplotlib>=3.6",
     "numpy>=1.23",
     "pandas>=1.5",
     "plotly>=5.11",
```

### Comparing `seismic-rna-0.1.3/src/seismic_rna.egg-info/PKG-INFO` & `seismic-rna-0.2.0/src/seismic_rna.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.3
+Version: 0.2.0
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,16 @@
 
 
 # SEISMIC-RNA
 
 RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and
 Clustering
 
+![Logo of SEISMIC-RNA](logo.png "SEISMIC-RNA")
+
 
 ## About
 
 SEISMIC-RNA analyzes deep sequencing datasets from RNA mutational profiling
 experiments, such as [DMS-MaPseq](https://www.nature.com/articles/nmeth.4057)
 and [SHAPE-MaP](https://www.nature.com/articles/nmeth.3029).
 This software introduces an optimized implementation of the original algorithm
```

### Comparing `seismic-rna-0.1.3/src/seismic_rna.egg-info/SOURCES.txt` & `seismic-rna-0.2.0/src/seismic_rna.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 src/seismicrna/graph/__init__.py
 src/seismicrna/graph/base.py
 src/seismicrna/graph/color.py
 src/seismicrna/graph/default.py
 src/seismicrna/graph/hist.py
 src/seismicrna/graph/main.py
 src/seismicrna/graph/seq.py
+src/seismicrna/logo/__init__.py
+src/seismicrna/logo/logo.py
 src/seismicrna/mask/__init__.py
 src/seismicrna/mask/load.py
 src/seismicrna/mask/main.py
 src/seismicrna/mask/report.py
 src/seismicrna/mask/write.py
 src/seismicrna/relate/__init__.py
 src/seismicrna/relate/export.py
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/align/fq2bam.py` & `seismic-rna-0.2.0/src/seismicrna/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/align/fqutil.py` & `seismic-rna-0.2.0/src/seismicrna/align/fqutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,18 +60,18 @@
       from one reference sequence in one sample
     """
 
     MAX_PHRED_ENC = 127  # 2^7 - 1
 
     KEY_SINGLE = "fastqs"
     KEY_INTER = "fastqi"
-    KEY_MATED = "fastqm"
+    KEY_MATED = "fastqp"
     KEY_DSINGLE = "dmfastqs"
     KEY_DINTER = "dmfastqi"
-    KEY_DMATED = "dmfastqm"
+    KEY_DMATED = "dmfastqp"
     KEY_MATE1 = "fastq1"
     KEY_MATE2 = "fastq2"
 
     BOWTIE2_FLAGS = {KEY_SINGLE: "-U",
                      KEY_INTER: "--interleaved",
                      KEY_MATE1: "-1",
                      KEY_MATE2: "-2"}
@@ -275,18 +275,18 @@
         ----------
         phred_enc: int
             ASCII offset for encoding Phred scores
         fastq_args: list[Path]
             FASTQ files, given as lists of paths:
             - fastqs: FASTQ files of single-end reads
             - fastqi: FASTQ files of interleaved paired-end reads
-            - fastqm: mated FASTQ files of paired-end reads
+            - fastqp: mated FASTQ files of paired-end reads
             - dmfastqs: demultiplexed FASTQ files of single-end reads
             - dmfastqi: demultiplexed FASTQ files of interleaved paired-end reads
-            - dmfastqm: demultiplexed mated FASTQ files of paired-end reads
+            - dmfastqp: demultiplexed mated FASTQ files of paired-end reads
 
         Yield
         -----
         FastqUnit
             FastqUnit representing the FASTQ or pair of FASTQ files.
             The order is determined primarily by the order of keyword
             arguments; within each keyword argument, by the order of
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/align/main.py` & `seismic-rna-0.2.0/src/seismicrna/align/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from click import command
 
 from .fq2bam import get_bam_files
 from .fqutil import FastqUnit
 from ..core import docdef, path
 from ..core.cli import (opt_fasta,
-                        opt_fastqs, opt_fastqi, opt_fastqm,
-                        opt_dmfastqs, opt_dmfastqi, opt_dmfastqm,
+                        opt_fastqs, opt_fastqi, opt_fastqp,
+                        opt_dmfastqs, opt_dmfastqi, opt_dmfastqp,
                         opt_phred_enc,
                         opt_out_dir, opt_temp_dir,
                         opt_rerun, opt_save_temp,
                         opt_parallel, opt_max_procs,
                         opt_fastqc, opt_qc_extract,
                         opt_cutadapt,
                         opt_cut_a1, opt_cut_g1, opt_cut_a2, opt_cut_g2,
@@ -36,18 +36,18 @@
 
 # Parameters for command line interface
 params = [
     # Inputs
     opt_fasta,
     opt_fastqs,
     opt_fastqi,
-    opt_fastqm,
+    opt_fastqp,
     opt_dmfastqs,
     opt_dmfastqi,
-    opt_dmfastqm,
+    opt_dmfastqp,
     opt_phred_enc,
     # Outputs
     opt_out_dir,
     opt_temp_dir,
     opt_rerun,
     opt_save_temp,
     # Parallelization
@@ -102,18 +102,18 @@
 @lock_temp_dir
 @docdef.auto()
 def run(*,
         # Inputs
         fasta: str,
         fastqs: tuple[str, ...],
         fastqi: tuple[str, ...],
-        fastqm: tuple[str, ...],
+        fastqp: tuple[str, ...],
         dmfastqs: tuple[str, ...],
         dmfastqi: tuple[str, ...],
-        dmfastqm: tuple[str, ...],
+        dmfastqp: tuple[str, ...],
         phred_enc: int,
         # Outputs
         out_dir: str,
         temp_dir: str,
         save_temp: bool,
         rerun: bool,
         # Parallelization
@@ -179,18 +179,18 @@
 
     # FASTQ files of read sequences may come from up to seven different
     # sources (i.e. each argument beginning with "fq_unit"). This step
     # collects all of them into one list (fq_units) and also bundles
     # together pairs of FASTQ files containing mate 1 and mate 2 reads.
     fq_units = list(FastqUnit.from_paths(fastqs=list(map(Path, fastqs)),
                                          fastqi=list(map(Path, fastqi)),
-                                         fastqm=list(map(Path, fastqm)),
+                                         fastqp=list(map(Path, fastqp)),
                                          dmfastqs=list(map(Path, dmfastqs)),
                                          dmfastqi=list(map(Path, dmfastqi)),
-                                         dmfastqm=list(map(Path, dmfastqm)),
+                                         dmfastqp=list(map(Path, dmfastqp)),
                                          phred_enc=phred_enc))
 
     # Generate and return a BAM file for every FASTQ-reference pair.
     return get_bam_files(fq_units=fq_units,
                          fasta=Path(fasta),
                          out_dir=Path(out_dir),
                          temp_dir=Path(temp_dir),
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/align/strandedness.py` & `seismic-rna-0.2.0/src/seismicrna/align/strandedness.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/cluster/compare.py` & `seismic-rna-0.2.0/src/seismicrna/cluster/compare.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 Cluster Comparison Module
 ========================================================================
 Auth: Matty
 
 Collect and compare the results from independent runs of EM clustering.
 """
 
+from __future__ import annotations
+
 from itertools import combinations
+from typing import Callable, Iterable
 
 import numpy as np
 import pandas as pd
 
 from .em import EmClustering
 from .names import EXP_NAME, OBS_NAME, ORD_NAME
 
@@ -208,7 +211,93 @@
         # Variation of information defaults to 0 if no pairs exist.
         return 0.
     # Find the mean variation of information among pairs of EM runs.
     # FIXME: This part can be made more computationally efficient by caching each resps and each props1 and props2.
     return sum(calc_var_info_run_pair(runs[i1].output_resps(),
                                       runs[i2].output_resps())
                for i1, i2 in pairs) / len(pairs)
+
+
+def iter_all_likelihoods(p: np.ndarray):
+    """ Yield every bit vector likelihood from greatest to least. """
+    if p.ndim != 1:
+        raise ValueError(f"p must have 1 dimension, but got {p.ndim}")
+    # If no bits remain, then just return the base value.
+    if p.size == 0:
+        return iter([0.])
+    if np.min(p) < 0. or np.max(p) > 1.:
+        raise ValueError(f"p must all be in [0, 1], but got {p}")
+    # Remove any bits that are certain to be 0 or 1.
+    p = p[np.logical_not(np.logical_or(p == 0., p == 1.))]
+    # If no bits remain, then just return the base value.
+    if p.size == 0:
+        return iter([0.])
+    # Compute the log probabilities (p) and anti-probabilities (q).
+    log_p = np.log(p)
+    log_q = np.log(1. - p)
+    # Sum the larger of the two as the "base" weight.
+    log_base = float(np.sum(np.maximum(log_p, log_q)))
+    # Compute the difference in logs and sort from least to greatest.
+    log_diffs = np.abs(log_p - log_q)
+    log_diffs.sort()
+
+    class LikelihoodSeries(object):
+
+        def __init__(self, weight: float, inner: Callable[[], Iterable]):
+            self._weight = weight
+            self._inner = inner
+            self._values = list()
+
+        def _cache(self, value: float):
+            """ Store a value in the values list. """
+            self._values.append(value)
+            return value
+
+        def iter(self):
+            """ Iterate over the values. """
+            # Check if the values were already computed.
+            if self._values:
+                # If the values were already computed, then yield them.
+                yield from self._values
+            else:
+                # Otherwise, make iterators for the inner series and the
+                # weighted series.
+                inner = iter(self._inner())
+                weighted = iter(ival - self._weight for ival in self._inner())
+                # Get the first element from each iterator. Both should
+                # have > 0 items and should not raise StopIteration.
+                ival = next(inner)
+                wval = next(weighted)
+                # Yield elements until the both iterators are exhausted.
+                while True:
+                    # Yield the larger value and advance its iterator.
+                    if ival is not None and ival >= wval:
+                        # Yield the inner value.
+                        yield self._cache(ival)
+                        # Get the next inner value, or None if empty.
+                        ival = next(inner, None)
+                    else:
+                        # Yield the weighted value.
+                        yield self._cache(wval)
+                        try:
+                            # Get the next weighted value, if any.
+                            wval = next(weighted)
+                        except StopIteration:
+                            # There are no more weighted values.
+                            break
+                # Confirm that there are no more inner values.
+                try:
+                    next(inner)
+                except StopIteration:
+                    # There are no more inner values: success.
+                    return
+                # There were more inner values: failure.
+                raise ValueError(
+                    "Weighted values were exhausted before inner values")
+
+    # Make series of log likelihoods.
+    series = LikelihoodSeries(log_diffs[0], lambda: [0.])
+    for log_diff in log_diffs[1:]:
+        series = LikelihoodSeries(log_diff, series.iter)
+
+    # Return an iterator of log likelihood values adjusted by the base.
+    return iter(value + log_base for value in series.iter())
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/cluster/em.py` & `seismic-rna-0.2.0/src/seismicrna/cluster/em.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/cluster/krun.py` & `seismic-rna-0.2.0/src/seismicrna/cluster/krun.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/cluster/load.py` & `seismic-rna-0.2.0/src/seismicrna/cluster/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/cluster/report.py` & `seismic-rna-0.2.0/src/seismicrna/cluster/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/cluster/write.py` & `seismic-rna-0.2.0/src/seismicrna/cluster/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/bitcall.py` & `seismic-rna-0.2.0/src/seismicrna/core/bitcall.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/bitvect.py` & `seismic-rna-0.2.0/src/seismicrna/core/bitvect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/cli.py` & `seismic-rna-0.2.0/src/seismicrna/core/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,521 +24,678 @@
 BOWTIE2_ORIENT_FR = "fr"
 BOWTIE2_ORIENT_RF = "rf"
 BOWTIE2_ORIENT_FF = "ff"
 BOWTIE2_ORIENT = BOWTIE2_ORIENT_FR, BOWTIE2_ORIENT_RF, BOWTIE2_ORIENT_FF
 
 ADAPTER_SEQ_ILLUMINA_3P = "AGATCGGAAGAGC"
 
-FORMAT_ORC = "orc"
-FORMAT_PARQ = "parquet"
-FORMATS_APACHE = FORMAT_ORC, FORMAT_PARQ
+CLUST_INDIV = "indiv"
+CLUST_ORDER = "order"
+CLUST_UNITE = "unite"
+CLUST_ARRANGE_OPTIONS = CLUST_INDIV, CLUST_ORDER, CLUST_UNITE
+
 
 # Configuration options
-opt_config = Option(("--config", "-c"),
-                    type=Path(exists=True, dir_okay=False),
-                    help="Configuration file for parameters")
+opt_config = Option(
+    ("--config", "-g"),
+    type=Path(exists=True, dir_okay=False),
+    help="Configuration file for parameters")
 
 # Input/output options
-opt_out_dir = Option(("--out-dir", "-o"),
-                     type=Path(file_okay=False),
-                     default=os.path.join(".", "out"),
-                     help="Where to output all finished files")
-opt_temp_dir = Option(("--temp-dir",),
-                      type=Path(file_okay=False),
-                      default=os.path.join(".", "temp"),
-                      help="Where to write all temporary files")
-opt_save_temp = Option(("--save-temp/--no-save-temp",),
-                       type=bool,
-                       default=False,
-                       help=("Whether to save temporary files when the "
-                             "program exits"))
+
+opt_input_file = Option(
+    ("--input-file", "-i"),
+    type=Path(exists=True),
+    multiple=True,
+    default=(),
+    help="File containing input data")
+
+opt_out_dir = Option(
+    ("--out-dir", "-o"),
+    type=Path(file_okay=False),
+    default=os.path.join(".", "out"),
+    help="Where to output all finished files")
+
+opt_temp_dir = Option(
+    ("--temp-dir", "-t"),
+    type=Path(file_okay=False),
+    default=os.path.join(".", "temp"),
+    help="Where to write all temporary files")
+
+opt_save_temp = Option(
+    ("--save-temp/--no-save-temp",),
+    type=bool,
+    default=False,
+    help=("Whether to save temporary files when the "
+          "program exits"))
 
 # Resource usage options
-opt_parallel = Option(("--parallel/--no-parallel",),
-                      type=bool,
-                      default=True,
-                      help="Whether to run multiple tasks in parallel")
-opt_max_procs = Option(("--max-procs",),
-                       type=int,
-                       default=NUM_CPUS,
-                       help="Maximum number of simultaneous processes")
+opt_parallel = Option(
+    ("--parallel/--no-parallel",),
+    type=bool,
+    default=True,
+    help="Whether to run multiple tasks in parallel")
+
+opt_max_procs = Option(
+    ("--max-procs",),
+    type=int,
+    default=NUM_CPUS,
+    help="Maximum number of simultaneous processes")
 
 # Experiment and analysis setup options
-opt_library = Option(("--library", "-L"),
-                     type=Path(dir_okay=False),
-                     default="",
-                     help="Library CSV file")
-opt_samples = Option(("--samples", "-S"),
-                     type=Path(dir_okay=False),
-                     default="",
-                     help="Samples file")
-opt_rerun = Option(("--rerun/--no-rerun",),
-                   type=bool,
-                   default=False,
-                   help="Whether to regenerate files that already exist")
+
+opt_sections_file = Option(
+    ("--sections-file", "-s"),
+    type=Path(dir_okay=False),
+    default="",
+    help="CSV file of sections by name, reference, and coordinates/primers")
+
+opt_samples = Option(
+    ("--samples", "-S"),
+    type=Path(dir_okay=False),
+    default="",
+    help="Samples file")
+
+opt_rerun = Option(
+    ("--rerun/--no-rerun",),
+    type=bool,
+    default=False,
+    help="Whether to regenerate files that already exist")
 
 # Reference sequence (FASTA) files
-opt_fasta = Option(("--fasta", "-a"),
-                   type=Path(exists=True, dir_okay=False),
-                   help="FASTA file of all reference sequences")
+opt_fasta = Option(
+    ("--fasta", "-a"),
+    type=Path(exists=True, dir_okay=False),
+    help="FASTA file of all reference sequences")
 
 # Sequencing read (FASTQ) files
-opt_fastqs = Option(("--fastqs", "-s"),
-                    type=Path(exists=True),
-                    multiple=True,
-                    default=(),
-                    help="FASTQ files of single-end reads")
-opt_fastqi = Option(("--fastqi", "-i"),
-                    type=Path(exists=True),
-                    multiple=True,
-                    default=(),
-                    help="FASTQ files of interleaved paired reads")
-opt_fastqm = Option(("--fastqm", "-m"),
-                    type=Path(exists=True),
-                    multiple=True,
-                    default=(),
-                    help="FASTQ files of mate 1 and mate 2 paired-end reads")
+opt_fastqs = Option(
+    ("--fastqs", "-x"),
+    type=Path(exists=True),
+    multiple=True,
+    default=(),
+    help="FASTQ files of single-end reads")
+
+opt_fastqi = Option(
+    ("--fastqi", "-y"),
+    type=Path(exists=True),
+    multiple=True,
+    default=(),
+    help="FASTQ files of paired-end reads interleaved in 1 file")
+
+opt_fastqp = Option(
+    ("--fastqp", "-z"),
+    type=Path(exists=True),
+    multiple=True,
+    default=(),
+    help="FASTQ files of paired-end reads separated into 2 files")
 
 # Sequencing read (FASTQ/BAM) options
-opt_phred_enc = Option(("--phred-enc",),
-                       type=int,
-                       default=DEFAULT_PHRED_ENC,
-                       help="Phred score encoding in FASTQ/SAM/BAM files")
-opt_min_phred = Option(("--min-phred",),
-                       type=int,
-                       default=DEFAULT_MIN_PHRED,
-                       help="Minimum Phred score to use a base call")
-opt_fastqc = Option(("--fastqc/--no-fastqc",),
-                    type=bool,
-                    default=True,
-                    help="Whether to check quality of FASTQ files")
-opt_qc_extract = Option(("--qc-extract/--qc-no-extract",),
-                        type=bool,
-                        default=False,
-                        help="Whether to unzip FASTQC reports")
+opt_phred_enc = Option(
+    ("--phred-enc",),
+    type=int,
+    default=DEFAULT_PHRED_ENC,
+    help="Phred score encoding in FASTQ/SAM/BAM files")
+
+opt_min_phred = Option(
+    ("--min-phred",),
+    type=int,
+    default=DEFAULT_MIN_PHRED,
+    help="Minimum Phred score to use a base call")
+
+opt_fastqc = Option(
+    ("--fastqc/--no-fastqc",),
+    type=bool,
+    default=True,
+    help="Whether to check quality of FASTQ files")
+
+opt_qc_extract = Option(
+    ("--qc-extract/--qc-no-extract",),
+    type=bool,
+    default=False,
+    help="Whether to unzip FASTQC reports")
 
 # Demultiplexing options
 
-opt_demultiplex = Option(("--demult-on/--demult-off",),
-                         type=bool,
-                         default=False,
-                         help="Whether to run demultiplexing")
-
-opt_parallel_demultiplexing = Option(("--parallel_demultiplexing",),
-                                     type=bool,
-                                     default=False,
-                                     help="Whether to run demultiplexing at maximum speed by submitting multithreaded "
-                                          "grep functions")
-
-opt_clipped_demultiplexing = Option(("--clipped",),
-                                    type=int,
-                                    default=0,
-                                    help="Designates the amount of clipped patterns to search for in the sample, will raise compution time")
-
-opt_mismatch_tolerence = Option(("--mismatch_tolerence",),
-                                type=int,
-                                default=0,
-                                help="Designates the allowable amount of mismatches allowed in a string and still be considered a valid pattern find. \
+opt_demultiplex = Option(
+    ("--demult-on/--demult-off",),
+    type=bool,
+    default=False,
+    help="Whether to run demultiplexing")
+
+opt_parallel_demultiplexing = Option(
+    ("--parallel-demultiplexing",),
+    type=bool,
+    default=False,
+    help="Whether to run demultiplexing at maximum speed by submitting multithreaded "
+         "grep functions")
+
+opt_clipped_demultiplexing = Option(
+    ("--clipped",),
+    type=int,
+    default=0,
+    help="Designates the amount of clipped patterns to search for in the sample, will raise compution time")
+
+opt_mismatch_tolerence = Option(
+    ("--mismatch-tolerence",),
+    type=int,
+    default=0,
+    help="Designates the allowable amount of mismatches allowed in a string and still be considered a valid pattern find. \
                             will increase non-parallel computation at a factorial rate. use caution going above 2 mismatches. does not apply to clipped sequences.")
 
-opt_index_tolerence = Option(("--index_tolerance",),
-                             type=int,
-                             default=0,
-                             help="Designates the allowable amount of distance you allow the pattern to be found in a read from the reference index")
-
-opt_barcode_start = Option(("--barcode-start",),
-                           type=int,
-                           default=0,
-                           help="index of start of barcode")
-opt_barcode_length = Option(("--barcode-length",),
-                            type=int,
-                            default=0,
-                            help="length of barcode")
-opt_demulti_overwrite = Option(("--demulti-overwrite",),
-                               type=bool,
-                               default=False,
-                               help="desiginates whether to overwrite the grepped fastq. should only be used if changing setting on the same sample")
+opt_index_tolerence = Option(
+    ("--index-tolerance",),
+    type=int,
+    default=0,
+    help="Designates the allowable amount of distance you allow the pattern to be found in a read from the reference index")
+
+opt_barcode_start = Option(
+    ("--barcode-start",),
+    type=int,
+    default=0,
+    help="index of start of barcode")
+
+opt_barcode_length = Option(
+    ("--barcode-length",),
+    type=int,
+    default=0,
+    help="length of barcode")
+
+opt_demulti_overwrite = Option(
+    ("--demulti-overwrite",),
+    type=bool,
+    default=False,
+    help="desiginates whether to overwrite the grepped fastq. should only be used if changing setting on the same sample")
 
 # Demultiplexed sequencing read (FASTQ) directories
-opt_dmfastqs = Option(("--dmfastqs", "-S"),
-                      type=Path(exists=True, file_okay=False),
-                      multiple=True,
-                      default=(),
-                      help="Demultiplexed FASTQ files of single-end reads")
-opt_dmfastqi = Option(("--dmfastqi", "-I"),
-                      type=Path(exists=True, file_okay=False),
-                      multiple=True,
-                      default=(),
-                      help="Demultiplexed FASTQ files of interleaved paired-end reads")
-opt_dmfastqm = Option(("--dmfastqm", "-M"),
-                      type=Path(exists=True, file_okay=False),
-                      multiple=True,
-                      default=(),
-                      help="Demultiplexed FASTQ files of mate 1 and mate 2 reads")
-
-# Alignment map (BAM) files
-opt_bam = Option(("--bam", "-b"),
-                 type=Path(exists=True),
-                 multiple=True,
-                 default=(),
-                 help="BAM files")
+opt_dmfastqs = Option(
+    ("--dmfastqs", "-X"),
+    type=Path(exists=True, file_okay=False),
+    multiple=True,
+    default=(),
+    help="Demultiplexed FASTQ files of single-end reads")
+
+opt_dmfastqi = Option(
+    ("--dmfastqi", "-Y"),
+    type=Path(exists=True, file_okay=False),
+    multiple=True,
+    default=(),
+    help="Demultiplexed FASTQ files of paired-end reads interleaved in one file")
+
+opt_dmfastqp = Option(
+    ("--dmfastqp", "-Z"),
+    type=Path(exists=True, file_okay=False),
+    multiple=True,
+    default=(),
+    help="Demultiplexed FASTQ files of mate 1 and mate 2 reads")
 
 # Adapter trimming options with Cutadapt
-opt_cutadapt = Option(("--cut/--no-cut",),
-                      type=bool,
-                      default=True,
-                      help="Whether to trim reads with Cutadapt before alignment")
-opt_cut_q1 = Option(("--cut-q1",),
-                    type=int,
-                    default=DEFAULT_MIN_PHRED,
-                    help="Phred score for read 1 quality trimming")
-opt_cut_q2 = Option(("--cut-q2",),
-                    type=int,
-                    default=DEFAULT_MIN_PHRED,
-                    help="Phred score for read 2 quality trimming")
-opt_cut_g1 = Option(("--cut-g1",),
-                    type=str,
-                    multiple=True,
-                    default=(),
-                    help="5' adapter for read 1")
-opt_cut_a1 = Option(("--cut-a1",),
-                    type=str,
-                    multiple=True,
-                    default=(ADAPTER_SEQ_ILLUMINA_3P,),
-                    help="3' adapter for read 1")
-opt_cut_g2 = Option(("--cut-g2",),
-                    type=str,
-                    multiple=True,
-                    default=(),
-                    help="5' adapter for read 2")
-opt_cut_a2 = Option(("--cut-a2",),
-                    type=str,
-                    multiple=True,
-                    default=(ADAPTER_SEQ_ILLUMINA_3P,),
-                    help="3' adapter for read 2")
-opt_cut_o = Option(("--cut-O",),
-                   type=int,
-                   default=6,
-                   help="Minimum overlap of read and adapter")
-opt_cut_e = Option(("--cut-e",),
-                   type=float,
-                   default=0.1,
-                   help="Error tolerance for adapters")
-opt_cut_indels = Option(("--cut-indels/--cut-no-indels",),
-                        type=bool,
-                        default=True,
-                        help="Whether to allow indels in adapters")
-opt_cut_nextseq = Option(("--cut-nextseq/--cut-no-nextseq",),
-                         type=bool,
-                         default=False,
-                         help="Whether to trim high-quality Gs from 3' end")
+opt_cutadapt = Option(
+    ("--cut/--no-cut",),
+    type=bool,
+    default=True,
+    help="Whether to trim reads with Cutadapt before alignment")
+
+opt_cut_q1 = Option(
+    ("--cut-q1",),
+    type=int,
+    default=DEFAULT_MIN_PHRED,
+    help="Phred score for read 1 quality trimming")
+
+opt_cut_q2 = Option(
+    ("--cut-q2",),
+    type=int,
+    default=DEFAULT_MIN_PHRED,
+    help="Phred score for read 2 quality trimming")
+
+opt_cut_g1 = Option(
+    ("--cut-g1",),
+    type=str,
+    multiple=True,
+    default=(),
+    help="5' adapter for read 1")
+
+opt_cut_a1 = Option(
+    ("--cut-a1",),
+    type=str,
+    multiple=True,
+    default=(ADAPTER_SEQ_ILLUMINA_3P,),
+    help="3' adapter for read 1")
+
+opt_cut_g2 = Option(
+    ("--cut-g2",),
+    type=str,
+    multiple=True,
+    default=(),
+    help="5' adapter for read 2")
+
+opt_cut_a2 = Option(
+    ("--cut-a2",),
+    type=str,
+    multiple=True,
+    default=(ADAPTER_SEQ_ILLUMINA_3P,),
+    help="3' adapter for read 2")
+
+opt_cut_o = Option(
+    ("--cut-O",),
+    type=int,
+    default=6,
+    help="Minimum overlap of read and adapter")
+
+opt_cut_e = Option(
+    ("--cut-e",),
+    type=float,
+    default=0.1,
+    help="Error tolerance for adapters")
+
+opt_cut_indels = Option(
+    ("--cut-indels/--cut-no-indels",),
+    type=bool,
+    default=True,
+    help="Whether to allow indels in adapters")
+
+opt_cut_nextseq = Option(
+    ("--cut-nextseq/--cut-no-nextseq",),
+    type=bool,
+    default=False,
+    help="Whether to trim high-quality Gs from 3' end")
+
 opt_cut_discard_trimmed = Option(
     ("--cut-discard-trimmed/--cut-keep-trimmed",),
     type=bool,
     default=False,
     help="Whether to discard reads in which an adapter was found")
+
 opt_cut_discard_untrimmed = Option(
     ("--cut-discard-untrimmed/--cut-keep-untrimmed",),
     type=bool,
     default=False,
     help="Whether to discard reads in which no adapter was found")
-opt_cut_m = Option(("--cut-m",),
-                   type=int,
-                   default=20,
-                   help="Discard reads shorter than this length after trimming")
+
+opt_cut_m = Option(
+    ("--cut-m",),
+    type=int,
+    default=20,
+    help="Discard reads shorter than this length after trimming")
 
 # Alignment options with Bowtie2
-opt_bt2_local = Option(("--bt2-local/--bt2-end-to-end",),
-                       type=bool,
-                       default=True,
-                       help="Whether to perform local or end-to-end alignment. "
-                            "Use local with fragmented samples, on which "
-                            "end-to-end yields false positives at read ends. "
-                            "Use end-to-end with amplicon-based samples, on "
-                            "which local yields false negatives at read ends.")
-opt_bt2_discordant = Option(("--bt2-discordant/--bt2-no-discordant",),
-                            type=bool,
-                            default=False,
-                            help="Whether to output discordant alignments")
-opt_bt2_mixed = Option(("--bt2-mixed/--bt2-no-mixed",),
-                       type=bool,
-                       default=False,
-                       help="Whether to align individual mates of unaligned pairs")
-opt_bt2_dovetail = Option(("--bt2-dovetail/--bt2-no-dovetail",),
-                          type=bool,
-                          default=False,
-                          help="Whether to treat dovetailed mate pairs as concordant")
-opt_bt2_contain = Option(("--bt2-contain/--bt2-no-contain",),
-                         type=bool,
-                         default=True,
-                         help="Whether to treat nested mate pairs as concordant")
-opt_bt2_unal = Option(("--bt2-unal/--bt2-no-unal",),
-                      type=bool,
-                      default=False,
-                      help="Whether to output unaligned reads")
-opt_bt2_i = Option(("--bt2-I",),
-                   type=int,
-                   default=0,
-                   help="Minimum fragment length for valid paired-end alignments")
-opt_bt2_x = Option(("--bt2-X",),
-                   type=int,
-                   default=600,
-                   help="Maximum fragment length for valid paired-end alignments")
-opt_bt2_score_min_e2e = Option(("--bt2-score-min-e2e",),
-                               type=str,
-                               default="L,-1,-0.5",
-                               help="Minimum score for a valid end-to-end alignment")
-opt_bt2_score_min_loc = Option(("--bt2-score-min-loc",),
-                               type=str,
-                               default="L,1,0.5",
-                               help="Minimum score for a valid local alignment")
-opt_bt2_s = Option(("--bt2-i", "bt2_s"),
-                   type=str,
-                   default="L,1,0.1",
-                   help="Seed interval")
-opt_bt2_l = Option(("--bt2-L",),
-                   type=int,
-                   default=12,
-                   help="Seed length")
-opt_bt2_gbar = Option(("--bt2-gbar",),
-                      type=int,
-                      default=4,
-                      help="Minimum distance of a gap from end of a read")
-opt_bt2_d = Option(("--bt2-D",),
-                   type=int,
-                   default=4,
-                   help="Maximum number of failed seed extensions")
-opt_bt2_r = Option(("--bt2-R",),
-                   type=int,
-                   default=2,
-                   help="Maximum number of times to re-seed")
-opt_bt2_dpad = Option(("--bt2-dpad",),
-                      type=int,
-                      default=2,
-                      help="Width of padding on alignment matrix, to allow gaps")
-opt_bt2_orient = Option(("--bt2-orient",),
-                        type=Choice(BOWTIE2_ORIENT, case_sensitive=False),
-                        default=BOWTIE2_ORIENT[0],
-                        help="Valid orientations of paired-end mates")
+opt_bt2_local = Option(
+    ("--bt2-local/--bt2-end-to-end",),
+    type=bool,
+    default=True,
+    help="Whether to perform local or end-to-end alignment. "
+         "Use local with fragmented samples, on which "
+         "end-to-end yields false positives at read ends. "
+         "Use end-to-end with amplicon-based samples, on "
+         "which local yields false negatives at read ends.")
+
+opt_bt2_discordant = Option(
+    ("--bt2-discordant/--bt2-no-discordant",),
+    type=bool,
+    default=False,
+    help="Whether to output discordant alignments")
+
+opt_bt2_mixed = Option(
+    ("--bt2-mixed/--bt2-no-mixed",),
+    type=bool,
+    default=False,
+    help="Whether to align individual mates of unaligned pairs")
+
+opt_bt2_dovetail = Option(
+    ("--bt2-dovetail/--bt2-no-dovetail",),
+    type=bool,
+    default=False,
+    help="Whether to treat dovetailed mate pairs as concordant")
+
+opt_bt2_contain = Option(
+    ("--bt2-contain/--bt2-no-contain",),
+    type=bool,
+    default=True,
+    help="Whether to treat nested mate pairs as concordant")
+
+opt_bt2_unal = Option(
+    ("--bt2-unal/--bt2-no-unal",),
+    type=bool,
+    default=False,
+    help="Whether to output unaligned reads")
+
+opt_bt2_i = Option(
+    ("--bt2-I",),
+    type=int,
+    default=0,
+    help="Minimum fragment length for valid paired-end alignments")
+
+opt_bt2_x = Option(
+    ("--bt2-X",),
+    type=int,
+    default=600,
+    help="Maximum fragment length for valid paired-end alignments")
+
+opt_bt2_score_min_e2e = Option(
+    ("--bt2-score-min-e2e",),
+    type=str,
+    default="L,-1,-0.5",
+    help="Minimum score for a valid end-to-end alignment")
+
+opt_bt2_score_min_loc = Option(
+    ("--bt2-score-min-loc",),
+    type=str,
+    default="L,1,0.5",
+    help="Minimum score for a valid local alignment")
+
+opt_bt2_s = Option(
+    ("--bt2-i", "bt2_s"),
+    type=str,
+    default="L,1,0.1",
+    help="Seed interval")
+
+opt_bt2_l = Option(
+    ("--bt2-L",),
+    type=int,
+    default=12,
+    help="Seed length")
+
+opt_bt2_gbar = Option(
+    ("--bt2-gbar",),
+    type=int,
+    default=4,
+    help="Minimum distance of a gap from end of a read")
+
+opt_bt2_d = Option(
+    ("--bt2-D",),
+    type=int,
+    default=4,
+    help="Maximum number of failed seed extensions")
+
+opt_bt2_r = Option(
+    ("--bt2-R",),
+    type=int,
+    default=2,
+    help="Maximum number of times to re-seed")
+
+opt_bt2_dpad = Option(
+    ("--bt2-dpad",),
+    type=int,
+    default=2,
+    help="Width of padding on alignment matrix, to allow gaps")
+
+opt_bt2_orient = Option(
+    ("--bt2-orient",),
+    type=Choice(BOWTIE2_ORIENT, case_sensitive=False),
+    default=BOWTIE2_ORIENT[0],
+    help="Valid orientations of paired-end mates")
 
 # Reference section specification options
-opt_coords = Option(("--coords", "-x"),
-                    type=(str, int, int),
-                    multiple=True,
-                    default=(),
-                    help=("Reference name, 5' end, and 3' end of a section; "
-                          "coordinates are 1-indexed and include both ends"))
-opt_primers = Option(("--primers",),
-                     type=(str, str, str),
-                     multiple=True,
-                     default=(),
-                     help=("Reference name, forward primer, and reverse primer "
-                           "of a section; reverse primer must be given 5' to 3'"))
-opt_primer_gap = Option(("--primer-gap",),
-                        type=int,
-                        default=2,
-                        help=("Number of bases to leave as a gap between the "
-                              "end of a primer and the end of the section"))
+opt_coords = Option(
+    ("--coords", "-c"),
+    type=(str, int, int),
+    multiple=True,
+    default=(),
+    help=("Reference name, 5' end, and 3' end of a section; "
+          "coordinates are 1-indexed and include both ends"))
+
+opt_primers = Option(
+    ("--primers", "-p"),
+    type=(str, str, str),
+    multiple=True,
+    default=(),
+    help=("Reference name, forward primer, and reverse primer "
+          "of a section; reverse primer must be given 5' to 3'"))
+
+opt_primer_gap = Option(
+    ("--primer-gap",),
+    type=int,
+    default=2,
+    help=("Number of bases to leave as a gap between the "
+          "end of a primer and the end of the section"))
 
 # Relate
-opt_min_reads = Option(("--min-reads", "-n"),
-                       type=int,
-                       default=1000,
-                       help=("Do not analyze datasets with fewer than this "
-                             "minimum number of reads"))
-opt_batch_size = Option(("--batch-size",),
-                        type=float,
-                        default=256.,
-                        help=("Target size of each batch of mutation vectors, "
-                              "in millions of base calls"))
-opt_ambrel = Option(("--ambrel/--no-ambrel",),
-                    type=bool,
-                    default=True,
-                    help=("Whether to find and label all ambiguous "
-                          "insertions and deletions (improves accuracy "
-                          "but runs slower)"))
+opt_min_reads = Option(
+    ("--min-reads", "-n"),
+    type=int,
+    default=1000,
+    help=("Do not analyze datasets with fewer than this "
+          "minimum number of reads"))
+
+opt_batch_size = Option(
+    ("--batch-size",),
+    type=float,
+    default=256.,
+    help=("Target size of each batch of mutation vectors, "
+          "in millions of base calls"))
+
+opt_ambrel = Option(
+    ("--ambrel/--no-ambrel",),
+    type=bool,
+    default=True,
+    help=("Whether to find and label all ambiguous "
+          "insertions and deletions (improves accuracy "
+          "but runs slower)"))
 
 # Mask
-opt_report = Option(("--report", "-r"),
-                    type=Path(exists=True),
-                    multiple=True,
-                    default=(),
-                    help="Report file.")
-opt_count_del = Option(("--count-del/--discount-del",),
-                       type=bool,
-                       default=False,
-                       help='Whether to count deletions as mutations')
-opt_count_ins = Option(("--count-ins/--discount-ins",),
-                       type=bool,
-                       default=False,
-                       help='Whether to count insertions as mutations')
-opt_discount_mut = Option(("--discount-mut",),
-                          type=str,
-                          multiple=True,
-                          default=(),
-                          help="Do not count a specific type of mutation")
-opt_exclude_polya = Option(("--exclude-polya",),
-                           type=int,
-                           default=5,
-                           help="Exclude stretches of consecutive A bases of "
-                                "at least this length. If 0, exclude none.")
-opt_exclude_gu = Option(("--exclude-gu/--include-gu",),
-                        type=bool,
-                        default=True,
-                        help="Exclude positions with G and U bases (which DMS "
-                             "methylates very weakly at physiological pH).")
-opt_exclude_pos = Option(("--exclude-pos",),
-                         type=(str, int),
-                         default=(),
-                         multiple=True,
-                         help="Exclude positions arbitrarily. Must be given as "
-                              "(reference, position).")
-opt_min_finfo_read = Option(("--min-finfo-read",),
-                            type=float,
-                            default=0.9,
-                            help="Filter out reads with less than this "
-                                 "fraction of informative positions.")
-opt_max_fmut_read = Option(("--max-fmut-read",),
-                           type=float,
-                           default=0.1,
-                           help="Filter out reads with more than this fraction "
-                                "of mutated positions.")
-opt_min_mut_gap = Option(("--min-mut-gap",),
-                         type=int,
-                         default=3,
-                         help="Filter out reads with any pair of mutations "
-                              "that are separated by fewer than this number of "
-                              "non-mutated bases. If 0, filter out no reads.")
-opt_min_ninfo_pos = Option(("--min-ninfo-pos",),
-                           type=int,
-                           default=1000,
-                           help="Filter out positions with fewer than this "
-                                "number of informative reads.")
-opt_max_fmut_pos = Option(("--max-fmut-pos",),
-                          type=float,
-                          default=0.5,
-                          help="Filter out positions with more than this "
-                               "fraction of mutated reads.")
+
+opt_count_del = Option(
+    ("--count-del/--discount-del",),
+    type=bool,
+    default=False,
+    help='Whether to count deletions as mutations')
+
+opt_count_ins = Option(
+    ("--count-ins/--discount-ins",),
+    type=bool,
+    default=False,
+    help='Whether to count insertions as mutations')
+
+opt_discount_mut = Option(
+    ("--discount-mut",),
+    type=str,
+    multiple=True,
+    default=(),
+    help="Do not count a specific type of mutation")
+
+opt_exclude_polya = Option(
+    ("--exclude-polya",),
+    type=int,
+    default=5,
+    help="Exclude stretches of consecutive A bases of at least this length. "
+         "If 0, exclude none.")
+
+opt_exclude_gu = Option(
+    ("--exclude-gu/--include-gu",),
+    type=bool,
+    default=True,
+    help="Exclude positions with G and U bases (which DMS methylates very "
+         "weakly at physiological pH).")
+
+opt_exclude_pos = Option(
+    ("--exclude-pos",),
+    type=(str, int),
+    default=(),
+    multiple=True,
+    help="Exclude arbitrary positions, given as (reference, position).")
+
+
+opt_min_ncall_read = Option(
+    ("--min-ncall-read",),
+    type=int,
+    default=1,
+    help="Filter reads with less than this number of base calls.")
+
+opt_min_finfo_read = Option(
+    ("--min-finfo-read",),
+    type=float,
+    default=0.95,
+    help="Filter reads with less than this fraction of informative positions.")
+
+opt_max_fmut_read = Option(
+    ("--max-fmut-read",),
+    type=float,
+    default=0.05,
+    help="Filter reads with more than this fraction of mutated positions.")
+
+opt_min_mut_gap = Option(
+    ("--min-mut-gap",),
+    type=int,
+    default=3,
+    help="Filter out reads with any pair of mutations "
+         "that are separated by fewer than this number of "
+         "non-mutated bases. If 0, filter out no reads.")
+
+opt_min_ninfo_pos = Option(
+    ("--min-ninfo-pos",),
+    type=int,
+    default=1000,
+    help="Filter positions with less than this number of informative reads.")
+
+opt_max_fmut_pos = Option(
+    ("--max-fmut-pos",),
+    type=float,
+    default=0.5,
+    help="Filter positions with more than this fraction of mutated reads.")
 
 # Clustering options
-opt_max_clusters = Option(("--max-clusters", "-k"),
-                          type=int,
-                          default=0,
-                          help="End the clustering step after attempting this "
-                               "number of clusters, even if it yields the best "
-                               "(smallest) BIC observed thus far. If 0, do not "
-                               "run clustering.")
-opt_em_runs = Option(("--em-runs", "-e"),
-                     type=int,
-                     default=6,
-                     help="Run clustering this many times for each number of "
-                          "clusters, randomly initializing each run.")
-opt_min_em_iter = Option(("--min-em-iter",),
-                         type=int,
-                         default=10,
-                         help="Run every EM run for at least this number times "
-                              "k iterations, even if the likelihood value has "
-                              "already converged.")
-opt_max_em_iter = Option(("--max-em-iter",),
-                         type=int,
-                         default=300,
-                         help="Stop every EM run after this number times k "
-                              "iterations, even if the likelihood value has "
-                              "not yet converged.")
-opt_em_thresh = Option(("--em-thresh",),
-                       type=float,
-                       default=0.01,
-                       help="Consider an EM run to have converged when the log "
-                            "likelihood value has increased by less than this "
-                            "threshold between two consecutive iterations.")
+opt_max_clusters = Option(
+    ("--max-clusters", "-k"),
+    type=int,
+    default=0,
+    help="End the clustering step after attempting this "
+         "number of clusters, even if it yields the best "
+         "(smallest) BIC observed thus far. If 0, do not "
+         "run clustering.")
+
+opt_em_runs = Option(
+    ("--em-runs", "-e"),
+    type=int,
+    default=6,
+    help="Run clustering this many times for each number of "
+         "clusters, randomly initializing each run.")
+
+opt_min_em_iter = Option(
+    ("--min-em-iter",),
+    type=int,
+    default=10,
+    help="Run every EM run for at least this number times "
+         "k iterations, even if the likelihood value has "
+         "already converged.")
+
+opt_max_em_iter = Option(
+    ("--max-em-iter",),
+    type=int,
+    default=300,
+    help="Stop every EM run after this number times k "
+         "iterations, even if the likelihood value has "
+         "not yet converged.")
+
+opt_em_thresh = Option(
+    ("--em-thresh",),
+    type=float,
+    default=0.01,
+    help="Consider an EM run to have converged when the log "
+         "likelihood value has increased by less than this "
+         "threshold between two consecutive iterations.")
 
 # Tables
 
-opt_table = Option(("--table", "-t"),
-                   type=Path(exists=True),
-                   multiple=True,
-                   default=(),
-                   help="Table file.")
-
-opt_table_cols = Option(("--table-cols", "-c"),
-                        default="",
-                        type=str,
-                        help="Output columns of these relationships")
+opt_rels = Option(
+    ("--rels", "-r"),
+    default="",
+    type=str,
+    help="Output these relationships between the read and the reference")
 
 # RNA structure prediction
 
-opt_fold = Option(("--fold/--no-fold",),
-                  type=bool,
-                  default=True,
-                  help="Whether to predict the RNA structure using Fold")
-
-opt_dms_quantile = Option(("--dms-quantile", "-q"),
-                          type=float,
-                          default=0.9,
-                          help="Quantile of DMS reactivities for normalization")
+opt_fold = Option(
+    ("--fold/--no-fold",),
+    type=bool,
+    default=False,
+    help="Whether to predict the RNA structure using Fold")
+
+opt_quantile = Option(
+    ("--quantile", "-q"),
+    type=float,
+    default=0.9,
+    help="Quantile of reactivities for normalization")
+
 
 # Graphing
 
-opt_stack = Option(("--stack", "-s"),
-                   default="",
-                   type=str,
-                   help="Draw stacked graphs of these relationships")
-
-opt_csp = Option(("--csp/--no-csp",),
-                 type=bool,
-                 default=True,
-                 help="Whether to output clusters as subplots in one file")
-
-opt_xfrac = Option(("--xfrac/--xcount",),
-                   default=False,
-                   type=bool,
-                   help="Whether the x-axis represents counts or fractions")
-
-opt_yfrac = Option(("--yfrac/--ycount",),
-                   default=True,
-                   type=bool,
-                   help="Whether the y-axis represents counts or fractions")
-
-opt_hist_bins = Option(("--hist-bins",),
-                       default=24,
-                       type=int,
-                       help="Number of bins in each histogram (≥ 1)")
-
-opt_csv = Option(("--csv/--no-csv",),
-                 default=True,
-                 type=bool,
-                 help="Whether to output the source data for each graph "
-                      "as a CSV file")
-
-opt_html = Option(("--html/--no-html",),
-                  default=True,
-                  type=bool,
-                  help="Whether to output each graph as an HTML file")
-
-opt_pdf = Option(("--pdf/--no-pdf",),
-                 default=False,
-                 type=bool,
-                 help="Whether to output each graph as a PDF file")
+opt_stack = Option(
+    ("--stack/--no-stack",),
+    type=bool,
+    default=False,
+    help="Whether to stack relationships")
+
+opt_arrange = Option(
+    ("--arrange",),
+    type=Choice(CLUST_ARRANGE_OPTIONS),
+    default=CLUST_ORDER,
+    help="Whether to graph each INDIVidual cluster in its own file, "
+         "graph each ORDER of clusters in its own file, "
+         "or UNITE all clusters in one file containing all orders.")
+
+opt_x_ratio = Option(
+    ("--x-ratio/--x-count",),
+    default=False,
+    type=bool,
+    help="Whether the x-axis depicts counts or ratios")
+
+opt_y_ratio = Option(
+    ("--y-ratio/--y-count",),
+    default=True,
+    type=bool,
+    help="Whether the y-axis depicts counts or ratios")
+
+opt_hist_bins = Option(
+    ("--hist-bins",),
+    default=24,
+    type=int,
+    help="Number of bins in each histogram (≥ 1)")
+
+opt_csv = Option(
+    ("--csv/--no-csv",),
+    default=True,
+    type=bool,
+    help="Whether to output the source data for each graph "
+         "as a CSV file")
+
+opt_html = Option(
+    ("--html/--no-html",),
+    default=True,
+    type=bool,
+    help="Whether to output each graph as an HTML file")
+
+opt_pdf = Option(
+    ("--pdf/--no-pdf",),
+    default=False,
+    type=bool,
+    help="Whether to output each graph as a PDF file")
 
 # Logging options
-opt_verbose = Option(("--verbose", "-v"),
-                     count=True,
-                     help="Print info or info+debug messages to stdout")
-opt_quiet = Option(("--quiet", "-q"),
-                   count=True,
-                   help="Suppress warnings or warnings+errors to stdout")
-opt_log = Option(("--log",),
-                 type=Path(exists=False, dir_okay=False),
-                 default=os.path.join(CWD, "log", datetime.now().strftime(
-                     "seismic-rna_%Y-%m-%d_%H-%M-%S.log")),
-                 help="File in which to log all messages (except profiling)")
-opt_profile = Option(("--profile",),
-                     type=Path(exists=False, dir_okay=False),
-                     default="",
-                     help="Profile code performance and log results to the given file")
+opt_verbose = Option(
+    ("--verbose", "-v"),
+    count=True,
+    help="Print info or info+debug messages to stdout")
+
+opt_quiet = Option(
+    ("--quiet",),
+    count=True,
+    help="Suppress warnings or warnings+errors to stdout")
+
+opt_log = Option(
+    ("--log",),
+    type=Path(exists=False, dir_okay=False),
+    default=os.path.join(CWD, "log", datetime.now().strftime(
+        "seismic-rna_%Y-%m-%d_%H-%M-%S.log")),
+    help="File in which to log all messages (except profiling)")
+
+opt_profile = Option(
+    ("--profile",),
+    type=Path(exists=False, dir_okay=False),
+    default="",
+    help="Profile code performance and log results to the given file")
 
 
 def merge_params(*param_lists: list[Parameter]):
     """ Merge lists of Click parameters, dropping duplicates. """
     params = list()
     names = set()
     for param_list in param_lists:
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/depend.py` & `seismic-rna-0.2.0/src/seismicrna/core/depend.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/docdef.py` & `seismic-rna-0.2.0/src/seismicrna/core/docdef.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/docstring.py` & `seismic-rna-0.2.0/src/seismicrna/core/docstring.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/dump.py` & `seismic-rna-0.2.0/src/seismicrna/core/dump.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/files.py` & `seismic-rna-0.2.0/src/seismicrna/core/files.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/load.py` & `seismic-rna-0.2.0/src/seismicrna/core/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/logs.py` & `seismic-rna-0.2.0/src/seismicrna/core/logs.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/mu.py` & `seismic-rna-0.2.0/src/seismicrna/core/mu.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/mu_test.py` & `seismic-rna-0.2.0/src/seismicrna/core/mu_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/parallel.py` & `seismic-rna-0.2.0/src/seismicrna/core/parallel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/path.py` & `seismic-rna-0.2.0/src/seismicrna/core/path.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/rel.py` & `seismic-rna-0.2.0/src/seismicrna/core/rel.py`

 * *Files 1% similar despite different names*

```diff
@@ -581,18 +581,18 @@
             # Determine the read(s) corresponding to this relation vector.
             degen, qual, cigar, end5, end3 = relvec_to_read(refseq, relvec,
                                                             MAX_QUAL, MIN_QUAL,
                                                             ins_len)
             if n_ins > 0:
                 # If there are insertions, find their positions.
                 ins_pos = list(find_cigar_op_pos(cigar, CIG_INSRT))
-                # Remove the quality codes of inserted bases because for
+                # Remove quality codes of inserted bases because -- for
                 # the purpose of aggregating reads based on sequence,
-                # quality score, and position, the "fake" quality scores
-                # of inserted bases should not be considered.
+                # quality score, and position -- the "fake" quality
+                # scores of inserted bases should not be considered.
                 qual_no_ins = bytes(q for i, q in enumerate(qual, start=1)
                                     if i not in ins_pos)
             else:
                 qual_no_ins = qual
             # Count the mutations in the CIGAR string.
             nmuts = count_cigar_muts(cigar)
             for read in expand_degenerate_seq(degen):
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/rel_test.py` & `seismic-rna-0.2.0/src/seismicrna/core/rel_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/report.py` & `seismic-rna-0.2.0/src/seismicrna/core/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,14 @@
 from .seq import DNA
 
 logger = getLogger(__name__)
 
 
 # Field class
 
-def identity(value: Any):
-    """ Identity function. """
-    return value
-
-
-def truthy(*_: Any):
-    """ Truthy function. """
-    return True
-
-
 class Field(object):
     __slots__ = ["key", "title", "dtype", "iconv", "oconv",
                  "check_val", "check_rep_val"]
 
     def __init__(self, key: str, title: str, dtype: type, *,
                  iconv: Callable[[Any], Any] | None = None,
                  oconv: Callable[[Any], Any] | None = None,
@@ -73,28 +63,30 @@
             and return True if the value is valid and False otherwise.
             If None, the value is not validated -- only its data type.
         """
         self.key = key
         self.title = title
         self.dtype = dtype
         self.iconv = self.dtype if iconv is None else iconv
-        self.oconv = identity if oconv is None else oconv
-        self.check_val = truthy if check_val is None else check_val
-        self.check_rep_val = truthy if check_rep_val is None else check_rep_val
+        self.oconv = oconv
+        self.check_val = check_val
+        self.check_rep_val = check_rep_val
 
     def validate(self, report: Report, value: Any):
         # Validate the type.
         if not isinstance(value, self.dtype):
             raise TypeError(f"{self} expected value to be {self.dtype}, "
                             f"but got {type(value)}")
         # Validate the value.
-        if not self.check_val(value):
-            raise ValueError(f"{self} got invalid value: {value}")
-        if not self.check_rep_val(report, value):
-            raise ValueError(f"{self} got invalid value: {value}")
+        if self.check_val is not None:
+            if not self.check_val(value):
+                raise ValueError(f"{self} got invalid value: {value}")
+        if self.check_rep_val is not None:
+            if not self.check_rep_val(report, value):
+                raise ValueError(f"{self} got invalid value: {value}")
 
     def __str__(self):
         return f"Report Field '{self.title}' ({self.key})"
 
 
 # Field calculation functions
 
@@ -566,24 +558,28 @@
     return {field.title: field for field in fields() if field.title}
 
 
 def lookup_key(key: str) -> Field:
     try:
         return field_keys()[key]
     except KeyError:
-        raise ValueError(f"No Report Field is keyed '{key}'")
+        # Suppress exception chaining.
+        pass
+    raise ValueError(f"No Report Field is keyed '{key}'")
 
 
 def lookup_title(title: str) -> Field:
     if not title:
         raise ValueError("Got blank title for field")
     try:
         return field_titles()[title]
     except KeyError:
-        raise ValueError(f"No field is titled '{title}'")
+        # Suppress exception chaining.
+        pass
+    raise ValueError(f"No Report Field is titled '{title}'")
 
 
 # Report classes
 
 class Report(ABC):
     """ Abstract base class for a report from a step. """
     __slots__ = "out_dir",
@@ -639,15 +635,19 @@
         """ Return a dict of raw values of the fields, keyed by the
         titles of their fields. """
         odata = dict()
         for key in self.__slots__:
             field = lookup_key(key)
             if field.title:
                 # Output only the fields with non-blank titles.
-                odata[field.title] = field.oconv(self.get_field(field))
+                value = self.get_field(field)
+                if field.oconv is not None:
+                    # Convert the value to the proper output value.
+                    value = field.oconv(value)
+                odata[field.title] = value
         return odata
 
     def save(self):
         with open(self.get_path(), "w") as f:
             json.dump(self.to_dict(), f, indent=4)
         logger.info(f"Wrote {self} to {self.get_path()}")
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/rna.py` & `seismic-rna-0.2.0/src/seismicrna/core/rna.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/sect.py` & `seismic-rna-0.2.0/src/seismicrna/core/sect.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 FIELD_REF = "Reference"
 FIELD_SECT = "Section"
 FIELD_END5 = "5' End"
 FIELD_END3 = "3' End"
 FIELD_PFWD = "Forward Primer"
 FIELD_PREV = "Reverse Primer"
 
-SectionTuple = namedtuple("PrimerTuple", ["pos5", "pos3"])
+SectionTuple = namedtuple("PrimerTuple", ("pos5", "pos3"))
 
 
 def encode_primer(ref: str, fwd: str, rev: str):
     """ Convert a pair of primers from strings to DNA objects. """
     return ref, DNA.parse(fwd), DNA.parse(rev)
 
 
@@ -52,22 +52,47 @@
             except Exception as error:
                 logger.error(f"Failed to encode primer {primer}: {error}")
                 enc_primers[primer] = None
     # Return a list of all encoded primers with None values removed.
     return list(filter(None, enc_primers.values()))
 
 
-def get_section_coords_primers(library_file: Path):
-    """ Return a map from the names of """
+def get_sect_coords_primers(sects_file: Path):
+    """
+    Parse a file defining each section by the name of its reference and
+    either its 5' and 3' coordinates or its forward and reverse primer
+    sequences. Return one map from each reference and 5'/3' coordinate
+    pair to the name of the corresponding section, and another from each
+    reference and primer pair to the name of the corresponding section.
+
+    Parameters
+    ----------
+    sects_file: Path
+        CSV file of a table that defines the sections. The table must
+        have columns labeled "Reference", "Section", "5' End", "3' End",
+        "Forward Primer", and "Reverse Primer". Others are ignored.
+
+    Returns
+    -------
+    tuple[dict[tuple[str, int, int], str],
+          dict[tuple[str, DNA, DNA], str]]
+        Two mappings, the first from (ref name, 5' coord, 3' coord) to
+        each section, the second from (ref name, fwd primer, rev primer)
+        to each section. If the section is named in the "Section" column
+        of the table, then that name will be used as the section name.
+        Otherwise, the section name will be an empty string.
+    """
+
     # Initialize dictionaries mapping references and coordinates/primers
     # to section names.
     coords: dict[tuple[str, int, int], str] = dict()
     primers: dict[tuple[str, DNA, DNA], str] = dict()
 
     def map_sect(mapping: dict[tuple, str], key: tuple, value: str):
+        """ Add one section to the map if not already present. """
         # Check whether the mapping already contains the key.
         try:
             prev = mapping[key]
         except KeyError:
             # The mapping does not already contain the key: add it.
             mapping[key] = value
         else:
@@ -77,19 +102,19 @@
                 # If so, then warn about it.
                 logger.warning(f"Key {key} mapped to '{value}' multiple times")
             else:
                 # If not, then raise an error because it is ambiguous
                 # which value to use.
                 raise ValueError(f"Key {key} mapped to '{prev}' and '{value}'")
 
-    # Read every row of the library file data.
-    library = pd.read_csv(library_file)
-    lines = zip(library[FIELD_REF], library[FIELD_SECT],
-                library[FIELD_END5], library[FIELD_END3],
-                library[FIELD_PFWD], library[FIELD_PREV])
+    # Read every row of the sections file.
+    sections = pd.read_csv(sects_file)
+    lines = zip(sections[FIELD_REF], sections[FIELD_SECT],
+                sections[FIELD_END5], sections[FIELD_END3],
+                sections[FIELD_PFWD], sections[FIELD_PREV])
     for i, (ref, sect, end5, end3, fwd, rev) in enumerate(lines, start=1):
         try:
             # The reference name must have a value.
             if pd.isnull(ref):
                 raise ValueError(f"Missing {FIELD_REF}")
             else:
                 ref = str(ref)
@@ -107,15 +132,15 @@
             elif has_primers:
                 # Map the reference and primers to the section.
                 map_sect(primers, (ref, DNA.parse(fwd), DNA.parse(rev)), sect)
             else:
                 raise ValueError(f"Got neither coordinates nor primers")
         except Exception as error:
             logger.error(f"Failed to make a section from line {i} of "
-                         f"{library_file}: {error}")
+                         f"{sects_file}: {error}")
     return coords, primers
 
 
 def seq_pos_to_index(seq: DNA, positions: Sequence[int], start: int):
     """
     Convert a sequence and positions to indexes, where each index is a
     tuple of (position, base).
@@ -549,30 +574,30 @@
 
 
 class RefSections(object):
     """ A collection of sections, grouped by reference. """
 
     def __init__(self,
                  refseqs: Iterable[tuple[str, DNA]], *,
-                 library: Path | None = None,
+                 sects_file: Path | None = None,
                  coords: Iterable[tuple[str, int, int]] = (),
                  primers: Iterable[tuple[str, DNA, DNA]] = (),
                  primer_gap: int):
-        # Get the names of the sections from the library, if any.
+        # Get the names of the sections from the sections file, if any.
         sect_coords = dict()
         sect_primers = dict()
-        if library is not None:
+        if sects_file is not None:
             try:
-                sect_coords, sect_primers = get_section_coords_primers(library)
-                # Combines the coordinates from the library and from the
+                sect_coords, sect_primers = get_sect_coords_primers(sects_file)
+                # Combines the coordinates from the sections_file and from the
                 # coord parameter.
                 coords = list(coords) + list(sect_coords)
                 primers = list(primers) + list(sect_primers)
             except Exception as error:
-                logger.error(f"Failed to add coordinates from library: {error}")
+                logger.error(f"Failed to add coordinates from sections_file: {error}")
 
         # Group coordinates and primers by reference.
         ref_coords = get_coords_by_ref(coords)
         ref_primers = get_coords_by_ref(primers)
 
         # For each reference, generate sections from the coordinates.
         self._sections: dict[str, dict[tuple[int, int], Section]] = dict()
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/sect_test.py` & `seismic-rna-0.2.0/src/seismicrna/core/sect_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/seq.py` & `seismic-rna-0.2.0/src/seismicrna/core/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/seq_test.py` & `seismic-rna-0.2.0/src/seismicrna/core/seq_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/shell.py` & `seismic-rna-0.2.0/src/seismicrna/core/shell.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/sim.py` & `seismic-rna-0.2.0/src/seismicrna/core/sim.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/sim_test.py` & `seismic-rna-0.2.0/src/seismicrna/core/sim_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/types.py` & `seismic-rna-0.2.0/src/seismicrna/core/types.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/core/xam.py` & `seismic-rna-0.2.0/src/seismicrna/core/xam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/demult/demultiplex.py` & `seismic-rna-0.2.0/src/seismicrna/demult/demultiplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 import fastqsplitter
 import pandas as pd
 
 from ..align.fqutil import FastqUnit
 from ..core.cli import (
     opt_barcode_length, opt_barcode_start, opt_parallel_demultiplexing, opt_clipped_demultiplexing,
-    opt_mismatch_tolerence, opt_index_tolerence, opt_demulti_overwrite, opt_fasta, opt_library, opt_fastqm)
+    opt_mismatch_tolerence, opt_index_tolerence, opt_demulti_overwrite, opt_fasta, opt_sections_file, opt_fastqp)
 
 # from scipy import signal
 
 # secondary barcode names: secondary_signiture
 params = [
     # Inputs
     opt_fasta,
-    opt_fastqm,
-    opt_library,
+    opt_fastqp,
+    opt_sections_file,
     opt_barcode_start,
     opt_barcode_length,
 
     # options
     opt_parallel_demultiplexing,
     opt_clipped_demultiplexing,
     opt_mismatch_tolerence,
@@ -442,15 +442,15 @@
     for i in range(0, len(fa), 2):
         temp_dict[fa[i][1:].strip()] = fa[i + 1].strip()
 
     return temp_dict
 
 
 """
-input csv, library that represents each sequence to be dumultiplexed with many different coloumns 
+input csv, sections_file that represents each sequence to be dumultiplexed with many different coloumns 
 
 workspace directory that demultiplexing is being done in 
 
 fq1/fq2 path for big fastq which will be demultiplexed? maybe should be removed
 
 
 this whole method could be replaced with a dataframe that organizes all of these attributes
@@ -1014,21 +1014,21 @@
 
     print(working_directory + "demultiplex_info.csv")
     df.to_csv(working_directory + "demultiplex_info.csv", index=False)
 
 
 """
 split is default to 10. disregarding extremes, the higher the split the lighter the memeory load
-library csv 
+sections_file csv 
     each construct must have a secondary signiture start index and len in order to process, 
     barcode given in main arguements 
 """
 
 
-def demultiplex_run(library_csv, demulti_workspace, report_folder, fq_unit: FastqUnit, fasta, barcode_start=0,
+def demultiplex_run(sections_file_csv, demulti_workspace, report_folder, fq_unit: FastqUnit, fasta, barcode_start=0,
                     barcode_length=0, split: int = 10, clipped: int = 0, rev_clipped: int = 0, index_tolerance: int = 0,
                     parallel: bool = False, mismatch_tolerence: int = 0, overwrite: bool = False):
     sample_name = fq_unit.sample
     mixed_fastq1, mixed_fastq2 = fq_unit.paths.values()  # only works if the FASTQ has paired-end reads in two separate files
 
     """
     makes dictionary of sequence objects
@@ -1046,15 +1046,15 @@
     all the little stuff gets stored per sequence here, at least temporarily 
     """
     seq_data_folder = temp_ws + "sequence_data/"
 
     os.makedirs(seq_data_folder, exist_ok=True)
 
     sequence_objects = make_sequence_objects_from_csv(
-        input_csv=library_csv,
+        input_csv=sections_file_csv,
         barcode_start=barcode_start,
         barcode_length=barcode_length,
         fasta=fasta,
         fastq1_path=mixed_fastq1,
         fastq2_path=mixed_fastq2,
         paired=True,
         workspace=seq_data_folder)
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/demult/main.py` & `seismic-rna-0.2.0/src/seismicrna/demult/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from click import command
 from pathlib import Path
 
 from ..demult.demultiplex import demultiplex_run
 from ..align.fqutil import FastqUnit
 from ..core.cli import (
     opt_barcode_length, opt_barcode_start, opt_parallel_demultiplexing, opt_clipped_demultiplexing,
-    opt_mismatch_tolerence, opt_index_tolerence, opt_demulti_overwrite, opt_fasta, opt_library, opt_fastqm, opt_out_dir,
+    opt_mismatch_tolerence, opt_index_tolerence, opt_demulti_overwrite, opt_fasta, opt_sections_file, opt_fastqp, opt_out_dir,
     opt_phred_enc)
 
 params = [
     # Inputs
     opt_fasta,
-    opt_fastqm,
+    opt_fastqp,
     opt_phred_enc,
-    opt_library,
+    opt_sections_file,
     opt_barcode_start,
     opt_barcode_length,
     opt_out_dir,
 
     # options
     opt_parallel_demultiplexing,
     opt_clipped_demultiplexing,
@@ -32,20 +32,20 @@
 
 @command("demultiplex", params=params)
 def cli(*args, **kwargs):
     """ Split multiplexed FASTQ files by their barcodes. """
     return run(*args, **kwargs)
 
 
-def run(library: str, out_dir: str, temp_dir: str, fastqm: tuple[str, ...], phred_enc: int, fasta: str, barcode_start=0,
+def run(sections_file: str, out_dir: str, temp_dir: str, fastqp: tuple[str, ...], phred_enc: int, fasta: str, barcode_start=0,
         barcode_length=0, clipped: int = 0, index_tolerance: int = 0, parallel_demultiplexing: bool = False,
         mismatch_tolerence: int = 0, demulti_overwrite: bool = False):
-    fq_units = list(FastqUnit.from_paths(fastqm=list(map(Path, fastqm)),
+    fq_units = list(FastqUnit.from_paths(fastqp=list(map(Path, fastqp)),
                                          phred_enc=phred_enc))
-    return [demultiplex_run(library_csv=library,
+    return [demultiplex_run(sections_file_csv=sections_file,
                             overwrite=demulti_overwrite,
                             demulti_workspace=temp_dir,
                             report_folder=out_dir,
                             fq_unit=fq_unit,
                             barcode_start=barcode_start,
                             barcode_length=barcode_length,
                             clipped=clipped,
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/draw/main.py` & `seismic-rna-0.2.0/src/seismicrna/draw/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/draw/manipulator.py` & `seismic-rna-0.2.0/src/seismicrna/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/draw/plotter.py` & `seismic-rna-0.2.0/src/seismicrna/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/draw/study.py` & `seismic-rna-0.2.0/src/seismicrna/draw/study.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/draw/util.py` & `seismic-rna-0.2.0/src/seismicrna/draw/util.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/graph/base.py` & `seismic-rna-0.2.0/src/seismicrna/graph/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from logging import getLogger
 from functools import cache, cached_property
 from pathlib import Path
-from typing import Any
+from typing import Any, Iterable
 
-import pandas as pd
 from plotly import graph_objects as go
+from plotly.subplots import make_subplots
 
 from .color import ColorMap, get_cmap
 from ..core import path
 from ..core.seq import DNA
 from ..table.base import Table
 from ..table.load import load, TableLoader, PosTableLoader
 
@@ -26,67 +26,47 @@
 
 
 class GraphBase(ABC):
 
     def __init__(self, cmap: str | None = None):
         self._cmap_name = cmap
 
-    @classmethod
-    @abstractmethod
-    def get_data_type(cls) -> type | tuple[type, ...]:
-        """ Type of the data. """
-        return tuple()
-
-    @abstractmethod
-    def _get_data(self) -> pd.DataFrame | pd.Series:
-        """ Get the data of the graph. """
-        return pd.DataFrame()
-
     @cached_property
+    @abstractmethod
     def data(self) -> Any:
         """ Data of the graph. """
-        data = self._get_data()
-        if not isinstance(data, self.get_data_type()):
-            raise TypeError(f"{self.__class__.__name__} expected data "
-                            f"of type '{self.get_data_type().__name__}', "
-                            f"but got type '{type(data).__name__}'")
-        return data
 
     @property
     @abstractmethod
-    def title(self):
+    def title(self) -> str:
         """ Title of the graph. """
-        return ""
 
     @classmethod
     @abstractmethod
-    def get_cmap_type(cls):
+    def get_cmap_type(cls) -> type[ColorMap]:
         """ Type of the color map. """
-        return ColorMap
 
     @property
     def cmap(self) -> ColorMap:
         """ Color map of the graph. """
         return get_cmap(self.get_cmap_type(), self._cmap_name)
 
     @abstractmethod
-    def get_traces(self):
+    def get_traces(self) -> Iterable[tuple[tuple[int, int], go.Trace]]:
         """ Data traces of the graph. """
-        return list()
 
     @property
     @abstractmethod
-    def out_dir(self):
+    def out_dir(self) -> Path:
         """ Output directory. """
-        return Path()
 
     @property
     @abstractmethod
     def graph_filename(self):
-        return ""
+        """ Name of the graph file. """
 
     @classmethod
     def get_path_segs(cls):
         """ Path segments. """
         return path.ModSeg, path.GraphSeg
 
     def get_path_fields(self):
@@ -97,36 +77,58 @@
 
     def get_path(self, ext: str):
         """ Path to the output file of the graph. """
         return path.buildpar(*self.get_path_segs(),
                              **self.get_path_fields(),
                              ext=ext)
 
-    def _init_figure(self):
+    @property
+    @abstractmethod
+    def nrows(self) -> int:
+        """ Number of rows of subplots. """
+
+    @property
+    @abstractmethod
+    def ncols(self) -> int:
+        """ Number of columns of subplots. """
+
+    @property
+    @abstractmethod
+    def subplot_titles(self):
+        """ Titles of the subplots. """
+
+    def _figure_init(self):
         """ Initialize the figure. """
-        return go.Figure(data=self.get_traces())
+        return make_subplots(rows=self.nrows, cols=self.ncols)
+
+    def _figure_data(self, fig: go.Figure):
+        """ Add data to the figure. """
+        for (row, col), trace in self.get_traces():
+            fig.add_trace(trace, row=row, col=col)
 
-    def _layout_figure(self, fig: go.Figure):
+    def _figure_layout(self, fig: go.Figure):
         """ Update the figure's layout. """
         fig.update_layout(title=self.title,
                           plot_bgcolor="#ffffff",
                           paper_bgcolor="#ffffff")
         fig.update_xaxes(linewidth=1,
                          linecolor="#000000",
                          autorange=True)
         fig.update_yaxes(gridcolor="#d0d0d0",
                          linewidth=1,
                          linecolor="#000000",
                          autorange=True)
-        return fig
 
     @cache
     def get_figure(self):
         """ Figure object. """
-        return self._layout_figure(self._init_figure())
+        fig = self._figure_init()
+        self._figure_data(fig)
+        self._figure_layout(fig)
+        return fig
 
     def write_csv(self):
         """ Write the graph's source data to a CSV file. """
         file = self.get_path(ext=path.CSV_EXT)
         if file.is_file():
             logger.warning(f"File exists: {file}")
         else:
@@ -272,29 +274,29 @@
     def seq(self):
         return self.table.seq
 
 
 class CartesianGraph(GraphBase, ABC):
     """ Graph with one pair of x and y axes. """
 
+    @property
     @abstractmethod
-    def get_xattr(self):
-        """ Name of the x-axis attribute. """
-        return ""
+    def x_title(self) -> str:
+        """ Title of the x-axis. """
 
+    @property
     @abstractmethod
-    def get_yattr(self):
-        """ Name of the y-axis attribute. """
-        return ""
+    def y_title(self) -> str:
+        """ Title of the y-axis. """
 
-    def _layout_figure(self, fig: go.Figure):
-        fig = super()._layout_figure(fig)
-        fig.update_layout(xaxis=dict(title=self.get_xattr()),
-                          yaxis=dict(title=self.get_yattr()))
-        return fig
+    def _figure_init(self):
+        return make_subplots(rows=self.nrows, cols=self.ncols,
+                             shared_xaxes="all", shared_yaxes="all",
+                             x_title=self.x_title, y_title=self.y_title,
+                             subplot_titles=self.subplot_titles)
 
 
 class GraphWriter(ABC):
     """ Write the proper types of graphs for a given table. """
 
     def __init__(self, table_file: Path):
         self.table_file = table_file
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/graph/color.py` & `seismic-rna-0.2.0/src/seismicrna/graph/color.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     def _set_colors(self, *, a: str, c: str, g: str, t: str):
         return {A_INT: a, C_INT: c, G_INT: g, T_INT: t}
 
 
 class RelColorMap(ColorMap):
     """ Color map for relationships. """
 
-    def __init__(self, name: str, b: str, n: str, r: str, m: str,
+    def __init__(self, name: str, v: str, n: str, r: str, m: str,
                  d: str, i: str, s: str, a: str, c: str, g: str, t: str):
-        super().__init__(name, b=b, n=n, r=r, m=m,
+        super().__init__(name, v=v, n=n, r=r, m=m,
                          d=d, i=i, s=s, a=a, c=c, g=g, t=t)
 
     def _set_colors(self, **kwargs):
         colors = dict()
         for key, field in REL_CODES.items():
             colors[field] = kwargs.pop(key)
         if kwargs:
@@ -53,23 +53,26 @@
         return colors
 
 
 basic = SeqColorMap("basic", a="#FF0000", c="#0000FF", g="#FFC000", t="#008000")
 water = SeqColorMap("water", a="#A15252", c="#3D427D", g="#E3CC7B", t="#76B887")
 earth = SeqColorMap("earth", a="#D17777", c="#464EA6", g="#E3CC7B", t="#336140")
 steel = SeqColorMap("steel", a="#663328", c="#716B80", g="#91B8AC", t="#D9D5B4")
+tetra = SeqColorMap("tetra", a="#C05F15", c="#597DE4", g="#743B4A", t="#9BD1D0")
 
-crayons = RelColorMap("crayons", b="#424242", n="#A9A9A9", r="#942193",
+crayons = RelColorMap("crayons", v="#424242", n="#A9A9A9", r="#942193",
                       m="#929000", d="#FF2600", i="#00FA92", s="#FF40FF",
                       a="#73FCD6", c="#FFD479", g="#7A81FF", t="#FF8AD8")
-
+sexta = RelColorMap("sexta", v="#FBED94", n="#C05F15", r="#597DE4",
+                    m="#0F155F", d="#FBED94", i="#0F155F", s="#743B4A",
+                    a="#C05F15", c="#597DE4", g="#743B4A", t="#9BD1D0")
 
 DEFAULTS: dict[type[ColorMap], ColorMap] = {
-    RelColorMap: crayons,
-    SeqColorMap: earth,
+    RelColorMap: sexta,
+    SeqColorMap: tetra,
 }
 
 
 @cache
 def get_colormaps(cmap_class: type[ColorMap]):
     """ Return a dict of all color maps of a given class. """
     colormaps: dict[str, cmap_class] = dict()
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/graph/default.py` & `seismic-rna-0.2.0/src/seismicrna/graph/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,9 +70,9 @@
                     if count:
                         yield MaskCountSerialPosBarGraph(table=self.table,
                                                          codes=field)
                     else:
                         yield MaskFracSerialPosBarGraph(table=self.table,
                                                         codes=field)
         elif isinstance(self.table, ClusterPosTableLoader):
-            for cluster in self.table.clusters:
+            for cluster in self.table.ord_clust:
                 yield ClustPosBarGraph(table=self.table, cluster=cluster)
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/graph/hist.py` & `seismic-rna-0.2.0/src/seismicrna/graph/hist.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 from click import command
 from plotly import graph_objects as go
 
 from .base import (find_tables, GraphWriter, CartesianGraph, OneTableGraph,
                    OneSampGraph)
 from .color import RelColorMap
 from ..core import docdef
-from ..core.cli import (opt_table, opt_table_cols,
-                        opt_yfrac, opt_hist_bins,
+from ..core.cli import (opt_table, opt_rels,
+                        opt_y_ratio, opt_hist_bins,
                         opt_csv, opt_html, opt_pdf,
                         opt_max_procs, opt_parallel)
 from ..core.parallel import dispatch
 from ..table.base import Table
 from ..table.load import (RelReadTableLoader,
                           MaskReadTableLoader, ClustReadTableLoader)
 
 # Number of digits to which to round decimals.
 PRECISION = 6
 
 params = [
     opt_table,
-    opt_table_cols,
+    opt_rels,
     opt_hist_bins,
-    opt_yfrac,
+    opt_y_ratio,
     opt_csv,
     opt_html,
     opt_pdf,
     opt_max_procs,
     opt_parallel,
 ]
 
@@ -44,48 +44,48 @@
     return run(*args, **kwargs)
 
 
 @docdef.auto()
 def run(table: tuple[str, ...],
         fields: str,
         hist_bins: int,
-        yfrac: bool, *,
+        y_ratio: bool, *,
         csv: bool,
         html: bool,
         pdf: bool,
         max_procs: int,
         parallel: bool) -> list[Path]:
     """ Run the graph read module. """
     writers = list(map(ReadHistogramWriter, find_tables(table)))
     return list(chain(*dispatch([writer.write for writer in writers],
                                 max_procs, parallel, pass_n_procs=False,
-                                kwargs=dict(fields=fields, count=yfrac,
+                                kwargs=dict(fields=fields, count=y_ratio,
                                             group=group, bins=hist_bins,
                                             csv=csv, html=html, pdf=pdf))))
 
 
 class ReadHistogramWriter(GraphWriter):
 
     def iter(self, fields: str, bins: int, count: bool, group: bool):
         if isinstance(self.table, RelReadTableLoader):
             if group:
                 yield RelReadHist(table=self.table, codes=fields,
-                                  xfrac=bins, yfrac=count)
+                                  x_ratio=bins, y_ratio=count)
             else:
                 for field in fields:
                     yield RelReadHist(table=self.table, codes=field,
-                                      xfrac=bins, yfrac=count)
+                                      x_ratio=bins, y_ratio=count)
         elif isinstance(self.table, MaskReadTableLoader):
             if group:
                 yield MaskReadHist(table=self.table, codes=fields,
-                                   xfrac=bins, yfrac=count)
+                                   x_ratio=bins, y_ratio=count)
             else:
                 for field in fields:
                     yield MaskReadHist(table=self.table, codes=field,
-                                       xfrac=bins, yfrac=count)
+                                       x_ratio=bins, y_ratio=count)
 
 
 class ReadHistogram(CartesianGraph, OneTableGraph, OneSampGraph, ABC):
     """ Histogram of an attribute of reads. """
 
     def __init__(self, *args,
                  table: (Table | RelReadTableLoader
@@ -112,25 +112,25 @@
     def get_cmap_type(cls):
         return RelColorMap
 
 
 class FieldReadHist(ReadHistogram, ABC):
     """ Read histogram of fields from a table. """
 
-    def __init__(self, *args, codes: str, xfrac: int, yfrac: bool, **kwargs):
+    def __init__(self, *args, codes: str, x_ratio: int, y_ratio: bool, **kwargs):
         super().__init__(*args, **kwargs)
         self.codes = codes
-        self.xfrac = xfrac
-        self.yfrac = yfrac
+        self.x_ratio = x_ratio
+        self.y_ratio = y_ratio
 
     def get_xattr(self):
-        return "Fraction" if self.xfrac else "Count"
+        return "Fraction" if self.x_ratio else "Count"
 
     def get_yattr(self):
-        return "Read" + ("Fraction" if self.yfrac else "Count")
+        return "Read" + ("Fraction" if self.y_ratio else "Count")
 
     @property
     def title(self):
         fields = '/'.join(sorted(Table.REL_CODES[c] for c in self.codes))
         return (f"{self.get_yattr()}s of {self.get_source()} {fields} bases "
                 f"per read from sample {self.sample} over reference {self.ref}")
 
@@ -139,35 +139,35 @@
         sort_codes = "".join(sorted(self.codes))
         fname = f"{self.get_source()}_{self.get_yattr()}_{sort_codes}_per-read"
         return fname.lower()
 
     def get_table_field(self, field_code: str):
         """ Load the data for one field from the table. """
         return (self.table.fract_rel(field_code).round(PRECISION)
-                if self.xfrac else self.table.count_rel(field_code))
+                if self.x_ratio else self.table.count_rel(field_code))
 
     @cache
     def _find_data_max(self):
         """ Find the maximum value in the data table. """
         return max(np.nanmax(self.get_table_field(code)) for code in self.codes)
 
     @cache
     def _get_bins(self):
         """ Get the bin edges for the histogram. """
-        if self.xfrac < 0:
-            raise ValueError(f"xfrac must be ≥ 0, but got {self.xfrac}")
-        if self.xfrac == 0:
+        if self.x_ratio < 0:
+            raise ValueError(f"x_ratio must be ≥ 0, but got {self.x_ratio}")
+        if self.x_ratio == 0:
             # Each bin has width 1, with the maximum being the smallest
             # integer larger than every value in the data set.
             max_bin = int(self._find_data_max()) + 1
             n_bins = max_bin
         else:
-            # The maximum value is 1, and the number of bins is xfrac.
+            # The maximum value is 1, and the number of bins is x_ratio.
             max_bin = 1
-            n_bins = self.xfrac
+            n_bins = self.x_ratio
         return np.linspace(0, max_bin, n_bins + 1)
 
     def _get_data(self):
         data = dict()
         bins = self._get_bins()
         for code in self.codes:
             # Compute the histogram for the field.
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/graph/seq.py` & `seismic-rna-0.2.0/src/seismicrna/table/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,263 +1,341 @@
 from abc import ABC, abstractmethod
-from functools import cache
-from itertools import chain
-from logging import getLogger
-import os
+from functools import cache, cached_property
 from pathlib import Path
+from typing import Any
 
-from click import command
 import pandas as pd
-from plotly import graph_objects as go
 
-from .base import (PRECISION, find_tables, GraphWriter, CartesianGraph,
-                   OneTableSeqGraph, OneSampGraph)
-from .color import RelColorMap, SeqColorMap
-from ..core import docdef
-from ..core.cli import (opt_table, opt_table_cols, opt_stack, opt_yfrac,
-                        opt_csv, opt_html, opt_pdf, opt_max_procs, opt_parallel)
-from ..core.parallel import dispatch
-from ..core.sect import BASE_NAME, POS_NAME
-from ..core.seq import BASES
-from ..core.types import get_subclasses_module
-from ..table.base import RelTypeTable, REL_CODES
-from ..table.load import (TableLoader, RelPosTableLoader,
-                          MaskPosTableLoader, ClustPosTableLoader)
-
-logger = getLogger(__name__)
-
-# Number of digits to which to round decimals.
-
-params = [
-    opt_table,
-    opt_table_cols,
-    opt_stack,
-    opt_yfrac,
-    opt_csv,
-    opt_html,
-    opt_pdf,
-    opt_max_procs,
-    opt_parallel,
-]
-
-
-@command(__name__.split(os.path.extsep)[-1], params=params)
-def cli(*args, **kwargs):
-    """ Create bar graphs of positional attributes. """
-    return run(*args, **kwargs)
-
-
-@docdef.auto()
-def run(table: tuple[str, ...],
-        table_cols: str,
-        stack: bool,
-        yfrac: bool, *,
-        csv: bool,
-        html: bool,
-        pdf: bool,
-        max_procs: int,
-        parallel: bool) -> list[Path]:
-    """ Run the graph pos module. """
-    writers = list(map(SeqGraphWriter, find_tables(table)))
-    return list(chain(*dispatch([writer.write for writer in writers],
-                                max_procs, parallel, pass_n_procs=False,
-                                kwargs=dict(rels=table_cols, stack=stack,
-                                            yfrac=yfrac, csv=csv,
-                                            html=html, pdf=pdf))))
-
-
-class SeqGraphWriter(GraphWriter):
-
-    def iter(self, rels: str, stack: str, yfrac: bool):
-        for rel in rels:
-            for graph_type in get_subclasses_module(SerialSeqGraph, __name__):
-                if type(self.table) in graph_type.sources():
-                    yield graph_type(table=self.table, codes=rel, yfrac=yfrac)
-        if stack:
-            for graph_type in get_subclasses_module(StackedSeqGraph, __name__):
-                if type(self.table) in graph_type.sources():
-                    yield graph_type(table=self.table, codes=stack, yfrac=yfrac)
-
-
-# Base Sequence Graphs #################################################
-
-class SeqGraph(CartesianGraph, OneTableSeqGraph, OneSampGraph, ABC):
-    """ Bar graph wherein each bar represents one sequence position. """
-
-    def __init__(self, *args,
-                 table: (RelPosTableLoader
-                         | MaskPosTableLoader
-                         | ClustPosTableLoader),
-                 codes: str,
-                 yfrac: bool,
-                 **kwargs):
-        super().__init__(*args, **kwargs)
-        self.table = table
-        self.codes = codes
-        self.yfrac = yfrac
+from ..cluster.names import CLS_NAME, ORD_NAME
+from ..core import path
+from ..core.sect import index_to_pos, index_to_seq
+
+# General fields
+READ_TITLE = "Read Name"
+R_OBS_TITLE = "Reads Observed"
+R_ADJ_TITLE = "Reads Adjusted"
+REL_NAME = "Relationship"
+CLUST_INDEX_NAMES = ORD_NAME, CLS_NAME, REL_NAME
+
+# Count relationships
+COVER_REL = "Covered"
+INFOR_REL = "Informed"
+MATCH_REL = "Matched"
+MUTAT_REL = "Mutated"
+DELET_REL = "Deleted"
+INSRT_REL = "Inserted"
+SUBST_REL = "Subbed"
+SUB_A_REL = "Subbed-A"
+SUB_C_REL = "Subbed-C"
+SUB_G_REL = "Subbed-G"
+SUB_T_REL = "Subbed-T"
+
+# One-letter codes for each type of relationship
+REL_CODES = {
+    'v': COVER_REL,
+    'n': INFOR_REL,
+    'r': MATCH_REL,
+    'm': MUTAT_REL,
+    's': SUBST_REL,
+    'a': SUB_A_REL,
+    'c': SUB_C_REL,
+    'g': SUB_G_REL,
+    't': SUB_T_REL,
+    'd': DELET_REL,
+    'i': INSRT_REL,
+}
 
-    @classmethod
-    @abstractmethod
-    def sources(cls) -> dict[type[TableLoader], str]:
-        """ Names of the sources of data. """
-        return dict()
+# Columns of each relation-based table
+TABLE_COLUMNS = [rel for rel in REL_CODES.values() if rel != INFOR_REL]
 
-    @property
-    def source(self):
-        """ Source of the data. """
-        table_type = type(self.table)
-        try:
-            return self.sources()[table_type]
-        except KeyError:
-            raise TypeError(f"Invalid table for {self}: {table_type.__name__}")
 
-    @classmethod
-    def get_cmap_type(cls):
-        return SeqColorMap
+# Table Base Classes ###################################################
 
-    def get_xattr(self):
-        return POS_NAME
+class Table(ABC):
+    """ Table base class. """
 
-    def get_yattr(self):
-        return "Fraction" if self.yfrac else "Count"
+    @property
+    @abstractmethod
+    def out_dir(self):
+        """ Path of the table's output directory. """
+        return Path()
 
     @property
-    def title(self):
-        fields = '/'.join(sorted(REL_CODES[c] for c in self.codes))
-        return (f"{self.get_yattr()}s of {fields} bases in {self.source} reads "
-                f"from {self.sample} per position in {self.ref}:{self.sect}")
+    @abstractmethod
+    def sample(self):
+        """ Name of the table's sample. """
+        return ""
 
     @property
     @abstractmethod
-    def sort_codes(self):
-        return "".join(sorted(self.codes))
+    def ref(self):
+        """ Name of the table's reference. """
+        return ""
 
     @property
-    def graph_filename(self):
-        return f"{self.source}_{self.sort_codes}_{self.get_yattr()}".lower()
+    @abstractmethod
+    def sect(self):
+        """ Name of the table's section. """
+        return ""
 
-    def get_table_field(self, table: RelTypeTable | TableLoader, code: str):
-        return (table.fract_rel(code).round(PRECISION) if self.yfrac
-                else table.count_rel(code))
+    @cached_property
+    @abstractmethod
+    def data(self) -> pd.DataFrame:
+        """ Table's data frame. """
+        return pd.DataFrame()
 
+    @classmethod
+    @abstractmethod
+    def kind(cls) -> str:
+        """ Kind of table. """
+        return ""
 
-# Sequence Graphs by Source ############################################
+    @classmethod
+    @abstractmethod
+    def by_read(cls):
+        """ Whether the table contains data for each read. """
+        return False
 
-class PopAvgSeqGraph(SeqGraph, ABC):
+    @classmethod
+    def path_segs(cls):
+        """ Table's path segments. """
+        return (path.ModSeg, path.SampSeg, path.RefSeg, path.SectSeg,
+                path.MutTabSeg)
 
     @classmethod
-    def sources(cls) -> dict[type[TableLoader], str]:
-        return {RelPosTableLoader: "Related",
-                MaskPosTableLoader: "Masked"}
+    def gzipped(cls):
+        """ Whether the table's file is compressed with gzip. """
+        return cls.by_read()
 
+    @classmethod
+    def ext(cls):
+        """ Table's file extension: either '.csv' or '.csv.gz'. """
+        return path.CSVZIP_EXT if cls.gzipped() else path.CSV_EXT
 
-class ClustSeqGraph(SeqGraph, ABC):
+    @property
+    def path_fields(self) -> dict[str, Any]:
+        """ Table's path fields. """
+        return {path.TOP: self.out_dir,
+                path.MOD: path.MOD_TABLE,
+                path.SAMP: self.sample,
+                path.REF: self.ref,
+                path.SECT: self.sect,
+                path.TABLE: self.kind(),
+                path.EXT: self.ext()}
+
+    @cached_property
+    def path(self):
+        """ Path of the table's CSV file (possibly gzipped). """
+        return path.buildpar(*self.path_segs(), **self.path_fields)
 
-    @classmethod
-    def sources(cls) -> dict[type[TableLoader], str]:
-        return {ClustPosTableLoader: "Clustered"}
+    def __str__(self):
+        return f"{self.__class__.__name__} at {self.path}"
 
-    @classmethod
-    def get_data_type(cls):
-        return pd.DataFrame
+
+class RelTypeTable(Table, ABC):
+    """ Table with multiple types of relationships. """
+
+    @property
+    def _rel_level_index(self):
+        """ Index of the column level indicating the relationship. """
+        return self.data.columns.names.index(REL_NAME)
+
+    def _switch_rel(self, column: tuple, new_rel: str):
+        """ Switch the relationship in a column label. """
+        return new_rel,
+
+    @cache
+    def _count_col(self, column: tuple):
+        """ Count the bits for a column. """
+        # Determine the relationship to count.
+        if column[self._rel_level_index] == INFOR_REL:
+            # Sum the matched and mutated bits.
+            match_col = self._switch_rel(column, MATCH_REL)
+            mutat_col = self._switch_rel(column, MUTAT_REL)
+            return self._count_col(match_col) + self._count_col(mutat_col)
+        try:
+            # The relationship should appear in the table, so return it
+            # as a Series.
+            return self.data.loc[:, column].squeeze()
+        except KeyError:
+            # Suppress exception chaining.
+            pass
+        raise ValueError(f"{self} was not built with column {column}")
+
+    @cache
+    def _ratio_col(self, column: tuple, precision: int | None = None):
+        """ Compute the ratio for a column. """
+        # Determine the relationship to use as the numerator.
+        numer_rel = column[self._rel_level_index]
+        # Determine the relationship to use as the denominator.
+        denom_rel = COVER_REL if numer_rel == INFOR_REL else INFOR_REL
+        # Determine the column to use as the denominator.
+        denom_col = self._switch_rel(column, denom_rel)
+        # Compute the ratio of the numerator and the denominator.
+        ratio = self._count_col(column) / self._count_col(denom_col)
+        # Round the ratio to the desired precision.
+        if precision is not None:
+            ratio = ratio.round(precision)
+        return ratio
+
+    @staticmethod
+    def _format_selection(**kwargs) -> dict[str, list]:
+        """ Format keyword arguments into a valid column selection. """
+        selection = dict()
+        for key, level in dict(order=ORD_NAME,
+                               cluster=CLS_NAME,
+                               rels=REL_NAME).items():
+            try:
+                selection[level] = kwargs[key]
+            except KeyError:
+                pass
+        return selection
+
+    def _get_indexer(self, selection: dict[str, list]):
+        """ Format a column selection into a column indexer. """
+        return selection.get(REL_NAME, slice(None))
+
+    def select(self, ratio: bool, precision: int | None = None, **kwargs: list):
+        """ Output selected data from the table as a DataFrame. """
+        # Instantiate an empty DataFrame with the index and columns.
+        indexer = self._get_indexer(self._format_selection(**kwargs))
+        columns = self.data.loc[:, indexer].columns
+        data = pd.DataFrame(index=self.data.index, columns=columns, dtype=float)
+        # Fill in the DataFrame one column at a time.
+        for column in columns:
+            data.loc[:, column] = (self._ratio_col(column, precision) if ratio
+                                   else self._count_col(column))
+        return data
+
+
+# Table by Source (relate/mask/cluster) ################################
+
+class RelTable(RelTypeTable, ABC):
+    pass
+
+
+class MaskTable(RelTypeTable, ABC):
+    pass
+
+
+class ClustTable(RelTypeTable, ABC):
+
+    @cached_property
+    def ord_clust(self):
+        """ MultiIndex of all order-cluster pairs. """
+        return self.data.columns.droplevel(REL_NAME).drop_duplicates()
+
+    @cached_property
+    def orders(self):
+        """ Index of all order numbers. """
+        return self.data.columns.get_level_values(ORD_NAME).drop_duplicates()
+
+    def get_clusters(self, orders: list):
+        """ Index of cluster numbers for the given orders. """
+        data = self.data.loc[:, orders]
+        return data.columns.get_level_values(CLS_NAME).drop_duplicates()
+
+    def _switch_rel(self, column: tuple, new_rel: str):
+        return (column[: self._rel_level_index]
+                + (new_rel,)
+                + column[self._rel_level_index + 1:])
+
+    def _get_indexer(self, selection: dict[str, list]):
+        return tuple(selection.get(level, slice(None))
+                     for level in self.data.columns.names)
 
 
-# Sequence Graphs by Series Type #######################################
+# Table by Index (position/read/frequency) #############################
 
-class SerialSeqGraph(SeqGraph, ABC):
-    """ Bar graph with a single series of data. """
+class PosTable(RelTypeTable, ABC):
+    """ Table indexed by position. """
+
+    @classmethod
+    def by_read(cls):
+        return False
 
-    def get_traces(self):
-        traces = list()
-        # Construct a trace for each type of base.
-        for base in BASES:
-            letter = chr(base)
-            # Find the position of every base of that type.
-            seq_mask = self.data.index.get_level_values(BASE_NAME) == letter
-            # Get the values at those positions, excluding NaN values.
-            vals = self.data.loc[seq_mask].dropna()
-            # Set the index of the values to the numerical positions.
-            vals.index = vals.index.get_level_values(POS_NAME)
-            # Check if there are any values to graph.
-            if vals.size > 0:
-                # Define the text shown on hovering over a bar.
-                hovertext = [f"{letter}{x}: {y}" for x, y in vals.items()]
-                # Create a trace comprising all bars for this base type.
-                traces.append(go.Bar(name=letter, x=vals.index, y=vals,
-                                     marker_color=self.cmap[base],
-                                     hovertext=hovertext,
-                                     hoverinfo="text"))
-        return traces
+    @cached_property
+    def seq(self):
+        return index_to_seq(self.data.index)
 
     @property
-    def code(self):
-        """ The code of the field to graph. """
-        if len(self.codes) != 1:
-            raise ValueError(f"Expected 1 code, but got {len(self.codes)}")
-        return self.codes[0]
+    def positions(self):
+        return index_to_pos(self.data.index)
 
     @property
-    def sort_codes(self):
-        return "-".join(["serial", super().sort_codes])
+    def end5(self):
+        return int(self.positions[0])
 
-    def _get_data(self) -> pd.Series:
-        return self.get_table_field(self.table, self.code)
+    @property
+    def end3(self):
+        return int(self.positions[-1])
 
 
-class StackedSeqGraph(SeqGraph, ABC):
-    """ Stacked bar graph wherein each stacked bar represents multiple
-    outcomes for a base in a sequence. """
+class ReadTable(RelTypeTable, ABC):
+    """ Table indexed by read. """
 
     @classmethod
-    def get_cmap_type(cls):
-        return RelColorMap
+    def by_read(cls):
+        return True
 
     @property
-    def sort_codes(self):
-        return "-".join(["stacked", super().sort_codes])
+    def reads(self):
+        return self.data.index.values
 
-    def _get_data(self):
-        data = dict()
-        for code in self.codes:
-            series = self.get_table_field(self.table, code)
-            data[series.name] = series
-        return pd.DataFrame.from_dict(data)
 
-    def get_traces(self):
-        traces = list()
-        # Construct a trace for each field.
-        for field, vals in self.data.items():
-            # Get the sequence and positions.
-            bases = vals.index.get_level_values(BASE_NAME)
-            pos = vals.index.get_level_values(POS_NAME)
-            # Define the text shown on hovering over a bar.
-            hovertext = [f"{base}{x} {field}: {y}"
-                         for base, x, y in zip(bases, pos, vals, strict=True)]
-            # Create a trace comprising all bars for this field.
-            traces.append(go.Bar(name=field, x=pos, y=vals,
-                                 marker_color=self.cmap[field],
-                                 hovertext=hovertext,
-                                 hoverinfo="text"))
-        return traces
+# Table by Source and Index ############################################
+
+class RelPosTable(RelTable, PosTable, ABC):
+
+    @classmethod
+    def kind(cls):
+        return path.RELATE_POS_TAB
 
-    @cache
-    def get_figure(self):
-        fig = super().get_figure()
-        # Stack the bars at each position.
-        fig.update_layout(barmode="stack")
-        return fig
 
+class MaskPosTable(MaskTable, PosTable, ABC):
+
+    @classmethod
+    def kind(cls):
+        return path.MASKED_POS_TAB
 
-# Instantiable Sequence Graphs #########################################
 
-class PopAvgSerialSeqGraph(PopAvgSeqGraph, SerialSeqGraph):
+class ClustPosTable(ClustTable, PosTable, ABC):
 
     @classmethod
-    def get_data_type(cls):
-        return pd.Series
+    def kind(cls):
+        return path.CLUST_POS_TAB
 
 
-class PopAvgStackedSeqGraph(PopAvgSeqGraph, StackedSeqGraph):
+class RelReadTable(RelTable, ReadTable, ABC):
 
     @classmethod
-    def get_data_type(cls):
-        return pd.DataFrame
+    def kind(cls):
+        return path.RELATE_READ_TAB
+
+
+class MaskReadTable(MaskTable, ReadTable, ABC):
+
+    @classmethod
+    def kind(cls):
+        return path.MASKED_READ_TAB
+
+
+class ClustReadTable(ClustTable, ReadTable, ABC):
+
+    @classmethod
+    def kind(cls):
+        return path.CLUST_READ_TAB
+
+
+class ClustFreqTable(Table, ABC):
+
+    @classmethod
+    def kind(cls):
+        return path.CLUST_FREQ_TAB
+
+    @classmethod
+    def by_read(cls):
+        return False
+
+    @property
+    def clusters(self):
+        return self.data.index.values
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/main.py` & `seismic-rna-0.2.0/src/seismicrna/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,35 +40,33 @@
         out_dir: str,
         temp_dir: str,
         save_temp: bool,
         rerun: bool,
         max_procs: int,
         parallel: bool,
         # Input files
+        input_file: tuple[str, ...],
         fasta: str,
         fastqs: tuple[str, ...],
         fastqi: tuple[str, ...],
-        fastqm: tuple[str, ...],
+        fastqp: tuple[str, ...],
         phred_enc: int,
-        bam: tuple[str, ...],
-        report: tuple[str, ...],
-        table: tuple[str, ...],
         # Demultiplexing
         demulti_overwrite: bool,
         demult_on: bool,
         parallel_demultiplexing: bool,
         clipped: int,
         mismatch_tolerence: int,
         index_tolerance: int,
         barcode_start: int,
         barcode_length: int,
         # Alignment
         dmfastqs: tuple[str, ...],
         dmfastqi: tuple[str, ...],
-        dmfastqm: tuple[str, ...],
+        dmfastqp: tuple[str, ...],
         fastqc: bool,
         qc_extract: bool,
         cut: bool,
         cut_q1: int,
         cut_q2: int,
         cut_g1: tuple[str, ...],
         cut_a1: tuple[str, ...],
@@ -103,15 +101,15 @@
         min_reads: int,
         ambrel: bool,
         batch_size: float,
         # Masking
         coords: tuple[tuple[str, int, int], ...],
         primers: tuple[tuple[str, str, str], ...],
         primer_gap: int,
-        library: str,
+        sections_file: str,
         count_del: bool,
         count_ins: bool,
         discount_mut: tuple[str, ...],
         exclude_polya: int,
         exclude_gu: bool,
         exclude_pos: tuple[tuple[str, int], ...],
         min_finfo_read: float,
@@ -122,53 +120,53 @@
         # Clustering
         max_clusters: int,
         em_runs: int,
         min_em_iter: int,
         max_em_iter: int,
         em_thresh: float,
         # Tabulation
-        table_cols: str,
+        rels: str,
         # Folding
         fold: bool,
-        dms_quantile: float):
+        quantile: float):
     """ Run entire pipeline. """
     # Demultiplexing
     if demult_on:
         for dms, dmi, dmm in demultiplex_mod.run(
                 fasta=fasta,
-                library=library,
+                sections_file=sections_file,
                 out_dir=out_dir,
                 temp_dir=temp_dir,
                 demulti_overwrite=demulti_overwrite,
-                fastqm=fastqm,
+                fastqp=fastqp,
                 clipped=clipped,
                 index_tolerance=index_tolerance,
                 mismatch_tolerence=mismatch_tolerence,
                 parallel_demultiplexing=parallel_demultiplexing,
                 barcode_start=barcode_start,
                 barcode_length=barcode_length,
                 phred_enc=phred_enc):
             dmfastqs = dmfastqs + dms
             dmfastqi = dmfastqi + dmi
-            dmfastqm = dmfastqm + dmm
+            dmfastqp = dmfastqp + dmm
     # Alignment
-    bam += tuple(map(str, align_mod.run(
+    input_file += tuple(map(str, align_mod.run(
         out_dir=out_dir,
         temp_dir=temp_dir,
         save_temp=save_temp,
         rerun=rerun,
         max_procs=max_procs,
         parallel=parallel,
         fasta=fasta,
         fastqs=fastqs,
         fastqi=fastqi,
-        fastqm=fastqm,
+        fastqp=fastqp,
         dmfastqs=dmfastqs,
         dmfastqi=dmfastqi,
-        dmfastqm=dmfastqm,
+        dmfastqp=dmfastqp,
         phred_enc=phred_enc,
         fastqc=fastqc,
         qc_extract=qc_extract,
         cut=cut,
         cut_q1=cut_q1,
         cut_q2=cut_q2,
         cut_g1=cut_g1,
@@ -197,36 +195,36 @@
         bt2_s=bt2_s,
         bt2_d=bt2_d,
         bt2_r=bt2_r,
         bt2_dpad=bt2_dpad,
         bt2_orient=bt2_orient
     )))
     # Relating
-    report += tuple(map(str, relate_mod.run(
+    input_file += tuple(map(str, relate_mod.run(
         fasta=fasta,
-        bam=bam,
+        input_file=input_file,
         out_dir=out_dir,
         temp_dir=temp_dir,
         phred_enc=phred_enc,
         min_phred=min_phred,
         min_reads=min_reads,
         ambrel=ambrel,
         batch_size=batch_size,
         max_procs=max_procs,
         parallel=parallel,
         rerun=rerun,
         save_temp=save_temp,
     )))
     # Masking
-    report += tuple(map(str, mask_mod.run(
-        report=report,
+    input_file += tuple(map(str, mask_mod.run(
+        input_file=input_file,
         coords=coords,
         primers=primers,
         primer_gap=primer_gap,
-        library=library,
+        sections_file=sections_file,
         count_del=count_del,
         count_ins=count_ins,
         discount_mut=discount_mut,
         exclude_polya=exclude_polya,
         exclude_gu=exclude_gu,
         exclude_pos=exclude_pos,
         min_finfo_read=min_finfo_read,
@@ -235,43 +233,43 @@
         min_ninfo_pos=min_ninfo_pos,
         max_fmut_pos=max_fmut_pos,
         max_procs=max_procs,
         parallel=parallel,
         rerun=rerun,
     )))
     # Clustering
-    report += tuple(map(str, cluster_mod.run(
-        report=report,
+    input_file += tuple(map(str, cluster_mod.run(
+        input_file=input_file,
         max_clusters=max_clusters,
         em_runs=em_runs,
         min_em_iter=min_em_iter,
         max_em_iter=max_em_iter,
         em_thresh=em_thresh,
         max_procs=max_procs,
         parallel=parallel,
         rerun=rerun,
     )))
     # Table
-    table += tuple(map(str, table_mod.run(
-        report=report,
-        table_cols=table_cols,
+    input_file += tuple(map(str, table_mod.run(
+        input_file=input_file,
+        rels=rels,
         max_procs=max_procs,
         parallel=parallel,
         rerun=rerun,
     )))
     # Fold
     if fold:
         fold_mod.run(
-            table=table,
+            input_file=input_file,
             fasta=fasta,
-            library=library,
+            sections_file=sections_file,
             coords=coords,
             primers=primers,
             primer_gap=primer_gap,
-            dms_quantile=dms_quantile,
+            quantile=quantile,
             temp_dir=temp_dir,
             save_temp=save_temp,
             max_procs=max_procs,
             parallel=parallel,
             rerun=rerun,
         )
     # Graph
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/mask/load.py` & `seismic-rna-0.2.0/src/seismicrna/mask/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         for batch in self.iter_batches_personal():
             yield batch.values
 
     def get_read_names(self):
         """ Return an array naming all reads that were kept. """
         if self.num_batches > 0:
             # Concatenate all indexes, which have the read names.
-            return np.hstack(self.iter_read_batches())
+            return np.hstack(list(self.iter_read_batches()))
         # If there are no batches, return an empty array.
         return np.array([], dtype=str)
 
     def process_batch(self, imported_batch: pd.DataFrame,
                       private_batch: pd.Series, *,
                       bit_caller: BitCaller | None = None,
                       merge: bool = False, invert: bool = False):
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/mask/main.py` & `seismic-rna-0.2.0/src/seismicrna/mask/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from typing import Iterable
 
 from click import command
 
 from .write import mask_section
 from ..relate.load import open_reports
 from ..core import docdef, path
-from ..core.cli import (opt_report,
-                        opt_coords, opt_primers, opt_primer_gap, opt_library,
+from ..core.cli import (opt_input_file,
+                        opt_coords, opt_primers, opt_primer_gap, opt_sections_file,
                         opt_count_del, opt_count_ins, opt_discount_mut,
                         opt_exclude_polya, opt_exclude_gu, opt_exclude_pos,
                         opt_min_finfo_read, opt_max_fmut_read, opt_min_mut_gap,
                         opt_min_ninfo_pos, opt_max_fmut_pos,
                         opt_max_procs, opt_parallel, opt_rerun)
 from ..core.parallel import dispatch
 from ..core.sect import encode_primers, RefSections
 from ..core.seq import DNA
 
 logger = getLogger(__name__)
 
 params = [
     # Input/output paths
-    opt_report,
+    opt_input_file,
     # Sections
-    opt_coords, opt_primers, opt_primer_gap, opt_library,
+    opt_coords, opt_primers, opt_primer_gap, opt_sections_file,
     # Mutation counting
     opt_count_del, opt_count_ins, opt_discount_mut,
     # Filtering
     opt_exclude_polya, opt_exclude_gu, opt_exclude_pos,
     opt_min_finfo_read, opt_max_fmut_read, opt_min_mut_gap,
     opt_min_ninfo_pos, opt_max_fmut_pos,
     # Parallelization
@@ -42,20 +42,20 @@
 def cli(*args, **kwargs):
     """ Select a section of the reference, define which relationships
     count as mutations, and filter out unusable positions and reads. """
     return run(*args, **kwargs)
 
 
 @docdef.auto()
-def run(report: tuple[str, ...], *,
+def run(input_file: tuple[str, ...], *,
         # Sections
         coords: tuple[tuple[str, int, int], ...],
         primers: tuple[tuple[str, str, str], ...],
         primer_gap: int,
-        library: str,
+        sections_file: str,
         # Mutation counting
         count_del: bool,
         count_ins: bool,
         discount_mut: tuple[str, ...],
         # Filtering
         exclude_polya: int,
         exclude_gu: bool,
@@ -68,20 +68,21 @@
         # Parallelization
         max_procs: int,
         parallel: bool,
         # Effort
         rerun: bool) -> list[Path]:
     """ Run the filtering module. """
     # Open all relation vector loaders and get the sections for each.
-    loaders, sections = open_sections(map(Path, report),
+    loaders, sections = open_sections(map(Path, input_file),
                                       coords=coords,
                                       primers=encode_primers(primers),
                                       primer_gap=primer_gap,
-                                      library=(Path(library) if library
-                                               else None))
+                                      sections_file=(Path(sections_file)
+                                                     if sections_file
+                                                     else None))
     # List the relation loaders and their sections.
     args = [(loader, section) for loader in loaders
             for section in sections.list(loader.ref)]
     # Define the keyword arguments.
     kwargs = dict(count_del=count_del,
                   count_ins=count_ins,
                   discount=discount_mut,
@@ -100,15 +101,15 @@
     return list(map(Path, reports))
 
 
 def open_sections(report_paths: Iterable[Path],
                   coords: Iterable[tuple[str, int, int]],
                   primers: Iterable[tuple[str, DNA, DNA]],
                   primer_gap: int,
-                  library: Path | None = None):
+                  sections_file: Path | None = None):
     """ Open sections of relate reports. """
     report_files = path.find_files_chain(report_paths, [path.RelateRepSeg])
     loaders = open_reports(report_files)
     sections = RefSections({(rep.ref, rep.seq) for rep in loaders},
                            coords=coords, primers=primers, primer_gap=primer_gap,
-                           library=library)
+                           sects_file=sections_file)
     return loaders, sections
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/mask/report.py` & `seismic-rna-0.2.0/src/seismicrna/mask/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/mask/write.py` & `seismic-rna-0.2.0/src/seismicrna/mask/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/export.py` & `seismic-rna-0.2.0/src/seismicrna/relate/export.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/load.py` & `seismic-rna-0.2.0/src/seismicrna/relate/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/main.py` & `seismic-rna-0.2.0/src/seismicrna/relate/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 from logging import getLogger
 from pathlib import Path
 
 from click import command
 
 from .write import relate_all, get_relaters
 from ..core import docdef, path
-from ..core.cli import (opt_fasta, opt_bam,
+from ..core.cli import (opt_fasta, opt_input_file,
                         opt_out_dir, opt_temp_dir,
                         opt_phred_enc, opt_min_phred,
                         opt_min_reads, opt_batch_size, opt_ambrel,
                         opt_parallel, opt_max_procs,
                         opt_rerun, opt_save_temp)
 from ..core.parallel import lock_temp_dir
 
 logger = getLogger(__name__)
 
 # Parameters for command line interface
 params = [
     # Input files
     opt_fasta,
-    opt_bam,
+    opt_input_file,
     # Output directories
     opt_out_dir,
     opt_temp_dir,
     # SAM options
     opt_phred_enc,
     opt_min_phred,
     # Vectoring options
@@ -54,15 +54,15 @@
     the reference base to which it aligned. """
     return run(**kwargs)
 
 
 @lock_temp_dir
 @docdef.auto()
 def run(fasta: str,
-        bam: tuple[str, ...],
+        input_file: tuple[str, ...],
         *,
         out_dir: str,
         temp_dir: str,
         phred_enc: int,
         min_phred: int,
         min_reads: int,
         batch_size: float,
@@ -81,15 +81,15 @@
     """
 
     if not fasta:
         logger.critical(f"No FASTA file given to {path.MOD_REL}")
         return list()
 
     # For each BAM file, create a relation writer.
-    relaters = get_relaters(path.find_files_chain(map(Path, bam),
+    relaters = get_relaters(path.find_files_chain(map(Path, input_file),
                                                   [path.SampSeg, path.XamSeg]),
                             Path(fasta),
                             min_reads=min_reads,
                             max_procs=max_procs,
                             parallel=parallel)
 
     # Compute and write relation vectors for each relation writer.
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/relate.py` & `seismic-rna-0.2.0/src/seismicrna/relate/relate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/report.py` & `seismic-rna-0.2.0/src/seismicrna/relate/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/sam.py` & `seismic-rna-0.2.0/src/seismicrna/relate/sam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/seqpos.py` & `seismic-rna-0.2.0/src/seismicrna/relate/seqpos.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/test.py` & `seismic-rna-0.2.0/src/seismicrna/relate/test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.3/src/seismicrna/relate/write.py` & `seismic-rna-0.2.0/src/seismicrna/relate/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,16 @@
     relframe = pd.DataFrame(data=relmatrix,
                             index=read_names,
                             columns=columns,
                             copy=False)
     # Build the path to the batch file.
     batch_path = RelateReport.build_batch_path(out_dir, batch, sample=sample,
                                                ref=ref, ext=path.PARQ_EXTS[0])
-    relframe.to_parquet(batch_path, index=True)
+    relframe.to_parquet(batch_path, index=True, engine="pyarrow",
+                        compression="brotli")
     logger.info(f"Ended writing sample '{sample}' reference '{ref}' "
                 f"batch {batch} to {batch_path}")
     return batch_path
 
 
 def _relate_record(read_name: bytes, line1: bytes, line2: bytes, *,
                    blank_rv: bytearray, refseq: bytes, ref: str,
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/struct/main.py` & `seismic-rna-0.2.0/src/seismicrna/struct/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from logging import getLogger
 from pathlib import Path
 
 from click import command
 
 from .rnastructure import fold, ct2dot
 from ..core import docdef, path
-from ..core.cli import (opt_temp_dir, opt_save_temp, opt_table,
-                        opt_fasta, opt_library,
+from ..core.cli import (opt_temp_dir, opt_save_temp, opt_input_file,
+                        opt_fasta, opt_sections_file,
                         opt_coords, opt_primers, opt_primer_gap,
-                        opt_dms_quantile,
+                        opt_quantile,
                         opt_max_procs, opt_parallel, opt_rerun)
 from ..core.depend import confirm_dependency
 from ..core.parallel import as_list_of_tuples, dispatch, lock_temp_dir
 from ..core.rna import RnaProfile
 from ..core.sect import RefSections, Section, encode_primers
 from ..core.seq import parse_fasta
 from ..core.shell import RNASTRUCTURE_FOLD_CMD
 from ..table.load import load, MaskPosTableLoader, ClustPosTableLoader
 
 logger = getLogger(__name__)
 
 params = [
-    opt_table,
+    opt_input_file,
     opt_fasta,
-    opt_library,
+    opt_sections_file,
     opt_coords,
     opt_primers,
     opt_primer_gap,
-    opt_dms_quantile,
+    opt_quantile,
     opt_temp_dir,
     opt_save_temp,
     opt_max_procs,
     opt_parallel,
     opt_rerun,
 ]
 
@@ -41,22 +41,22 @@
     """ Predict the structure(s) of an RNA using mutation rates from the
     individual clusters or the ensemble average ('mask' step). """
     return run(*args, **kwargs)
 
 
 @lock_temp_dir
 @docdef.auto()
-def run(table: tuple[str, ...],
+def run(input_file: tuple[str, ...],
         *,
         fasta: str,
-        library: str | None,
+        sections_file: str | None,
         coords: tuple[tuple[str, int, int], ...],
         primers: tuple[tuple[str, str, str], ...],
         primer_gap: int,
-        dms_quantile: float,
+        quantile: float,
         temp_dir: str,
         save_temp: bool,
         max_procs: int,
         parallel: bool,
         rerun: bool):
     """
     Run the structure module.
@@ -66,43 +66,43 @@
 
     if not fasta:
         logger.critical(f"No FASTA file given to {path.MOD_STRUCT}")
         return list()
 
     # Get the sections for every reference sequence.
     ref_sections = RefSections(parse_fasta(Path(fasta)),
-                               library=Path(library) if library else None,
+                               sects_file=(Path(sections_file) if sections_file
+                                           else None),
                                coords=coords,
                                primers=encode_primers(primers),
                                primer_gap=primer_gap)
     # Initialize the table loaders.
-    files = path.find_files_chain(map(Path, table), [path.MutTabSeg])
+    tab_files = path.find_files_chain(map(Path, input_file), [path.MutTabSeg])
     loaders = [loader for loader in dispatch(load, max_procs, parallel,
-                                             args=as_list_of_tuples(files),
+                                             args=as_list_of_tuples(tab_files),
                                              pass_n_procs=False)
-               if isinstance(loader, (MaskPosTableLoader,
-                                      ClustPosTableLoader))]
+               if isinstance(loader, (MaskPosTableLoader, ClustPosTableLoader))]
     # Fold the RNA profiles.
     return dispatch(fold_rna, max_procs, parallel,
                     args=[(loader, ref_sections.list(loader.ref))
                           for loader in loaders],
                     kwargs=dict(temp_dir=Path(temp_dir), save_temp=save_temp,
-                                dms_quantile=dms_quantile, rerun=rerun),
+                                quantile=quantile, rerun=rerun),
                     pass_n_procs=True)
 
 
 def fold_rna(loader: MaskPosTableLoader | ClustPosTableLoader,
              sections: list[Section], n_procs: int, **kwargs):
     """ Fold an RNA molecule from one table of reactivities. """
     return dispatch(fold_profile, n_procs, parallel=True,
                     args=[(profile,)
                           for profile in loader.iter_profiles(sections)],
                     kwargs=dict(out_dir=loader.out_dir, **kwargs),
                     pass_n_procs=False)
 
 
-def fold_profile(rna: RnaProfile, out_dir: Path, dms_quantile: float, **kwargs):
+def fold_profile(rna: RnaProfile, out_dir: Path, quantile: float, **kwargs):
     """ Fold a section of an RNA from one mutational profile. """
-    ct_file = fold(rna, out_dir=out_dir, dms_quantile=dms_quantile, **kwargs)
+    ct_file = fold(rna, out_dir=out_dir, quantile=quantile, **kwargs)
     dot_file = ct2dot(ct_file)
-    varnac_file = rna.to_varnac(out_dir, dms_quantile)
+    varnac_file = rna.to_varnac(out_dir, quantile)
     return ct_file, dot_file, varnac_file
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/struct/rnastructure.py` & `seismic-rna-0.2.0/src/seismicrna/struct/rnastructure.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from ..core.shell import run_cmd, RNASTRUCTURE_FOLD_CMD
 
 logger = getLogger(__name__)
 
 
 def fold(rna: RnaProfile, *,
          out_dir: Path, temp_dir: Path, save_temp: bool,
-         dms_quantile: float,
+         quantile: float,
          rerun: bool):
     """ Run the 'Fold' program of RNAstructure. """
     ct_file = rna.ct_file(out_dir)
     if rerun or not ct_file.is_file():
         cmd = [RNASTRUCTURE_FOLD_CMD]
-        if dms_quantile > 0.:
+        if quantile > 0.:
             # Write the DMS reactivities file for the RNA.
-            cmd.extend(["--DMS", rna.to_dms(temp_dir, dms_quantile)])
+            cmd.extend(["--DMS", rna.to_dms(temp_dir, quantile)])
         # Write a temporary FASTA file for the RNA.
         cmd.append(fasta := rna.to_fasta(temp_dir))
         try:
             # Get the path of the output CT file.
             cmd.append(ct_file)
             # Run the command.
             run_cmd(cmd, check_is_after=[ct_file])
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/table/tabulate.py` & `seismic-rna-0.2.0/src/seismicrna/table/tabulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from abc import ABC, abstractmethod
 from functools import cache, cached_property
 from logging import getLogger
 
 import numpy as np
 import pandas as pd
 
-from .base import (TOTAL_REL, DELET_REL, INSRT_REL, MATCH_REL, MUTAT_REL,
+from .base import (COVER_REL, DELET_REL, INSRT_REL, MATCH_REL, MUTAT_REL,
                    SUBST_REL, SUB_A_REL, SUB_C_REL, SUB_G_REL, SUB_T_REL,
                    CLUST_INDEX_NAMES, REL_NAME, R_ADJ_TITLE, R_OBS_TITLE,
-                   REL_CODES)
-from ..cluster.names import READ_NAME
+                   READ_TITLE, REL_CODES, TABLE_COLUMNS)
 from ..cluster.load import ClustLoader
 from ..core.bitcall import BitCaller, SemiBitCaller
 from ..core.bitvect import BitCounter, ClustBitCounter
 from ..core.mu import calc_f_obs_df, calc_mu_adj_df
-from ..core.sect import Section
+from ..core.sect import Section, INDEX_NAMES
 from ..mask.load import MaskLoader
 from ..relate.load import RelateLoader
 
 logger = getLogger(__name__)
 
+# These relationships must be computed, else adjust_counts() will fail.
+REQUIRED_RELS = MATCH_REL, MUTAT_REL
+
 
 # Tabulator Classes ####################################################
 
 class Tabulator(ABC):
     """ Base class for tabulating data for multiple tables from a report
     loader. """
 
     def __init__(self, loader: RelateLoader | MaskLoader | ClustLoader,
                  rel_codes: str):
         self._loader = loader
+        # The table must contain COVER, MATCH, and MUTAT.
         self._rel_codes = rel_codes
 
     @property
     def out_dir(self):
         """ Output directory. """
         return self._loader.out_dir
 
@@ -57,19 +60,14 @@
         """ Section covered by the table. """
         return self._loader.section
 
     def iter_bit_callers(self):
         """ Yield a BitCaller for each relationship in the table. """
         yield from iter_bit_callers(self.section, self._rel_codes)
 
-    @cached_property
-    def rels(self):
-        """ Relationships counted in the table. """
-        return [rel for rel, _, _ in self.iter_bit_callers()]
-
     @property
     def seq_array(self):
         """ Array of the bases of the section at unmasked positions. """
         return self._loader.seq.to_str_array()
 
     @property
     @abstractmethod
@@ -82,159 +80,175 @@
         """ Return BitCounters for the batches of relation vectors. """
 
     @classmethod
     @abstractmethod
     def get_null_value(cls) -> int | float:
         """ The null value for a count: either 0 or NaN. """
 
+    @abstractmethod
     def tabulate_by_pos(self):
-        return pd.DataFrame.from_dict({rel: counter.n_affi_per_pos
+        """ Count the bits per position. """
+
+    @abstractmethod
+    def tabulate_by_read(self):
+        """ Count the bits per read. """
+
+
+class AvgTabulator(Tabulator, ABC):
+
+    @property
+    def columns(self):
+        return pd.Index(TABLE_COLUMNS, name=REL_NAME)
+
+    def tabulate_by_pos(self):
+        # Assemble the DataFrame from the bit counts.
+        data = pd.DataFrame.from_dict({rel: counter.n_affi_per_pos
                                        for rel, counter
                                        in self.bit_counts.items()})
+        # Rename the index of the positions and bases.
+        data.index.rename(INDEX_NAMES, inplace=True)
+        # Include all columns of relationships, even those not counted.
+        return data.reindex(columns=self.columns)
 
     def tabulate_by_read(self):
-        return pd.DataFrame.from_dict({rel: counter.n_affi_per_read
+        """ Count the bits per read. """
+        data = pd.DataFrame.from_dict({rel: counter.n_affi_per_read
                                        for rel, counter
                                        in self.bit_counts.items()})
+        # Rename the index of the read names.
+        data.index.rename(READ_TITLE, inplace=True)
+        # Include all columns of relationships, even those not counted.
+        return data.reindex(columns=self.columns)
 
 
-class RelTabulator(Tabulator):
+class NullableTabulator(Tabulator, ABC):
 
     @classmethod
     def get_null_value(cls):
-        return 0
+        return np.nan
 
-    @property
-    def columns(self):
-        return pd.Index(self.rels, name=REL_NAME)
+
+class RelTabulator(AvgTabulator):
+
+    @classmethod
+    def get_null_value(cls):
+        return 0
 
     @cached_property
     def bit_counts(self):
         bit_counts = dict()
         for name, bit_caller, kwargs in self.iter_bit_callers():
             if kwargs:
                 bit_caller = BitCaller.inter(bit_caller, **kwargs)
             bit_counts[name] = BitCounter(
                 self.section,
                 bit_caller.iter(self._loader.iter_batches_processed())
             )
         return bit_counts
 
 
-class MaskTabulator(Tabulator):
-
-    @classmethod
-    def get_null_value(cls):
-        return np.nan
-
-    @property
-    def columns(self):
-        return pd.Index(self.rels, name=REL_NAME)
+class MaskTabulator(AvgTabulator, NullableTabulator):
 
     @cached_property
     def bit_counts(self):
         return {
             rel: BitCounter(self.section,
                             self._loader.iter_batches_processed(bit_caller=bc,
                                                                 **kwargs))
             for rel, bc, kwargs in self.iter_bit_callers()
         }
 
     def tabulate_by_pos(self):
         # Count every type of relationship at each position, in the same
-        # way as for the superclass.
-        counts_obs = super().tabulate_by_pos()
-        # Adjust the counts to correct for observer bias.
-        return adjust_counts(counts_obs,
+        # way as for the superclass, then adjust for observer bias.
+        return adjust_counts(super().tabulate_by_pos(),
                              self._loader.section,
                              self._loader.min_mut_gap)
 
 
-class ClustTabulator(Tabulator):
-
-    @classmethod
-    def get_null_value(cls):
-        return np.nan
+class ClusterTabulator(NullableTabulator):
 
     @property
-    def clusters(self):
+    def ord_clust(self):
         """ Order and number of each cluster. """
         return self._loader.clusters
 
     def get_read_names(self):
         return self._loader.import_loader.get_read_names()
 
     @cached_property
     def columns(self):
         return pd.MultiIndex.from_tuples([(order, cluster, rel)
-                                          for order, cluster in self.clusters
-                                          for rel in self.rels],
+                                          for order, cluster in self.ord_clust
+                                          for rel in TABLE_COLUMNS],
                                          names=CLUST_INDEX_NAMES)
 
     @cached_property
     def bit_counts(self):
         return dict(
             (rel, ClustBitCounter(
                 self.section,
-                self.clusters,
+                self.ord_clust,
                 self._loader.iter_batches_processed(bit_caller=bc, **kwargs)
             )) for rel, bc, kwargs in self.iter_bit_callers()
         )
 
     @cache
     def tabulate_by_pos(self):
         """ DataFrame of the bit count for each position and caller. """
-        # Initialize an empty DataFrame.
-        counts_obs = pd.DataFrame(self.get_null_value(),
+        # Initialize an empty DataFrame of adjusted counts.
+        counts_adj = pd.DataFrame(self.get_null_value(),
                                   index=self._loader.section.unmasked,
                                   columns=self.columns)
-        # Fill in the DataFrame column by column.
-        for col in self.columns:
-            nk, k, rel = col
-            counts_obs[col] = self.bit_counts[rel].n_affi_per_pos.loc[:, (nk, k)]
-        # Adjust the counts to correct for observer bias.
-        counts_adj = dict()
-        for order, k in self.clusters:
-            for rel, adj in adjust_counts(counts_obs.loc[:, (order, k)],
-                                          self._loader.section,
-                                          self._loader.min_mut_gap).items():
-                counts_adj[order, k, rel] = adj
-        counts_adj = pd.DataFrame.from_dict(counts_adj)
-        counts_adj.columns.rename(counts_obs.columns.names, inplace=True)
+        # Fill in the DataFrame one cluster at a time.
+        for order, k in self.ord_clust:
+            # Initialize a DataFrame of observed counts for the cluster.
+            counts_obs = pd.DataFrame(self.get_null_value(),
+                                      index=self._loader.section.unmasked,
+                                      columns=TABLE_COLUMNS)
+            # Fill in the observed counts column by column.
+            for rel in counts_obs.columns.to_list():
+                counts = self.bit_counts[rel].n_affi_per_pos.loc[:, (order, k)]
+                counts_obs.loc[:, rel] = counts
+            # Adjust the counts to correct for observer bias.
+            counts = adjust_counts(counts_obs,
+                                   self._loader.section,
+                                   self._loader.min_mut_gap)
+            counts_adj.loc[:, (order, k)] = counts.values
         return counts_adj
 
     def tabulate_by_read(self):
         """ DataFrame of the bit count for each read and caller. """
         # Initialize an empty DataFrame.
         counts = pd.DataFrame(self.get_null_value(),
                               index=pd.Index(self.get_read_names(),
-                                             name=READ_NAME),
+                                             name=READ_TITLE),
                               columns=self.columns)
         # Fill in the DataFrame column by column.
         for col in self.columns:
             # Split the column label into the clustering order, cluster
-            # number, and type of relationship.
+            # number (k), and type of relationship (rel).
             order, k, rel = col
+            ok = order, k
             # Get the bit counter for the relationship and select the
             # column for the clustering order and cluster number.
-            counts[col] = self.bit_counts[rel].n_affi_per_read.loc[:, (order, k)]
+            counts.loc[:, col] = self.bit_counts[rel].n_affi_per_read.loc[:, ok]
         return counts
 
     def tabulate_by_clust(self):
         """ Return the adjusted number of reads in each cluster as a
         Series with dimension (clusters). """
         return pd.DataFrame.from_dict({
             R_OBS_TITLE: self._loader.n_reads_obs,
             R_ADJ_TITLE: self._loader.n_reads_adj,
         })
 
 
 # Helper functions #####################################################
 
-
 def iter_mut_semi_callers():
     """ Yield a SemiBitCaller for each type of mutation to tabulate. """
     yield SUBST_REL, SemiBitCaller.from_counts(count_sub=True)
     yield SUB_A_REL, SemiBitCaller("ca", "ga", "ta")
     yield SUB_C_REL, SemiBitCaller("ac", "gc", "tc")
     yield SUB_G_REL, SemiBitCaller("ag", "cg", "tg")
     yield SUB_T_REL, SemiBitCaller("at", "ct", "gt")
@@ -249,33 +263,35 @@
     # Call mutations.
     mutc = SemiBitCaller.from_counts(count_sub=True,
                                      count_del=True,
                                      count_ins=True)
     # Create a standard bit caller for all matches and mutations.
     bitc = BitCaller(section, mutc, refc)
     # Count all base calls (everything but the bytes 0 and 255).
-    yield TOTAL_REL, bitc, dict(merge=True)
+    yield COVER_REL, bitc, dict(merge=True)
     # Count matches to the reference sequence.
     yield MATCH_REL, bitc, dict(invert=True)
     # Count all types of mutations, relative to reference matches.
     yield MUTAT_REL, bitc, dict()
     # Count each type of mutation, relative to reference matches.
     for mut, mutc in iter_mut_semi_callers():
         yield mut, BitCaller(section, mutc, refc), dict()
 
 
 def iter_bit_callers(section: Section, rel_codes: str):
     """ Yield a BitCaller for each type of relationship to tabulate. """
     # Determine which types of relationships to call.
     if rel_codes:
-        # Use only the selected types of relationships.
+        # Use the selected relationships and two required relationships:
+        # MATCH and MUTAT.
         call_rels = {REL_CODES[code] for code in rel_codes}
+        call_rels.update(REQUIRED_RELS)
     else:
         # Use all types of relationships.
-        call_rels = set(REL_CODES.values())
+        call_rels = set(TABLE_COLUMNS)
     # Yield a BitCaller for each selected type of relationship.
     for rel, bit_caller, kwargs in _iter_bit_callers(section):
         if rel in call_rels:
             yield rel, bit_caller, kwargs
 
 
 def adjust_counts(counts_obs: pd.DataFrame,
@@ -292,83 +308,93 @@
         position (index) in the section of interest.
     section: Section
         The section of interest.
     min_mut_gap: int
         Minimum number of non-mutated bases permitted between mutations.
     """
     logger.debug(f"Adjusting mutation counts of table\n{counts_obs}")
+    # Initialize an empty DataFrame of the adjusted counts with the same
+    # index and columns as the observed counts.
+    counts_adj = pd.DataFrame(np.nan,
+                              index=counts_obs.index,
+                              columns=counts_obs.columns)
     # Compute the observed fraction of mutations at each position.
     nrefs_obs = counts_obs.loc[:, MATCH_REL]
     nmuts_obs = counts_obs.loc[:, MUTAT_REL]
     ninfo_obs = nrefs_obs + nmuts_obs
     with np.errstate(divide="ignore"):
         # Ignore division by zero, which is acceptable here because any
         # NaN values will be zeroed out subsequently.
         fmuts_obs = nmuts_obs / ninfo_obs
     # Fill missing NaN values with zero.
     fmuts_obs.fillna(0., inplace=True)
     # Adjust the fraction of mutations to correct the observer bias.
-    mu_adj = calc_mu_adj_df(fmuts_obs.to_frame(),
-                            section, min_mut_gap).squeeze(axis=1)
+    fmuts_adj = calc_mu_adj_df(fmuts_obs.to_frame(), section,
+                               min_mut_gap).squeeze()
     # Compute the fraction of reads that would be observed.
-    f_obs = float(calc_f_obs_df(mu_adj.to_frame(), section, min_mut_gap)[0])
-    # Initialize new data for the adjusted counts.
-    counts_adj = dict()
+    f_obs = float(calc_f_obs_df(fmuts_adj.to_frame(), section,
+                                min_mut_gap)[0])
     # Assume that the total number of base calls including unobserved
     # reads is the number observed divided by the fraction of the total
     # reads that were observed.
-    counts_adj[TOTAL_REL] = counts_obs.loc[:, TOTAL_REL] / f_obs
+    counts_adj.loc[:, COVER_REL] = counts_obs.loc[:, COVER_REL] / f_obs
     # Two conditions must be met:
     # : The number of informative bases (matches + mutations) after
     #   adjustment must equal the number before adjustment divided
     #   by the fraction of reads that were observed:
     #   (nrefs_adj + nmuts_adj) = (nrefs_obs + nmuts_obs) / f_obs
     # : The fraction of mutations at each position after adjustment
     #   must equal the adjusted number of mutations divided by the
     #   adjusted number of informative bases:
-    #   nmuts_adj / (nrefs_adj + nmuts_adj) = mu_adj
+    #   nmuts_adj / (nrefs_adj + nmuts_adj) = fmuts_adj
     # The two unknown variables (nrefs_adj and nmuts_adj) can be
     # solved using the above system of two equations. By solving for
     # (nrefs_adj + nmuts_adj) in both equations, we get:
     # : (nrefs_adj + nmuts_adj) = (nrefs_obs + nmuts_obs) / f_obs
-    # : (nrefs_adj + nmuts_adj) = nmuts_adj / mu_adj, if mu_adj > 0
+    # : (nrefs_adj + nmuts_adj) = nmuts_adj / fmuts_adj {fmuts_adj > 0}
     # Setting both right hand sides equal, nmuts_adj is solved:
-    # : (nrefs_obs + nmuts_obs) / f_obs = nmuts_adj / mu_adj
-    # : nmuts_adj = (nrefs_obs + nmuts_obs) * (mu_adj / f_obs)
-    nmuts_adj = ninfo_obs * (mu_adj / f_obs)
+    # : (nrefs_obs + nmuts_obs) / f_obs = nmuts_adj / fmuts_adj
+    # : nmuts_adj = (nrefs_obs + nmuts_obs) * (fmuts_adj / f_obs)
+    nmuts_adj = ninfo_obs * (fmuts_adj / f_obs)
     # Then, plugging this solution into the second equation:
-    # : nrefs_adj = nmuts_adj / mu_adj - nmuts_adj
-    #             = nmuts_adj * (1 / mu_adj - 1), if mu_adj > 0
-    # If, on the other hand, mu_adj = 0, then
-    # : nmuts_adj = mu_adj * (nrefs_adj + nmuts_adj) = 0
+    # : nrefs_adj = nmuts_adj / fmuts_adj - nmuts_adj
+    #             = nmuts_adj * (1 / fmuts_adj - 1) {fmuts_adj > 0}
+    # If, on the other hand, fmuts_adj = 0, then
+    # : nmuts_adj = fmuts_adj * (nrefs_adj + nmuts_adj) = 0
     # Thus, we solve for nrefs_adj using the first equation instead:
     # : (nrefs_adj + nmuts_adj) = (nrefs_obs + nmuts_obs) / f_obs
     # : nrefs_adj = nrefs_obs / f_obs
     with np.errstate(divide="ignore"):
         # Ignore division-by-zero warnings in np.reciprocal because
-        # positions where mu_adj = 0 are just skipped by np.where.
-        nrefs_adj = np.where(mu_adj > 0.,
-                             nmuts_adj * (np.reciprocal(mu_adj) - 1.),
+        # positions where fmuts_adj = 0 are just skipped by np.where.
+        nrefs_adj = np.where(fmuts_adj > 0.,
+                             nmuts_adj * (np.reciprocal(fmuts_adj) - 1.),
                              nrefs_obs / f_obs)
-    counts_adj[MATCH_REL] = nrefs_adj
-    counts_adj[MUTAT_REL] = nmuts_adj
-    # Compute the factor by which nmuts was adjusted:
-    nmuts_fac = nmuts_adj / nmuts_obs
+        # Compute the factor by which nmuts was adjusted. Division by 0
+        # is possible if no mutations were observed, resulting in NaN
+        # values. Fill them with 1 so that the NaNs do not propagate
+        # when multiplying the number of mutations by nmuts_fac.
+        nmuts_fac = (nmuts_adj / nmuts_obs).fillna(1.)
+    counts_adj.loc[:, MATCH_REL] = nrefs_adj
+    counts_adj.loc[:, MUTAT_REL] = nmuts_adj
     # Adjust every type of mutation by this factor.
     for mut in (SUBST_REL, SUB_A_REL, SUB_C_REL, SUB_G_REL, SUB_T_REL,
                 DELET_REL, INSRT_REL):
-        counts_adj[mut] = counts_obs.loc[:, mut] * nmuts_fac
-    # Assemble the adjusted counts into a new DataFrame.
-    return pd.DataFrame.from_dict(counts_adj)
+        try:
+            counts_adj.loc[:, mut] = counts_obs.loc[:, mut] * nmuts_fac
+        except KeyError:
+            # The mutation was not in the table.
+            pass
+    return counts_adj
 
 
 def tabulate_loader(report_loader: RelateLoader | MaskLoader | ClustLoader,
                     rel_codes: str):
     """ Return a new DataLoader, choosing the subclass based on the type
     of the argument `report_loader`. """
     if isinstance(report_loader, RelateLoader):
         return RelTabulator(report_loader, rel_codes)
     if isinstance(report_loader, MaskLoader):
         return MaskTabulator(report_loader, rel_codes)
     if isinstance(report_loader, ClustLoader):
-        return ClustTabulator(report_loader, rel_codes)
+        return ClusterTabulator(report_loader, rel_codes)
     raise TypeError(f"Invalid loader type: {type(report_loader).__name__}")
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/table/write.py` & `seismic-rna-0.2.0/src/seismicrna/table/write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import ABC, abstractmethod
 from logging import getLogger
 from pathlib import Path
 
 import pandas as pd
 
-from .base import (READ_TITLE, Table, PosTable, ReadTable,
+from .base import (Table, PosTable, ReadTable,
                    RelPosTable, RelReadTable, MaskPosTable, MaskReadTable,
                    ClustPosTable, ClustReadTable, ClustFreqTable)
-from .tabulate import (Tabulator, RelTabulator, MaskTabulator, ClustTabulator,
+from .tabulate import (Tabulator, RelTabulator, MaskTabulator, ClusterTabulator,
                        tabulate_loader)
 from ..cluster.load import ClustLoader
 from ..core import path
 from ..mask.load import MaskLoader
 from ..relate.load import RelateLoader
 
 logger = getLogger(__name__)
@@ -20,15 +20,15 @@
 
 
 # Table Writer Base Classes ############################################
 
 class TableWriter(Table, ABC):
     """ Write a table to a file. """
 
-    def __init__(self, tabulator: Tabulator | ClustTabulator):
+    def __init__(self, tabulator: Tabulator | ClusterTabulator):
         self._tab = tabulator
 
     @property
     def out_dir(self):
         return self._tab.out_dir
 
     @property
@@ -71,19 +71,15 @@
         all_positions = self._tab.section.range
         return self._tab.tabulate_by_pos().reindex(index=all_positions)
 
 
 class ReadTableWriter(TableWriter, ReadTable, ABC):
 
     def load_data(self):
-        # Load the data for each read.
-        data = self._tab.tabulate_by_read()
-        # Rename the index.
-        data.index.rename(READ_TITLE, inplace=True)
-        return data
+        return self._tab.tabulate_by_read()
 
 
 # Instantiable Table Writers ###########################################
 
 class RelPosTableWriter(PosTableWriter, RelPosTable):
     pass
 
@@ -138,28 +134,28 @@
 
 
 def get_tabulator_writer_types(tabulator: Tabulator):
     if isinstance(tabulator, RelTabulator):
         return RelPosTableWriter, RelReadTableWriter
     if isinstance(tabulator, MaskTabulator):
         return MaskPosTableWriter, MaskReadTableWriter
-    if isinstance(tabulator, ClustTabulator):
+    if isinstance(tabulator, ClusterTabulator):
         return ClustPosTableWriter, ClustReadTableWriter, ClustFreqTableWriter
     raise TypeError(f"Invalid tabulator type: {type(tabulator).__name__}")
 
 
 def get_tabulator_writers(tabulator: Tabulator):
     for writer_type in get_tabulator_writer_types(tabulator):
         yield writer_type(tabulator)
 
 
-def write(report_file: Path, table_cols: str, rerun: bool):
+def write(report_file: Path, rels: str, rerun: bool):
     """ Helper function to write a table from a report file. """
     # Determine the needed type of report loader.
     report_loader_type = infer_report_loader_type(report_file)
     # Load the report.
     report_loader = report_loader_type.open(report_file)
     # Create the tabulator for the report's data.
-    tabulator = tabulate_loader(report_loader, table_cols)
+    tabulator = tabulate_loader(report_loader, rels)
     # For each table associated with this tabulator, create the table,
     # write it, and return the path to the table output file.
     return [table.write(rerun) for table in get_tabulator_writers(tabulator)]
```

### Comparing `seismic-rna-0.1.3/src/seismicrna/test/main.py` & `seismic-rna-0.2.0/src/seismicrna/test/main.py`

 * *Files identical despite different names*

