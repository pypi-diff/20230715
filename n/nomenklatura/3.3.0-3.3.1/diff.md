# Comparing `tmp/nomenklatura-3.3.0.tar.gz` & `tmp/nomenklatura-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.3.0.tar", last modified: Sat Jul 15 05:57:54 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.1.tar", last modified: Sat Jul 15 09:19:55 2023, max compression
```

## Comparing `nomenklatura-3.3.0.tar` & `nomenklatura-3.3.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:57:54.912878 nomenklatura-3.3.0/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:57:11.000000 nomenklatura-3.3.0/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 05:57:54.000000 nomenklatura-3.3.0/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 05:57:54.916878 nomenklatura-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-15 05:55:35.000000 nomenklatura-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:19:08.000000 nomenklatura-3.3.1/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/setup.py
```

### Comparing `nomenklatura-3.3.0/LICENSE` & `nomenklatura-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/PKG-INFO` & `nomenklatura-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.0
+Version: 3.3.1
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -91,7 +92,9 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
+
+
```

### Comparing `nomenklatura-3.3.0/README.md` & `nomenklatura-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/cache.py` & `nomenklatura-3.3.1/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/cli.py` & `nomenklatura-3.3.1/nomenklatura/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from followthemoney.cli.util import path_entities, write_entity
 from followthemoney.cli.aggregate import sorted_aggregate
 
 from nomenklatura.cache import Cache
 from nomenklatura.matching import train_v2_matcher, train_v1_matcher
 from nomenklatura.store import load_entity_file_store
 from nomenklatura.resolver import Resolver
-from nomenklatura.dataset import Dataset
+from nomenklatura.dataset import Dataset, DefaultDataset
 from nomenklatura.entity import CompositeEntity as Entity
 from nomenklatura.enrich import Enricher, make_enricher, match, enrich
 from nomenklatura.statement import Statement, CSV, FORMATS
 from nomenklatura.matching import get_algorithm, DefaultAlgorithm
 from nomenklatura.statement import write_statements, read_path_statements
 from nomenklatura.senzing import senzing_record
 from nomenklatura.xref import xref as run_xref
@@ -272,26 +272,30 @@
     with path_writer(outpath) as outfh:
         write_statements(outfh, out_format, statements)
 
 
 @cli.command("aggregate-statements", help="Roll up statements into entities")
 @click.option("-i", "--infile", type=InPath, default="-")
 @click.option("-o", "--outpath", type=OutPath, default="-")
+@click.option("-d", "--dataset", type=str, default=DefaultDataset.name)
 @click.option("-f", "--format", type=click.Choice(FORMATS), default=CSV)
-def statements_aggregate(infile: Path, outpath: Path, format: str) -> None:
+def statements_aggregate(
+    infile: Path, outpath: Path, dataset: str, format: str
+) -> None:
+    dataset_ = Dataset.make({"name": dataset, "title": dataset})
     with path_writer(outpath) as outfh:
         statements: List[Statement] = []
         for stmt in read_path_statements(
             infile, format=format, statement_type=Statement
         ):
             if len(statements) and statements[0].canonical_id != stmt.canonical_id:
-                entity = Entity.from_statements(statements)
+                entity = Entity.from_statements(dataset_, statements)
                 write_entity(outfh, entity)
                 statements = []
             statements.append(stmt)
         if len(statements):
