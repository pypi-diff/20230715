# Comparing `tmp/nomenklatura-3.2.2.tar.gz` & `tmp/nomenklatura-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.2.2.tar", last modified: Thu Jul 13 09:56:37 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.0.tar", last modified: Sat Jul 15 05:57:54 2023, max compression
```

## Comparing `nomenklatura-3.2.2.tar` & `nomenklatura-3.3.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.734102 nomenklatura-3.2.2/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:56:37.730101 nomenklatura-3.2.2/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:55:49.000000 nomenklatura-3.2.2/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 09:56:37.000000 nomenklatura-3.2.2/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:56:37.738103 nomenklatura-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 09:54:17.000000 nomenklatura-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:57:11.000000 nomenklatura-3.3.0/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/setup.py
```

### Comparing `nomenklatura-3.2.2/LICENSE` & `nomenklatura-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/PKG-INFO` & `nomenklatura-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.2.2
+Version: 3.3.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.2.2/README.md` & `nomenklatura-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/cache.py` & `nomenklatura-3.3.0/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/cli.py` & `nomenklatura-3.3.0/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.0/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.0/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.0/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.0/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.0/nomenklatura/dataset/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,78 +46,72 @@
         cdata = data.get("coverage")
         self.coverage = DataCoverage(cdata) if cdata is not None else None
         self.resources: List[DataResource] = []
         for rdata in data.get("resources", []):
             if rdata is not None:
                 self.resources.append(DataResource(rdata))
 
-        # TODO: get rid of the legacy namings
-        self._parents = set(string_list(data.get("parents", [])))
-        self._parents.update(string_list(data.get("collections", [])))
         self._children = set(string_list(data.get("children", [])))
         self._children.update(string_list(data.get("datasets", [])))
 
-    @property
+    @cached_property
     def children(self: DS) -> Set[DS]:
         children: Set[DS] = set()
         for child_name in self._children:
             children.add(self.catalog.require(child_name))
-        for other in self.catalog.datasets:
-            if self.name in other._parents:
-                children.add(other)
         if self in children:
             children.remove(self)
         return children
 
     @cached_property
+    def is_collection(self: DS) -> bool:
+        return len(self.children) > 0
+
+    @property
     def datasets(self: DS) -> Set[DS]:
         current: Set[DS] = set([self])
         for child in self.children:
             current.update(child.datasets)
         return current
 
     @property
-    def parents(self: DS) -> Set[DS]:
-        current: Set[DS] = set()
-        for other in self.catalog.datasets:
-            if self in other.datasets:
-                current.add(other)
-        if self in current:
-            current.remove(self)
-        return current
+    def dataset_names(self: DS) -> List[str]:
+        return [d.name for d in self.datasets]
 
     @property
-    def dataset_names(self) -> List[str]:
-        return [d.name for d in self.datasets]
+    def leaves(self: DS) -> Set[DS]:
+        """All contained datasets which are not collections (can be 'self')."""
+        return set([d for d in self.datasets if not d.is_collection])
 
-    @cached_property
-    def scope_names(self) -> Set[str]:
-        """This is based on the premise that collections (ie. datasets which have children)
-        never contain entities themselves that need to be queried."""
-        if len(self.children):
-            return {d.name for d in self.children}
-        return {self.name}
+    @property
+    def leaf_names(self: DS) -> Set[str]:
+        return {d.name for d in self.leaves}
 
     def __repr__(self) -> str:
         return f"<Dataset({self.name})>"  # pragma: no cover
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self: DS) -> Dict[str, Any]:
         data: Dict[str, Any] = {
             "name": self.name,
             "title": self.title,
             "license": self.license,
             "summary": self.summary,
             "description": self.description,
             "url": self.url,
             "version": self.version,
             "updated_at": self.updated_at,
             "category": self.category,
             "resources": [r.to_dict() for r in self.resources],
-            "children": [c.name for c in self.children],
         }
