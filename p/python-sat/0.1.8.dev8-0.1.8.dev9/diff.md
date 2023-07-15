# Comparing `tmp/python-sat-0.1.8.dev8.tar.gz` & `tmp/python-sat-0.1.8.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-0.1.8.dev8.tar", last modified: Wed Jul 12 00:36:48 2023, max compression
+gzip compressed data, was "python-sat-0.1.8.dev9.tar", last modified: Sat Jul 15 01:37:35 2023, max compression
```

## Comparing `python-sat-0.1.8.dev8.tar` & `python-sat-0.1.8.dev9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.163040 python-sat-0.1.8.dev8/
--rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-07-12 00:36:48.163135 python-sat-0.1.8.dev8/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567    14204 2023-07-12 00:06:38.000000 python-sat-0.1.8.dev8/README.rst
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.131056 python-sat-0.1.8.dev8/allies/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev8/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev8/allies/approxmc.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.133831 python-sat-0.1.8.dev8/cardenc/
--rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev8/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.137786 python-sat-0.1.8.dev8/examples/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev8/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-0.1.8.dev8/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev8/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev8/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-0.1.8.dev8/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    67270 2023-06-09 06:00:18.000000 python-sat-0.1.8.dev8/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.141240 python-sat-0.1.8.dev8/pysat/
--rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-07-12 00:28:24.000000 python-sat-0.1.8.dev8/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev8/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev8/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) 907548567   185523 2023-07-12 00:05:58.000000 python-sat-0.1.8.dev8/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.143056 python-sat-0.1.8.dev8/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567     1922 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/requirements.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-07-12 00:36:48.163496 python-sat-0.1.8.dev8/setup.cfg
--rw-r--r--   0 aign0002 (892519254) 907548567     6596 2023-07-11 23:32:23.000000 python-sat-0.1.8.dev8/setup.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.153193 python-sat-0.1.8.dev8/solvers/
--rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev8/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev8/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    88105 2023-07-11 23:37:13.000000 python-sat-0.1.8.dev8/solvers/glucose421.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.160068 python-sat-0.1.8.dev8/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev8/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev8/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    66579 2023-07-11 23:55:20.000000 python-sat-0.1.8.dev8/solvers/patches/glucose421.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev8/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev8/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev8/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    25883 2023-07-11 23:55:38.000000 python-sat-0.1.8.dev8/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) 907548567   240042 2023-07-11 23:31:01.000000 python-sat-0.1.8.dev8/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.162679 python-sat-0.1.8.dev8/tests/
--rw-r--r--   0 aign0002 (892519254) 907548567      987 2023-07-12 00:04:49.000000 python-sat-0.1.8.dev8/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) 907548567     2432 2023-07-12 00:04:57.000000 python-sat-0.1.8.dev8/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev8/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) 907548567      890 2023-07-12 00:05:05.000000 python-sat-0.1.8.dev8/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      650 2023-07-12 00:05:10.000000 python-sat-0.1.8.dev8/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.626553 python-sat-0.1.8.dev9/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-07-15 01:37:35.626638 python-sat-0.1.8.dev9/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567    14204 2023-07-12 00:06:38.000000 python-sat-0.1.8.dev9/README.rst
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.602739 python-sat-0.1.8.dev9/allies/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev9/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev9/allies/approxmc.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.605612 python-sat-0.1.8.dev9/cardenc/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev9/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.607714 python-sat-0.1.8.dev9/examples/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev9/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-0.1.8.dev9/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev9/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev9/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-0.1.8.dev9/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    67270 2023-06-09 06:00:18.000000 python-sat-0.1.8.dev9/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.609603 python-sat-0.1.8.dev9/pysat/
+-rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-07-15 01:30:26.000000 python-sat-0.1.8.dev9/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev9/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev9/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   185523 2023-07-12 00:05:58.000000 python-sat-0.1.8.dev9/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.610632 python-sat-0.1.8.dev9/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-07-15 01:37:35.000000 python-sat-0.1.8.dev9/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567     1922 2023-07-15 01:37:35.000000 python-sat-0.1.8.dev9/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-07-15 01:37:35.000000 python-sat-0.1.8.dev9/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-07-15 01:37:35.000000 python-sat-0.1.8.dev9/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-07-15 01:37:35.000000 python-sat-0.1.8.dev9/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-07-15 01:37:35.626922 python-sat-0.1.8.dev9/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) 907548567     6596 2023-07-11 23:32:23.000000 python-sat-0.1.8.dev9/setup.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.617696 python-sat-0.1.8.dev9/solvers/
+-rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev9/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev9/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    88105 2023-07-11 23:37:13.000000 python-sat-0.1.8.dev9/solvers/glucose421.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.623794 python-sat-0.1.8.dev9/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev9/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev9/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    68942 2023-07-15 01:30:10.000000 python-sat-0.1.8.dev9/solvers/patches/glucose421.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev9/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev9/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev9/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    25883 2023-07-11 23:55:38.000000 python-sat-0.1.8.dev9/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   240042 2023-07-11 23:31:01.000000 python-sat-0.1.8.dev9/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-15 01:37:35.626311 python-sat-0.1.8.dev9/tests/
+-rw-r--r--   0 aign0002 (892519254) 907548567      987 2023-07-12 00:04:49.000000 python-sat-0.1.8.dev9/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     2432 2023-07-12 00:04:57.000000 python-sat-0.1.8.dev9/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev9/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      890 2023-07-12 00:05:05.000000 python-sat-0.1.8.dev9/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev9/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      650 2023-07-12 00:05:10.000000 python-sat-0.1.8.dev9/tests/test_warmstart.py
```

### Comparing `python-sat-0.1.8.dev8/LICENSE.txt` & `python-sat-0.1.8.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/PKG-INFO` & `python-sat-0.1.8.dev9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev8
+Version: 0.1.8.dev9
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev8/README.rst` & `python-sat-0.1.8.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/allies/approxmc.py` & `python-sat-0.1.8.dev9/allies/approxmc.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/bitwise.hh` & `python-sat-0.1.8.dev9/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/card.hh` & `python-sat-0.1.8.dev9/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/clset.hh` & `python-sat-0.1.8.dev9/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/common.hh` & `python-sat-0.1.8.dev9/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/itot.hh` & `python-sat-0.1.8.dev9/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/ladder.hh` & `python-sat-0.1.8.dev9/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/mto.hh` & `python-sat-0.1.8.dev9/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/pairwise.hh` & `python-sat-0.1.8.dev9/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/ptypes.hh` & `python-sat-0.1.8.dev9/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/pycard.cc` & `python-sat-0.1.8.dev9/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/seqcounter.hh` & `python-sat-0.1.8.dev9/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/sortcard.hh` & `python-sat-0.1.8.dev9/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/cardenc/utils.hh` & `python-sat-0.1.8.dev9/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/fm.py` & `python-sat-0.1.8.dev9/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/genhard.py` & `python-sat-0.1.8.dev9/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/hitman.py` & `python-sat-0.1.8.dev9/examples/hitman.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/lbx.py` & `python-sat-0.1.8.dev9/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/lsu.py` & `python-sat-0.1.8.dev9/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/mcsls.py` & `python-sat-0.1.8.dev9/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/models.py` & `python-sat-0.1.8.dev9/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/musx.py` & `python-sat-0.1.8.dev9/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/optux.py` & `python-sat-0.1.8.dev9/examples/optux.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/rc2.py` & `python-sat-0.1.8.dev9/examples/rc2.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/examples/usage.py` & `python-sat-0.1.8.dev9/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/pysat/__init__.py` & `python-sat-0.1.8.dev9/pysat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##  Created on: Mar 4, 2017
 ##      Author: Alexey S. Ignatiev
 ##      E-mail: aignatiev@ciencias.ulisboa.pt
 ##
 
 # current version
 #==============================================================================