-            entity = Entity.from_statements(statements)
+            entity = Entity.from_statements(dataset_, statements)
             write_entity(outfh, entity)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `nomenklatura-3.3.0/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.1/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.1/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.1/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.1/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.1/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.1/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.1/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/dataset/util.py` & `nomenklatura-3.3.1/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/db.py` & `nomenklatura-3.3.1/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.1/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.1/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/common.py` & `nomenklatura-3.3.1/nomenklatura/enrich/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,20 +118,15 @@
             if cache_days is not None and cache_days > 0:
                 self.cache.set_json(cache_key, resp_data)
         return resp_data
 
     def _make_data_entity(
         self, entity: CE, data: Dict[str, Any], cleaned: bool = True
     ) -> CE:
-        return type(entity).from_dict(
-            model,
-            data,
-            default_dataset=self.dataset,
-            cleaned=cleaned,
-        )
+        return type(entity).from_data(self.dataset, data, cleaned=cleaned)
 
     def load_entity(self, entity: CE, data: Dict[str, Any]) -> CE:
         proxy = self._make_data_entity(entity, data, cleaned=False)
         for prop in proxy.iterprops():
             if prop.stub:
                 proxy.pop(prop)
         return proxy
```

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.1/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.1/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.1/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/entity.py` & `nomenklatura-3.3.1/nomenklatura/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,21 @@
     """An entity object that can link to a set of datasets that it is sourced from."""
 
     __slots__ = (
         "schema",
         "id",
         "_caption",
         "extra_referents",
-        "default_dataset",
+        "dataset",
         "statement_type",
         "last_change",
         "_statements",
     )
 
-    def __init__(
-        self,
-        model: "Model",
-        data: Dict[str, Any],
-        cleaned: bool = True,
-        default_dataset: Dataset = DefaultDataset,
-    ):
+    def __init__(self, dataset: Dataset, data: Dict[str, Any], cleaned: bool = True):
         data = dict(data or {})
         schema = model.get(data.pop("schema", None))
         if schema is None:
             raise InvalidData(gettext("No schema for entity."))
         self.schema = schema
 
         self._caption: Optional[str] = None
@@ -55,15 +49,17 @@
 
         self.extra_referents: Set[str] = set(data.pop("referents", []))
         """The IDs of all entities which are included in this canonical entity."""
 
         self.last_change: Optional[str] = None
         """The last time this entity was changed."""
 
-        self.default_dataset = default_dataset
+        self.dataset = dataset
+        """The default dataset for new statements."""
+
         self.id: Optional[str] = data.pop("id", None)
         self._statements: Dict[str, Set[Statement]] = {}
 
         properties = data.pop("properties", None)
         # external = data.pop("external", None)
         if isinstance(properties, Mapping):
             for key, value in properties.items():
@@ -95,15 +91,15 @@
         if self.id is not None:
             yield Statement(
                 canonical_id=self.id,
                 entity_id=self.id,
                 prop=BASE_ID,
                 schema=self.schema.name,
                 value=self.checksum(),
-                dataset=self.default_dataset.name,
+                dataset=self.dataset.name,
             )
         yield from self._iter_stmt()
 
     @property
     def first_seen(self) -> Optional[str]:
         seen = (s.first_seen for s in self._iter_stmt() if s.first_seen is not None)
         return min(seen, default=None)
@@ -134,15 +130,15 @@
         for stmt in self._iter_stmt():
             if stmt.entity_id is not None and stmt.entity_id != self.id:
                 referents.add(stmt.entity_id)
         return referents
 
     @property
     def key_prefix(self) -> Optional[str]:
-        return self.default_dataset.name
+        return self.dataset.name
 
     @key_prefix.setter
     def key_prefix(self, dataset: str) -> None:
         raise NotImplementedError()
 
     def _pick_caption(self) -> str:
         is_thing = self.schema.is_a("Thing")
@@ -169,25 +165,26 @@
         # TODO: change target, schema etc. based on data
         if not self.schema.is_a(stmt.schema):
             try:
                 self.schema = model.common_schema(self.schema, stmt.schema)
             except InvalidData as exc:
                 raise InvalidData(f"{self.id}: {exc}") from exc
 
-        if stmt.prop != BASE_ID:
+        if stmt.prop == BASE_ID:
+            if stmt.first_seen is not None:
+                # The last_change attribute describes the latest checksum change
+                # of any emitted component of the entity, which is stored in the BASE
+                # field.
+                if self.last_change is None:
+                    self.last_change = stmt.first_seen
+                else:
+                    self.last_change = max(self.last_change, stmt.first_seen)
+        else:
             self._statements.setdefault(stmt.prop, set())
             self._statements[stmt.prop].add(stmt)