+        children = [c.name for c in self.children if c != self]
+        if len(children):
+            data["children"] = children
+        datasets = [c.name for c in self.datasets if c != self]
+        if len(datasets):
+            data["datasets"] = datasets
         if self.coverage is not None:
             data["coverage"] = self.coverage.to_dict()
         if self.publisher is not None:
             data["publisher"] = self.publisher.to_dict()
         return cleanup(data)
 
     def get_resource(self, name: str) -> DataResource:
```

### Comparing `nomenklatura-3.2.2/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.0/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.0/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/dataset/util.py` & `nomenklatura-3.3.0/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/db.py` & `nomenklatura-3.3.0/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.0/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.0/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/common.py` & `nomenklatura-3.3.0/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.0/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.0/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.0/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/entity.py` & `nomenklatura-3.3.0/nomenklatura/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
 from typing import Generator, Iterable, Tuple, Type, TypeVar
 from followthemoney import model
 from followthemoney.model import Model
 from followthemoney.exc import InvalidData
 from followthemoney.types.common import PropertyType
 from followthemoney.property import Property
-from followthemoney.util import gettext, value_list
+from followthemoney.util import gettext
 from followthemoney.proxy import P
 from followthemoney.types import registry
 from followthemoney.proxy import EntityProxy
 
 from nomenklatura.dataset import DS, Dataset, DefaultDataset
 from nomenklatura.publish.names import pick_name
 from nomenklatura.statement.statement import Statement
@@ -29,14 +29,15 @@
     __slots__ = (
         "schema",
         "id",
         "_caption",
         "extra_referents",
         "default_dataset",
         "statement_type",
+        "last_change",
         "_statements",
     )
 
     def __init__(
         self,
         model: "Model",
         data: Dict[str, Any],
@@ -51,14 +52,17 @@
 
         self._caption: Optional[str] = None
         """A pre-computed label for this entity."""
 
         self.extra_referents: Set[str] = set(data.pop("referents", []))
         """The IDs of all entities which are included in this canonical entity."""
 
+        self.last_change: Optional[str] = None
+        """The last time this entity was changed."""
+
         self.default_dataset = default_dataset
         self.id: Optional[str] = data.pop("id", None)
         self._statements: Dict[str, Set[Statement]] = {}
 
         properties = data.pop("properties", None)
         # external = data.pop("external", None)
         if isinstance(properties, Mapping):
@@ -164,17 +168,26 @@
     def add_statement(self, stmt: Statement) -> None:
         # TODO: change target, schema etc. based on data
         if not self.schema.is_a(stmt.schema):
             try:
                 self.schema = model.common_schema(self.schema, stmt.schema)
             except InvalidData as exc:
                 raise InvalidData(f"{self.id}: {exc}") from exc
+
         if stmt.prop != BASE_ID:
             self._statements.setdefault(stmt.prop, set())
             self._statements[stmt.prop].add(stmt)
+        elif stmt.first_seen is not None:
+            # The last_change attribute describes the latest checksum change
+            # of any emitted component of the entity, which is stored in the BASE
+            # field.
+            if self.last_change is None:
+                self.last_change = stmt.first_seen
+            else:
+                self.last_change = max(self.last_change, stmt.first_seen)
 
     def get(self, prop: P, quiet: bool = False) -> List[str]:
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is None or prop_name not in self._statements:
             return []
         return list({s.value for s in self._statements[prop_name]})
 
@@ -249,15 +262,15 @@
         schema: Optional[str] = None,
         dataset: Optional[str] = None,
         seen: Optional[str] = None,
         lang: Optional[str] = None,
         original_value: Optional[str] = None,
     ) -> None:
         """Add a statement to the entity, possibly the value."""
-        if value is None:
+        if value is None or len(value) == 0:
             return
 
         # Don't allow setting the reverse properties:
         if prop.stub:
             if quiet:
                 return None
             msg = gettext("Stub property (%s): %s")
@@ -362,14 +375,16 @@
             "referents": list(self.referents),
             "datasets": list(self.datasets),
         }
         if self.first_seen is not None:
             data["first_seen"] = self.first_seen
         if self.last_seen is not None:
             data["last_seen"] = self.last_seen