-VERSION = (0, 1, 8, "dev", 8)
+VERSION = (0, 1, 8, "dev", 9)
 
 
 # PEP440 Format
 #==============================================================================
 __version__ = "%d.%d.%d.%s%d" % VERSION if len(VERSION) == 5 else \
               "%d.%d.%d" % VERSION
```

### Comparing `python-sat-0.1.8.dev8/pysat/_fileio.py` & `python-sat-0.1.8.dev9/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/pysat/_utils.py` & `python-sat-0.1.8.dev9/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/pysat/card.py` & `python-sat-0.1.8.dev9/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/pysat/formula.py` & `python-sat-0.1.8.dev9/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/pysat/pb.py` & `python-sat-0.1.8.dev9/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/pysat/process.py` & `python-sat-0.1.8.dev9/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/pysat/solvers.py` & `python-sat-0.1.8.dev9/pysat/solvers.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/python_sat.egg-info/PKG-INFO` & `python-sat-0.1.8.dev9/python_sat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev8
+Version: 0.1.8.dev9
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev8/python_sat.egg-info/SOURCES.txt` & `python-sat-0.1.8.dev9/python_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/setup.py` & `python-sat-0.1.8.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/cadical103.tar.gz` & `python-sat-0.1.8.dev9/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/cadical153.tar.gz` & `python-sat-0.1.8.dev9/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/glucose30.tar.gz` & `python-sat-0.1.8.dev9/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/glucose41.tar.gz` & `python-sat-0.1.8.dev9/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/glucose421.tar.gz` & `python-sat-0.1.8.dev9/solvers/glucose421.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/lingeling.tar.gz` & `python-sat-0.1.8.dev9/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/maplechrono.zip` & `python-sat-0.1.8.dev9/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/maplecm.zip` & `python-sat-0.1.8.dev9/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/maplesat.zip` & `python-sat-0.1.8.dev9/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/mergesat3.tar.gz` & `python-sat-0.1.8.dev9/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/minicard.tar.gz` & `python-sat-0.1.8.dev9/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/minisat22.tar.gz` & `python-sat-0.1.8.dev9/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/minisatgh.zip` & `python-sat-0.1.8.dev9/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/cadical103.patch` & `python-sat-0.1.8.dev9/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/cadical153.patch` & `python-sat-0.1.8.dev9/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/glucose30.patch` & `python-sat-0.1.8.dev9/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/glucose41.patch` & `python-sat-0.1.8.dev9/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/glucose421.patch` & `python-sat-0.1.8.dev9/solvers/patches/glucose421.patch`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,10 @@
-diff -Naur solvers/glucose421/Makefile solvers/g421/Makefile
---- solvers/glucose421/Makefile	1970-01-01 10:00:00
-+++ solvers/g421/Makefile	2023-07-12 09:52:06
-@@ -0,0 +1,37 @@
-+### Makefile ---
-+
-+## Author: aign
-+## Keywords:
-+
-+# main parameters
-+CXX      := c++
-+CXXFLAGS := -std=c++11 -fPIC -Wall -Wno-deprecated -fno-strict-aliasing -Wno-parentheses -DINCREMENTAL
-+CXXOPT   := -O3 -DNDEBUG
-+CXXDEBUG := -O0 -g3
-+CXXPROF  := -O3 -g3 -fno-inline -fno-omit-frame-pointer -pg -DNDEBUG
-+INCLUDES := -I..
-+LIBS     := -L.
-+SOURCES  := core/lcm.cc core/Solver.cc utils/Options.cc utils/System.cc
-+OBJECTS  := $(SOURCES:.cc=.o)
-+TRGT     :=  glucose421
-+
-+# gather compiler options
-+CXXARGS := $(CXXFLAGS) $(INCLUDES) $(CXXOPT)
-+
-+# targets
-+.PHONY: all clean lib
-+
-+all: lib
-+
-+lib: $(OBJECTS)
-+	@-ar cr lib$(TRGT).a $(OBJECTS)
-+
-+%.o: %.cc
-+	$(CXX) $(CXXARGS) -c $< -o $@
-+
-+clean:
-+	@-rm $(OBJECTS)
-+
-+allclean:
-+	@-find . -name '*.o' -delete
-+	@-find . -name '*.a' -delete
-diff -Naur solvers/glucose421/core/BoundedQueue.h solvers/g421/core/BoundedQueue.h
---- solvers/glucose421/core/BoundedQueue.h	2023-05-09 23:19:52
-+++ solvers/g421/core/BoundedQueue.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/core/BoundedQueue.h solvers/glucose421/core/BoundedQueue.h
+--- build/solvers/glucose421/core/BoundedQueue.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/core/BoundedQueue.h	2023-07-14 09:25:04.459944737 +0200
 @@ -48,14 +48,14 @@
   **************************************************************************************************/
  
  
 -#ifndef BoundedQueue_h
 -#define BoundedQueue_h
 +#ifndef Glucose421_BoundedQueue_h
@@ -57,17 +16,223 @@
  //=================================================================================================
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  template <class T>
  class bqueue {
-diff -Naur solvers/glucose421/core/Solver.cc solvers/g421/core/Solver.cc
---- solvers/glucose421/core/Solver.cc	2023-05-09 23:19:52
-+++ solvers/g421/core/Solver.cc	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/core/lcm.cc solvers/glucose421/core/lcm.cc
+--- build/solvers/glucose421/core/lcm.cc	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/core/lcm.cc	2023-07-14 09:25:04.459944737 +0200
+@@ -1,6 +1,7 @@
+-#include "Solver.h"
+-#include "mtl/Sort.h"
+-using namespace Glucose;
++#include "glucose421/core/Solver.h"
++#include "glucose421/mtl/Sort.h"
++
++using namespace Glucose421;
+ 
+ 
+ 
+@@ -25,18 +26,18 @@
+ 
+             Lit imp = wbin[k].blocker;
+ 
+-            if (value(imp) == l_False){
++            if (value(imp) == g421l_False){
+                 return wbin[k].cref;
+             }
+ 
+-            if (value(imp) == l_Undef){
++            if (value(imp) == g421l_Undef){
+                 simpleUncheckEnqueue(imp, wbin[k].cref);
+             }
+         }
+         for (i = j = (Watcher*)ws, end = i + ws.size(); i != end;){
+             // Try to avoid inspecting the clause:
+             Lit blocker = i->blocker;
+-            if (value(blocker) == l_True){
++            if (value(blocker) == g421l_True){
+                 *j++ = *i++; continue;
+             }
+ 
+@@ -54,7 +55,7 @@
+             // why not simply do i->blocker=first in this case?
+             Lit     first = c[0];
+             //  Watcher w     = Watcher(cr, first);
+-            if (first != blocker && value(first) == l_True){
++            if (first != blocker && value(first) == g421l_True){
+                 i->blocker = first;
+                 *j++ = *i++; continue;
+             }
+@@ -63,7 +64,7 @@
+             if (incremental){ // ----------------- INCREMENTAL MODE
+                 int choosenPos = -1;
+                 for (int k = 2; k < c.size(); k++){
+-                    if (value(c[k]) != l_False){
++                    if (value(c[k]) != g421l_False){
+                         if (decisionLevel()>assumptions.size()){
+                             choosenPos = k;
+                             break;
+@@ -71,7 +72,7 @@
+                         else{
+                             choosenPos = k;
+ 
+-                            if (value(c[k]) == l_True || !isSelector(var(c[k]))) {
++                            if (value(c[k]) == g421l_True || !isSelector(var(c[k]))) {
+                                 break;
+                             }
+                         }
+@@ -91,7 +92,7 @@
+             else{  // ----------------- DEFAULT  MODE (NOT INCREMENTAL)
+                 for (int k = 2; k < c.size(); k++){
+ 
+-                    if (value(c[k]) != l_False){
++                    if (value(c[k]) != g421l_False){
+                         // watcher i is abandonned using i++, because cr watches now ~c[k] instead of p
+                         // the blocker is first in the watcher. However,
+                         // the blocker in the corresponding watcher in ~first is not c[1]
+@@ -106,7 +107,7 @@
+             // Did not find watch -- clause is unit under assignment:
+             i->blocker = first;
+             *j++ = *i++;
+-            if (value(first) == l_False){
++            if (value(first) == g421l_False){
+                 confl = cr;
+                 qhead = trail.size();
+                 // Copy the remaining watches:
+@@ -138,7 +139,7 @@
+     for(i = j = (Watcher *) ws, end = i + ws.size(); i != end;) {
+         // Try to avoid inspecting the clause:
+         Lit blocker = i->blocker;
+-        if(value(blocker) == l_True) {
++        if(value(blocker) == g421l_True) {
+             *j++ = *i++;
+             continue;
+         }
+@@ -155,7 +156,7 @@
+         i++;
+         Watcher w = Watcher(cr, c[0]);
+         for(int k = 1; k < c.size(); k++) {
+-            if(value(c[k]) != l_False) {
++            if(value(c[k]) != g421l_False) {
+                 c[0] = c[k];
+                 c[k] = false_lit;
+                 unaryWatches[~c[0]].push(w);
+@@ -181,7 +182,7 @@
+ 
+ 
+ void Solver::simpleUncheckEnqueue(Lit p, CRef from){
+-    assert(value(p) == l_Undef);
++    assert(value(p) == g421l_Undef);
+     assigns[var(p)] = lbool(!sign(p)); // this makes a lbool object whose value is sign(p)
+     vardata[var(p)].reason = from;
+     trail.push_(p);
+@@ -192,7 +193,7 @@
+     for (int c = trail.size() - 1; c >= trailRecord; c--)
+     {
+         Var x = var(trail[c]);
+-        assigns[x] = l_Undef;
++        assigns[x] = g421l_Undef;
+ 
+     }
+     qhead = trailRecord;
+@@ -224,9 +225,9 @@
+             Clause& c = ca[confl];
+             // Special case for binary clauses
+             // The first one has to be SAT
+-            if (p != lit_Undef && c.size() == 2 && value(c[0]) == l_False) {
++            if (p != lit_Undef && c.size() == 2 && value(c[0]) == g421l_False) {
+ 
+-                assert(value(c[1]) == l_True);
++                assert(value(c[1]) == g421l_True);
+                 Lit tmp = c[0];
+                 c[0] = c[1], c[1] = tmp;
+             }
+@@ -274,8 +275,8 @@
+     CRef confl;
+ 
+     for (i = 0, j = 0; i < c.size(); i++){
+-        if (value(c[i]) == l_Undef){
+-            //printf("///@@@ uncheckedEnqueue:index = %d. l_Undef\n", i);
++        if (value(c[i]) == g421l_Undef){
++            //printf("///@@@ uncheckedEnqueue:index = %d. g421l_Undef\n", i);
+             simpleUncheckEnqueue(~c[i]);
+             c[j++] = c[i];
+             confl = simplePropagate();
+@@ -284,8 +285,8 @@
+             }
+         }
+         else{
+-            if (value(c[i]) == l_True){
+-                //printf("///@@@ uncheckedEnqueue:index = %d. l_True\n", i);
++            if (value(c[i]) == g421l_True){
++                //printf("///@@@ uncheckedEnqueue:index = %d. g421l_True\n", i);
+                 c[j++] = c[i];
+                 True_confl = true;
+                 confl = reason(var(c[i]));
+@@ -293,7 +294,7 @@
+             }
+             else{
+                 falseLit.push(c[i]);
+-                //printf("///@@@ uncheckedEnqueue:index = %d. l_False\n", i);
++                //printf("///@@@ uncheckedEnqueue:index = %d. g421l_False\n", i);
+             }
+         }
+     }
+@@ -350,11 +351,11 @@
+             if (!removed(cr)){
+                 sat = false_lit = false;
+                 for (int i = 0; i < c.size(); i++){
+-                    if (value(c[i]) == l_True){
++                    if (value(c[i]) == g421l_True){
+                         sat = true;
+                         break;
+                     }
+-                    else if (value(c[i]) == l_False){
++                    else if (value(c[i]) == g421l_False){
+                         false_lit = true;
+                     }
+                 }
+@@ -366,7 +367,7 @@
+ 
+                     if (false_lit){
+                         for (li = lj = 0; li < c.size(); li++){
+-                            if (value(c[li]) != l_False){
++                            if (value(c[li]) != g421l_False){
+                                 c[lj++] = c[li];
+                             }
+                         }
+@@ -444,11 +445,11 @@
+             if (!removed(cr)){
+                 sat = false_lit = false;
+                 for (int i = 0; i < c.size(); i++){
+-                    if (value(c[i]) == l_True){
++                    if (value(c[i]) == g421l_True){
+                         sat = true;
+                         break;
+                     }
+-                    else if (value(c[i]) == l_False){
++                    else if (value(c[i]) == g421l_False){
+                         false_lit = true;
+                     }
+                 }
+@@ -460,7 +461,7 @@
+ 
+                     if (false_lit){
+                         for (li = lj = 0; li < c.size(); li++){
+-                            if (value(c[li]) != l_False){
++                            if (value(c[li]) != g421l_False){
+                                 c[lj++] = c[li];
+                             }
+                         }
+diff -Naur build/solvers/glucose421/core/Solver.cc solvers/glucose421/core/Solver.cc
+--- build/solvers/glucose421/core/Solver.cc	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/core/Solver.cc	2023-07-14 09:31:03.200225963 +0200
 @@ -49,13 +49,12 @@
  
  #include <math.h>
  
 -#include "utils/System.h"
 -#include "mtl/Sort.h"
 -#include "core/Solver.h"
@@ -220,24 +385,24 @@
  
  void Solver::uncheckedEnqueue(Lit p, CRef from) {
 -    assert(value(p) == l_Undef);
 +    assert(value(p) == g421l_Undef);
      assigns[var(p)] = lbool(!sign(p));
      vardata[var(p)] = mkVarData(from, decisionLevel());
      trail.push_(p);
-@@ -962,7 +964,59 @@
+@@ -962,6 +964,58 @@
      return;
  }
  
 +//=================================================================================================
 +// Propagate and check (added for PySat):
 +bool Solver::prop_check(const vec<Lit>& assumps, vec<Lit>& prop, int psaving)
 +{
 +    prop.clear();
- 
++
 +    if (!ok)
 +        return false;
 +
 +    bool    st = true;
 +    int  level = decisionLevel();
 +    CRef confl = CRef_Undef;
 +
@@ -276,18 +441,17 @@
 +
 +    // restoring phase saving
 +    phase_saving = psaving_copy;
 +
 +    return st && confl == CRef_Undef;
 +}
 +
-+
+ 
  /*_________________________________________________________________________________________________
  |
- |  propagate : [void]  ->  [Clause*]
 @@ -993,11 +1047,11 @@
  
              Lit imp = wbin[k].blocker;
  
 -            if(value(imp) == l_False) {
 +            if(value(imp) == g421l_False) {
                  return wbin[k].cref;
@@ -550,17 +714,17 @@
 +    if(!ok) return g421l_False;
      double curTime = cpuTime();
  
      solves++;
  
 +    for (int i = 0; i < assumptions.size(); i++)
 +      assump[var(assumptions[i])] = true;
++
  
 -    lbool status = l_Undef;
-+
 +    lbool status = g421l_Undef;
      if(!incremental && verbosity >= 1) {
          printf("c ========================================[ MAGIC CONSTANTS ]==============================================\n");
          printf("c | Constants are supposed to work well together :-)                                                      |\n");
 @@ -1757,7 +1814,7 @@
  
      // Search:
@@ -575,88 +739,93 @@
  
      if(certifiedUNSAT) { // Want certified output
 -        if(status == l_False) {
 +        if(status == g421l_False) {
              if(vbyte) {
                  write_char('a');
                  write_lit(0);
-@@ -1782,23 +1839,23 @@
+@@ -1778,27 +1835,27 @@
+                 fprintf(certifiedOutput, "0\n");
+             }
+         }
+-        fclose(certifiedOutput);
++        //fclose(certifiedOutput);
      }
  
  
 -    if(status == l_True) {
 +    if(status == g421l_True) {
          // Extend & copy model:
          model.growTo(nVars());
          for(int i = 0; i < nVars(); i++) model[i] = value(i);
 -    } else if(status == l_False && conflict.size() == 0)
 +    } else if(status == g421l_False && conflict.size() == 0)
          ok = false;
  
+-
+-    cancelUntil(0);
+-
 +    //cancelUntil(0);
 +    if (!warm_start || status != g421l_True)  // no 'default' backtracking in case of warm restarts
 +        cancelUntil(0);
  
--    cancelUntil(0);
--
--
      double finalTime = cpuTime();
 -    if(status == l_True) {
 +    if(status == g421l_True) {
          nbSatCalls++;
          totalTime4Sat += (finalTime - curTime);
      }
 -    if(status == l_False) {
 +    if(status == g421l_False) {
          nbUnsatCalls++;
          totalTime4Unsat += (finalTime - curTime);
      }
-@@ -1808,11 +1865,198 @@
+@@ -1808,7 +1865,181 @@
  
  }
  
 +//=================================================================================================
 +// Add a clause in the warm start mode:
 +bool Solver::addClauseWarm(vec<Lit>& ps)
 +{
 +    if (!ok) return false;
 +    if (!warm_start || decisionLevel() == 0) return addClause(ps);
- 
++
 +    // checking if clause is satisfied and remove false/duplicate literals
 +    sort(ps);
 +    Lit p; int i, j, nws, max_i;
 +    vec<int> ws(2, -1);  // potentially watched literals
 +    for (i = j = nws = max_i = 0, p = lit_Undef; i < ps.size(); i++) {
 +        Var x = var(ps[i]);
 +        if ((value(ps[i]) == g421l_True && level(x) == 0) || ps[i] == ~p)
 +            return true;
 +        else if ((value(ps[i]) != g421l_False || level(x) > 0) && ps[i] != p) {
 +            if (value(ps[i]) != g421l_False && nws < 2)
 +                ws[nws++] = j;
 +            if (level(x) > level(var(ps[max_i])))
 +                max_i = j;
- 
++
 +            ps[j++] = p = ps[i];
 +        }
 +    }
 +    ps.shrink(i - j);
- 
++
 +    // analyzing which level to backtrack to (if any)
 +    if (ps.size() != 0) {
 +        if (ps.size() > 1) {
 +            if (nws) {
 +                p = ps[0]; ps[0] = ps[ws[0]]; ps[ws[0]] = p;
 +                if (nws == 2) {
 +                    p = ps[1]; ps[1] = ps[ws[1]]; ps[ws[1]] = p;
 +                }
 +            }
 +            else {
 +                // no satisfied literals in this clause
 +                p = ps[max_i]; ps[max_i] = ps[0]; ps[0] = p;
- 
++
 +                max_i = 1;
 +                for (int i = 2; i < ps.size(); ++i) {
 +                    if (level(var(ps[i])) > level(var(ps[max_i])))
 +                        max_i = i;
 +                }
 +
 +                p = ps[max_i]; ps[max_i] = ps[1]; ps[1] = p;
@@ -688,15 +857,15 @@
 +        cancelUntil(0);
 +        ok = false;
 +    }
 +
 +    return ok;
 +}
 +
- //=================================================================================================
++//=================================================================================================
 +// Resolve conflicts, if appear after adding a clause in the warm start mode:
 +bool Solver::resolveConflicts(CRef confl)
 +{
 +    int backtrack_level;
 +    vec <Lit> learnt_clause, selectors;
 +    unsigned int nblevels, szWithoutSelectors = 0;
 +    bool blocked = false;
@@ -735,40 +904,27 @@
 +            stats[nbstopsrestarts]++;
 +            if(!blocked) {
 +                stats[lastblockatrestart] = starts;
 +                stats[nbstopsrestartssame]++;
 +                blocked = true;
 +            }
 +        }
-+
+ 
 +        learnt_clause.clear();
 +        selectors.clear();
 +
 +        analyze(confl, learnt_clause, selectors, backtrack_level, nblevels, szWithoutSelectors);
 +
 +        lbdQueue.push(nblevels);
 +        sumLBD += nblevels;
 +
 +        cancelUntil(backtrack_level);
 +
-+        if(certifiedUNSAT) {
-+            if(vbyte) {
-+                write_char('a');
-+                for(int i = 0; i < learnt_clause.size(); i++)
-+                    write_lit(2 * (var(learnt_clause[i]) + 1) + sign(learnt_clause[i]));
-+                write_lit(0);
-+            }
-+            else {
-+                for(int i = 0; i < learnt_clause.size(); i++)
-+                    fprintf(certifiedOutput, "%i ", var(learnt_clause[i]) *
-+                                                    (-2 * sign(learnt_clause[i]) + 1));
-+                fprintf(certifiedOutput, "0\n");
-+            }
-+        }
-+
++        if(certifiedUNSAT)
++            addToDrat(learnt_clause, true);
 +
 +        if(learnt_clause.size() == 1) {
 +            uncheckedEnqueue(learnt_clause[0]);
 +            stats[nbUn]++;
 +            parallelExportUnaryClause(learnt_clause[0]);
 +        } else {
 +            CRef cr;
@@ -798,51 +954,47 @@
 +        claDecayActivity();
 +
 +        confl = propagate();
 +    }
 +
 +    return true;
 +}
-+
-+
-+
-+//=================================================================================================
- // Writing CNF to DIMACS:
- //
- // FIXME: this needs to be rewritten completely.
-@@ -1830,7 +2074,7 @@
+ 
+ 
+ 
+@@ -1830,7 +2061,7 @@
      if(satisfied(c)) return;
  
      for(int i = 0; i < c.size(); i++)
 -        if(value(c[i]) != l_False)
 +        if(value(c[i]) != g421l_False)
              fprintf(f, "%s%d ", sign(c[i]) ? "-" : "", mapVar(var(c[i]), map, max) + 1);
      fprintf(f, "0\n");
  }
-@@ -1866,7 +2110,7 @@
+@@ -1866,7 +2097,7 @@
          if(!satisfied(ca[clauses[i]])) {
              Clause &c = ca[clauses[i]];
              for(int j = 0; j < c.size(); j++)
 -                if(value(c[j]) != l_False)
 +                if(value(c[j]) != g421l_False)
                      mapVar(var(c[j]), map, max);
          }
  
-@@ -1876,7 +2120,7 @@
+@@ -1876,7 +2107,7 @@
      fprintf(f, "p cnf %d %d\n", max, cnt);
  
      for(int i = 0; i < assumptions.size(); i++) {
 -        assert(value(assumptions[i]) != l_False);
 +        assert(value(assumptions[i]) != g421l_False);
          fprintf(f, "%s%d 0\n", sign(assumptions[i]) ? "-" : "", mapVar(var(assumptions[i]), map, max) + 1);
      }
  
-diff -Naur solvers/glucose421/core/Solver.h solvers/g421/core/Solver.h
---- solvers/glucose421/core/Solver.h	2023-05-09 23:19:52
-+++ solvers/g421/core/Solver.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/core/Solver.h solvers/glucose421/core/Solver.h
+--- build/solvers/glucose421/core/Solver.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/core/Solver.h	2023-07-14 09:30:44.959603189 +0200
 @@ -47,20 +47,20 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
   **************************************************************************************************/
  
 -#ifndef Glucose_Solver_h
 -#define Glucose_Solver_h
 +#ifndef Glucose421_Solver_h
@@ -964,37 +1116,45 @@
 +inline bool     Solver::solve         (Lit p)               { budgetOff(); assumptions.clear(); assumptions.push(p); return solve_() == g421l_True; }
 +inline bool     Solver::solve         (Lit p, Lit q)        { budgetOff(); assumptions.clear(); assumptions.push(p); assumptions.push(q); return solve_() == g421l_True; }
 +inline bool     Solver::solve         (Lit p, Lit q, Lit r) { budgetOff(); assumptions.clear(); assumptions.push(p); assumptions.push(q); assumptions.push(r); return solve_() == g421l_True; }
 +inline bool     Solver::solve         (const vec<Lit>& assumps){ budgetOff(); assumps.copyTo(assumptions); return solve_() == g421l_True; }
  inline lbool    Solver::solveLimited  (const vec<Lit>& assumps){ assumps.copyTo(assumptions); return solve_(); }
  inline bool     Solver::okay          ()      const   { return ok; }
  
-@@ -601,7 +610,10 @@
+@@ -601,6 +610,9 @@
  inline void     Solver::toDimacs     (const char* file, Lit p, Lit q){ vec<Lit> as; as.push(p); as.push(q); toDimacs(file, as); }
  inline void     Solver::toDimacs     (const char* file, Lit p, Lit q, Lit r){ vec<Lit> as; as.push(p); as.push(q); as.push(r); toDimacs(file, as); }
  
 +// Warm start mode:
 +inline void     Solver::setStartMode (bool warm) { warm_start = warm; cancelUntil(0); }
- 
 +
+ 
  /************************************************************
   * Compute LBD functions
-  *************************************************************/
 @@ -646,7 +658,7 @@
  
  inline void Solver::printLit(Lit l)
  {
 -    printf("%s%d:%c", sign(l) ? "-" : "", var(l)+1, value(l) == l_True ? '1' : (value(l) == l_False ? '0' : 'X'));
 +    printf("%s%d:%c", sign(l) ? "-" : "", var(l)+1, value(l) == g421l_True ? '1' : (value(l) == g421l_False ? '0' : 'X'));
  }
  
  
-diff -Naur solvers/glucose421/core/SolverStats.h solvers/g421/core/SolverStats.h
---- solvers/glucose421/core/SolverStats.h	2023-05-09 23:19:52
-+++ solvers/g421/core/SolverStats.h	2023-07-12 09:52:06
+@@ -685,7 +697,7 @@
+             fprintf(certifiedOutput, "d ");
+ 
+         for(int i = 0; i < lits.size(); i++)
+-            fprintf(certifiedOutput, "%i ", (var(lits[i]) + 1) * (-2 * sign(lits[i]) + 1));
++            fprintf(certifiedOutput, "%i ", var(lits[i]) * (-2 * sign(lits[i]) + 1));
+         fprintf(certifiedOutput, "0\n");
+     }
+ }
+diff -Naur build/solvers/glucose421/core/SolverStats.h solvers/glucose421/core/SolverStats.h
+--- build/solvers/glucose421/core/SolverStats.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/core/SolverStats.h	2023-07-14 09:25:04.463944874 +0200
 @@ -47,12 +47,12 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
   **************************************************************************************************/
  
 -#ifndef SOLVERSTATS_H
 -#define	SOLVERSTATS_H
 +#ifndef Glucose421_SolverStats_h
@@ -1004,17 +1164,17 @@
 +#include "glucose421/mtl/Map.h"
  #include <string>
 -namespace Glucose {
 +namespace Glucose421 {
  
      class SolverStats {
      protected:
-diff -Naur solvers/glucose421/core/SolverTypes.h solvers/g421/core/SolverTypes.h
---- solvers/glucose421/core/SolverTypes.h	2023-05-09 23:19:52
-+++ solvers/g421/core/SolverTypes.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/core/SolverTypes.h solvers/glucose421/core/SolverTypes.h
+--- build/solvers/glucose421/core/SolverTypes.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/core/SolverTypes.h	2023-07-14 09:25:04.463944874 +0200
 @@ -48,21 +48,26 @@
   **************************************************************************************************/
  
  
 -#ifndef Glucose_SolverTypes_h
 -#define Glucose_SolverTypes_h
 +#ifndef Glucose421_SolverTypes_h
@@ -1055,226 +1215,103 @@
 -#define l_Undef (Glucose::lbool((uint8_t)2))
 +#define g421l_True  (Glucose421::lbool((uint8_t)0)) // gcc does not do constant propagation if these are real constants.
 +#define g421l_False (Glucose421::lbool((uint8_t)1))
 +#define g421l_Undef (Glucose421::lbool((uint8_t)2))
  
  class lbool {
      uint8_t value;
-diff -Naur solvers/glucose421/core/lcm.cc solvers/g421/core/lcm.cc
---- solvers/glucose421/core/lcm.cc	2023-05-09 23:19:52
-+++ solvers/g421/core/lcm.cc	2023-07-12 09:52:06
-@@ -1,9 +1,10 @@
--#include "Solver.h"
--#include "mtl/Sort.h"
--using namespace Glucose;
-+#include "glucose421/core/Solver.h"
-+#include "glucose421/mtl/Sort.h"
- 
-+using namespace Glucose421;
- 
- 
+diff -Naur build/solvers/glucose421/Makefile solvers/glucose421/Makefile
+--- build/solvers/glucose421/Makefile	1970-01-01 01:00:00.000000000 +0100
++++ solvers/glucose421/Makefile	2023-07-14 09:25:04.463944874 +0200
+@@ -0,0 +1,41 @@
++### Makefile ---
 +
- // simplify All
- //
- CRef Solver::simplePropagate()
-@@ -25,18 +26,18 @@
- 
-             Lit imp = wbin[k].blocker;
- 
--            if (value(imp) == l_False){
-+            if (value(imp) == g421l_False){
-                 return wbin[k].cref;
-             }
- 
--            if (value(imp) == l_Undef){
-+            if (value(imp) == g421l_Undef){
-                 simpleUncheckEnqueue(imp, wbin[k].cref);
-             }
-         }
-         for (i = j = (Watcher*)ws, end = i + ws.size(); i != end;){
-             // Try to avoid inspecting the clause:
-             Lit blocker = i->blocker;
--            if (value(blocker) == l_True){
-+            if (value(blocker) == g421l_True){
-                 *j++ = *i++; continue;
-             }
- 
-@@ -54,7 +55,7 @@
-             // why not simply do i->blocker=first in this case?
-             Lit     first = c[0];
-             //  Watcher w     = Watcher(cr, first);
--            if (first != blocker && value(first) == l_True){
-+            if (first != blocker && value(first) == g421l_True){
-                 i->blocker = first;
-                 *j++ = *i++; continue;
-             }
-@@ -63,7 +64,7 @@
-             if (incremental){ // ----------------- INCREMENTAL MODE
-                 int choosenPos = -1;
-                 for (int k = 2; k < c.size(); k++){
--                    if (value(c[k]) != l_False){
-+                    if (value(c[k]) != g421l_False){
-                         if (decisionLevel()>assumptions.size()){
-                             choosenPos = k;
-                             break;
-@@ -71,7 +72,7 @@
-                         else{
-                             choosenPos = k;
- 
--                            if (value(c[k]) == l_True || !isSelector(var(c[k]))) {
-+                            if (value(c[k]) == g421l_True || !isSelector(var(c[k]))) {
-                                 break;
-                             }
-                         }
-@@ -91,7 +92,7 @@
-             else{  // ----------------- DEFAULT  MODE (NOT INCREMENTAL)
-                 for (int k = 2; k < c.size(); k++){
- 
--                    if (value(c[k]) != l_False){
-+                    if (value(c[k]) != g421l_False){
-                         // watcher i is abandonned using i++, because cr watches now ~c[k] instead of p
-                         // the blocker is first in the watcher. However,
-                         // the blocker in the corresponding watcher in ~first is not c[1]
-@@ -106,7 +107,7 @@
-             // Did not find watch -- clause is unit under assignment:
-             i->blocker = first;
-             *j++ = *i++;
--            if (value(first) == l_False){
-+            if (value(first) == g421l_False){
-                 confl = cr;
-                 qhead = trail.size();
-                 // Copy the remaining watches:
-@@ -138,7 +139,7 @@
-     for(i = j = (Watcher *) ws, end = i + ws.size(); i != end;) {
-         // Try to avoid inspecting the clause:
-         Lit blocker = i->blocker;
--        if(value(blocker) == l_True) {
-+        if(value(blocker) == g421l_True) {
-             *j++ = *i++;
-             continue;
-         }
-@@ -155,7 +156,7 @@
-         i++;
-         Watcher w = Watcher(cr, c[0]);
-         for(int k = 1; k < c.size(); k++) {
--            if(value(c[k]) != l_False) {
-+            if(value(c[k]) != g421l_False) {
-                 c[0] = c[k];
-                 c[k] = false_lit;
-                 unaryWatches[~c[0]].push(w);
-@@ -181,7 +182,7 @@
- 
- 
- void Solver::simpleUncheckEnqueue(Lit p, CRef from){
--    assert(value(p) == l_Undef);
-+    assert(value(p) == g421l_Undef);
-     assigns[var(p)] = lbool(!sign(p)); // this makes a lbool object whose value is sign(p)
-     vardata[var(p)].reason = from;
-     trail.push_(p);
-@@ -192,7 +193,7 @@
-     for (int c = trail.size() - 1; c >= trailRecord; c--)
-     {
-         Var x = var(trail[c]);
--        assigns[x] = l_Undef;
-+        assigns[x] = g421l_Undef;
- 
-     }
-     qhead = trailRecord;
-@@ -224,9 +225,9 @@
-             Clause& c = ca[confl];
-             // Special case for binary clauses
-             // The first one has to be SAT
--            if (p != lit_Undef && c.size() == 2 && value(c[0]) == l_False) {
-+            if (p != lit_Undef && c.size() == 2 && value(c[0]) == g421l_False) {
- 
--                assert(value(c[1]) == l_True);
-+                assert(value(c[1]) == g421l_True);
-                 Lit tmp = c[0];
-                 c[0] = c[1], c[1] = tmp;
-             }
-@@ -274,8 +275,8 @@
-     CRef confl;
- 
-     for (i = 0, j = 0; i < c.size(); i++){
--        if (value(c[i]) == l_Undef){
--            //printf("///@@@ uncheckedEnqueue:index = %d. l_Undef\n", i);
-+        if (value(c[i]) == g421l_Undef){
-+            //printf("///@@@ uncheckedEnqueue:index = %d. g421l_Undef\n", i);
-             simpleUncheckEnqueue(~c[i]);
-             c[j++] = c[i];
-             confl = simplePropagate();
-@@ -284,8 +285,8 @@
-             }
-         }
-         else{
--            if (value(c[i]) == l_True){
--                //printf("///@@@ uncheckedEnqueue:index = %d. l_True\n", i);
-+            if (value(c[i]) == g421l_True){
-+                //printf("///@@@ uncheckedEnqueue:index = %d. g421l_True\n", i);
-                 c[j++] = c[i];
-                 True_confl = true;
-                 confl = reason(var(c[i]));
-@@ -293,7 +294,7 @@
-             }
-             else{
-                 falseLit.push(c[i]);
--                //printf("///@@@ uncheckedEnqueue:index = %d. l_False\n", i);
-+                //printf("///@@@ uncheckedEnqueue:index = %d. g421l_False\n", i);
-             }
-         }
-     }
-@@ -350,11 +351,11 @@
-             if (!removed(cr)){
-                 sat = false_lit = false;
-                 for (int i = 0; i < c.size(); i++){
--                    if (value(c[i]) == l_True){
-+                    if (value(c[i]) == g421l_True){
-                         sat = true;
-                         break;
-                     }
--                    else if (value(c[i]) == l_False){
-+                    else if (value(c[i]) == g421l_False){
-                         false_lit = true;
-                     }
-                 }
-@@ -366,7 +367,7 @@
- 
-                     if (false_lit){
-                         for (li = lj = 0; li < c.size(); li++){
--                            if (value(c[li]) != l_False){
-+                            if (value(c[li]) != g421l_False){
-                                 c[lj++] = c[li];
-                             }
-                         }
-@@ -444,11 +445,11 @@
-             if (!removed(cr)){
-                 sat = false_lit = false;
-                 for (int i = 0; i < c.size(); i++){
--                    if (value(c[i]) == l_True){
-+                    if (value(c[i]) == g421l_True){
-                         sat = true;
-                         break;
-                     }
--                    else if (value(c[i]) == l_False){
-+                    else if (value(c[i]) == g421l_False){
-                         false_lit = true;
-                     }
-                 }
-@@ -460,7 +461,7 @@
- 
-                     if (false_lit){
-                         for (li = lj = 0; li < c.size(); li++){
--                            if (value(c[li]) != l_False){
-+                            if (value(c[li]) != g421l_False){
-                                 c[lj++] = c[li];
-                             }
-                         }
-diff -Naur solvers/glucose421/mtl/Alg.h solvers/g421/mtl/Alg.h
---- solvers/glucose421/mtl/Alg.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Alg.h	2023-07-12 09:52:06
++## Author: aign
++## Keywords:
++
++# main parameters
++#CXX      := c++
++#CXXFLAGS := -std=c++11 -fPIC -Wall -Wno-deprecated -fno-strict-aliasing -DINCREMENTAL
++
++CXX      := g++
++CXXFLAGS := -Wall -Wno-parentheses -std=c++11 -D __STDC_LIMIT_MACROS -D __STDC_FORMAT_MACROS -fPIC
++CXXOPT   := -O3 -DNDEBUG
++CXXDEBUG := -O0 -g3
++CXXPROF  := -O3 -g3 -fno-inline -fno-omit-frame-pointer -pg -DNDEBUG
++INCLUDES := -I..
++LIBS     := -L.
++SOURCES  := core/lcm.cc core/Solver.cc utils/Options.cc utils/System.cc
++OBJECTS  := $(SOURCES:.cc=.o)
++TRGT     :=  glucose421
++
++# gather compiler options
++CXXARGS := $(CXXFLAGS) $(INCLUDES) $(CXXOPT)
++
++# targets
++.PHONY: all clean lib
++
++all: lib
++
++lib: $(OBJECTS)
++	@-ar cvq lib$(TRGT).a $(OBJECTS)
++	## @-ar cr lib$(TRGT).a $(OBJECTS)
++
++%.o: %.cc
++	$(CXX) $(CXXARGS) -c $< -o $@
++
++clean:
++	@-rm $(OBJECTS) lib$(TRGT).a
++
++allclean:
++	@-find . -name '*.o' -delete
++	@-find . -name '*.a' -delete
+diff -Naur build/solvers/glucose421/Makefile.old solvers/glucose421/Makefile.old
+--- build/solvers/glucose421/Makefile.old	1970-01-01 01:00:00.000000000 +0100
++++ solvers/glucose421/Makefile.old	2023-07-14 09:25:04.463944874 +0200
+@@ -0,0 +1,37 @@
++### Makefile ---
++
++## Author: aign
++## Keywords:
++
++# main parameters
++CXX      := c++
++CXXFLAGS := -std=c++11 -fPIC -Wall -Wno-deprecated -fno-strict-aliasing -DINCREMENTAL
++CXXOPT   := -O3 -DNDEBUG
++CXXDEBUG := -O0 -g3
++CXXPROF  := -O3 -g3 -fno-inline -fno-omit-frame-pointer -pg -DNDEBUG
++INCLUDES := -I..
++LIBS     := -L.
++SOURCES  := core/Solver.cc core/lmc.cc utils/Options.cc utils/System.cc
++OBJECTS  := $(SOURCES:.cc=.o)
++TRGT     :=  glucose421
++
++# gather compiler options
++CXXARGS := $(CXXFLAGS) $(INCLUDES) $(CXXOPT)
++
++# targets
++.PHONY: all clean lib
++
++all: lib
++
++lib: $(OBJECTS)
++	@-ar cr lib$(TRGT).a $(OBJECTS)
++
++%.o: %.cc
++	$(CXX) $(CXXARGS) -c $< -o $@
++
++clean:
++	@-rm $(OBJECTS)
++
++allclean:
++	@-find . -name '*.o' -delete
++	@-find . -name '*.a' -delete
+diff -Naur build/solvers/glucose421/mtl/Alg.h solvers/glucose421/mtl/Alg.h
+--- build/solvers/glucose421/mtl/Alg.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Alg.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,12 +18,12 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_Alg_h
 -#define Glucose_Alg_h
 +#ifndef Glucose421_Alg_h
@@ -1284,17 +1321,17 @@
 +#include "glucose421/mtl/Vec.h"
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //=================================================================================================
  // Useful functions on vector-like types:
-diff -Naur solvers/glucose421/mtl/Alloc.h solvers/g421/mtl/Alloc.h
---- solvers/glucose421/mtl/Alloc.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Alloc.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/Alloc.h solvers/glucose421/mtl/Alloc.h
+--- build/solvers/glucose421/mtl/Alloc.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Alloc.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,13 +18,13 @@
  **************************************************************************************************/
  
  
 -#ifndef Glucose_Alloc_h
 -#define Glucose_Alloc_h
 +#ifndef Glucose421_Alloc_h
@@ -1306,32 +1343,32 @@
 +#include "glucose421/mtl/Vec.h"
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //=================================================================================================
  // Simple Region-based memory allocator:
-diff -Naur solvers/glucose421/mtl/Clone.h solvers/g421/mtl/Clone.h
---- solvers/glucose421/mtl/Clone.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Clone.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/Clone.h solvers/glucose421/mtl/Clone.h
+--- build/solvers/glucose421/mtl/Clone.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Clone.h	2023-07-14 09:25:04.463944874 +0200
 @@ -1,8 +1,8 @@
 -#ifndef Glucose_Clone_h
 -#define Glucose_Clone_h
 +#ifndef Glucose421_Clone_h
 +#define Glucose421_Clone_h
  
  
 -namespace Glucose {
 +namespace Glucose421 {
  
      class Clone {
          public:
-diff -Naur solvers/glucose421/mtl/Heap.h solvers/g421/mtl/Heap.h
---- solvers/glucose421/mtl/Heap.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Heap.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/Heap.h solvers/glucose421/mtl/Heap.h
+--- build/solvers/glucose421/mtl/Heap.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Heap.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,12 +18,12 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_Heap_h
 -#define Glucose_Heap_h
 +#ifndef Glucose421_Heap_h
@@ -1341,17 +1378,17 @@
 +#include "glucose421/mtl/Vec.h"
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //=================================================================================================
  // A heap implementation with support for decrease/increase key.
-diff -Naur solvers/glucose421/mtl/Map.h solvers/g421/mtl/Map.h
---- solvers/glucose421/mtl/Map.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Map.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/Map.h solvers/glucose421/mtl/Map.h
+--- build/solvers/glucose421/mtl/Map.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Map.h	2023-07-14 09:25:04.463944874 +0200
 @@ -17,15 +17,15 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_Map_h
 -#define Glucose_Map_h
 +#ifndef Glucose421_Map_h
@@ -1365,17 +1402,17 @@
  #include <unordered_map>
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //=================================================================================================
  // Default hash/equals functions
-diff -Naur solvers/glucose421/mtl/Queue.h solvers/g421/mtl/Queue.h
---- solvers/glucose421/mtl/Queue.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Queue.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/Queue.h solvers/glucose421/mtl/Queue.h
+--- build/solvers/glucose421/mtl/Queue.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Queue.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,12 +18,12 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_Queue_h
 -#define Glucose_Queue_h
 +#ifndef Glucose421_Queue_h
@@ -1385,17 +1422,17 @@
 +#include "glucose421/mtl/Vec.h"
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //=================================================================================================
  
-diff -Naur solvers/glucose421/mtl/Sort.h solvers/g421/mtl/Sort.h
---- solvers/glucose421/mtl/Sort.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Sort.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/Sort.h solvers/glucose421/mtl/Sort.h
+--- build/solvers/glucose421/mtl/Sort.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Sort.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,16 +18,16 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_Sort_h
 -#define Glucose_Sort_h
 +#ifndef Glucose421_Sort_h
@@ -1409,17 +1446,17 @@
  
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  template<class T>
  struct LessThan_default {
-diff -Naur solvers/glucose421/mtl/Vec.h solvers/g421/mtl/Vec.h
---- solvers/glucose421/mtl/Vec.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/Vec.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/Vec.h solvers/glucose421/mtl/Vec.h
+--- build/solvers/glucose421/mtl/Vec.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/Vec.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,17 +18,17 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_Vec_h
 -#define Glucose_Vec_h
 +#ifndef Glucose421_Vec_h
@@ -1444,17 +1481,17 @@
      if (cap >= min_cap) return;
      int add = imax((min_cap - cap + 1) & ~1, ((cap >> 1) + 2) & ~1);   // NOTE: grow by approximately 3/2
 -    if (add > INT_MAX - cap || ((data = (T*)::realloc(data, (cap += add) * sizeof(T))) == NULL) && errno == ENOMEM)
 +    if (add > INT_MAX - cap || (((data = (T*)::realloc(data, (cap += add) * sizeof(T))) == NULL) && errno == ENOMEM))
          throw OutOfMemoryException();
   }
  
-diff -Naur solvers/glucose421/mtl/VecThreads.h solvers/g421/mtl/VecThreads.h
---- solvers/glucose421/mtl/VecThreads.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/VecThreads.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/VecThreads.h solvers/glucose421/mtl/VecThreads.h
+--- build/solvers/glucose421/mtl/VecThreads.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/VecThreads.h	2023-07-14 09:25:04.463944874 +0200
 @@ -19,17 +19,17 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_VecThreads_h
 -#define Glucose_VecThreads_h
 +#ifndef Glucose421_VecThreads_h
@@ -1470,17 +1507,17 @@
  #include<string.h>
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //=================================================================================================
  // Automatically resizable arrays
-diff -Naur solvers/glucose421/mtl/XAlloc.h solvers/g421/mtl/XAlloc.h
---- solvers/glucose421/mtl/XAlloc.h	2023-05-09 23:19:52
-+++ solvers/g421/mtl/XAlloc.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/mtl/XAlloc.h solvers/glucose421/mtl/XAlloc.h
+--- build/solvers/glucose421/mtl/XAlloc.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/mtl/XAlloc.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,14 +18,14 @@
  **************************************************************************************************/
  
  
 -#ifndef Glucose_XAlloc_h
 -#define Glucose_XAlloc_h
 +#ifndef Glucose421_XAlloc_h
@@ -1491,17 +1528,17 @@
  #include <stdio.h>
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //=================================================================================================
  // Simple layer on top of malloc/realloc to catch out-of-memory situtaions and provide some typing:
-diff -Naur solvers/glucose421/utils/Options.cc solvers/g421/utils/Options.cc
---- solvers/glucose421/utils/Options.cc	2023-05-09 23:19:52
-+++ solvers/g421/utils/Options.cc	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/utils/Options.cc solvers/glucose421/utils/Options.cc
+--- build/solvers/glucose421/utils/Options.cc	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/utils/Options.cc	2023-07-14 09:25:04.463944874 +0200
 @@ -17,13 +17,13 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#include "mtl/Sort.h"
 -#include "utils/Options.h"
 -#include "utils/ParseUtils.h"
@@ -1533,17 +1570,17 @@
          fprintf(stderr, usage, argv[0]);
  
 -        sort(Option::getOptionList(), Option::OptionLt());
 +    sort(Option::getOptionList(), Option::OptionLt());
  
      const char* prev_cat  = NULL;
      const char* prev_type = NULL;
-diff -Naur solvers/glucose421/utils/Options.h solvers/g421/utils/Options.h
---- solvers/glucose421/utils/Options.h	2023-05-09 23:19:52
-+++ solvers/g421/utils/Options.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/utils/Options.h solvers/glucose421/utils/Options.h
+--- build/solvers/glucose421/utils/Options.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/utils/Options.h	2023-07-14 09:25:04.463944874 +0200
 @@ -17,19 +17,19 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_Options_h
 -#define Glucose_Options_h
 +#ifndef Glucose421_Options_h
@@ -1562,33 +1599,41 @@
 +#include "glucose421/utils/ParseUtils.h"
  
 -namespace Glucose {
 +namespace Glucose421 {
  
  //==================================================================================================
  // Top-level option parse/help functions:
-diff -Naur solvers/glucose421/utils/ParseUtils.h solvers/g421/utils/ParseUtils.h
---- solvers/glucose421/utils/ParseUtils.h	2023-05-09 23:19:52
-+++ solvers/g421/utils/ParseUtils.h	2023-07-12 09:52:06
-@@ -18,110 +18,14 @@
+@@ -60,7 +60,7 @@
+     struct OptionLt {
+         bool operator()(const Option* x, const Option* y) {
+             int test1 = strcmp(x->category, y->category);
+-            return test1 < 0 || test1 == 0 && strcmp(x->type_name, y->type_name) < 0;
++            return test1 < 0 || (test1 == 0 && strcmp(x->type_name, y->type_name) < 0);
+         }
+     };
+ 
+diff -Naur build/solvers/glucose421/utils/ParseUtils.h solvers/glucose421/utils/ParseUtils.h
+--- build/solvers/glucose421/utils/ParseUtils.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/utils/ParseUtils.h	2023-07-14 09:25:04.463944874 +0200
+@@ -18,109 +18,13 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_ParseUtils_h
 -#define Glucose_ParseUtils_h
 +#ifndef Glucose421_ParseUtils_h
 +#define Glucose421_ParseUtils_h
  
  #include <stdlib.h>
  #include <stdio.h>
 -#include <math.h>
- 
+-
 -#include <zlib.h>
-+namespace Glucose421 {
- 
+-
 -namespace Glucose {
 -
 -//-------------------------------------------------------------------------------------------------
 -// A simple buffered character stream class:
 -
 -static const int buffer_size = 1048576;
 -
@@ -1674,19 +1719,19 @@
 -    if      (*in == '-') neg = true, ++in;
 -    else if (*in == '+') ++in;
 -    if (*in < '0' || *in > '9') fprintf(stderr, "PARSE ERROR! Unexpected char: %c\n", *in), exit(3);
 -    while (*in >= '0' && *in <= '9')
 -        val = val*10 + (*in - '0'),
 -        ++in;
 -    return neg ? -val : val; }
--
--
+ 
++namespace Glucose421 {
+ 
  // String matching: in case of a match the input iterator will be advanced the corresponding
  // number of characters.
- template<class B>
 @@ -136,16 +40,6 @@
      return true; 
  }
  
 -// String matching: consumes characters eagerly, but does not require random access iterator.
 -template<class B>
 -static bool eagerMatch(B& in, const char* str) {
@@ -1696,17 +1741,17 @@
 -    return true; }
 -
 -
 -//=================================================================================================
  }
  
  #endif
-diff -Naur solvers/glucose421/utils/System.cc solvers/g421/utils/System.cc
---- solvers/glucose421/utils/System.cc	2023-05-09 23:19:52
-+++ solvers/g421/utils/System.cc	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/utils/System.cc solvers/glucose421/utils/System.cc
+--- build/solvers/glucose421/utils/System.cc	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/utils/System.cc	2023-07-14 09:25:04.463944874 +0200
 @@ -18,14 +18,14 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#include "utils/System.h"
 +#include "glucose421/utils/System.h"
  
@@ -1749,17 +1794,17 @@
      return (double)t.max_size_in_use / (1024*1024); }
  
  #else
 -double Glucose::memUsed() { 
 +double Glucose421::memUsed() { 
      return 0; }
  #endif
-diff -Naur solvers/glucose421/utils/System.h solvers/g421/utils/System.h
---- solvers/glucose421/utils/System.h	2023-05-09 23:19:52
-+++ solvers/g421/utils/System.h	2023-07-12 09:52:06
+diff -Naur build/solvers/glucose421/utils/System.h solvers/glucose421/utils/System.h
+--- build/solvers/glucose421/utils/System.h	2023-05-09 15:19:52.000000000 +0200
++++ solvers/glucose421/utils/System.h	2023-07-14 09:25:04.463944874 +0200
 @@ -18,18 +18,18 @@
  OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  **************************************************************************************************/
  
 -#ifndef Glucose_System_h
 -#define Glucose_System_h
 +#ifndef Glucose421_System_h
```