-        elif stmt.first_seen is not None:
-            # The last_change attribute describes the latest checksum change
-            # of any emitted component of the entity, which is stored in the BASE
-            # field.
-            if self.last_change is None:
-                self.last_change = stmt.first_seen
-            else:
-                self.last_change = max(self.last_change, stmt.first_seen)
 
     def get(self, prop: P, quiet: bool = False) -> List[str]:
         prop_name = self._prop_name(prop, quiet=quiet)
         if prop_name is None or prop_name not in self._statements:
             return []
         return list({s.value for s in self._statements[prop_name]})
 
@@ -290,15 +287,15 @@
             original_value = value
 
         stmt = Statement(
             entity_id=self.id,
             prop=prop.name,
             schema=schema or self.schema.name,
             value=clean,
-            dataset=dataset or self.default_dataset.name,
+            dataset=dataset or self.dataset.name,
             lang=lang,
             original_value=original_value,
             first_seen=seen,
         )
         self.add_statement(stmt)
 
     def pop(self, prop: P, quiet: bool = True) -> List[str]:
@@ -345,19 +342,15 @@
         return {p: list({s.value for s in vs}) for p, vs in self._statements.items()}
 
     def iterprops(self) -> List[Property]:
         return [self.schema.properties[p] for p in self._statements.keys()]
 
     def clone(self: CE) -> CE:
         data = {"schema": self.schema.name, "id": self.id}
-        cloned = type(self).from_dict(
-            self.schema.model,
-            data,
-            default_dataset=self.default_dataset,
-        )
+        cloned = type(self)(self.dataset, data)
         for stmt in self._iter_stmt():
             cloned.add_statement(stmt)
         return cloned
 
     def merge(self: CE, other: "CompositeEntity") -> CE:
         for stmt in other._iter_stmt():
             if self.id is not None:
@@ -414,26 +407,34 @@
 
     @classmethod
     def from_dict(
         cls: Type[CE],
         model: Model,
         data: Dict[str, Any],
         cleaned: bool = True,
-        default_dataset: Dataset = DefaultDataset,
+        default_dataset: Optional[Dataset] = None,
+    ) -> CE:
+        # Exists only for backwards compatibility.
+        dataset = default_dataset or DefaultDataset
+        return cls(dataset, data, cleaned=cleaned)
+
+    @classmethod
+    def from_data(
+        cls: Type[CE], dataset: Dataset, data: Dict[str, Any], cleaned: bool = True
     ) -> CE:
-        return cls(model, data, cleaned=cleaned, default_dataset=default_dataset)
+        return cls(dataset, data, cleaned=cleaned)
 
     @classmethod
     def from_statements(
         cls: Type[CE],
+        dataset: Dataset,
         statements: Iterable[Statement],
-        default_dataset: Dataset = DefaultDataset,
     ) -> CE:
         obj: Optional[CE] = None
         for stmt in statements:
             if obj is None:
                 data = {"schema": stmt.schema, "id": stmt.canonical_id}
-                obj = cls(model, data, default_dataset=default_dataset)
+                obj = cls(dataset, data)
             obj.add_statement(stmt)
         if obj is None:
             raise ValueError("No statements given!")
         return obj
```

### Comparing `nomenklatura-3.3.0/nomenklatura/index/entry.py` & `nomenklatura-3.3.1/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/index/index.py` & `nomenklatura-3.3.1/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.1/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/judgement.py` & `nomenklatura-3.3.1/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.1/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.1/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.1/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.1/nomenklatura/matching/pairs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import json
 from typing import Generator
 from followthemoney import model
+from followthemoney.proxy import EntityProxy
 
 from nomenklatura.entity import CompositeEntity
 from nomenklatura.judgement import Judgement
 from nomenklatura.util import PathLike
 
 
 class JudgedPair(object):
     """A pair of two entities which have been judged to be the same
     (or not) by a user."""
 
     __slots__ = ("left", "right", "judgement")
 
     def __init__(
-        self, left: CompositeEntity, right: CompositeEntity, judgement: Judgement
+        self, left: EntityProxy, right: EntityProxy, judgement: Judgement
     ) -> None:
         self.left = left
         self.right = right
         self.judgement = judgement
 
 
 def read_pairs(pairs_file: PathLike) -> Generator[JudgedPair, None, None]:
     """Read judgement pairs (training data) from a JSON file."""
     with open(pairs_file, "r") as fh:
         while line := fh.readline():
             data = json.loads(line)