+        if self.last_change is not None:
+            data["last_change"] = self.last_change
         return data
 
     def __len__(self) -> int:
         return len(list(self._iter_stmt())) + 1
 
     def _to_nested_dict(
         self: CE, view: "View[DS, CE]", depth: int, path: List[str]
```

### Comparing `nomenklatura-3.2.2/nomenklatura/index/entry.py` & `nomenklatura-3.3.0/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/index/index.py` & `nomenklatura-3.3.0/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.0/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/judgement.py` & `nomenklatura-3.3.0/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.0/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.0/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.0/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.0/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/types.py` & `nomenklatura-3.3.0/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/util.py` & `nomenklatura-3.3.0/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.0/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.0/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.0/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.0/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.0/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.0/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.0/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.0/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.0/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.0/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.0/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.0/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/publish/dates.py` & `nomenklatura-3.3.0/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/publish/edges.py` & `nomenklatura-3.3.0/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/publish/names.py` & `nomenklatura-3.3.0/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.0/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.0/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.0/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/senzing.py` & `nomenklatura-3.3.0/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.0/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/statement/statement.py` & `nomenklatura-3.3.0/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/store/__init__.py` & `nomenklatura-3.3.0/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/store/base.py` & `nomenklatura-3.3.0/nomenklatura/store/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         return f"<{type(self).__name__}({self.store!r})>"
 
 
 class View(Generic[DS, CE]):
     def __init__(self, store: Store[DS, CE], scope: DS, external: bool = False):
         self.store = store
         self.scope = scope
-        self.scope_names = scope.scope_names
+        self.dataset_names = scope.leaf_names
         self.external = external
 
     def get_entity(self, id: str) -> Optional[CE]:
         raise NotImplementedError()
 
     def get_inverted(self, id: str) -> Generator[Tuple[Property, CE], None, None]:
         raise NotImplementedError()
```

### Comparing `nomenklatura-3.2.2/nomenklatura/store/level.py` & `nomenklatura-3.3.0/nomenklatura/store/level.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,12 +129,12 @@
             for k in it:
                 _, entity_id, dataset = k.decode("utf-8").split(":", 2)
                 if entity_id != current_id:
                     current_id = entity_id
                     current_match = False
                 if current_match:
                     continue
-                if dataset in self.scope_names:
+                if dataset in self.dataset_names:
                     current_match = True
                     entity = self.get_entity(entity_id)
                     if entity is not None:
                         yield entity
```

### Comparing `nomenklatura-3.2.2/nomenklatura/store/memory.py` & `nomenklatura-3.3.0/nomenklatura/store/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,13 +85,13 @@
                 continue
             for prop, value in entity.itervalues():
                 if value == id and prop.reverse is not None:
                     yield prop.reverse, entity
 
     def entities(self) -> Generator[CE, None, None]:
         entity_ids: Set[str] = set()
-        for scope in self.scope_names:
+        for scope in self.dataset_names:
             entity_ids.update(self.store.entities.get(scope, []))
         for entity_id in entity_ids:
             entity = self.get_entity(entity_id)
             if entity is not None:
                 yield entity
```

### Comparing `nomenklatura-3.2.2/nomenklatura/store/util.py` & `nomenklatura-3.3.0/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/tui/app.py` & `nomenklatura-3.3.0/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.0/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/tui/util.py` & `nomenklatura-3.3.0/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura/util.py` & `nomenklatura-3.3.0/nomenklatura/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     if value is None:
         return []
     if isinstance(value, (str, bytes)):
         text = sanitize_text(value)
         if text is None:
             return []
         return [text]
-    if not isinstance(value, Sequence):
+    if not isinstance(value, (Sequence, set)):
         value = [value]
     texts: List[str] = []
     for inner in value:
         if isinstance(inner, Mapping):
             text = inner.get("id")
             if text is not None:
                 texts.append(text)
```

### Comparing `nomenklatura-3.2.2/nomenklatura/xref.py` & `nomenklatura-3.3.0/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.0/nomenklatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.2.2
+Version: 3.3.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.2.2/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.0/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.2.2/setup.py` & `nomenklatura-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.2.2",
+    version="3.3.0",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

