# Comparing `tmp/auraxium-0.2.4.tar.gz` & `tmp/auraxium-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auraxium-0.2.4.tar", last modified: Sun May 28 21:42:46 2023, max compression
+gzip compressed data, was "auraxium-0.3.0.tar", last modified: Sat Jul 15 15:12:17 2023, max compression
```

## Comparing `auraxium-0.2.4.tar` & `auraxium-0.3.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.781984 auraxium-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-28 21:42:25.000000 auraxium-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-28 21:42:46.781984 auraxium-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-28 21:42:25.000000 auraxium-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium/census/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34687 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/census/_urlgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium/event/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21405 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/event/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/event/_trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.777984 auraxium-0.2.4/auraxium/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_ability.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_achievement.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_armour.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_character.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_depot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    18276 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_experience.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_faction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_fire.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_metagame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_outfit.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_projectile.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_resist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_weapon.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.781984 auraxium-0.2.4/auraxium/ps2/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_ability.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_achievement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_armour.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_depot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_experience.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_faction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_fire.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_metagame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_outfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_projectile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_resist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_weapon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/ps2/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-28 21:42:25.000000 auraxium-0.2.4/auraxium/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:42:46.773984 auraxium-0.2.4/auraxium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 21:42:46.000000 auraxium-0.2.4/auraxium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:42:46.781984 auraxium-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-28 21:42:25.000000 auraxium-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:17.253054 auraxium-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-15 15:11:59.000000 auraxium-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-07-15 15:12:17.253054 auraxium-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-07-15 15:11:59.000000 auraxium-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:17.245054 auraxium-0.3.0/auraxium/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:17.245054 auraxium-0.3.0/auraxium/census/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34687 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/census/_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/census/_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/census/_urlgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:17.245054 auraxium-0.3.0/auraxium/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/event/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/event/_trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:17.249054 auraxium-0.3.0/auraxium/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_armour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_depot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_fire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_metagame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_outfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_projectile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_resist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_weapon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:17.253054 auraxium-0.3.0/auraxium/ps2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_armour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_depot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_fire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_metagame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_outfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_projectile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_resist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_weapon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/ps2/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-15 15:11:59.000000 auraxium-0.3.0/auraxium/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:17.245054 auraxium-0.3.0/auraxium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-07-15 15:12:17.000000 auraxium-0.3.0/auraxium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-15 15:12:17.000000 auraxium-0.3.0/auraxium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:12:17.000000 auraxium-0.3.0/auraxium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:12:17.000000 auraxium-0.3.0/auraxium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 15:12:17.000000 auraxium-0.3.0/auraxium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 15:12:17.000000 auraxium-0.3.0/auraxium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:12:17.253054 auraxium-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-15 15:11:59.000000 auraxium-0.3.0/setup.py
```

### Comparing `auraxium-0.2.4/LICENSE` & `auraxium-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/PKG-INFO` & `auraxium-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auraxium
-Version: 0.2.4
+Version: 0.3.0
 Summary: A python wrapper for the PlanetSide 2 Census API.
 Home-page: https://github.com/leonhard-s/auraxium
 Author: Leonhard S.
 Author-email: leonhard-sei@outlook.com
 License: MIT
 Keywords: auraxium python daybreak census planetside ps2
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,18 +18,18 @@
 
 # <img src="https://raw.githubusercontent.com/leonhard-s/auraxium/master/assets/icon_256.png" align="left" height="140"/>Auraxium
 
 Auraxium is an object-oriented, pure-Python wrapper for the [PlanetSide 2](https://www.planetside2.com/) API.  
 It provides a simple object model that can be used by players and outfits without requiring deep knowledge of the API and its idiosyncrasies.
 
 ![PyPI - License](https://img.shields.io/pypi/l/auraxium)
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/pythonunittest.yml?label=tests)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/ci-testing.yaml?label=tests)
 [![Coveralls github branch](https://img.shields.io/coveralls/github/leonhard-s/auraxium/master)](https://coveralls.io/github/leonhard-s/auraxium)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/auraxium)
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/pythonpublish.yml)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/publish-package.yaml)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/leonhard-s/auraxium)](https://www.codefactor.io/repository/github/leonhard-s/auraxium)
 [![PyPI](https://img.shields.io/pypi/v/auraxium)](https://pypi.org/project/auraxium/)
 [![Read the Docs](https://img.shields.io/readthedocs/auraxium)](https://auraxium.readthedocs.io/en/latest/)
 
 ***
 
 - Clean, Pythonic API
@@ -173,15 +173,15 @@
 
 This is useful if you have a commonly encountered event (like [`event.DEATH`](https://auraxium.readthedocs.io/en/latest/api/event.html#auraxium.event.DEATH)) and would like your action to only run if the event data matches some other requirement (for example "the killing player must be part of my outfit").
 
 #### Actions
 
 The trigger's action is a method or function that will be run when the event fires and all conditions evaluate to True.
 
-If the action is a coroutine according to [`asyncio.iscoroutinefunction()`](https://docs.python.org/3/library/asyncio-task.html#asyncio.iscoroutinefunction), it will be awaited.
+If the action is a coroutine according to [`inspect.iscoroutinefunction()`](https://docs.python.org/3/library/inspect.html#inspect.iscoroutinefunction), it will be awaited.
 
 The only argument passed to the function set as the trigger action is the event received:
 
 ```py
 async def example_action(event: Event) -> None:
     """Example function to showcase the signature used for actions.
```

### Comparing `auraxium-0.2.4/README.md` & `auraxium-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # <img src="https://raw.githubusercontent.com/leonhard-s/auraxium/master/assets/icon_256.png" align="left" height="140"/>Auraxium
 
 Auraxium is an object-oriented, pure-Python wrapper for the [PlanetSide 2](https://www.planetside2.com/) API.  
 It provides a simple object model that can be used by players and outfits without requiring deep knowledge of the API and its idiosyncrasies.
 
 ![PyPI - License](https://img.shields.io/pypi/l/auraxium)
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/pythonunittest.yml?label=tests)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/ci-testing.yaml?label=tests)
 [![Coveralls github branch](https://img.shields.io/coveralls/github/leonhard-s/auraxium/master)](https://coveralls.io/github/leonhard-s/auraxium)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/auraxium)
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/pythonpublish.yml)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/publish-package.yaml)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/leonhard-s/auraxium)](https://www.codefactor.io/repository/github/leonhard-s/auraxium)
 [![PyPI](https://img.shields.io/pypi/v/auraxium)](https://pypi.org/project/auraxium/)
 [![Read the Docs](https://img.shields.io/readthedocs/auraxium)](https://auraxium.readthedocs.io/en/latest/)
 
 ***
 
 - Clean, Pythonic API
@@ -155,15 +155,15 @@
 
 This is useful if you have a commonly encountered event (like [`event.DEATH`](https://auraxium.readthedocs.io/en/latest/api/event.html#auraxium.event.DEATH)) and would like your action to only run if the event data matches some other requirement (for example "the killing player must be part of my outfit").
 
 #### Actions
 
 The trigger's action is a method or function that will be run when the event fires and all conditions evaluate to True.
 
-If the action is a coroutine according to [`asyncio.iscoroutinefunction()`](https://docs.python.org/3/library/asyncio-task.html#asyncio.iscoroutinefunction), it will be awaited.
+If the action is a coroutine according to [`inspect.iscoroutinefunction()`](https://docs.python.org/3/library/inspect.html#inspect.iscoroutinefunction), it will be awaited.
 
 The only argument passed to the function set as the trigger action is the event received:
 
 ```py
 async def example_action(event: Event) -> None:
     """Example function to showcase the signature used for actions.
```

### Comparing `auraxium-0.2.4/auraxium/__init__.py` & `auraxium-0.3.0/auraxium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     'ps2',
     'Ps2Object',
     'SequenceProxy',
     'Trigger'
 ]
 
 __author__ = 'Leonhard S.'
-__version__ = '0.2.4'
+__version__ = '0.3.0'
```

### Comparing `auraxium-0.2.4/auraxium/_cache.py` & `auraxium-0.3.0/auraxium/_cache.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/_client.py` & `auraxium-0.3.0/auraxium/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import warnings
 from typing import Any, Callable, List, Optional, Type, TypeVar, cast
 
 from .base import Named, Ps2Object
 from .census import Query
 from .errors import NotFoundError, PayloadError
-from .ps2 import Character
+from .ps2 import Character, World
 from ._rest import RequestClient, extract_payload, extract_single
 from .types import CensusData
 
 __all__ = [
     'Client'
 ]
 
@@ -139,15 +139,15 @@
 
         :param type_: The object type to search for.
         :type type_: type[auraxium.base.Ps2Object]
         :param int id_: The unique ID of the object.
         :return: The entry with the matching ID, or :obj:`None` if not
            found.
         """
-        filters: CensusData = {type_.id_field: id_}
+        filters: dict[str, Any] = {type_.id_field: id_}
         data = await self.find(type_, results=1, **filters)
         if data and not isinstance(data[0], type_):
             raise RuntimeError(  # pragma: no cover
                 f'Expected {type_} instance, got {type(data[0])} instead, '
                 'please report this bug to the project maintainers')
         if data:
             return data[0]
@@ -191,15 +191,25 @@
             _log.debug('%r restored from cache', instance)
             return instance
         _log.debug('%s "%s"[%s] not cached, generating API query...',
                    type_.__name__, name, locale)
         query = Query(type_.collection, service_id=self.service_id)
         if issubclass(type_, Character):
             query.add_term(field='name.first_lower', value=name.lower())
+        elif issubclass(type_, World):
+            return cast(_NamedT, await self._get_world_by_name(name, locale))
         else:
             query.case(False).add_term(field=f'name.{locale}', value=name)
         payload = await self.request(query)
         try:
             payload = extract_single(payload, type_.collection)
         except NotFoundError:  # pragma: no cover
             return None
         return cast(_NamedT, type_(payload, locale=locale, client=self))
+
+    async def _get_world_by_name(self, name: str, locale: str = 'en',
+                                 ) -> Optional[World]:
+        all_worlds = await self.find(World, results=100)
+        for world in all_worlds:
+            if getattr(world.name, locale).lower() == name.lower():
+                return world
+        return None
```

### Comparing `auraxium-0.2.4/auraxium/_log.py` & `auraxium-0.3.0/auraxium/_log.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/_proxy.py` & `auraxium-0.3.0/auraxium/_proxy.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/_rest.py` & `auraxium-0.3.0/auraxium/_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,17 @@
             namespace, collection = get_components(url)
             # NOTE: This error is returned if either the namespace or
             # collection are unknown
             if collection is None:
                 raise UnknownCollectionError(
                     f'The namespace "{namespace}" does not exist.',
                     url, namespace, collection)
-            help_url = Query(namespace=namespace)
+            with warnings.catch_warnings():
+                warnings.simplefilter('ignore', UserWarning)
+                help_url = Query(namespace=namespace).url()
             raise UnknownCollectionError(
                 f'No collection at "{namespace}/{collection}", try {help_url} '
                 f'for a the list of valid collections, or an error message if '
                 f'the the namespace "{namespace}" is invalid.',
                 url, namespace, collection)
         if msg == 'Bad request syntax.':
             raise BadRequestSyntaxError(
@@ -460,17 +462,20 @@
         tries: int = details['tries']
         _log.warning('Giving up on query and re-raising exception after %.2f '
                      'seconds and %d attempt[s]: %s', elapsed, tries, url)
         _, exc_value, _ = sys.exc_info()
         assert exc_value is not None
         raise exc_value
 
-    backoff_errors = (aiohttp.ClientResponseError,
-                      aiohttp.ClientConnectionError,
-                      MaintenanceError)
+    backoff_errors = (
+        aiohttp.ClientResponseError,
+        aiohttp.ClientConnectionError,
+        MaintenanceError,
+        ServiceUnavailableError,
+    )
 
     # NOTE: As of backoff v2.1.2, "backoff.expo" only takes integer arguments.
     # We therefore scale everything down to meet the original timings
     def backoff_gen() -> Generator[float, None, None]:
         for wait in backoff.expo(base=10, factor=1, max_value=10_000):
             # NOTE: backoff returns None as the first send() - no idea why
             yield wait * 0.001 if wait is not None else None  # type: ignore
```

### Comparing `auraxium-0.2.4/auraxium/_support.py` & `auraxium-0.3.0/auraxium/_support.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/base.py` & `auraxium-0.3.0/auraxium/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,29 +116,29 @@
 
         This will take the form of ``<Class:id>``, e.g.
         ``<Weapon:108>``.
         """
         return f'<{self.__class__.__name__}:{self.id}>'
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.count`')  # pragma: no cover
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.count`')  # pragma: no cover
     async def count(cls, client: RequestClient, **kwargs: Any) -> int:
         """Return the number of items matching the given terms.
 
         :param auraxium.Client client: The client through which to
            perform the request.
         :param kwargs: Any number of query filters to apply.
         :return: The number of entries entries.
         """
         # NOTE: The following is a runtime-only compatibility hack and violates
         # type hinting. This is scheduled for removal as per the decorator.
         return await client.count(cls, **kwargs)  # type: ignore
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.find`')  # pragma: no cover
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.find`')  # pragma: no cover
     async def find(cls: Type[Ps2ObjectT], results: int = 10, *,
                    offset: int = 0, promote_exact: bool = False,
                    check_case: bool = True, client: RequestClient,
                    **kwargs: Any) -> List[Ps2ObjectT]:
         """Return a list of entries matching the given terms.
 
         This returns up to as many entries as indicated by the results
@@ -162,15 +162,15 @@
         # NOTE: The following is a runtime-only compatibility hack and violates
         # type hinting. This is scheduled for removal as per the decorator.
         return await client.find(  # type: ignore
             cls, results=results, offset=offset, promote_exact=promote_exact,
             check_case=check_case, **kwargs)
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
     async def get(cls: Type[Ps2ObjectT], client: RequestClient,
                   check_case: bool = True, **kwargs: Any
                   ) -> Optional[Ps2ObjectT]:
         """Return the first entry matching the given terms.
 
         Like :meth:`Ps2Object.get`, but will only return one item.
 
@@ -183,15 +183,15 @@
         """
         # NOTE: The following is a runtime-only compatibility hack and violates
         # type hinting. This is scheduled for removal as per the decorator.
         return await client.get(  # type: ignore
             cls, results=1, check_case=check_case, **kwargs)
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
     async def get_by_id(cls: Type[Ps2ObjectT], id_: int, *,
                         client: RequestClient) -> Optional[Ps2ObjectT]:
         """Retrieve an object by its unique Census ID.
 
         :param int id\\_: The unique ID of the object.
         :param auraxium.Client client: The client through which to
            perform the request.
@@ -246,15 +246,15 @@
         :param auraxium.Client client: The client used to retrieve the
            object.
         """
         super().__init__(data=data, client=client)
         self._cache.add(self.id, self)
 
     @classmethod
-    def __init_subclass__(  # pylint: disable=unexpected-special-method-signature
+    def __init_subclass__(
             cls, cache_size: int, cache_ttu: float = 0.0) -> None:
         """Initialise a cacheable subclass.
 
         This sets up the TLRU cache for the given subclass using the
         keyword arguments provided in the class definitions.
 
         :param int cache_size: The maximum number of items in the
@@ -287,15 +287,15 @@
             raise ValueError(f'{size} is not a valid cache size')
         cls._cache.clear()
         cls._cache.size = size
         if ttu is not None:
             cls._cache.ttu = ttu
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
     async def get_by_id(cls: Type[CachedT], id_: int, *,
                         client: RequestClient) -> Optional[CachedT]:
         """Retrieve an object by by ID.
 
         This query uses caches and might return an existing instance if
         the object has been recently retrieved.
 
@@ -358,15 +358,15 @@
 
         This retrieves the :atr:``Named.name`` attribute for the
         English locale.
         """
         return str(self.name)
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')  # pragma: no cover
     async def get_by_name(cls: Type[NamedT], name: str, *, locale: str = 'en',
                           client: RequestClient) -> Optional[NamedT]:
         """Retrieve an object by its unique name.
 
         If the same query has been performed recently, it may be
         restored from cache instead.
```

### Comparing `auraxium-0.2.4/auraxium/census/__init__.py` & `auraxium-0.3.0/auraxium/census/__init__.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/census/_query.py` & `auraxium-0.3.0/auraxium/census/_query.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/census/_support.py` & `auraxium-0.3.0/auraxium/census/_support.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/census/_urlgen.py` & `auraxium-0.3.0/auraxium/census/_urlgen.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/endpoints.py` & `auraxium-0.3.0/auraxium/endpoints.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/errors.py` & `auraxium-0.3.0/auraxium/errors.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/event/__init__.py` & `auraxium-0.3.0/auraxium/event/__init__.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/event/_client.py` & `auraxium-0.3.0/auraxium/event/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     .. attribute:: triggers
        :type: list[auraxium.event.Trigger]
 
        The list of :class:`Triggers <auraxium.event.Trigger>`
        registered for the client.
 
     .. attribute:: websocket
-       :type: websockets.client.legacy.WebSocketClientProtocol | None
+       :type: websockets.client.WebSocketClientProtocol | None
 
        The websocket client used for the real-time event stream. This
        will be automatically opened and closed by the client as event
        triggers are added and removed.
     """
 
     def __init__(self, *args: Any,
@@ -326,15 +326,15 @@
     def trigger(self, event: Union[str, Type[Event]],
                 *args: Union[str, Type[Event]], name: Optional[str] = None,
                 **kwargs: Any) -> Callable[[_CallbackT[Event]], None]:
         # Generic fallback variant (callback argument type not checked)
         ...   # pragma: no cover
 
     def trigger(self, event: Union[str, Type[Event]],
-                *args: Union[str, Type[_EventT]], name: Optional[str] = None,
+                *args: Union[str, Type[Event]], name: Optional[str] = None,
                 **kwargs: Any) -> Callable[[_CallbackT[Event]], None]:
         """Create and add a trigger for the given action.
 
         If no name is specified, the call-back function's name will be
         used as the trigger name.
 
         Keep in mind that a trigger's name must be unique. A
@@ -349,16 +349,16 @@
            specified, the decorated function's name will be used.
         :type name: str | None
         :raises KeyError: Raised if a trigger with the given name
            already exists.
         """
         trigger = Trigger(event, *args, name=name, **kwargs)
 
-        def wrapper(func: _CallbackT[_EventT]) -> None:
-            trigger.action = func  # type: ignore
+        def wrapper(func: _CallbackT[Event]) -> None:
+            trigger.action = func
             # If the trigger name has not been specified, use the call-back
             # function's name instead
             if trigger.name is None:
                 trigger.name = func.__name__
             # Ensure the trigger name is unique before adding the trigger
             if any(t.name == trigger.name for t in self.triggers):
                 raise KeyError(f'The trigger "{trigger.name}" already exists')
@@ -381,21 +381,18 @@
         data: CensusData = json.loads(response)
         service = data.get('service')
         # Event messages
         if service == 'event':
             if data['type'] == 'serviceMessage':
                 try:
                     event = _event_factory(cast(CensusData, data['payload']))
-                except pydantic.ValidationError:  # pragma: no cover
+                except pydantic.ValidationError as err:  # pragma: no cover
                     _log.warning(
-                        'Ignoring unsupported payload: %s\n'
-                        'This message means that the Auraxium data model must '
-                        'be updated. Please ensure you are on the latest '
-                        'version of the Auraxium library and report this '
-                        'message to the project maintainers.', data['payload'])
+                        'Ignoring unsupported payload: %s\nPayload: %s\n',
+                        err, data['payload'])
                     return
                 _log.debug('%s event received, dispatching...',
                            event.event_name)
                 self.dispatch(event)
             elif data['type'] == 'heartbeat':  # pragma: no cover
                 servers = cast(Dict[str, str], data['online'])
                 self._endpoint_status = {
```

### Comparing `auraxium-0.2.4/auraxium/event/_trigger.py` & `auraxium-0.3.0/auraxium/event/_trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import asyncio
 import datetime
+import inspect
 import json
 import warnings
 from typing import (Any, Callable, Coroutine, Dict, Iterable, List, Optional,
                     Set, Type, Union)
 
 from ..errors import CensusError
 from ..models import CharacterEvent, Event, GainExperience
@@ -128,15 +128,15 @@
             self.worlds = [w if isinstance(w, int) else w.id for w in worlds]
 
     def callback(self, func: _Action) -> None:
         """Set the given function as the trigger action.
 
         The action may be a regular callable or a coroutine.
         Any callable that is a coroutine function according to
-        :func:`asyncio.iscoroutinefunction` will be awaited.
+        :func:`inspect.iscoroutinefunction` will be awaited.
 
         This method can be used as a decorator.
 
         .. code-block:: python3
 
            my_trigger = Trigger('Death')
 
@@ -228,12 +228,12 @@
         """
         self.last_run = datetime.datetime.utcnow()
         if self.action is None:  # pragma: no cover
             warnings.warn(f'Trigger {self.name} run with no action specified')
             return
         try:
             ret = self.action(event)
-            if asyncio.iscoroutinefunction(self.action):
+            if inspect.iscoroutinefunction(self.action):
                 assert ret is not None
                 await ret
         except CensusError as err:  # pragma: no cover
             warnings.warn(f'Trigger {self.name} callback cancelled: {err}')
```

### Comparing `auraxium-0.2.4/auraxium/models/__init__.py` & `auraxium-0.3.0/auraxium/models/__init__.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/models/_ability.py` & `auraxium-0.3.0/auraxium/models/_ability.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 __all__ = [
     'AbilityData',
     'AbilityTypeData',
     'ResourceTypeData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class AbilityData(RESTPayload):
     """Data class for :class:`auraxium.ps2.Ability`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_character.py` & `auraxium-0.3.0/auraxium/models/_character.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 __all__ = [
     'CharacterAchievement',
     'CharacterData',
     'CharacterDirective',
     'TitleData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class CharacterAchievement(RESTPayload):
     """Data container for a character's achievement status.
 
     .. attribute:: character_id
        :type: int
 
@@ -192,15 +190,15 @@
            case-insensitive name lookups without requiring the use of
            a case-insensitive query.
         """
 
         first: str
         first_lower: str
 
-        @deprecated('0.2', '0.3', replacement=':attr:`auraxium.models.'
+        @deprecated('0.2', '0.4', replacement=':attr:`auraxium.models.'
                     'CharacterData.Name.name`')
         def __call__(self, locale: str = 'en') -> str:  # pragma: no cover
             return self.first
 
         def __str__(self) -> str:
             return self.first
```

### Comparing `auraxium-0.2.4/auraxium/models/_depot.py` & `auraxium-0.3.0/auraxium/models/_depot.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from ..types import LocaleData
 
 __all__ = [
     'MarketingBundleData',
     'MarketingBundleSingleData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class MarketingBundleData(RESTPayload):
     """Data class for :class:`auraxium.ps2.MarketingBundle`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_directive.py` & `auraxium-0.3.0/auraxium/models/_directive.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 __all__ = [
     'DirectiveData',
     'DirectiveTierData',
     'DirectiveTreeData',
     'DirectiveTreeCategoryData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class DirectiveData(RESTPayload, ImageData):
     """Data class for :class:`auraxium.ps2.Directive`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_effect.py` & `auraxium-0.3.0/auraxium/models/_effect.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 __all__ = [
     'EffectData',
     'EffectTypeData',
     'ZoneEffectData',
     'ZoneEffectTypeData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class EffectData(RESTPayload):
     """Data class for :class:`auraxium.ps2.Effect`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_events.py` & `auraxium-0.3.0/auraxium/models/_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     'PlayerFacilityDefend',
     'PlayerLogin',
     'PlayerLogout',
     'SkillAdded',
     'VehicleDestroy'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class AchievementAdded(Event, CharacterEvent):
     """A character has earned a new achievement.
 
     Achievements are either weapon medals or service ribbons.
 
     .. attribute:: character_id
@@ -137,14 +135,19 @@
        ID of the :class:`~auraxium.ps2.Item` used by the attacker.
 
        .. important::
 
          The reference above is not an error, this field reports the
          item ID of the weapon, not the weapon ID.
 
+    .. attribute:: attacker_team_id
+       :type: int
+
+       ID of the team of the attacker.
+
     .. attribute:: character_id
        :type: int
 
        ID of the :class:`~auraxium.ps2.Character` that was killed.
 
     .. attribute:: character_loadout_id
        :type: int
@@ -161,14 +164,19 @@
           This value is always false.
 
     .. attribute:: is_headshot
        :type: bool
 
        Whether the killing blow was dealt via headshot.
 
+    .. attribute:: team_id
+       :type: int
+
+       Team ID of the victim.
+
     .. attribute:: vehicle_id
        :type: int | None
 
        The type of :class:`~auraxium.ps2.Vehicle` the victim was in at
        the time of death, if any.
 
     .. attribute:: zone_id
@@ -190,19 +198,21 @@
     """
 
     attacker_character_id: int
     attacker_fire_mode_id: int
     attacker_loadout_id: int
     attacker_vehicle_id: int
     attacker_weapon_id: int
+    attacker_team_id: int
     character_id: int
     character_loadout_id: int
-    is_critical: Optional[bool]  # Always false
+    is_critical: Optional[bool] = None  # Always false
     is_headshot: bool
-    vehicle_id: Optional[int]
+    team_id: int
+    vehicle_id: Optional[int] = None
     zone_id: int
 
 
 class FacilityControl(Event, WorldEvent):
     """A facility has switched factions.
 
     This is generally due to hostile takeover, but is also dispatched
@@ -652,14 +662,19 @@
        ID of the :class:`~auraxium.ps2.Item` used by the attacker.
 
        .. important::
 
          The reference above is not an error, this field reports the
          item ID of the weapon, not the weapon ID.
 
+    .. attribute:: attacker_team_id
+       :type: int
+
+       The ID of the team of the attacker
+
     .. attribute:: character_id
        :type: int
 
        ID of the :class:`~auraxium.ps2.Character` that was killed.
 
     .. attribute:: facility_id
        :type: int
@@ -673,14 +688,19 @@
           data.
 
     .. attribute:: faction_id
        :type: int
 
        The :class:`~auraxium.ps2.Faction` of the vehicle.
 
+    .. attribute:: team_id
+       :type: int
+
+       Team ID of the destroyed vehicle.
+
     .. attribute:: vehicle_id
        :type: int | None
 
        The type of :class:`~auraxium.ps2.Vehicle` that was destroyed.
 
     .. attribute:: zone_id
        :type: int
@@ -700,17 +720,19 @@
        endpoint broadcast the event.
     """
 
     attacker_character_id: int
     attacker_loadout_id: int
     attacker_vehicle_id: int
     attacker_weapon_id: int
+    attacker_team_id: int
     character_id: int
     facility_id: int
     faction_id: int
+    team_id: int
     vehicle_id: int
     zone_id: int
 
 
 class ContinentLock(Event, WorldEvent):
     """A continent has been locked.
```

### Comparing `auraxium-0.2.4/auraxium/models/_experience.py` & `auraxium-0.3.0/auraxium/models/_experience.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from ..types import LocaleData
 
 __all__ = [
     'ExperienceData',
     'ExperienceRankData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class ExperienceData(RESTPayload):
     """Data class for :class:`auraxium.ps2.Experience`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_faction.py` & `auraxium-0.3.0/auraxium/models/_profile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,32 @@
-"""Data classes for :mod:`auraxium.ps2._faction`."""
+"""Data classes for :mod:`auraxium.ps2._profile`."""
 
-from .base import ImageData, RESTPayload
-from ..types import LocaleData
+from .base import RESTPayload
 
 __all__ = [
-    'FactionData'
+    'LoadoutData',
+    'ProfileData'
 ]
 
-# pylint: disable=too-few-public-methods
 
-
-class FactionData(RESTPayload, ImageData):
-    """Data class for :class:`auraxium.ps2.Faction`.
+class LoadoutData(RESTPayload):
+    """Data class for :class:`auraxium.ps2.Loadout`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
 
+    loadout_id: int
+    profile_id: int
     faction_id: int
-    name: LocaleData
-    code_tag: str
-    user_selectable: bool
+    code_name: str
+
+
+class ProfileData(RESTPayload):
+    """Data class for :class:`auraxium.ps2.Profile`.
+
+    This class mirrors the payload data returned by the API, you may
+    use its attributes as keys in filters or queries.
+    """
+
+    profile_id: int
+    description: str
```

### Comparing `auraxium-0.2.4/auraxium/models/_fire.py` & `auraxium-0.3.0/auraxium/models/_fire.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from ..types import LocaleData
 
 __all__ = [
     'FireModeData',
     'FireGroupData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class FireModeData(RESTPayload):
     """Data class for :class:`auraxium.ps2.FireMode`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_item.py` & `auraxium-0.3.0/auraxium/models/_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 __all__ = [
     'ItemCategoryData',
     'ItemData',
     'ItemTypeData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class ItemCategoryData(RESTPayload):
     """Data class for :class:`auraxium.ps2.ItemCategory`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_map.py` & `auraxium-0.3.0/auraxium/models/_map.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 __all__ = [
     'FacilityTypeData',
     'MapHexData',
     'MapRegionData',
     'RegionData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class FacilityTypeData(RESTPayload):
     """Data class for :class:`auraxium.ps2.FacilityType`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_metagame.py` & `auraxium-0.3.0/auraxium/models/_metagame.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .base import RESTPayload
 from ..types import LocaleData
 
 __all__ = [
     'MetagameEventData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class MetagameEventData(RESTPayload):
     """Data class for :class:`auraxium.ps2.MetagameEvent`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_objective.py` & `auraxium-0.3.0/auraxium/models/_objective.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .base import RESTPayload
 
 __all__ = [
     'ObjectiveData',
     'ObjectiveTypeData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class ObjectiveData(RESTPayload):
     """Data class for :class:`auraxium.ps2.Objective`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_outfit.py` & `auraxium-0.3.0/auraxium/models/_outfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 __all__ = [
     'OutfitData',
     'OutfitMemberData',
     'OutfitRankData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class OutfitData(RESTPayload):
     """Data class for :class:`auraxium.ps2.Outfit`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_projectile.py` & `auraxium-0.3.0/auraxium/models/_projectile.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 from .base import RESTPayload
 
 __all__ = [
     'ProjectileData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class ProjectileData(RESTPayload):
     """Data class for :class:`auraxium.ps2.Projectile`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_resist.py` & `auraxium-0.3.0/auraxium/models/_resist.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .base import RESTPayload
 
 __all__ = [
     'ResistInfoData',
     'ResistTypeData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class ResistInfoData(RESTPayload):
     """Data class for :class:`auraxium.ps2.ResistInfo`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_reward.py` & `auraxium-0.3.0/auraxium/models/_reward.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .base import RESTPayload
 
 __all__ = [
     'RewardData',
     'RewardTypeData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class RewardData(RESTPayload):
     """Data class for :class:`auraxium.ps2.Reward`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_skill.py` & `auraxium-0.3.0/auraxium/models/_skill.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 __all__ = [
     'SkillData',
     'SkillCategoryData',
     'SkillLineData',
     'SkillSetData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class SkillData(RESTPayload, ImageData):
     """Data class for :class:`auraxium.ps2.Skill`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_states.py` & `auraxium-0.3.0/auraxium/models/_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 from .base import RESTPayload
 
 __all__ = [
     'PlayerStateGroup'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class PlayerStateGroup(RESTPayload):
     """A fire-mode-specific state group.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
```

### Comparing `auraxium-0.2.4/auraxium/models/_vehicle.py` & `auraxium-0.3.0/auraxium/models/_vehicle.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from ..types import LocaleData
 
 __all__ = [
     'VehicleAttachmentData',
     'VehicleData'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class VehicleAttachmentData(RESTPayload):
     """Data class for :class:`auraxium.ps2.VehicleAttachment`.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
     """
```

### Comparing `auraxium-0.2.4/auraxium/models/_weapon.py` & `auraxium-0.3.0/auraxium/models/_weapon.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 __all__ = [
     'WeaponAmmoSlot',
     'WeaponData',
     'WeaponDatasheet'
 ]
 
-# pylint: disable=too-few-public-methods
-
 
 class WeaponAmmoSlot(RESTPayload):
     """Data class for weapon ammo slot data.
 
     This class mirrors the payload data returned by the API, you may
     use its attributes as keys in filters or queries.
```

### Comparing `auraxium-0.2.4/auraxium/models/base.py` & `auraxium-0.3.0/auraxium/models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,53 @@
 """Shared base classes for API data model implementations."""
 
 import abc
 import datetime
-from typing import Any, Optional, TypeVar, cast
+from typing import Optional, TypeVar
 
 import pydantic
 
 from ..types import CensusData
 
-# pylint: disable=too-few-public-methods
-
 _T = TypeVar('_T')
 
 
-class Payload(pydantic.BaseModel):  # pylint: disable=no-member
+class Payload(pydantic.BaseModel):
     """A payload received through the REST or WebSocket interface.
 
     Instances of this class are read-only.
     """
 
-    class Config:
-        """Pydantic model configuration.
-
-        :meta private:
-        """
-
-        allow_mutation = False
-
-    # Weird workaround for pydantic.BaseModel overwriting __hash__ with
-    # None, at least according to Pylance.
-
-    def _override__hash__(self) -> int:  # pragma: no cover
-        # NOTE: pydantic has a beta setting called `frozen=True` that would
-        # generate a hash method, but it is not part of the stable API and
-        # therefore not used here.
-        # It should replace allow_mutation here once it out of beta.
-        return hash(tuple(self.dict().items()))
-
-    __hash__ = cast(Any, _override__hash__)
+    model_config = pydantic.ConfigDict(extra='ignore', frozen=True)
 
 
 class RESTPayload(Payload):
     """A JSON payload received through the REST interface.
 
     This :class:`Payload` subclass implicitly converts NULL strings to
     :obj:`None`.
     """
 
-    @pydantic.validator('*', pre=True)  # type: ignore
+    @pydantic.field_validator('*', mode='before')
     @classmethod
-    def _convert_null(cls, value: _T) -> Optional[_T]:
+    def _convert_null(cls, value: _T,
+                      info: pydantic.FieldValidationInfo,
+                      ) -> Optional[_T]:
         """Replace any "NULL" string inputs with :obj:`None`.
 
         This is a pre-validator; it is run before any other validation
         or conversion takes place.
 
         By default, the API will omit any NULL fields in the
         response unless the ``c:includeNull`` flag is set. In Python,
         a missing value is instead. This also ensures that optional
         values can be type-hinted with :obj:`typing.Optional` without
         risk of errors.
         """
-        _ = cls
+        _ = cls, info
         if value == 'NULL':
             return None
         return value
 
 
 class FallbackMixin(metaclass=abc.ABCMeta):
     """A mixin class used to provide hard-coded fallback instances.
@@ -93,15 +75,15 @@
         :raises KeyError: Raised if no fallback data can be provided
            for the given `id_`.
         :return: A fallback payload to treat as if it came from the
            server.
         """
 
 
-class ImageData(pydantic.BaseModel):  # pylint: disable=no-member
+class ImageData(pydantic.BaseModel):
     """Mixin dataclass for types supporting image access.
 
     .. attribute:: image_id
        :type: int | None
 
        The default image ID of the object.
 
@@ -146,18 +128,21 @@
        endpoint broadcast the event.
     """
 
     event_name: str
     timestamp: datetime.datetime
     world_id: int
 
-    @pydantic.validator('timestamp', pre=True)  # type: ignore
+    @pydantic.field_validator('timestamp', mode='before')
     @classmethod
-    def _utc_from_timestamp(cls, value: str) -> datetime.datetime:
+    def _utc_from_timestamp(cls, value: str,
+                            info: pydantic.FieldValidationInfo,
+                            ) -> datetime.datetime:
         """Convert timestamps to UTC datetimes."""
+        _ = info
         return datetime.datetime.utcfromtimestamp(int(value))
 
     @property
     def age(self) -> float:
         """The age of the event in seconds."""
         now = datetime.datetime.utcnow()
         return (now - self.timestamp).total_seconds()
```

### Comparing `auraxium-0.2.4/auraxium/ps2/__init__.py` & `auraxium-0.3.0/auraxium/ps2/__init__.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_ability.py` & `auraxium-0.3.0/auraxium/ps2/_ability.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_achievement.py` & `auraxium-0.3.0/auraxium/ps2/_achievement.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_armour.py` & `auraxium-0.3.0/auraxium/ps2/_armour.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_character.py` & `auraxium-0.3.0/auraxium/ps2/_character.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
                       endpoint=self._client.endpoints[0],
                       character_id=','.join(character_ids))
         payload = await self._client.request(query)
         data = extract_payload(payload, self.collection)
         return [Character(d, client=self._client) for d in data]
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')
     async def get_by_name(cls: Type[NamedT], name: str, *, locale: str = 'en',
                           client: RequestClient
                           ) -> Optional[NamedT]:  # pragma: no cover
         """Retrieve an object by its unique name.
 
         This query is always case-insensitive.
         """
```

### Comparing `auraxium-0.2.4/auraxium/ps2/_currency.py` & `auraxium-0.3.0/auraxium/ps2/_currency.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_depot.py` & `auraxium-0.3.0/auraxium/ps2/_depot.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_directive.py` & `auraxium-0.3.0/auraxium/ps2/_directive.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_effect.py` & `auraxium-0.3.0/auraxium/ps2/_effect.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_experience.py` & `auraxium-0.3.0/auraxium/ps2/_experience.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_faction.py` & `auraxium-0.3.0/auraxium/ps2/_faction.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_fire.py` & `auraxium-0.3.0/auraxium/ps2/_fire.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_item.py` & `auraxium-0.3.0/auraxium/ps2/_item.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_map.py` & `auraxium-0.3.0/auraxium/ps2/_map.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_metagame.py` & `auraxium-0.3.0/auraxium/ps2/_metagame.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_objective.py` & `auraxium-0.3.0/auraxium/ps2/_objective.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_outfit.py` & `auraxium-0.3.0/auraxium/ps2/_outfit.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
     @property
     def tag(self) -> str:
         """Alias of :attr:`alias`."""
         return self.alias
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')
     async def get_by_name(cls: Type[NamedT], name: str, *, locale: str = 'en',
                           client: RequestClient
                           ) -> Optional[NamedT]:  # pragma: no cover
         """Retrieve an outfit by its unique name.
 
         This query is always case-insensitive.
         """
@@ -194,15 +194,15 @@
         try:
             payload = extract_single(data, cls.collection)
         except NotFoundError:
             return None
         return cls(payload, client=client)
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')
     async def get_by_tag(cls, tag: str, client: RequestClient
                          ) -> Optional['Outfit']:  # pragma: no cover
         """Return an outfit by its unique tag.
 
         This query is always case-insensitive.
         """
         log.debug('%s with tag "%s" requested, generating API query...',
```

### Comparing `auraxium-0.2.4/auraxium/ps2/_profile.py` & `auraxium-0.3.0/auraxium/ps2/_profile.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_projectile.py` & `auraxium-0.3.0/auraxium/ps2/_projectile.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_resist.py` & `auraxium-0.3.0/auraxium/ps2/_resist.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_reward.py` & `auraxium-0.3.0/auraxium/ps2/_reward.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_skill.py` & `auraxium-0.3.0/auraxium/ps2/_skill.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_states.py` & `auraxium-0.3.0/auraxium/ps2/_states.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_vehicle.py` & `auraxium-0.3.0/auraxium/ps2/_vehicle.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/_weapon.py` & `auraxium-0.3.0/auraxium/ps2/_weapon.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         query.add_term(field=self.id_field, value=self.id)
         query.limit(20)
         join = query.create_join(FireGroup.collection)
         join.set_fields(FireGroup.id_field)
         return SequenceProxy(FireGroup, query, client=self._client)
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')
     async def get_by_name(cls, name: str, *, locale: str = 'en',
                           client: RequestClient
                           ) -> Optional['Weapon']:  # pragma: no cover
         """Retrieve a weapon by name.
 
         This is a helper method provided as weapons themselves do not
         have a name. This looks up an item by name, then returns the
```

### Comparing `auraxium-0.2.4/auraxium/ps2/_world.py` & `auraxium-0.3.0/auraxium/ps2/_world.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         query.add_term(field=self.id_field, value=self.id)
         query.limit(1000)
         payload = await self._client.request(query)
         data = extract_payload(payload, collection=collection)
         return data
 
     @classmethod
-    @deprecated('0.2', '0.3', replacement=':meth:`auraxium.Client.get`')
+    @deprecated('0.2', '0.4', replacement=':meth:`auraxium.Client.get`')
     async def get_by_name(cls: Type[NamedT], name: str, *, locale: str = 'en',
                           client: RequestClient
                           ) -> Optional[NamedT]:  # pragma: no cover
         """Retrieve a world by name.
 
         This query is always case-insensitive.
         """
```

### Comparing `auraxium-0.2.4/auraxium/ps2/_zone.py` & `auraxium-0.3.0/auraxium/ps2/_zone.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/ps2/leaderboard.py` & `auraxium-0.3.0/auraxium/ps2/leaderboard.py`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/auraxium/types.py` & `auraxium-0.3.0/auraxium/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,22 @@
     'LocaleData'
 ]
 
 CensusData = Dict[
     str, Union[str, int, float, 'CensusData', List['CensusData']]]
 
 
-class LocaleData(pydantic.BaseModel):  # pylint: disable=no-member
+class LocaleData(pydantic.BaseModel):
     """Container for localised strings.
 
     Note that the ``tr`` locale is ignored as it was abandoned by the
     developers and is generally either missing or unpopulated.
     """
-    # pylint: disable=too-few-public-methods
 
-    class Config:
-        """Pydantic model configuration.
-
-        This inner class is used to namespace the pydantic
-        configuration options.
-        """
-        allow_mutation = False
+    model_config = pydantic.ConfigDict(extra='ignore', frozen=True)
 
     de: Optional[str] = None
     en: Optional[str] = None
     es: Optional[str] = None
     fr: Optional[str] = None
     it: Optional[str] = None
```

### Comparing `auraxium-0.2.4/auraxium.egg-info/PKG-INFO` & `auraxium-0.3.0/auraxium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auraxium
-Version: 0.2.4
+Version: 0.3.0
 Summary: A python wrapper for the PlanetSide 2 Census API.
 Home-page: https://github.com/leonhard-s/auraxium
 Author: Leonhard S.
 Author-email: leonhard-sei@outlook.com
 License: MIT
 Keywords: auraxium python daybreak census planetside ps2
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,18 +18,18 @@
 
 # <img src="https://raw.githubusercontent.com/leonhard-s/auraxium/master/assets/icon_256.png" align="left" height="140"/>Auraxium
 
 Auraxium is an object-oriented, pure-Python wrapper for the [PlanetSide 2](https://www.planetside2.com/) API.  
 It provides a simple object model that can be used by players and outfits without requiring deep knowledge of the API and its idiosyncrasies.
 
 ![PyPI - License](https://img.shields.io/pypi/l/auraxium)
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/pythonunittest.yml?label=tests)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/ci-testing.yaml?label=tests)
 [![Coveralls github branch](https://img.shields.io/coveralls/github/leonhard-s/auraxium/master)](https://coveralls.io/github/leonhard-s/auraxium)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/auraxium)
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/pythonpublish.yml)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/leonhard-s/auraxium/publish-package.yaml)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/leonhard-s/auraxium)](https://www.codefactor.io/repository/github/leonhard-s/auraxium)
 [![PyPI](https://img.shields.io/pypi/v/auraxium)](https://pypi.org/project/auraxium/)
 [![Read the Docs](https://img.shields.io/readthedocs/auraxium)](https://auraxium.readthedocs.io/en/latest/)
 
 ***
 
 - Clean, Pythonic API
@@ -173,15 +173,15 @@
 
 This is useful if you have a commonly encountered event (like [`event.DEATH`](https://auraxium.readthedocs.io/en/latest/api/event.html#auraxium.event.DEATH)) and would like your action to only run if the event data matches some other requirement (for example "the killing player must be part of my outfit").
 
 #### Actions
 
 The trigger's action is a method or function that will be run when the event fires and all conditions evaluate to True.
 
-If the action is a coroutine according to [`asyncio.iscoroutinefunction()`](https://docs.python.org/3/library/asyncio-task.html#asyncio.iscoroutinefunction), it will be awaited.
+If the action is a coroutine according to [`inspect.iscoroutinefunction()`](https://docs.python.org/3/library/inspect.html#inspect.iscoroutinefunction), it will be awaited.
 
 The only argument passed to the function set as the trigger action is the event received:
 
 ```py
 async def example_action(event: Event) -> None:
     """Example function to showcase the signature used for actions.
```

### Comparing `auraxium-0.2.4/auraxium.egg-info/SOURCES.txt` & `auraxium-0.3.0/auraxium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auraxium-0.2.4/setup.py` & `auraxium-0.3.0/setup.py`

 * *Files identical despite different names*

