# Comparing `tmp/dj_beatcloud-2.5.1b5.tar.gz` & `tmp/dj_beatcloud-2.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.5.1b5.tar", last modified: Thu Jun  8 15:18:58 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.6.0b0.tar", last modified: Sat Jul 15 20:44:14 2023, max compression
```

## Comparing `dj_beatcloud-2.5.1b5.tar` & `dj_beatcloud-2.6.0b0.tar`

### file list

```diff
@@ -1,73 +1,55 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.838005 dj_beatcloud-2.5.1b5/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b5/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.5.1b5/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-08 15:18:58.838113 dj_beatcloud-2.5.1b5/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.5.1b5/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.823467 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1853 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.824475 dj_beatcloud-2.5.1b5/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2495 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b5/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.827400 dj_beatcloud-2.5.1b5/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3691 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1214 2023-06-08 15:18:00.000000 dj_beatcloud-2.5.1b5/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13601 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)     1028 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-26 18:48:19.000000 dj_beatcloud-2.5.1b5/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4790 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.827637 dj_beatcloud-2.5.1b5/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.831062 dj_beatcloud-2.5.1b5/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1726 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6989 2023-06-08 15:09:39.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    21533 2023-06-08 14:34:28.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/playlist_combiner.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3483 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6848 2023-06-08 15:14:05.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5326 2023-06-08 14:59:58.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.833481 dj_beatcloud-2.5.1b5/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2288 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.835711 dj_beatcloud-2.5.1b5/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b5/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      669 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.837839 dj_beatcloud-2.5.1b5/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-06-08 15:18:27.000000 dj_beatcloud-2.5.1b5/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b5/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-06-08 15:18:58.838456 dj_beatcloud-2.5.1b5/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2425 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.137101 dj_beatcloud-2.6.0b0/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b0/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b0/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-15 20:44:14.137210 dj_beatcloud-2.6.0b0/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b0/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.130185 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1248 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.130675 dj_beatcloud-2.6.0b0/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2543 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1776 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.132313 dj_beatcloud-2.6.0b0/djtools/collections/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1434 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12878 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2408 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2515 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27150 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7584 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15833 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2405 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13832 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.133861 dj_beatcloud-2.6.0b0/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     3758 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1301 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13868 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.134013 dj_beatcloud-2.6.0b0/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.134604 dj_beatcloud-2.6.0b0/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.135287 dj_beatcloud-2.6.0b0/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3435 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7959 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4888 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.136769 dj_beatcloud-2.6.0b0/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b0/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b0/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b0/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-15 20:43:27.000000 dj_beatcloud-2.6.0b0/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b0/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-15 20:44:14.137549 dj_beatcloud-2.6.0b0/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2371 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/setup.py
```

### Comparing `dj_beatcloud-2.5.1b5/LICENSE` & `dj_beatcloud-2.6.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b5/PKG-INFO` & `dj_beatcloud-2.6.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.5.1b5
-Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
+Version: 2.6.0b0
+Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
-Keywords: MP3 Rekordbox XML spotify reddit aws s3
+Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b5 Summary: DJ Tools is
-a library for managing a collection of music and Rekordbox XML files. Home-
-page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
-alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
-spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: End Users/
-Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
-OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
-Language :: English Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
-System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Other/Nonlisted Topic Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: levenshtein License-File: LICENSE #
-DJ Tools [![image](https://img.shields.io/pypi/v/dj-beatcloud.svg)](https://
-pypi.org/project/dj-beatcloud/) Please see the [docs](https://a-rich.github.io/
-DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references! #
-Release Plan * 2.5.1 - [ ] [Stability issues with requests to the search
-endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58) -
-[ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/
-issues/38) - [ ] [Print ASCII histogram of tag statistics for Combiner
-playlists](https://github.com/a-rich/DJ-Tools/issues/87) - [x] [Deprecate
-registered_users.yaml](https://github.com/a-rich/DJ-Tools/issues/99) - [x]
-[Parameterize whether Beatcloud tracks should be read as
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b0 Summary: DJ Tools is
+a library for managing a collection of music. Home-page: https://github.com/a-
+rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
+License: GNU GPLv3 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
+Audience :: Other Audience Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Multimedia :: Sound/Audio Classifier: Topic :: Other/Nonlisted Topic
+Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
+levenshtein License-File: LICENSE # DJ Tools [![image](https://img.shields.io/
+pypi/v/dj-beatcloud.svg)](https://pypi.org/project/dj-beatcloud/) Please see
+the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides,
+conceptual guides, and references! # Release Plan * 2.5.1 - [ ] [Stability
+issues with requests to the search endpoint of the Spotify API](https://
+github.com/a-rich/DJ-Tools/issues/58) - [ ] [Make Spotify API calls
+asynchronous](https://github.com/a-rich/DJ-Tools/issues/38) - [ ] [Print ASCII
+histogram of tag statistics for Combiner playlists](https://github.com/a-rich/
+DJ-Tools/issues/87) - [x] [Deprecate registered_users.yaml](https://github.com/
+a-rich/DJ-Tools/issues/99) - [x] [Parameterize whether Beatcloud tracks should
+be read as
  or vice versa](https://github.com/a-rich/DJ-Tools/issues/95) * 2.6.0 - [ ]
 [Create serializers package for converting database files from other DJ
 software (e.g. Serato, Traktor, Denon, etc.) so that operations in the
 rekordbox package can be used on them](https://github.com/a-rich/DJ-Tools/
 issues/68) - [ ] [Improve Reddit submission title parsing in order to improve
 precision and recall of Spotify API search results](https://github.com/a-rich/
 DJ-Tools/issues/59) # Contribution Please see the [CONTRIBUTING]
```

### Comparing `dj_beatcloud-2.5.1b5/README.md` & `dj_beatcloud-2.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.5.1b5
-Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
+Version: 2.6.0b0
+Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
-Keywords: MP3 Rekordbox XML spotify reddit aws s3
+Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b5 Summary: DJ Tools is
-a library for managing a collection of music and Rekordbox XML files. Home-
-page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
-alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
-spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: End Users/
-Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
-OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
-Language :: English Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
-System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Other/Nonlisted Topic Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: levenshtein License-File: LICENSE #
-DJ Tools [![image](https://img.shields.io/pypi/v/dj-beatcloud.svg)](https://
-pypi.org/project/dj-beatcloud/) Please see the [docs](https://a-rich.github.io/
-DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references! #
-Release Plan * 2.5.1 - [ ] [Stability issues with requests to the search
-endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58) -
-[ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/
-issues/38) - [ ] [Print ASCII histogram of tag statistics for Combiner
-playlists](https://github.com/a-rich/DJ-Tools/issues/87) - [x] [Deprecate
-registered_users.yaml](https://github.com/a-rich/DJ-Tools/issues/99) - [x]
-[Parameterize whether Beatcloud tracks should be read as
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b0 Summary: DJ Tools is
+a library for managing a collection of music. Home-page: https://github.com/a-
+rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
+License: GNU GPLv3 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
+Audience :: Other Audience Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Multimedia :: Sound/Audio Classifier: Topic :: Other/Nonlisted Topic
+Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
+levenshtein License-File: LICENSE # DJ Tools [![image](https://img.shields.io/
+pypi/v/dj-beatcloud.svg)](https://pypi.org/project/dj-beatcloud/) Please see
+the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides,
+conceptual guides, and references! # Release Plan * 2.5.1 - [ ] [Stability
+issues with requests to the search endpoint of the Spotify API](https://
+github.com/a-rich/DJ-Tools/issues/58) - [ ] [Make Spotify API calls
+asynchronous](https://github.com/a-rich/DJ-Tools/issues/38) - [ ] [Print ASCII
+histogram of tag statistics for Combiner playlists](https://github.com/a-rich/
+DJ-Tools/issues/87) - [x] [Deprecate registered_users.yaml](https://github.com/
+a-rich/DJ-Tools/issues/99) - [x] [Parameterize whether Beatcloud tracks should
+be read as
  or vice versa](https://github.com/a-rich/DJ-Tools/issues/95) * 2.6.0 - [ ]
 [Create serializers package for converting database files from other DJ
 software (e.g. Serato, Traktor, Denon, etc.) so that operations in the
 rekordbox package can be used on them](https://github.com/a-rich/DJ-Tools/
 issues/68) - [ ] [Improve Reddit submission title parsing in order to improve
 precision and recall of Spotify API search results](https://github.com/a-rich/
 DJ-Tools/issues/59) # Contribution Please see the [CONTRIBUTING]
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/__init__.py` & `dj_beatcloud-2.6.0b0/djtools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,85 +5,85 @@
 instantiated. The optional C extension to accelerate edit distance computation,
 Levenshtein, is imported. The loop iterates all the supported top-level
 operations of the library and calls the corresponding function with the
 appropriate configuration object. Finally, the log file generated from this run
 is uploaded to the Beatcloud.
 """
 from .configs import build_config
-from .rekordbox import (
-    build_playlists,
+from .collections import (
+    COLLECTION_OPERATIONS,
+    collection_playlists,
     copy_playlists,
-    REKORDBOX_OPERATIONS,
     shuffle_playlists,
 )
 from .spotify import (
-    playlist_from_upload,
+    spotify_playlist_from_upload,
     SPOTIFY_OPERATIONS,
-    update_auto_playlists,
+    spotify_playlists,
 )
 from .sync import (
+    download_collection,
     download_music,
-    download_xml,
     SYNC_OPERATIONS,
+    upload_collection,
     upload_log,
     upload_music,
-    upload_xml,
 )
 from .utils import (
     compare_tracks,
     initialize_logger,
     UTILS_OPERATIONS,
     url_download,
 )
 from .version import __version__
 
 
 __all__ = (
     "build_config",
-    "build_playlists",
+    "COLLECTION_OPERATIONS",
+    "collection_playlists",
     "compare_tracks",
     "copy_playlists",
+    "download_collection",
     "download_music",
-    "download_xml",
     "initialize_logger",
-    "playlist_from_upload",
-    "REKORDBOX_OPERATIONS",
     "shuffle_playlists",
+    "spotify_playlist_from_upload",
+    "spotify_playlists",
     "SPOTIFY_OPERATIONS",
     "SYNC_OPERATIONS",
-    "update_auto_playlists",
     "upload_log",
+    "upload_collection",
     "upload_music",
-    "upload_xml",
     "UTILS_OPERATIONS",
     "url_download",
 )
 
 
 def main():
     """This is the entry point for the DJ Tools library."""
 
     logger, log_file = initialize_logger()
     config = build_config()
     logger.setLevel(config.LOG_LEVEL)
 
-    # Run "rekordbox", "spotify", "sync", and "utils" package operations if any
-    # of the flags to do so are present in the config.
+    # Run "collections", "spotify", "sync", and "utils" package operations if
+    # any of the flags to do so are present in the config.
     beatcloud_cache = []
     for package in [
-        REKORDBOX_OPERATIONS,
+        COLLECTION_OPERATIONS,
         SPOTIFY_OPERATIONS,
         UTILS_OPERATIONS,
         SYNC_OPERATIONS,
     ]:
         for operation, func in package.items():
             if not getattr(config, operation):
                 continue
             logger.info(f"{operation}")
             if operation in ["CHECK_TRACKS", "DOWNLOAD_MUSIC"]:
-                beatcloud_cache = func(  # pylint: disable=assignment-from-no-return,unexpected-keyword-arg
+                beatcloud_cache = func(  # pylint: disable=assignment-from-none,unexpected-keyword-arg
                     config, beatcloud_tracks=beatcloud_cache
                 )
             else:
                 func(config)
 
     upload_log(config, log_file)
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/configs/config.yaml` & `dj_beatcloud-2.6.0b0/djtools/configs/config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,50 @@
+collections:
+  COLLECTION_PLAYLISTS: false
+  COLLECTION_PLAYLISTS_REMAINDER: folder
+  COPY_PLAYLISTS: []
+  COPY_PLAYLISTS_DESTINATION: null
+  PLATFORM: rekordbox
+  SHUFFLE_PLAYLISTS: []
 configs:
   AWS_PROFILE: default
+  COLLECTION_PATH: null
   LOG_LEVEL: INFO
   VERBOSITY: 0
-  XML_PATH: null
-rekordbox:
-  BUILD_PLAYLISTS: false
-  BUILD_PLAYLISTS_REMAINDER: folder
-  COPY_PLAYLISTS: []
-  COPY_PLAYLISTS_DESTINATION: null
-  SHUFFLE_PLAYLISTS: []
 spotify:
-  AUTO_PLAYLIST_DEFAULT_LIMIT: 50
-  AUTO_PLAYLIST_DEFAULT_PERIOD: week
-  AUTO_PLAYLIST_DEFAULT_TYPE: hot
-  AUTO_PLAYLIST_FUZZ_RATIO: 70
-  AUTO_PLAYLIST_POST_LIMIT: 100
-  AUTO_PLAYLIST_SUBREDDITS: []
-  AUTO_PLAYLIST_UPDATE: false
-  PLAYLIST_FROM_UPLOAD: false
   REDDIT_CLIENT_ID: ''
   REDDIT_CLIENT_SECRET: ''
   REDDIT_USER_AGENT: ''
   SPOTIFY_CLIENT_ID: ''
   SPOTIFY_CLIENT_SECRET: ''
+  SPOTIFY_PLAYLISTS: false
+  SPOTIFY_PLAYLIST_DEFAULT_LIMIT: 50
+  SPOTIFY_PLAYLIST_DEFAULT_PERIOD: week
+  SPOTIFY_PLAYLIST_DEFAULT_TYPE: hot
+  SPOTIFY_PLAYLIST_FROM_UPLOAD: false
+  SPOTIFY_PLAYLIST_FUZZ_RATIO: 70
+  SPOTIFY_PLAYLIST_POST_LIMIT: 100
+  SPOTIFY_PLAYLIST_SUBREDDITS: []
   SPOTIFY_REDIRECT_URI: ''
   SPOTIFY_USERNAME: ''
 sync:
   ARTIST_FIRST: false
   AWS_USE_DATE_MODIFIED: false
   DISCORD_URL: ''
+  DOWNLOAD_COLLECTION: false
   DOWNLOAD_EXCLUDE_DIRS: []
   DOWNLOAD_INCLUDE_DIRS: []
   DOWNLOAD_MUSIC: false
-  DOWNLOAD_SPOTIFY: ''
-  DOWNLOAD_XML: false
+  DOWNLOAD_SPOTIFY_PLAYLIST: ''
   DRYRUN: false
   IMPORT_USER: ''
+  UPLOAD_COLLECTION: false
   UPLOAD_EXCLUDE_DIRS: []
   UPLOAD_INCLUDE_DIRS: []
   UPLOAD_MUSIC: false
-  UPLOAD_XML: false
   USB_PATH: null
   USER: ''
 utils:
   CHECK_TRACKS: false
   CHECK_TRACKS_FUZZ_RATIO: 80
   CHECK_TRACKS_LOCAL_DIRS: []
   CHECK_TRACKS_SPOTIFY_PLAYLISTS: []
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/configs/helpers.py` & `dj_beatcloud-2.6.0b0/djtools/configs/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 import logging
 from pathlib import Path
 import sys
 from typing import Any, Dict, List, Union
 
 import yaml
 
+from djtools.collections.config import CollectionConfig
 from djtools.configs.config import BaseConfig
-from djtools.rekordbox.config import RekordboxConfig
 from djtools.spotify.config import SpotifyConfig
 from djtools.sync.config import SyncConfig
 from djtools.utils.config import UtilsConfig
 from djtools.version import __version__
 
 
 logger = logging.getLogger(__name__)
 
 pkg_cfg = {
+    "collections": CollectionConfig,
     "configs": BaseConfig,
-    "rekordbox": RekordboxConfig,
     "spotify": SpotifyConfig,
     "sync": SyncConfig,
     "utils": UtilsConfig,
 }
 
 
 def arg_parse() -> argparse.Namespace:
@@ -45,80 +45,28 @@
         action="store_true",
         help=(
             "Indicate that Beatcloud tracks are in the format "
             "`Artist - Track Title` instead of `Track Title - Artist`"
         ),
     )
     parser.add_argument(
-        "--auto-playlist-default-limit",
-        type=int,
-        help="Default number of tracks for a Spotify auto-playlist",
-    )
-    parser.add_argument(
-        "--auto-playlist-default-period",
-        type=str,
-        help="Default Subreddit time filter for a Spotify auto-playlist",
-    )
-    parser.add_argument(
-        "--auto-playlist-default-type",
-        type=str,
-        help="Default Subreddit post filter for a Spotify auto-playlist",
-    )
-    parser.add_argument(
-        "--auto-playlist-fuzz-ratio",
-        type=int,
-        help="Minimum similarity to add track to an auto-playlist",
-    )
-    parser.add_argument(
-        "--auto-playlist-post-limit",
-        type=int,
-        help="Maximum Subreddit posts to query for each auto-playlist",
-    )
-    parser.add_argument(
-        "--auto-playlist-subreddits",
-        type=parse_yaml,
-        help=(
-            "List of Subreddits configs to generate playlists from; YAML "
-            'strings with "name", "type", "period", and "limit" keys'
-        ),
-    )
-    parser.add_argument(
-        "--auto-playlist-update",
-        action="store_true",
-        help="Trigger updating auto-playlists",
-    )
-    parser.add_argument(
         "--aws-profile",
         type=str,
         help="AWS config profile",
     )
     parser.add_argument(
         "--aws-use-date-modified",
         action="store_true",
         help=(
             'Drop --size-only flag for "aws s3 sync" command; '
             '"--aws-use-date-modified" will permit re-downloading/'
             "re-uploading files if the date modified field changes"
         ),
     )
     parser.add_argument(
-        "--build-playlists",
-        action="store_true",
-        help="Trigger automatic Rekordbox playlist creation",
-    )
-    parser.add_argument(
-        "--build-playlists-remainder",
-        type=str,
-        choices=["folder", "playlist"],
-        help=(
-            'Place remainder tracks in either an "Other" folder of playlists '
-            'or a single "Other" playlist'
-        ),
-    )
-    parser.add_argument(
         "--check-tracks",
         action="store_true",
         help=(
             "Trigger checking for track overlap between the Beatcloud and"
             "CHECK_TRACKS_LOCAL_DIRS and / or CHECK_TRACKS_SPOTIFY_PLAYLISTS"
         ),
     )
@@ -139,30 +87,57 @@
     parser.add_argument(
         "--check-tracks-spotify-playlists",
         type=str,
         nargs="+",
         help="List of Spotify playlist names to check against the Beatcloud",
     )
     parser.add_argument(
+        "--collection-path",
+        type=convert_to_paths,
+        help='Path to a collection database',
+    )
+    parser.add_argument(
+        "--collection-playlists",
+        action="store_true",
+        help="Trigger building collection playlists",
+    )
+    parser.add_argument(
+        "--collection-playlists-remainder",
+        type=str,
+        choices=["folder", "playlist"],
+        help=(
+            'Place remainder tracks in either an "Other" folder of playlists '
+            'or a single "Other" playlist'
+        ),
+    )
+    parser.add_argument(
         "--copy-playlists",
         type=str,
         nargs="+",
-        help="List of Rekordbox playlists to copy audio files from",
+        help="List of playlists to copy audio files from",
     )
     parser.add_argument(
         "--copy-playlists-destination",
         type=convert_to_paths,
-        help="Location to copy Rekordbox playlists' audio files to",
+        help="Location to copy playlists' audio files to",
     )
     parser.add_argument(
         "--discord-url",
         type=str,
         help="Discord webhook URL",
     )
     parser.add_argument(
+        "--download-collection",
+        action="store_true",
+        help=(
+            "Trigger downloading the collection of IMPORT_USER from the "
+            "Beatcloud"
+        ),
+    )
+    parser.add_argument(
         "--download-exclude-dirs",
         type=convert_to_paths,
         nargs="+",
         help="Paths to exclude when downloading from the Beatcloud",
     )
     parser.add_argument(
         "--download-include-dirs",
@@ -172,50 +147,43 @@
     )
     parser.add_argument(
         "--download-music",
         action="store_true",
         help="Trigger downloading new tracks from the Beatcloud",
     )
     parser.add_argument(
-        "--download-spotify",
+        "--download-spotify-playlist",
         type=str,
         help="Playlist name containing tracks to download from the Beatcloud",
     )
     parser.add_argument(
-        "--download-xml",
-        action="store_true",
-        help="Trigger downloading the XML of IMPORT_USER from the Beatcloud",
-    )
-    parser.add_argument(
         "--dryrun",
         action="store_true",
         help='Show result of "aws s3 sync" command without running it',
     )
     parser.add_argument(
         "--import-user",
         type=str,
-        help="USER whose XML_PATH you're downloading",
+        help="USER whose COLLECTION_PATH you're downloading",
     )
     parser.add_argument(
         "--link-configs",
         type=convert_to_paths,
         help="Location to symlink library configuration files to",
     )
     parser.add_argument(
         "--log-level",
         choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
         help="Logger level",
     )
     parser.add_argument(
-        "--playlist-from-upload",
-        action="store_true",
-        help=(
-            "Trigger creating a Spotify playlist using the Discord webhook "
-            "output of a music upload"
-        ),
+        "--platform",
+        type=str,
+        choices=["rekordbox"],
+        help="DJ platform to use for the collections package",
     )
     parser.add_argument(
         "--reddit-client-id",
         type=str,
         help="Reddit API client ID",
     )
     parser.add_argument(
@@ -228,35 +196,89 @@
         type=str,
         help="Reddit API user agent",
     )
     parser.add_argument(
         "--shuffle-playlists",
         type=str,
         nargs="+",
-        help="List of Rekordbox playlist names to randomize tracks in",
+        help="List of playlist names to randomize tracks in",
     )
     parser.add_argument(
         "--spotify-client-id",
         type=str,
         help="Spotify API client ID",
     )
     parser.add_argument(
         "--spotify-client-secret",
         type=str,
         help="Spotify API client secret",
     )
     parser.add_argument(
+        "--spotify-playlist-default-limit",
+        type=int,
+        help="Default number of tracks for a Spotify playlist",
+    )
+    parser.add_argument(
+        "--spotify-playlist-default-period",
+        type=str,
+        help="Default Subreddit time filter for a Spotify playlist",
+    )
+    parser.add_argument(
+        "--spotify-playlist-default-type",
+        type=str,
+        help="Default Subreddit post filter for a Spotify playlist",
+    )
+    parser.add_argument(
+        "--spotify-playlist-from-upload",
+        action="store_true",
+        help=(
+            "Trigger creating a Spotify playlist using the Discord webhook "
+            "output of a music upload"
+        ),
+    )
+    parser.add_argument(
+        "--spotify-playlist-fuzz-ratio",
+        type=int,
+        help="Minimum similarity to add track to a playlist",
+    )
+    parser.add_argument(
+        "--spotify-playlist-post-limit",
+        type=int,
+        help="Maximum Subreddit posts to query for each playlist",
+    )
+    parser.add_argument(
+        "--spotify-playlist-subreddits",
+        type=parse_yaml,
+        help=(
+            "List of Subreddits configs to generate playlists from; YAML "
+            'strings with "name", "type", "period", and "limit" keys'
+        ),
+    )
+    parser.add_argument(
+        "--spotify-playlists",
+        action="store_true",
+        help="Trigger building Spotify playlists",
+    )
+    parser.add_argument(
         "--spotify-redirect-uri",
         type=str,
         help="Spotify API redirect URI",
     )
     parser.add_argument(
         "--spotify-username",
         type=str,
-        help="Spotify user to maintain auto-playlists for",
+        help="Spotify user to maintain playlists for",
+    )
+    parser.add_argument(
+        "--upload-collection",
+        action="store_true",
+        help=(
+            "Trigger uploading the collection of IMPORT_USER from the "
+            "Beatcloud"
+        ),
     )
     parser.add_argument(
         "--upload-exclude-dirs",
         type=convert_to_paths,
         nargs="+",
         help="List of paths to exclude when uploading to the Beatcloud",
     )
@@ -268,19 +290,14 @@
     )
     parser.add_argument(
         "--upload-music",
         action="store_true",
         help="Trigger uploading new tracks from the Beatcloud",
     )
     parser.add_argument(
-        "--upload-xml",
-        action="store_true",
-        help="Trigger uploading the XML of IMPORT_USER from the Beatcloud",
-    )
-    parser.add_argument(
         "--url-download",
         type=str,
         help="URL to download audio file(s) from",
     )
     parser.add_argument(
         "--url-download-destination",
         type=convert_to_paths,
@@ -304,19 +321,14 @@
         help="Logging verbosity",
     )
     parser.add_argument(
         "--version",
         action="store_true",
         help="Display package version",
     )
-    parser.add_argument(
-        "--xml-path",
-        type=convert_to_paths,
-        help='Path to your exported Rekordbox XML database',
-    )
     args = parser.parse_args()
 
     if args.log_level:
         logger.setLevel(args.log_level)
 
     if args.version:
         print(__version__)
@@ -423,15 +435,17 @@
     if isinstance(paths, List):
         return list(map(Path, paths))
 
     return Path(paths)
 
 
 def filter_dict(
-    sub_config: Union[RekordboxConfig, SpotifyConfig, SyncConfig, UtilsConfig],
+    sub_config: Union[
+        CollectionConfig, SpotifyConfig, SyncConfig, UtilsConfig
+    ],
 ) -> Dict[Any, Any]:
     """Filters out the superclass key: value pairs of a subclass.
 
     Args:
         sub_config: Instance of any subclass of BaseConfig.
 
     Returns:
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.6.0b0/djtools/configs/collection_playlists.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-Combiner:
+combiner:
   name: Combinations
   playlists:
     - "(Dubstep | Hip Hop) | (Dubstep | Hip Hop)"
     - "{Hip Hop} & [85-87]"
     - "{Hip Hop} & [86]"
     - Dark & [2-5]
     - Dark & [5]
-MyTagParser:
-  name: My Tags
+tags:
+  name: "Tags"
   playlists:
     - name: _ignore
       playlists:
+        - Psychedelic Rock
+        - Soul
         - Vocal
         - Wave
-    - Dark
-    - Uplifting 
-GenreTagParser:
-  name: Genres
-  playlists:
-    - name: _ignore
+    - name: My Tags
       playlists:
-        - Psychedelic Rock
-        - Soul
-    - name: Bass
+        - Dark
+        - Uplifting 
+    - name: Genres
       playlists:
-        - name: Breaks
-          playlists:
-            - Breakstep
-            - Neurobreaks
-        - name: Hip Hop Beats
+        - name: Bass
           playlists:
-            - Halftime
-            - Hip Hop
-        - Space Bass
-        - name: "[___] Step"
+            - name: Breaks
+              playlists:
+                - Breakstep
+                - Neurobreaks
+            - name: Hip Hop Beats
+              playlists:
+                - Halftime
+                - Hip Hop
+                - Pure Halftime
+            - Space Bass
+            - name: "[___] Step"
+              playlists:
+                - Breakstep
+                - Dubstep
+                - Pure Dubstep
+        - Hip Hop
+        - Pure Hip Hop
+        - name: House
           playlists:
-            - Breakstep
-            - Dubstep
-            - Pure Dubstep
-    - Hip Hop
-    - name: House
-      playlists:
-        - Minimal Deep Tech
-    - name: Techno
-      playlists:
-        - Hard Techno
-        - name: Other Techno
+            - Minimal Deep Tech
+        - name: Techno
           playlists:
-            - Minimal Deep Tech
+            - Hard Techno
+            - name: Other Techno
+              playlists:
+                - Minimal Deep Tech
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/rekordbox/config.py` & `dj_beatcloud-2.6.0b0/djtools/collections/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,71 @@
-"""This module contains the configuration object for the rekordbox package.
-The attributes of this configuration object correspond with the "rekordbox" key
-of config.yaml
+"""This module contains the configuration objects for the collection package.
+The attributes of this configuration object correspond with the "collections"
+key of config.yaml
 """
+from __future__ import annotations
 import logging
 from pathlib import Path
-from typing import List
+from typing import List, Optional, Union
+from typing_extensions import Literal
+
+from pydantic import BaseModel, Extra
 
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
-class RekordboxConfig(BaseConfig):
-    """Configuration object for the rekordbox package."""
+class CollectionConfig(BaseConfig):
+    """Configuration object for the collections package."""
 
-    BUILD_PLAYLISTS: bool = False
-    BUILD_PLAYLISTS_REMAINDER: str = "folder"
+    COLLECTION_PLAYLISTS: bool = False
+    COLLECTION_PLAYLISTS_REMAINDER: Literal["folder", "playlist"] = "folder"
     COPY_PLAYLISTS:  List[str] = []
     COPY_PLAYLISTS_DESTINATION: Path = None
+    PLATFORM: Literal["rekordbox"] = "rekordbox"
     SHUFFLE_PLAYLISTS:  List[str] = []
 
     def __init__(self, *args, **kwargs):
         """Constructor.
         
         Raises:
-            RuntimeError: XML_PATH must be a valid rekordbox XML file.
-            RuntimeError: rekordbox_playlists.yaml must be a valid YAML file.
+            RuntimeError: COLLECTION_PATH must be a valid collection path.
+            RuntimeError: collection_playlists.yaml must be a valid YAML file.
         """
         super().__init__(*args, **kwargs)
 
         if any(
             [
-                self.BUILD_PLAYLISTS,
+                self.COLLECTION_PLAYLISTS,
                 self.COPY_PLAYLISTS,
                 self.SHUFFLE_PLAYLISTS,
             ]
-        ) and (not self.XML_PATH or not self.XML_PATH.exists()):
+        ) and (not self.COLLECTION_PATH or not self.COLLECTION_PATH.exists()):
             raise RuntimeError(
-                "Using the rekordbox package requires the config option "
-                "XML_PATH to be a valid rekordbox XML file"
+                "Using the collections package requires the config option "
+                "COLLECTION_PATH to be a valid collection path"
             )
 
-        if self.BUILD_PLAYLISTS:
+        if self.COLLECTION_PLAYLISTS:
             playlist_config = (
                 Path(__file__).parent.parent / "configs" /
-                "rekordbox_playlists.yaml"
+                "collection_playlists.yaml"
             )
             if not playlist_config.exists():
                 raise RuntimeError(
-                    "rekordbox_playlists.yaml must be a valid YAML to use the "
-                    "BUILD_PLAYLISTS feature"
+                    "collection_playlists.yaml must be a valid YAML to use the "
+                    "COLLECTION_PLAYLISTS feature"
                 )
+
+
+class PlaylistConfigContent(BaseModel, extra=Extra.forbid):
+    "A class for type checking the content of the playlist config YAML."
+    name: str
+    playlists: List[Union[PlaylistConfigContent, str]]
+
+
+class PlaylistConfig(BaseModel, extra=Extra.forbid):
+    "A class for type checking the playlist config YAML."
+    combiner: Optional[PlaylistConfigContent] = None
+    tags: Optional[PlaylistConfigContent] = None
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/rekordbox/playlist_combiner.py` & `dj_beatcloud-2.6.0b0/djtools/collections/collections.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,307 +1,365 @@
-"""The "Combiner" constructs Rekordbox playlists by evaluating arbitrary
-boolean algebra expressions provided as the playlist name.
+"""This module contains classes for collections of different DJ software
+platforms.
 
-The supported operands are:
-
-- string literals matching one of the possible returned tags from a TagParser
-    implementation (see GenreTagParser and MyTagParser)
-- playlist names enclosed in curly braces e.g. {My Favorites}
-- ratings in the inclusive range [0, 5], separated by commas with ranges
-    denoted using a dash; both styles are enclosed with square brackets e.g.
-    [0, 2-5]
-- BPMs in the inclusive range [6, inf], separated by commas with ranges denoted
-    using a dash; both styles are enclosed with square brackets e.g.
-    [80-90, 140, 160-180]
-
-NOTE: the use of an asterisk `*` in an operand will glob other tags. For
-example, the providing "* Techno" as an operand would match "Acid Techno" and
-"Hard Techno" but not "somethingTechno" (because of the space character).
-Providing "Deep *" as an operand would match "Deep House" as well as
-"Deep Dubstep".
-
-The supported operators are:
-
-- `&` a.k.a. AND a.k.a set intersection: resulting tracks must be in BOTH sets
-- `|` a.k.a. OR a.k.a set union: resulting tracks may be in EITHER sets
-- `~` a.k.a. NOT a.k.a set difference: resulting tracks are those from the
-    left-hand side of the operator with the tracks appearing on the right-hand
-    side of the operator removed
-- `(`, `)`: parentheses are used to control the order of operations
-
-Some example expressions:
-
-- "(([120-129] & *Techno) | [130-160]) ~ [5]" This will first match all tracks
-    in the BPM range 120-129 inclusive before intersecting those with tracks
-    with a tag containing "Techno" as a suffix before unioning with all tracks
-    in the BPM range 130-160. Lastly, any tracks having a rating of 5 are
-    removed from the playlist.
-- "(Chill | Melodic) ~ {All Bass}" This will first take the union of all tracks
-    with either a "Chill" tag or a "Melodic" tag before removing all tracks
-    that appear in a playlist called "All Bass".
-
-The "Combiner" configuration must specify a flat list of "playlists" which
-define the boolean algebra expressions used by the Combiner.
+Collection is an abstract base class which defines the interface expected of a
+collection; namely methods for (de)serialization to/from the representation
+recognized by the DJ software for which Collection is being sub-classed.
+
+RekordboxCollection is an implementation of Collection which operates on the
+XML format that Rekordbox exports. The CustomSubstitution and
+UnsortedAttributes classes are helpers for serializing a RekordboxCollection.
 """
-from collections import defaultdict
-import logging
+from __future__ import annotations
+from abc import ABC, abstractmethod
+from copy import copy
+from pathlib import Path
 import re
-from typing import Dict, List, Set, Tuple, Union
+from typing import Dict, Iterator, List, Optional, Tuple, Union
 
+import bs4
 from bs4 import BeautifulSoup
+from bs4.dammit import EntitySubstitution
+from bs4.formatter import XMLFormatter
 
-from djtools.rekordbox.helpers import BooleanNode
+from djtools.collections.playlists import Playlist, RekordboxPlaylist
+from djtools.collections.tracks import RekordboxTrack, Track
 
 
-logger = logging.getLogger(__name__)
+class Collection(ABC):
+    "Abstract base class for a collection."
 
+    @abstractmethod
+    def __init__(self, path: Path, *args, **kwargs):
+        """Deserializes a collection from the native format of a DJ software.
 
-class Combiner:
-    """Parses a boolean algebra expression to combine tag playlists."""
+        Args:
+            path: Path to a serialized collection.
+        """
 
-    def __init__(
-        self,
-        parser_config: Dict[str, Union[str, List[Union[str, Dict]]]],
-        rekordbox_database: BeautifulSoup,
-    ):
-        """Constructor.
+    def add_playlist(self, playlist: Playlist):
+        """Appends a playlist to the collection.
 
         Args:
-            parser_config: YAML playlist structure.
+            playlist: Playlist to append to the collection.
         """
-        self.parser_config = parser_config
-        self._tracks = defaultdict(lambda: defaultdict(list))
-        self._bpm_rating_lookup = {}
-        self._prescan(rekordbox_database)
-        self._operators = {
-            "&": set.intersection,
-            "|": set.union,
-            "~": set.difference,
-        }
+        self._playlists.add_playlist(playlist)  # pylint:disable=no-member
+
+    def get_playlists(
+        self, name: Optional[str] = None
+    ) -> Union[Playlist, List[Playlist]]:
+        """Returns Playlists with a matching name.
 
-    def __call__(
-        self, tracks: Dict[str, List[Tuple[str, List[str]]]]
-    ) -> Dict[str, Set[str]]:
-        """Evaluates boolean expressions creating playlists that combine tags.
+        If no playlist name is provided, then the root playlist is returned.
 
         Args:
-            tracks: Map of tags to lists of (track_id, tags) tuples.
+            name: Name of the Playlists to return.
 
         Returns:
-            Dict mapping boolean expression to a set of track IDs.
+            The Playlists with the same name.
         """
-        self._tracks.update({k: dict(v) for k, v in tracks.items()})
-        playlist_tracks = {
-            expression: self._parse_boolean_expression(expression)
-            for expression in self.parser_config.get("playlists", [])
-        }
+        if not name:
+            return self._playlists  # pylint:disable=no-member
 
-        return playlist_tracks
+        playlists = []
+        for playlist in self._playlists:  # pylint:disable=no-member
+            if playlist.get_name() == name:
+                playlists.append(playlist)
+            if playlist.is_folder():
+                for playlist in playlist:
+                    playlists.extend(playlist.get_playlists(name))
 
-    def _add_tag(self, tag: str, node: BooleanNode) -> str:
-        """Strips whitespace off of a tag and, if non-empty, adds it to a node.
+        return [playlist for playlist in playlists if playlist is not None]
 
-        Args:
-            tag: Potentially assembled tag string.
-            node: BooleanNode to potentially have tag added to it.
+    def get_tracks(self) -> Dict[str, Track]:
+        """Returns the tracks in the collection.
 
         Returns:
-            Empty tag string.
+            Dict of tracks.
         """
-        tag = tag.strip()
-        if tag:
-            node.tags.append(tag)
-
-        return ""
+        return self._tracks
 
-    def get_combiner_tracks(self) -> Dict[str, Dict[str, List]]:
-        """Returns tag / selector -> tracks mapping.
+    @abstractmethod
+    def reset_playlists(self):
+        """Resets the Playlists in the Collection to be empty."""
+
+    @abstractmethod
+    def serialize(self, *args, **kwargs) -> Path:
+        """Serialize a collection into the native format of a DJ software.
 
         Returns:
-            Map of tags / selectors to track_id.
+            A path to a serialized collection.
         """
-        return self._tracks
 
-    def get_playlist_mapping(
-        self,
-        rekordbox_database: BeautifulSoup,
-    ) -> Dict[str, List[Tuple[str, List]]]:
-        """Adds tags for playlist selectors.
+    def set_tracks(self, tracks: Dict[str, Track]):
+        """Sets the tracks of this collection.
 
         Args:
-            rekordbox_database: Parsed XML.
+            tracks: Tracks to set.
+        """
+        self._tracks = tracks  # pylint:disable=attribute-defined-outside-init
 
-        Raises:
-            LookupError: Playlists in expressions must exist in "XML_PATH".
 
-        Returns:
-            Map of playlist selectors to (track_id, tags) tuples.
+class RekordboxCollection(Collection):
+    "Collection implementation for usage with Rekordbox."
+
+    def __init__(self, path: Path):
+        """Deserializes a Collection from an XML file.
+
+        Args:
+            path: Path to a serialized collection.
         """
-        for playlist_name in self._playlists:
-            try:
-                playlist = rekordbox_database.find_all(
-                    "NODE", {"Name": playlist_name}
-                )[0]
-            except IndexError:
-                raise LookupError(f"{playlist_name} not found") from LookupError
-
-            self._tracks[f"{{{playlist_name}}}"] = {
-                track["Key"]: [] for track in playlist.children
-                if str(track).strip()
-            }
+        self._path = path
 
-        return self._tracks
+        # Parse the XML as a BeautifulSoup document.
+        with open(self._path, mode="r", encoding="utf-8") as _file:
+            self._collection = BeautifulSoup(_file.read(), "xml")
+
+        # Create a dict of tracks.
+        self._tracks = {
+            track["TrackID"]: RekordboxTrack(track)
+            for track in self._collection.find_all("TRACK")
+            if track.get("Location")
+        }
 
-    def _parse_boolean_expression(self, expression: str) -> Set[str]:
-        """Parses a boolean algebra expression by constructing a tree.
+        # Instantiate the Playlist(s) in this collection.
+        self._playlists = RekordboxPlaylist(
+            self._collection.find("NODE", {"Name": "ROOT", "Type": "0"}),
+            tracks=self._tracks,
+        )
 
-        Args:
-            expression: String representing boolean algebra expression.
+    def __repr__(self) -> str:
+        """Produce a string representation of this Collection.
 
         Returns:
-            Set of track IDs reduced from the evaluation of the expression.
+            Collection represented as a string.
         """
-        node = BooleanNode()
-        tag = ""
-        for char in expression:
-            if char == "(":
-                node = BooleanNode(parent=node)
-            elif char in self._operators:
-                tag = self._add_tag(tag, node)
-                node.operators.append(self._operators[char])
-            elif char == ")":
-                tag = self._add_tag(tag, node)
-                tracks = node(self._tracks)
-                node = node.parent
-                if tracks:
-                    node.tracks.append(tracks)
+        # Eventual repr string to return.
+        string = "{}({}\n)"
+        # Body to the repr string to fill out with Collection content.
+        body =  ""
+
+        # Dunder methods aren't represented. Public members (i.e methods)
+        # aren't represented either.
+        repr_attrs = {
+            key[1:]: value for key, value in self.__dict__.items()
+            if not(
+                key.startswith(f"_{type(self).__name__}")
+                or not key.startswith("_")
+                or key == "_collection"
+            )
+        }
+
+        # Build a representation of this Collection.
+        for key, value in repr_attrs.items():
+            # Skip representing this collection's playlists and tracks.
+            # Defer representation of the playlists attribute until the end.
+            if key in ["playlists", "tracks"]:
+                continue
+
+            # Represent string values with surrounding double quotes.
+            if isinstance(value, (Path, str)):
+                value=  f'"{value}"'
+
+            # Append the attribute's name and value to the representation.
+            body += f"\n{' ' * 4}{key}={value},"
+
+        # Now represent the playlists and tracks attributes as an indented list
+        # of playlists and number of tracks, respectively.
+        for key, value in repr_attrs.items():
+            if key not in ["playlists", "tracks"]:
+                continue
+            if isinstance(value, dict):
+                body += f"\n{' ' * 4}{key}={len(value)},"
             else:
-                tag += char
-        tag = self._add_tag(tag, node)
+                # TODO(a-rich): split and join with extra indents.
+                body += f"\n{' ' * 4}{key}=["
+                playlists = f"\n{' ' * 8}".join(repr(value).split("\n"))
+                body += f"\n{' ' * 8}{playlists}"
+                body += f"\n{' ' * 4}]"
 
-        return node(self._tracks)
+        return string.format(type(self).__name__, body)
 
-    def _parse_bpms_and_ratings(
-        self, bpm_rating_match: List[str]
-    ) -> List[Tuple]:
-        """Parses a string match of one or more BPM and / or rating selectors.
+    def __str__(self) -> str:
+        """Produces a string representation of this Collection.
+
+        Returns:
+            Collection represented as a string.
+        """
+        return str(self.serialize())
+
+    def reset_playlists(self):
+        """Resets the Playlists in the Collection to be empty."""
+        root = self._collection.find("NODE", {"Name": "ROOT", "Type": "0"})
+        for child in list(root.children):
+            child.extract()
+        self._playlists = RekordboxPlaylist(root, tracks=self._tracks)
+
+    def serialize(
+        self, *args, new_path: Optional[Path] = None, **kwargs
+    ) -> Path:
+        """Serializes this Collection as an XML file.
 
         Args:
-            bpm_rating_match: List of BPM or rating strings.
+            new_path: Path to output serialized collection to.
 
         Returns:
-            Tuple of BPM and rating lists.
+            Path to the serialized collection XML file.
         """
-        bpms, ratings = [], []
-        for bpm_rating in bpm_rating_match:
-            parts = map(str.strip, bpm_rating.split(","))
-            for part in parts:
-                number = _range = None
-                # If "part" is a digit, then it's an explicit BPM or rating to
-                # filter for.
-                if part.isdigit():
-                    number = int(part)
-                    if 0 <= number <= 5:
-                        ratings.append(str(number))
-                    elif number > 5:
-                        bpms.append(str(number))
-                # If "part" is two digits separated by a "-", then it's a range
-                # of BPMs or ratings to filter for.
-                elif (
-                    len(part.split("-")) == 2 and
-                    all(x.isdigit() for x in part.split("-"))
-                ):
-                    _range = list(map(int, part.split("-")))
-                    _range = range(min(_range), max(_range) + 1)
-                    if all(0 <= x <= 5 for x in _range):
-                        ratings.extend(map(str, _range))
-                    elif all(x > 5 for x in _range):
-                        bpms.extend(map(str, _range))
-                    else:
-                        logger.error(f"Bad BPM or rating number range: {part}")
-                        continue
-                else:
-                    logger.error(
-                        f"Malformed BPM or rating filter part: {part}"
+        # BeautifulSoup document.
+        doc = BeautifulSoup("", features="xml")
+
+        # Tag that contains all the playlist data.
+        root_tag_name = "DJ_PLAYLISTS"
+
+        # Retrieve this root tag from the existing document, rather than
+        # building it from scratch, in case the attributes ever change.
+        root_tag = bs4.Tag(
+            name=root_tag_name,
+            attrs=self._collection.find(root_tag_name).attrs,
+        )
+
+        # Similarly, we want to reference the existing attribute data on the
+        # product Tag.
+        root_tag.extend(
+            [bs4.NavigableString("\n"), copy(self._collection.find("PRODUCT"))]
+        )
+
+        # Build the collection Tag and serialize each track into it before
+        # adding the collection Tag to the root.
+        collection_tag = bs4.Tag(
+            name="COLLECTION", attrs={"Entries": str(len(self._tracks))}
+        )
+        for track in self._tracks.values():
+            collection_tag.extend(
+                [bs4.NavigableString("\n"), track.serialize()]
+            )
+        collection_tag.append(bs4.NavigableString("\n"))
+        root_tag.extend([bs4.NavigableString("\n"), collection_tag])
+
+        # Build the playlists Tag and serialize each Playlist into it before
+        # adding the playlist Tag to the root.
+        playlists_tag = bs4.Tag(name="PLAYLISTS")
+        playlists_root_tag = bs4.Tag(
+            name="NODE",
+            attrs={"Type": "0", "Name": "ROOT", "Count": len(self._playlists)},
+        )
+        for playlist in self._playlists:
+            playlists_root_tag.extend(
+                [bs4.NavigableString("\n"), playlist.serialize()]
+            )
+        playlists_root_tag.append(bs4.NavigableString("\n"))
+        playlists_tag.extend(
+            [
+                bs4.NavigableString("\n"),
+                playlists_root_tag,
+                bs4.NavigableString("\n"),
+            ]
+        )
+        root_tag.extend(
+            [
+                bs4.NavigableString("\n"),
+                playlists_tag,
+                bs4.NavigableString("\n"),
+            ]
+        )
+        doc.append(root_tag)
+
+        # If no new path is provided, use the original but prefix the file name
+        # with "auto_".
+        if not new_path:
+            new_path = self._path.parent / f"auto_{self._path.name}"
+
+        # Write the serialized Collection to a new file.
+        with open(new_path, mode="w", encoding="utf-8") as _file:
+            _file.write(
+                doc.prettify(
+                    # UnsortedAttributes formatter ensures attributes are
+                    # serialized in the same order as the original XML file.
+                    formatter=UnsortedAttributes(
+                        indent=2,
+                        # CustomSubstitution is used to substitute an expanded
+                        # character set in the serialized XML file.
+                        entity_substitution=CustomSubstitution.substitute_xml,
                     )
-                    continue
+                )
+            )
+
+        return new_path
 
-                self._bpm_rating_lookup[
-                    tuple(map(str, _range or [])) or str(number)
-                ] = f"[{part}]"
-
-        return bpms, ratings
-
-    def _prescan(self, rekordbox_database: BeautifulSoup):
-        """Populates track lookup using BPM and rating selectors.
-
-        Boolean expressions may contain zero or more indicators for selectors:
-            * BPM selectors: comma-delimited list of integers or integer ranges
-                (e.g. "6-666") greater than 5 enclosed in square brackets
-                (e.g. "[120, 137-143]").
-            * Rating selectors: comma-delimited list of integers or integer
-                ranges (e.g. "0-5") less than 6 enclosed in square brackets
-                (e.g. "[5, 2, 2-4]").
-            * Playlist selectors: exact matches to existing playlist name
-                enclosed in curly braces (e.g. "{All DnB}").
-        
-        Whether the numbers of a BPM / rating selector are interpreted as a BPM
-        or a rating depends on the value; if 0 <= number <= 5, then it's
-        interpreted as a rating, if number > 5, then it's interpreted as a BPM.
-
-        This method also initializes a set of playlist selectors but delays
-        populating them until any other TagParser implementations have been
-        called so as to ensure the Combiner logic evaluation includes the
-        complete set of tracks that may have been added to playlists by these
-        TagParsers.
-            
-        If you want to make a Combiner playlist that has all tracks in a
-        playlist called "All DnB" that have a 5 star rating and are in the BPM
-        range [170, 172], this can be expressed as:
-            "{All DnB} & [5, 170-172]"
+    @classmethod
+    def validate(cls, input_xml: Path, output_xml: Path):
+        """Validate the serialized Collection matches the original.
 
         Args:
-            rekordbox_database: Parsed XML.
+            input_xml: Path to an XML containing the original collection.
+            output_xml: Path to an XML containing the serialized collection.
 
         Raises:
-            LookupError: Playlists in expressions must exist in "XML_PATH".
+            AssertionError: A serialized Collection must exactly match the
+                original XML used to deserialize from.
         """
-        # Get the sets of BPMs, ratings, and playlists in order to pre-populate
-        # the track lookup.
-        bpms, ratings, self._playlists = set(), set(), set()
-        for expression in self.parser_config.get("playlists", []):
-            self._playlists.update(re.findall(r"(?<={)[^{}]*(?=})", expression))
-            bpm_rating_match = re.findall(r"(?<=\[)[^\[\]]*(?=\])", expression)
-            if not bpm_rating_match:
-                continue
-            _bpms, _ratings = self._parse_bpms_and_ratings(bpm_rating_match)
-            bpms.update(_bpms)
-            ratings.update(_ratings)
-
-        # Rekordbox stores rating values in the range [0, 255].
-        ratings_value_lookup = {
-            "0": "0",
-            "51": "1",
-            "102": "2",
-            "153": "3",
-            "204": "4",
-            "255": "5",
-        }
+        # Read the original and serialized collection XML files as
+        # strings.
+        with open(input_xml, mode="r", encoding="utf-8") as _file:
+            input_xml_string = _file.read()
+        with open(output_xml, mode="r", encoding="utf-8") as _file:
+            output_xml_string = _file.read()
+
+        # Rekordbox capitalizes "UTF-8" in the file declaration while
+        # BeautifulSoup does not.
+        xml_declaration = input_xml_string[:38]
+        output_xml_string = xml_declaration + output_xml_string[38:]
+
+        # Replace multiple occurrences of whitespace with a single whitespace.
+        whitespace = re.compile(r"/\s{2,}/g")
+        input_xml_string = re.sub(whitespace, input_xml_string, " ")
+        output_xml_string = re.sub(whitespace, output_xml_string, " ")
+
+        assert input_xml_string == output_xml_string, (
+            "Failed RekordboxCollection validation!"
+        )
+
+
+class CustomSubstitution(EntitySubstitution):
+    "Helper class to serialize Tags with proper character substitution."
+
+    # Regular expression to match brackets, ampersands, and quotes.
+    AMPERSAND_OR_BRACKET_OR_QUOTES = re.compile("([<>&'\"])")
+
+    @classmethod
+    def substitute_xml(
+        cls, value: str, make_quoted_attribute: bool = False
+    ) -> str:
+        """Substitute XML entities for special XML characters.
 
-        # Build out the lookup for BPMs and ratings.
-        values_set = bpms.union(ratings)
-        for track in rekordbox_database.find_all("TRACK"):
-            if not track.get("Location"):
-                continue
+        Args:
+            value: A string to be substituted.
+            make_quoted_attribute: If True, then the string will be quoted.
 
-            values = [
-                str(round(float(track["AverageBpm"]))),
-                ratings_value_lookup[track["Rating"]]
-            ]
-            for val in values:
-                if val in values_set:
-                    for value, tag in self._bpm_rating_lookup.items():
-                        if (
-                            (isinstance(value, str) and value == val) or
-                            (isinstance(value, tuple) and val in value)
-                        ):
-                            self._tracks[tag][track["TrackID"]] = []
+        Returns:
+            String value with it's characters substituted.
+        """
+        # Escape angle brackets, ampersands, single quotes, and double quotes.
+        value = cls.AMPERSAND_OR_BRACKET_OR_QUOTES.sub(
+            cls._substitute_xml_entity, value)
+
+        if make_quoted_attribute:
+            value = cls.quoted_attribute_value(value)  # pragma: no cover
+
+        return value
+
+
+class UnsortedAttributes(XMLFormatter):
+    "Helper class to serialize Tag attributes in their original order."
+
+    def attributes(self, tag: bs4.element.Tag) -> Iterator[Tuple[str, str]]:
+        """Generator that returns a Tag's attributes as key / value pairs.
+
+        Args:
+            tag: Tag from a Collection.
+
+        Yields:
+            Tuple containing a key / value representing an attribute.
+        """
+        for key, value in tag.attrs.items():
+            yield key, value
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/rekordbox/shuffle_playlists.py` & `dj_beatcloud-2.6.0b0/djtools/collections/shuffle_playlists.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,68 @@
 """This module is used to emulate shuffling the track order of one or more
-playlists. This is done by setting the Rekordbox tag (i.e. "TrackNumber") of
-tracks in the playlists to sequential numbers. After setting the TrackNumber
-tags of tracks in the provided playlists, those tracks must be re-imported
-for Rekordbox to be aware of the update.
+playlists. This is done by setting the track number attribute of each track in
+sequential order after collecting the set of Tracks from the provided
+playlist(s).
 """
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import as_completed, ThreadPoolExecutor
 import logging
 import os
 import random
 
-from bs4 import BeautifulSoup
 from tqdm import tqdm
 
-
 from djtools.configs.config import BaseConfig
-from djtools.rekordbox.helpers import get_playlist_tracks, set_track_number
+from djtools.collections.helpers import PLATFORM_REGISTRY
 
 
 logger = logging.getLogger(__name__)
 
 
 def shuffle_playlists(config: BaseConfig):
     """For each playlist in "SHUFFLE_PLAYLISTS", shuffle the tracks and
-    sequentially set the TrackNumber tag to a number to emulate track
-    randomization.
+    sequentially set the track number to emulate shuffling.
 
     Args:
         config: Configuration object.
     """
-    # Load Rekordbox database from XML.
-    with open(config.XML_PATH, mode="r", encoding="utf-8") as _file:
-        soup = BeautifulSoup(_file.read(), "xml")
-
-    # Create track ID lookup.
-    lookup = {}
-    for track in soup.find_all("TRACK"):
-        if not track.get("Location"):
-            continue
-        lookup[track["TrackID"]] = track
-
-    # Build a list of tracks to shuffle from the provided list of playlists.
-    seen_tracks = set()
-    shuffled_tracks = []
-    for playlist in config.SHUFFLE_PLAYLISTS:
-        try:
-            tracks = get_playlist_tracks(soup, playlist, seen_tracks)
-        except LookupError as exc:
-            raise LookupError(f"{playlist} not found") from exc
+    # Load collection.
+    collection = PLATFORM_REGISTRY[config.PLATFORM]["collection"](
+        path=config.COLLECTION_PATH
+    )
 
-        random.shuffle(tracks)
-        shuffled_tracks.extend(tracks)
+    # Build a dict of tracks to shuffle from the provided list of playlists.
+    shuffled_tracks = {}
+    for playlist_name in config.SHUFFLE_PLAYLISTS:
+        playlists = collection.get_playlists(playlist_name)
+        if not playlists:
+            raise LookupError(f"{playlist_name} not found")
+        for playlist in playlists:
+            tracks = playlist.get_tracks()
+            track_keys = list(tracks.keys())
+            random.shuffle(track_keys)
+            shuffled_tracks.update({key: tracks[key] for key in track_keys})
 
-    # Shuffle the track number field of the tracks.
-    shuffled_tracks = [lookup[x] for x in shuffled_tracks]
+    # Apply the shuffled track number to the attribute of the tracks.
+    shuffled_tracks = list(shuffled_tracks.values())
     payload = [shuffled_tracks, list(range(1, len(shuffled_tracks) + 1))]
     with ThreadPoolExecutor(max_workers=os.cpu_count() * 4) as executor:
-        _ = list(
-            tqdm(
-                executor.map(set_track_number, *payload),
-                total=len(shuffled_tracks),
-                desc=f"Randomizing {len(shuffled_tracks)} tracks",
-            )
+        futures = [
+            executor.submit(track.set_track_number, number)
+            for track, number in zip(*payload)
+        ]
+        for future in tqdm(
+            as_completed(futures),
+            total=len(futures),
+            desc=f"Randomizing {len(futures)} tracks",
+        ):
+            _ = future.result()
+
+    # Reset the collection's playlists and insert a new playlist containing
+    # just the shuffled tracks.
+    collection.reset_playlists()
+    collection.add_playlist(
+        PLATFORM_REGISTRY[config.PLATFORM]["playlist"].new_playlist(
+            name="SHUFFLE",
+            tracks={track.get_id(): track for track in shuffled_tracks},
         )
-
-    # Insert shuffled tracks playlist into the playlist root.
-    playlists_root = soup.find_all("NODE", {"Name": "ROOT", "Type": "0"})[0]
-    new_playlist = soup.new_tag(
-        "NODE", KeyType="0", Name="AUTO_SHUFFLE", Type="1"
     )
-    for track in shuffled_tracks:
-        new_playlist.append(soup.new_tag("TRACK", Key=track["TrackID"]))
-    playlists_root.insert(0, new_playlist)
-
-    # Write XML file.
-    _dir = config.XML_PATH.parent
-    _file = config.XML_PATH.name
-    auto_xml_path = _dir / f"auto_{_file}"
-    with open(
-        auto_xml_path, mode="wb", encoding=soup.orignal_encoding
-    ) as _file:
-        _file.write(soup.prettify("utf-8"))
+    _ = collection.serialize()
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/spotify/__init__.py` & `dj_beatcloud-2.6.0b0/djtools/spotify/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,23 @@
     * `config`: the configuration object for the `spotify` package
     * `helpers`: helper functions for `playlist_builder`
     * `playlist_builder`: constructs or updates Spotify playlists using either
         Subreddit posts or the Discord webhook output from `UPLOAD_MUSIC`
 """
 from djtools.spotify.config import SpotifyConfig
 from djtools.spotify.playlist_builder import (
-    playlist_from_upload, update_auto_playlists
+    spotify_playlist_from_upload, spotify_playlists
 )
 
 
 SPOTIFY_OPERATIONS = {
-    "PLAYLIST_FROM_UPLOAD": playlist_from_upload,
-    "AUTO_PLAYLIST_UPDATE": update_auto_playlists,
+    "SPOTIFY_PLAYLIST_FROM_UPLOAD": spotify_playlist_from_upload,
+    "SPOTIFY_PLAYLISTS": spotify_playlists,
 }
 
 
 __all__ = (
-    "playlist_from_upload",
+    "spotify_playlist_from_upload",
     "SpotifyConfig",
     "SPOTIFY_OPERATIONS",
-    "update_auto_playlists",
+    "spotify_playlists",
 )
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/spotify/config.py` & `dj_beatcloud-2.6.0b0/djtools/spotify/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
 class SubredditConfig(BaseModel):
-    """Configuration object for AUTO_PLAYLIST_SUBREDDITS."""
+    """Configuration object for SPOTIFY_PLAYLISTS."""
 
     name: str
     limit: NonNegativeInt= 50
     period: Literal[
         "all", "day", "hour", "month", "week", "year"
     ] = "week"
     type: Literal [
         "controversial", "hot", "new", "rising", "top"
     ] = "hot"
 
 
 class SpotifyConfig(BaseConfig):
     """Configuration object for the spotify package."""
 
-    AUTO_PLAYLIST_DEFAULT_LIMIT: NonNegativeInt = 50
-    AUTO_PLAYLIST_DEFAULT_PERIOD: str = "week"
-    AUTO_PLAYLIST_DEFAULT_TYPE: str = "hot"
-    AUTO_PLAYLIST_FUZZ_RATIO: NonNegativeInt = 70
-    AUTO_PLAYLIST_POST_LIMIT: NonNegativeInt = 100
-    AUTO_PLAYLIST_SUBREDDITS: List[SubredditConfig] = []
-    AUTO_PLAYLIST_UPDATE: bool = False
-    PLAYLIST_FROM_UPLOAD: bool = False
+    SPOTIFY_PLAYLIST_DEFAULT_LIMIT: NonNegativeInt = 50
+    SPOTIFY_PLAYLIST_DEFAULT_PERIOD: str = "week"
+    SPOTIFY_PLAYLIST_DEFAULT_TYPE: str = "hot"
+    SPOTIFY_PLAYLIST_FROM_UPLOAD: bool = False
+    SPOTIFY_PLAYLIST_FUZZ_RATIO: NonNegativeInt = 70
+    SPOTIFY_PLAYLIST_POST_LIMIT: NonNegativeInt = 100
+    SPOTIFY_PLAYLIST_SUBREDDITS: List[SubredditConfig] = []
+    SPOTIFY_PLAYLISTS: bool = False
     REDDIT_CLIENT_ID: str = ""
     REDDIT_CLIENT_SECRET: str = ""
     REDDIT_USER_AGENT: str = ""
     SPOTIFY_CLIENT_ID: str = ""
     SPOTIFY_CLIENT_SECRET: str = ""
     SPOTIFY_REDIRECT_URI: str = ""
     SPOTIFY_USERNAME: str  = ""
@@ -53,43 +53,43 @@
             RuntimeError: Spotify API credentials must exit.
             RuntimeError: Spotify API credentials must be valid.
             RuntimeError: Reddit API credentials must exist.
         """
         super().__init__(*args, **kwargs)
 
         if (
-            (self.AUTO_PLAYLIST_UPDATE or self.PLAYLIST_FROM_UPLOAD) and
+            (self.SPOTIFY_PLAYLISTS or self.SPOTIFY_PLAYLIST_FROM_UPLOAD) and
             not all(
                 [
                     self.SPOTIFY_CLIENT_ID,
                     self.SPOTIFY_CLIENT_SECRET,
                     self.SPOTIFY_REDIRECT_URI,
                     self.SPOTIFY_USERNAME
                 ]
             )
         ):
             raise RuntimeError(
                 "Without all the configuration options SPOTIFY_CLIENT_ID, "
                 "SPOTIFY_CLIENT_SECRET, SPOTIFY_REDIRECT_URI, and "
                 "SPOTIFY_USERNAME set to valid values, you cannot use "
-                "AUTO_PLAYLIST_UPDATE or PLAYLIST_FROM_UPLOAD"
+                "SPOTIFY_PLAYLISTS or SPOTIFY_PLAYLIST_FROM_UPLOAD"
             )
-        if self.AUTO_PLAYLIST_UPDATE or self.PLAYLIST_FROM_UPLOAD:
+        if self.SPOTIFY_PLAYLISTS or self.SPOTIFY_PLAYLIST_FROM_UPLOAD:
             from djtools.spotify.helpers import get_spotify_client
             spotify = get_spotify_client(self)
             try:
                 spotify.current_user()
             except Exception as exc:
                 raise RuntimeError("Spotify credentials are invalid!") from exc
 
-        if self.AUTO_PLAYLIST_UPDATE and not all(
+        if self.SPOTIFY_PLAYLISTS and not all(
             [
                 self.REDDIT_CLIENT_ID,
                 self.REDDIT_CLIENT_SECRET,
                 self.REDDIT_USER_AGENT,
             ]
         ):
             raise RuntimeError(
                 "Without all the configuration options REDDIT_CLIENT_ID, "
                 "REDDIT_CLIENT_SECRET, and REDDIT_USER_AGENT, set to valid "
-                "values, you cannot use AUTO_PLAYLIST_UPDATE"
+                "values, you cannot use SPOTIFY_PLAYLISTS"
             )
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/spotify/helpers.py` & `dj_beatcloud-2.6.0b0/djtools/spotify/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 
     Returns:
         List of Spotify track ("id", "name") tuples and SubredditConfig as a
             dictionary.
     """
     sub = await reddit.subreddit(subreddit["name"])
     func = getattr(sub, subreddit["type"])
-    kwargs = {"limit": config.AUTO_PLAYLIST_POST_LIMIT}
+    kwargs = {"limit": config.SPOTIFY_PLAYLIST_POST_LIMIT}
     if subreddit["type"]== "top":
         kwargs["time_filter"] = subreddit["period"]
     subs = [
         x async for x in catch(
             func(**kwargs), message="Failed to retrieve Reddit submission"
         )
     ]
@@ -291,15 +291,15 @@
             f"Searching Spotify for {len(submissions)} new submission(s) from "
             f'"r/{subreddit["name"]}"'
         )
         logger.info(msg)
         payload = [
             submissions,
             [spotify] * len(submissions),
-            [config.AUTO_PLAYLIST_FUZZ_RATIO] * len(submissions)
+            [config.SPOTIFY_PLAYLIST_FUZZ_RATIO] * len(submissions)
         ]
         with ThreadPoolExecutor(max_workers=8) as executor:
             new_tracks = list(
                 tqdm(
                     executor.map(process, *payload),
                     total=len(submissions),
                     desc=msg,
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.6.0b0/djtools/spotify/playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     logger = logging.getLogger(logger)
     logger.setLevel(logging.CRITICAL)
 logging.getLogger("asyncio").setLevel(logging.WARNING)
 
 logger = logging.getLogger(__name__)
 
 
-async def async_update_auto_playlists(config: BaseConfig):
+async def async_spotify_playlists(config: BaseConfig):
     """This function updates the contents of one or more Spotify playlists with
         the posts of one or more subreddits (currently only supports one
         subreddit per playlist).
 
     Args:
         config: Configuration object.
     """
@@ -66,15 +66,15 @@
                 spotify,
                 reddit,
                 subreddit,
                 config,
                 praw_cache,
             )
         )
-        for subreddit in config.AUTO_PLAYLIST_SUBREDDITS
+        for subreddit in config.SPOTIFY_PLAYLIST_SUBREDDITS
     ]
 
     for task in asyncio.as_completed(tasks):
         tracks, subreddit = await task
         playlist_ids = populate_playlist(
             playlist_name=subreddit["name"],
             playlist_ids=playlist_ids,
@@ -89,15 +89,15 @@
 
     write_playlist_ids(playlist_ids)
 
     with open(cache_file, mode="w", encoding="utf-8") as _file:
         yaml.dump(praw_cache, _file)
 
 
-def playlist_from_upload(config: BaseConfig):
+def spotify_playlist_from_upload(config: BaseConfig):
     """Generates a Spotify playlist using a Discord webhook output.
 
     If "upload_output", a path to a text file containing the pasted output of
     the upload_music Discord webhook output, is provided, this is used to
     generate a Spotify playlist of those uploaded tracks. If this is not
     provided, then the clipboard contents are used instead.
 
@@ -136,15 +136,15 @@
             continue
         if config.ARTIST_FIRST:
             track, artist = artist, track
         files.append((track, artist))
     files = list(filter(lambda x: len(x) == 2, files))
 
     # Query Spotify for files in upload output.
-    threshold = config.AUTO_PLAYLIST_FUZZ_RATIO
+    threshold = config.SPOTIFY_PLAYLIST_FUZZ_RATIO
     tracks = []
     for title, artist in files:
         query = f"track:{title} artist:{artist}"
         try:
             results = spotify.search(q=query, type="track", limit=50)
         except Exception as exc:
             logger.error(f'Error searching for "{title} - {artist}": {exc}')
@@ -167,14 +167,14 @@
         tracks=tracks,
         verbosity=config.VERBOSITY,
     )
 
     write_playlist_ids(playlist_ids)
 
 
-def update_auto_playlists(config: BaseConfig):
+def spotify_playlists(config: BaseConfig):
     """This function asynchronously updates Spotify playlists.
 
     Args:
         config: Configuration object.
     """
-    asyncio.run(async_update_auto_playlists(config))
+    asyncio.run(async_spotify_playlists(config))
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/sync/config.py` & `dj_beatcloud-2.6.0b0/djtools/sync/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 class SyncConfig(BaseConfig):
     """Configuration object for the sync package."""
 
     ARTIST_FIRST: bool = False
     AWS_USE_DATE_MODIFIED: bool = False
     DISCORD_URL: str = ""
+    DOWNLOAD_COLLECTION: bool = False
     DOWNLOAD_EXCLUDE_DIRS: List[Path] = []
     DOWNLOAD_INCLUDE_DIRS: List[Path] = []
     DOWNLOAD_MUSIC: bool = False
-    DOWNLOAD_SPOTIFY: str = ""
-    DOWNLOAD_XML: bool = False
+    DOWNLOAD_SPOTIFY_PLAYLIST: str = ""
     DRYRUN: bool = False
     IMPORT_USER: str = ""
+    UPLOAD_COLLECTION: bool = False
     UPLOAD_EXCLUDE_DIRS: List[Path] = []
     UPLOAD_INCLUDE_DIRS: List[Path] = []
     UPLOAD_MUSIC: bool = False
-    UPLOAD_XML: bool = False
     USB_PATH: Optional[Union[str, Path]] = None
     USER: str = ""
 
     def __init__(self, *args, **kwargs):
         """Constructor.
 
         Raises:
@@ -57,18 +57,18 @@
                 "DOWNLOAD_EXCLUDE_DIRS"
             )
             logger.critical(msg)
             raise ValueError(msg)
 
         if any(
             [
+                self.DOWNLOAD_COLLECTION,
                 self.DOWNLOAD_MUSIC,
-                self.DOWNLOAD_XML,
+                self.UPLOAD_COLLECTION,
                 self.UPLOAD_MUSIC,
-                self.UPLOAD_XML,
             ]
         ):
             if not self.AWS_PROFILE:
                 msg = "Config must include AWS_PROFILE for sync operations"
                 logger.critical(msg)
                 raise RuntimeError(msg)
 
@@ -85,17 +85,18 @@
 
         if self.UPLOAD_MUSIC and not self.DISCORD_URL:
             logger.warning(
                 'DISCORD_URL is not configured...set this for "New Music" '
                 "discord messages!"
             )
 
-        if self.DOWNLOAD_XML and not self.IMPORT_USER:
+        if self.DOWNLOAD_COLLECTION and not self.IMPORT_USER:
             raise RuntimeError(
-                f'Unable to import from XML of IMPORT_USER "{self.IMPORT_USER}"'
+                "Unable to import from collection of IMPORT_USER "
+                f'"{self.IMPORT_USER}"'
             )
 
     @validator("USB_PATH")
     @classmethod
     def usb_path_as_pathlib_path(cls, value: str) -> Union[Path, str]:
         """Validator to convert USB_PATH to a pathlib.Path.
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/sync/helpers.py` & `dj_beatcloud-2.6.0b0/djtools/sync/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """This module contains helper functions used by the "sync_operations" module.
 Helper functions include formatting "aws s3 sync" commands, formatting the
 output of "aws s3 sync" commands, posting uploaded tracks to Discord, and
-modifying IMPORT_USER's XML to point to tracks located at "USB_PATH".
+modifying IMPORT_USER's collection to point to tracks located at "USB_PATH".
 """
 from datetime import datetime, timedelta
 from itertools import groupby
 import logging
 from pathlib import Path
 from subprocess import Popen, PIPE, CalledProcessError
 from typing import Optional
-from urllib.parse import quote, unquote
 
-from bs4 import BeautifulSoup
 import requests
 
+from djtools.collections.helpers import PLATFORM_REGISTRY
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
 def parse_sync_command(
@@ -78,42 +77,35 @@
     if config.DRYRUN:
         _cmd.append("--dryrun")
     logger.info(" ".join(_cmd))
 
     return _cmd
 
 
-def rewrite_xml(config: BaseConfig, loc_prefix: str = "file://localhost"):
-    """This function modifies the "Location" field of track tags in a
-        downloaded Rekordbox XML replacing the "USB_PATH" written by
-        "IMPORT_USER" with the "USB_PATH" in "config.yaml".
+def rewrite_track_paths(config: BaseConfig, other_user_collection: Path):
+    """This function modifies the location of tracks in a collection.
+    
+    This is done by replacing the "USB_PATH" written by "IMPORT_USER" with the
+    "USB_PATH" in "config.yaml".
 
     Args:
         config: Configuration object.
-        loc_prefix: Prefix of the `Location` field.
+        other_user_collection: Path to another user's collection.
     """
-    xml_path = (
-        Path(config.XML_PATH).parent / f"{config.IMPORT_USER}_rekordbox.xml"
+    music_path = Path("DJ Music")
+    collection = PLATFORM_REGISTRY[config.PLATFORM]["collection"](
+        path=other_user_collection
     )
-    music_path = "DJ Music"
-    usb_path = config.USB_PATH.as_posix().strip("/")
-
-    with open(xml_path, mode="r", encoding="utf-8") as _file:
-        soup = BeautifulSoup(_file.read(), "xml")
-        for track in soup.find_all("TRACK"):
-            if not track.get("Location"):
-                continue
-            loc = unquote(track["Location"])
-            common_path = f"{music_path}/{loc.split(music_path + '/')[-1]}"
-            loc = f"{loc_prefix}/{usb_path}/{common_path}"
-            track["Location"] = quote(loc)
-
-
-    with open(xml_path, mode="wb", encoding=soup.orignal_encoding) as _file:
-        _file.write(soup.prettify("utf-8"))
+    for track in collection.get_tracks().values():
+        loc = str(track.get_location())
+        common_path = (
+            music_path / loc.split(str(music_path) + '/', maxsplit=-1)[-1]
+        )
+        track.set_location(config.USB_PATH / common_path)
+    collection.serialize(new_path=other_user_collection)
 
 
 def run_sync(_cmd: str) -> str:
     """Runs subprocess for "aws s3 sync" command. Output is collected and
         formatted such that uploaded tracks are grouped by their directories.
 
     Args:
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/sync/sync_operations.py` & `dj_beatcloud-2.6.0b0/djtools/sync/sync_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 """This module is responsible for syncing tracks between "USB_PATH" and the
-Beatcloud (upload and download). It also handles uploading the Rekordbox XML
-located at "XML_PATH" and downloading the Rekordbox XML uploaded to the
+Beatcloud (upload and download). It also handles uploading the collection
+located at "COLLECTION_PATH" and downloading the collection uploaded to the
 Beatcloud by "IMPORT_USER" before modifying it to point to track locations at
 "USB_PATH".
 """
 import logging
 from os.path import getmtime
 from pathlib import Path
 from subprocess import Popen
 from typing import List, Optional
 
 from djtools.configs.config import BaseConfig
 from djtools.sync.helpers import (
-    parse_sync_command, rewrite_xml, run_sync, webhook
+    parse_sync_command, rewrite_track_paths, run_sync, webhook
 )
 from djtools.utils.check_tracks import compare_tracks
 
 
 logger = logging.getLogger(__name__)
 
 
 def download_music(config: BaseConfig, beatcloud_tracks: Optional[List[str]] = None):
     """This function syncs tracks from the Beatcloud to "USB_PATH".
 
-    If "DOWNLOAD_SPOTIFY" is set to a playlist name that exists in
+    If "DOWNLOAD_SPOTIFY_PLAYLIST" is set to a playlist name that exists in
     "spotify_playlists.yaml", then "DOWNLOAD_INCLUDE_DIRS" will be populated
     with tracks in that playlist that match Beatcloud tracks.
 
     Args:
         config: Configuration object.
         beatcloud_tracks: List of track artist - titles from S3.
     """
-    if config.DOWNLOAD_SPOTIFY:
-        user = config.DOWNLOAD_SPOTIFY.split("Uploads")[0].strip()
+    if config.DOWNLOAD_SPOTIFY_PLAYLIST:
+        user = config.DOWNLOAD_SPOTIFY_PLAYLIST.split("Uploads")[0].strip()
         beatcloud_tracks, beatcloud_matches = compare_tracks(
             config,
             beatcloud_tracks=beatcloud_tracks,
-            download_spotify_playlist=config.DOWNLOAD_SPOTIFY,
+            download_spotify_playlist=config.DOWNLOAD_SPOTIFY_PLAYLIST,
         )
         config.DOWNLOAD_INCLUDE_DIRS = [
             (Path(user) / path.split(f"{Path(user)}/")[-1])
             for path in beatcloud_matches
         ]
         config.DOWNLOAD_EXCLUDE_DIRS = []
 
     dest = Path(config.USB_PATH) / "DJ Music"
     glob_path = (Path("**") / "*.*").as_posix()
     old = {str(p) for p in dest.rglob(glob_path)}
     logger.info(f"Found {len(old)} files")
 
-    logger.info("Syncing remote track collection...")
+    logger.info("Downloading track collection...")
     dest.mkdir(parents=True, exist_ok=True)
     cmd = [
         "aws", "s3", "sync", "s3://dj.beatcloud.com/dj/music/", dest.as_posix()
     ]
     run_sync(parse_sync_command(cmd, config))
 
     new = {str(p) for p in dest.rglob(glob_path)}
@@ -62,42 +62,47 @@
         logger.info(f"Found {len(difference)} new files")
         for diff in difference:
             logger.info(f"\t{diff}")
 
     return beatcloud_tracks
 
 
-def download_xml(config: BaseConfig):
-    """This function downloads the Beatcloud XML of "IMPORT_USER" and modifies
-        the "Location" field of all the tracks so that it points to USER's
-        "USB_PATH".
+def download_collection(config: BaseConfig):
+    """This function downloads the collection of "IMPORT_USER".
+    
+    After downloading "IMPORT_USER"'s collection, the location of all the
+    tracks are modified so that they point to USER's "USB_PATH".
 
     Args:
         config: Configuration object.
     """
-    logger.info("Syncing remote rekordbox.xml...")
-    xml_dir = Path(config.XML_PATH).parent
-    xml_dir.mkdir(parents=True, exist_ok=True)
-    _file = Path(xml_dir) / f'{config.IMPORT_USER}_rekordbox.xml'
+    logger.info(f"Downloading {config.IMPORT_USER}'s collection...")
+    collection_dir = config.COLLECTION_PATH.parent
+    collection_dir.mkdir(parents=True, exist_ok=True)
+    _file = (
+        Path(collection_dir) /
+        f'{config.IMPORT_USER}_{config.COLLECTION_PATH.name}'
+    )
     cmd = (
-        "aws s3 cp s3://dj.beatcloud.com/dj/xml/"
-        f'{config.IMPORT_USER}/rekordbox.xml {_file}'
+        "aws s3 cp s3://dj.beatcloud.com/dj/collections/"
+        f'{config.IMPORT_USER}/collection {_file}'
     )
     logger.info(cmd)
     with Popen(cmd, shell=True) as proc:
         proc.wait()
     if config.USER != config.IMPORT_USER:
-        rewrite_xml(config)
+        rewrite_track_paths(config, _file)
 
 
 def upload_music(config: BaseConfig):
     """This function syncs tracks from "USB_PATH" to the Beatcloud.
-        "AWS_USE_DATE_MODIFIED" can be used in order to re-upload tracks that
-        already exist in the Beatcloud but have been modified since the last
-        time they were uploaded (i.e. ID3 tags have been altered).
+
+    "AWS_USE_DATE_MODIFIED" can be used in order to re-upload tracks that
+    already exist in the Beatcloud but have been modified since the last time
+    they were uploaded (i.e. ID3 tags have been altered).
 
     Args:
         config: Configuration object.
     """
     hidden_files = set(
         (Path(config.USB_PATH) / "DJ Music").rglob(
             (Path("**") / ".*.*").as_posix()
@@ -105,32 +110,32 @@
     )
     if hidden_files:
         logger.info(f"Removed {len(hidden_files)} files...")
         for _file in hidden_files:
             logger.info(f"\t{_file}")
             _file.unlink()
 
-    logger.info("Syncing track collection...")
+    logger.info("Uploading track collection...")
     src = (Path(config.USB_PATH) / "DJ Music").as_posix()
     cmd = ["aws", "s3", "sync", src, "s3://dj.beatcloud.com/dj/music/"]
 
     if config.DISCORD_URL and not config.DRYRUN:
         webhook(
             config.DISCORD_URL,
             content=run_sync(parse_sync_command(cmd, config, upload=True)),
         )
     else:
         run_sync(parse_sync_command(cmd, config, upload=True))
 
 
-def upload_xml(config: BaseConfig):
-    """This function uploads "XML_PATH" to Beatcloud.
+def upload_collection(config: BaseConfig):
+    """This function uploads "COLLECTION_PATH" to the cloud.
 
     Args:
         config: Configuration object.
     """
-    logger.info(f"Uploading {config.USER}'s rekordbox.xml...")
-    dst = f"s3://dj.beatcloud.com/dj/xml/{config.USER}/"
-    cmd = f"aws s3 cp {config.XML_PATH} {dst}"
+    logger.info(f"Uploading {config.USER}'s collection...")
+    dst = f"s3://dj.beatcloud.com/dj/collections/{config.USER}/collection"
+    cmd = f"aws s3 cp {config.COLLECTION_PATH} {dst}"
     logger.info(cmd)
     with Popen(cmd, shell=True) as proc:
         proc.wait()
```

### Comparing `dj_beatcloud-2.5.1b5/djtools/utils/__init__.py` & `dj_beatcloud-2.6.0b0/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b5/djtools/utils/check_tracks.py` & `dj_beatcloud-2.6.0b0/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b5/djtools/utils/config.py` & `dj_beatcloud-2.6.0b0/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b5/djtools/utils/helpers.py` & `dj_beatcloud-2.6.0b0/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b5/djtools/utils/url_download.py` & `dj_beatcloud-2.6.0b0/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b5/setup.py` & `dj_beatcloud-2.6.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,35 +50,32 @@
 version_path = Path(__file__).parent / "djtools" / "version.py"
 with open(version_path, mode="r", encoding="utf-8") as _file:
     VERSION = _file.read().split("=")[-1].strip().replace('"', "")
 
 setup(
     name='dj_beatcloud',
     version=VERSION,
-    description=(
-        'DJ Tools is a library for managing a collection of music and '
-        'Rekordbox XML files.'
-    ),
+    description='DJ Tools is a library for managing a collection of music.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
     author='Alex Richards',
     author_email='alex.richards006@gmail.com',
     license='GNU GPLv3',
     packages=[
         "djtools",
         "djtools.configs",
-        "djtools.rekordbox",
+        "djtools.collections",
         "djtools.spotify",
         "djtools.sync",
         "djtools.utils",
     ],
     classifiers=CLASSIFIERS,
     install_requires=REQUIREMENTS,
     extras_require=EXTRAS,
     python_requires=">=3.6",
     include_package_data=True,
-    keywords='MP3 Rekordbox XML spotify reddit aws s3',
+    keywords='DJ Rekordbox spotify reddit aws s3',
     entry_points={
         'console_scripts': ['djtools=djtools:main']
     },
 )
```