-            left_entity = CompositeEntity.from_dict(model, data["left"])
-            right_entity = CompositeEntity.from_dict(model, data["right"])
+            left_entity = EntityProxy.from_dict(model, data["left"])
+            right_entity = EntityProxy.from_dict(model, data["right"])
             judgement = Judgement(data["judgement"])
             if judgement not in (Judgement.POSITIVE, Judgement.NEGATIVE):
                 continue
             yield JudgedPair(left_entity, right_entity, judgement)
```

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/types.py` & `nomenklatura-3.3.1/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/util.py` & `nomenklatura-3.3.1/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.1/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.1/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.1/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.1/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.1/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.1/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.1/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.1/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.1/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.1/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.1/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.1/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/publish/dates.py` & `nomenklatura-3.3.1/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/publish/edges.py` & `nomenklatura-3.3.1/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/publish/names.py` & `nomenklatura-3.3.1/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.1/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.1/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.1/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/senzing.py` & `nomenklatura-3.3.1/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.1/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/statement/statement.py` & `nomenklatura-3.3.1/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/store/__init__.py` & `nomenklatura-3.3.1/nomenklatura/store/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import orjson
 from pathlib import Path
 from typing import Optional
-from followthemoney import model
 
 from nomenklatura.store.base import Store, Writer, View
 from nomenklatura.store.memory import MemoryStore
 from nomenklatura.resolver import Resolver
 from nomenklatura.dataset import Dataset
 from nomenklatura.entity import CompositeEntity
 
@@ -33,15 +32,10 @@
     if dataset is None:
         dataset = Dataset.make({"name": path.stem, "title": path.stem})
     store = MemoryStore(dataset, resolver)
     with store.writer() as writer:
         with open(path, "rb") as fh:
             while line := fh.readline():
                 data = orjson.loads(line)
-                proxy = CompositeEntity.from_dict(
-                    model,
-                    data,
-                    cleaned=cleaned,
-                    default_dataset=dataset,
-                )
+                proxy = CompositeEntity.from_data(dataset, data, cleaned=cleaned)
                 writer.add_entity(proxy)
     return store
```

### Comparing `nomenklatura-3.3.0/nomenklatura/store/base.py` & `nomenklatura-3.3.1/nomenklatura/store/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,15 @@
 
     def assemble(self, statements: List[Statement]) -> Optional[CE]:
         if not len(statements):
             return None
         for stmt in statements:
             if stmt.prop_type == registry.entity.name:
                 stmt.value = self.resolver.get_canonical(stmt.value)
-        entity = self.entity_class.from_statements(
-            statements,
-            default_dataset=self.dataset,
-        )
+        entity = self.entity_class.from_statements(self.dataset, statements)
         if entity.id is not None:
             entity.extra_referents.update(self.resolver.get_referents(entity.id))
         return entity
 
     def update(self, id: StrIdent) -> None:
         canonical_id = self.resolver.get_canonical(id)
         with self.writer() as writer:
```

### Comparing `nomenklatura-3.3.0/nomenklatura/store/level.py` & `nomenklatura-3.3.1/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/store/memory.py` & `nomenklatura-3.3.1/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/store/util.py` & `nomenklatura-3.3.1/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/tui/app.py` & `nomenklatura-3.3.1/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.1/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/tui/util.py` & `nomenklatura-3.3.1/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/util.py` & `nomenklatura-3.3.1/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura/xref.py` & `nomenklatura-3.3.1/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.1/nomenklatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.0
+Version: 3.3.1
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -91,7 +92,9 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
+
+
```

### Comparing `nomenklatura-3.3.0/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.1/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.0/setup.py` & `nomenklatura-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.3.0",
+    version="3.3.1",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