### Comparing `python-sat-0.1.8.dev8/solvers/patches/gluecard30.patch` & `python-sat-0.1.8.dev9/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/gluecard41.patch` & `python-sat-0.1.8.dev9/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/lingeling.patch` & `python-sat-0.1.8.dev9/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/maplechrono.patch` & `python-sat-0.1.8.dev9/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/maplecm.patch` & `python-sat-0.1.8.dev9/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/maplesat.patch` & `python-sat-0.1.8.dev9/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/mergesat3.patch` & `python-sat-0.1.8.dev9/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/minicard.patch` & `python-sat-0.1.8.dev9/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/minisat22.patch` & `python-sat-0.1.8.dev9/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/patches/minisatgh.patch` & `python-sat-0.1.8.dev9/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/prepare.py` & `python-sat-0.1.8.dev9/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/solvers/pysolvers.cc` & `python-sat-0.1.8.dev9/solvers/pysolvers.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_accum_stats.py` & `python-sat-0.1.8.dev9/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_atmost1.py` & `python-sat-0.1.8.dev9/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_atmostk.py` & `python-sat-0.1.8.dev9/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_cnfplus.py` & `python-sat-0.1.8.dev9/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_equals1.py` & `python-sat-0.1.8.dev9/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_process.py` & `python-sat-0.1.8.dev9/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_unique_model.py` & `python-sat-0.1.8.dev9/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_unique_mus.py` & `python-sat-0.1.8.dev9/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev8/tests/test_warmstart.py` & `python-sat-0.1.8.dev9/tests/test_warmstart.py`

 * *Files identical despite different names*

