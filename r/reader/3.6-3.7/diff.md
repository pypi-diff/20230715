# Comparing `tmp/reader-3.6.tar.gz` & `tmp/reader-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reader-3.6.tar", last modified: Thu Jun 15 21:41:04 2023, max compression
+gzip compressed data, was "reader-3.7.tar", last modified: Sat Jul 15 15:40:43 2023, max compression
```

## Comparing `reader-3.6.tar` & `reader-3.7.tar`

### file list

```diff
@@ -1,241 +1,235 @@
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.479325 reader-3.6/
--rw-r--r--   0 lemon      (501) staff       (20)    54796 2023-06-15 21:40:39.000000 reader-3.6/CHANGES.rst
--rw-r--r--   0 lemon      (501) staff       (20)     1475 2021-04-07 12:51:45.000000 reader-3.6/LICENSE
--rw-r--r--   0 lemon      (501) staff       (20)      406 2022-06-28 21:13:50.000000 reader-3.6/MANIFEST.in
--rw-r--r--   0 lemon      (501) staff       (20)     5410 2023-06-15 21:41:04.479606 reader-3.6/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     3501 2023-04-30 15:42:17.000000 reader-3.6/README.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.290879 reader-3.6/docs/
--rw-r--r--   0 lemon      (501) staff       (20)      604 2020-10-28 07:20:55.000000 reader-3.6/docs/Makefile
--rw-r--r--   0 lemon      (501) staff       (20)     2956 2023-05-04 19:18:28.000000 reader-3.6/docs/api.rst
--rw-r--r--   0 lemon      (501) staff       (20)     3007 2023-06-08 16:51:43.000000 reader-3.6/docs/app.rst
--rw-r--r--   0 lemon      (501) staff       (20)       29 2020-10-28 07:20:55.000000 reader-3.6/docs/changelog.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2164 2023-06-08 16:56:19.000000 reader-3.6/docs/cli.rst
--rw-r--r--   0 lemon      (501) staff       (20)     3368 2023-06-05 20:23:53.000000 reader-3.6/docs/conf.py
--rw-r--r--   0 lemon      (501) staff       (20)     1147 2020-10-28 07:23:47.000000 reader-3.6/docs/config.rst
--rw-r--r--   0 lemon      (501) staff       (20)       33 2023-05-04 06:00:46.000000 reader-3.6/docs/contributing.rst
--rw-r--r--   0 lemon      (501) staff       (20)     3062 2023-04-29 12:30:57.000000 reader-3.6/docs/dev-app.rst
--rw-r--r--   0 lemon      (501) staff       (20)    15936 2023-06-08 17:00:43.000000 reader-3.6/docs/dev.rst
--rw-r--r--   0 lemon      (501) staff       (20)    29113 2023-05-12 22:28:36.000000 reader-3.6/docs/guide.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.291727 reader-3.6/docs/images/
--rw-r--r--   0 lemon      (501) staff       (20)    36483 2020-10-28 07:20:31.000000 reader-3.6/docs/images/redesign-01.png
--rw-r--r--   0 lemon      (501) staff       (20)     1595 2023-05-04 19:59:30.000000 reader-3.6/docs/index.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2920 2022-12-29 21:45:24.000000 reader-3.6/docs/install.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2227 2023-03-19 14:35:51.000000 reader-3.6/docs/internal.rst
--rw-r--r--   0 lemon      (501) staff       (20)      810 2020-10-28 07:19:52.000000 reader-3.6/docs/make.bat
--rw-r--r--   0 lemon      (501) staff       (20)     2092 2022-07-08 20:32:37.000000 reader-3.6/docs/plugins.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.315450 reader-3.6/docs/screenshots/
--rw-r--r--   0 lemon      (501) staff       (20)    68106 2020-10-28 07:20:31.000000 reader-3.6/docs/screenshots/dillo.png
--rw-r--r--   0 lemon      (501) staff       (20)   109426 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/entries-feed.png
--rw-r--r--   0 lemon      (501) staff       (20)    96393 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/entries.png
--rw-r--r--   0 lemon      (501) staff       (20)   277564 2022-07-09 07:30:35.000000 reader-3.6/docs/screenshots/entry-one.png
--rw-r--r--   0 lemon      (501) staff       (20)   128002 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/entry-two.png
--rw-r--r--   0 lemon      (501) staff       (20)    48411 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/feeds.png
--rw-r--r--   0 lemon      (501) staff       (20)   364336 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/lynx.png
--rw-r--r--   0 lemon      (501) staff       (20)   111458 2020-10-28 07:22:31.000000 reader-3.6/docs/screenshots/search.png
--rw-r--r--   0 lemon      (501) staff       (20)   135812 2022-06-27 22:00:00.000000 reader-3.6/docs/screenshots/twitter-one.png
--rw-r--r--   0 lemon      (501) staff       (20)   385070 2022-07-01 13:21:27.000000 reader-3.6/docs/screenshots/twitter-two.png
--rw-r--r--   0 lemon      (501) staff       (20)     9271 2023-01-16 22:55:01.000000 reader-3.6/docs/tutorial.rst
--rw-r--r--   0 lemon      (501) staff       (20)     2290 2023-05-04 20:38:52.000000 reader-3.6/docs/why.rst
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.322555 reader-3.6/examples/
--rw-r--r--   0 lemon      (501) staff       (20)     2713 2021-05-05 18:41:19.000000 reader-3.6/examples/config.yaml
--rw-r--r--   0 lemon      (501) staff       (20)     1639 2023-01-16 23:03:30.000000 reader-3.6/examples/parser_only.py
--rw-r--r--   0 lemon      (501) staff       (20)     1596 2022-01-20 22:05:30.000000 reader-3.6/examples/podcast.py
--rw-r--r--   0 lemon      (501) staff       (20)     1819 2020-12-23 13:16:52.000000 reader-3.6/examples/terminal.py
--rw-r--r--   0 lemon      (501) staff       (20)       90 2021-06-08 13:32:02.000000 reader-3.6/pyproject.toml
--rwxr-xr-x   0 lemon      (501) staff       (20)     3831 2023-05-04 14:35:44.000000 reader-3.6/run.sh
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.330830 reader-3.6/scripts/
--rw-r--r--   0 lemon      (501) staff       (20)    53248 2020-06-23 14:22:09.000000 reader-3.6/scripts/.coverage
--rwxr-xr-x   0 lemon      (501) staff       (20)      559 2023-01-28 10:01:54.000000 reader-3.6/scripts/backup.sh
--rw-r--r--   0 lemon      (501) staff       (20)    13837 2022-12-31 08:17:16.000000 reader-3.6/scripts/bench.py
--rw-r--r--   0 lemon      (501) staff       (20)     4340 2022-12-31 08:17:15.000000 reader-3.6/scripts/debug_storage_stats.py
--rw-r--r--   0 lemon      (501) staff       (20)      356 2022-06-28 20:55:42.000000 reader-3.6/scripts/generate_import_all.py
--rw-r--r--   0 lemon      (501) staff       (20)     5021 2020-10-28 07:24:20.000000 reader-3.6/scripts/jscontrols.html
--rw-r--r--   0 lemon      (501) staff       (20)     1211 2020-10-28 07:24:20.000000 reader-3.6/scripts/jscontrols.py
--rwxr-xr-x   0 lemon      (501) staff       (20)      764 2020-10-28 07:21:42.000000 reader-3.6/scripts/lines.sh
--rw-r--r--   0 lemon      (501) staff       (20)     4600 2022-12-31 08:17:15.000000 reader-3.6/scripts/release.py
--rw-r--r--   0 lemon      (501) staff       (20)     3398 2023-06-15 21:41:04.482902 reader-3.6/setup.cfg
--rw-r--r--   0 lemon      (501) staff       (20)       38 2021-04-26 16:52:55.000000 reader-3.6/setup.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.265334 reader-3.6/src/
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.355346 reader-3.6/src/reader/
--rw-r--r--   0 lemon      (501) staff       (20)     2532 2023-06-15 21:40:39.000000 reader-3.6/src/reader/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      381 2020-10-28 07:22:22.000000 reader-3.6/src/reader/__main__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.362072 reader-3.6/src/reader/_app/
--rw-r--r--   0 lemon      (501) staff       (20)    22629 2023-03-05 14:28:08.000000 reader-3.6/src/reader/_app/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     4329 2022-12-31 08:17:16.000000 reader-3.6/src/reader/_app/api_thing.py
--rw-r--r--   0 lemon      (501) staff       (20)     1457 2021-10-30 11:02:39.000000 reader-3.6/src/reader/_app/cli.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.363642 reader-3.6/src/reader/_app/static/
--rw-r--r--   0 lemon      (501) staff       (20)    14735 2022-06-23 20:50:42.000000 reader-3.6/src/reader/_app/static/controls.js
--rw-r--r--   0 lemon      (501) staff       (20)     4194 2022-06-22 19:10:26.000000 reader-3.6/src/reader/_app/static/style.css
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.370852 reader-3.6/src/reader/_app/templates/
--rw-r--r--   0 lemon      (501) staff       (20)      980 2021-10-27 17:55:28.000000 reader-3.6/src/reader/_app/templates/add_entry.html
--rw-r--r--   0 lemon      (501) staff       (20)    12029 2023-03-05 14:26:36.000000 reader-3.6/src/reader/_app/templates/entries.html
--rw-r--r--   0 lemon      (501) staff       (20)     3200 2023-02-14 22:28:37.000000 reader-3.6/src/reader/_app/templates/entry.html
--rw-r--r--   0 lemon      (501) staff       (20)     5083 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_app/templates/feeds.html
--rw-r--r--   0 lemon      (501) staff       (20)     1631 2022-03-11 23:07:17.000000 reader-3.6/src/reader/_app/templates/layout.html
--rw-r--r--   0 lemon      (501) staff       (20)     9375 2023-03-05 14:18:18.000000 reader-3.6/src/reader/_app/templates/macros.html
--rw-r--r--   0 lemon      (501) staff       (20)     2569 2022-07-30 08:02:27.000000 reader-3.6/src/reader/_app/templates/metadata.html
--rw-r--r--   0 lemon      (501) staff       (20)     1515 2021-08-17 08:51:46.000000 reader-3.6/src/reader/_app/templates/tags.html
--rw-r--r--   0 lemon      (501) staff       (20)     1150 2020-10-28 07:23:44.000000 reader-3.6/src/reader/_app/wsgi.py
--rw-r--r--   0 lemon      (501) staff       (20)    13132 2022-12-31 08:17:16.000000 reader-3.6/src/reader/_cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     4587 2022-07-16 20:45:27.000000 reader-3.6/src/reader/_config.py
--rw-r--r--   0 lemon      (501) staff       (20)     1531 2023-01-17 22:12:52.000000 reader-3.6/src/reader/_feedparser.py
--rw-r--r--   0 lemon      (501) staff       (20)     4074 2022-12-18 08:53:24.000000 reader-3.6/src/reader/_feedparser_lazy.py
--rw-r--r--   0 lemon      (501) staff       (20)     2980 2023-03-14 06:52:53.000000 reader-3.6/src/reader/_hash_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     2220 2022-12-31 08:18:29.000000 reader-3.6/src/reader/_html_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     7493 2023-06-08 21:12:49.000000 reader-3.6/src/reader/_http_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     5677 2023-01-17 22:12:52.000000 reader-3.6/src/reader/_jsonfeed.py
--rw-r--r--   0 lemon      (501) staff       (20)    24586 2023-03-19 13:56:03.000000 reader-3.6/src/reader/_parser.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.376954 reader-3.6/src/reader/_plugins/
--rw-r--r--   0 lemon      (501) staff       (20)     1617 2022-12-29 21:54:33.000000 reader-3.6/src/reader/_plugins/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     3201 2021-11-05 08:41:21.000000 reader-3.6/src/reader/_plugins/cli_status.py
--rw-r--r--   0 lemon      (501) staff       (20)     3065 2022-12-29 22:18:56.000000 reader-3.6/src/reader/_plugins/enclosure_tags.py
--rw-r--r--   0 lemon      (501) staff       (20)     4561 2023-01-01 10:20:44.000000 reader-3.6/src/reader/_plugins/preview_feed_list.py
--rw-r--r--   0 lemon      (501) staff       (20)     2931 2022-06-27 21:01:33.000000 reader-3.6/src/reader/_plugins/sqlite_releases.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.378209 reader-3.6/src/reader/_plugins/templates/
--rw-r--r--   0 lemon      (501) staff       (20)      815 2022-12-27 22:01:52.000000 reader-3.6/src/reader/_plugins/templates/preview_feed_list.html
--rw-r--r--   0 lemon      (501) staff       (20)     2094 2022-11-21 20:16:44.000000 reader-3.6/src/reader/_plugins/tumblr_gdpr.py
--rw-r--r--   0 lemon      (501) staff       (20)    26547 2023-06-15 21:32:39.000000 reader-3.6/src/reader/_plugins/twitter.py
--rw-r--r--   0 lemon      (501) staff       (20)     7785 2023-01-17 21:52:55.000000 reader-3.6/src/reader/_requests_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)      726 2023-01-01 10:22:19.000000 reader-3.6/src/reader/_requests_utils_lazy.py
--rw-r--r--   0 lemon      (501) staff       (20)     5623 2023-01-01 10:41:25.000000 reader-3.6/src/reader/_retrievers.py
--rw-r--r--   0 lemon      (501) staff       (20)    34166 2023-03-03 21:46:20.000000 reader-3.6/src/reader/_search.py
--rw-r--r--   0 lemon      (501) staff       (20)     8256 2022-12-31 09:50:28.000000 reader-3.6/src/reader/_sql_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    24243 2022-12-31 08:26:13.000000 reader-3.6/src/reader/_sqlite_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    53646 2023-03-19 14:35:50.000000 reader-3.6/src/reader/_storage.py
--rw-r--r--   0 lemon      (501) staff       (20)    16419 2023-03-14 06:54:33.000000 reader-3.6/src/reader/_types.py
--rw-r--r--   0 lemon      (501) staff       (20)    16725 2022-12-31 08:26:13.000000 reader-3.6/src/reader/_update.py
--rw-r--r--   0 lemon      (501) staff       (20)     4224 2022-12-31 08:10:27.000000 reader-3.6/src/reader/_url_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     9052 2022-12-31 08:26:29.000000 reader-3.6/src/reader/_utils.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.378839 reader-3.6/src/reader/_vendor/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2020-10-28 07:24:12.000000 reader-3.6/src/reader/_vendor/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.388612 reader-3.6/src/reader/_vendor/feedparser/
--rw-r--r--   0 lemon      (501) staff       (20)     2715 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)    16169 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/api.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.395132 reader-3.6/src/reader/_vendor/feedparser/datetimes/
--rw-r--r--   0 lemon      (501) staff       (20)     2905 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     2380 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/asctime.py
--rw-r--r--   0 lemon      (501) staff       (20)     4022 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/greek.py
--rw-r--r--   0 lemon      (501) staff       (20)     2945 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/hungarian.py
--rw-r--r--   0 lemon      (501) staff       (20)     5459 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/iso8601.py
--rw-r--r--   0 lemon      (501) staff       (20)     3354 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/korean.py
--rw-r--r--   0 lemon      (501) staff       (20)     2198 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/perforce.py
--rw-r--r--   0 lemon      (501) staff       (20)     5423 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/rfc822.py
--rw-r--r--   0 lemon      (501) staff       (20)     4506 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/datetimes/w3dtf.py
--rw-r--r--   0 lemon      (501) staff       (20)    21181 2022-02-12 10:04:56.000000 reader-3.6/src/reader/_vendor/feedparser/encodings.py
--rw-r--r--   0 lemon      (501) staff       (20)     1897 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/exceptions.py
--rw-r--r--   0 lemon      (501) staff       (20)    10791 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/html.py
--rw-r--r--   0 lemon      (501) staff       (20)     9834 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/http.py
--rw-r--r--   0 lemon      (501) staff       (20)    32296 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/mixin.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.403217 reader-3.6/src/reader/_vendor/feedparser/namespaces/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)    16998 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/_base.py
--rw-r--r--   0 lemon      (501) staff       (20)     2317 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/admin.py
--rw-r--r--   0 lemon      (501) staff       (20)     2866 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/cc.py
--rw-r--r--   0 lemon      (501) staff       (20)     4446 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/dc.py
--rw-r--r--   0 lemon      (501) staff       (20)    11399 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/georss.py
--rw-r--r--   0 lemon      (501) staff       (20)     4115 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/itunes.py
--rw-r--r--   0 lemon      (501) staff       (20)     5336 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/mediarss.py
--rw-r--r--   0 lemon      (501) staff       (20)     2839 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/namespaces/psc.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.405841 reader-3.6/src/reader/_vendor/feedparser/parsers/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     4729 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/json.py
--rw-r--r--   0 lemon      (501) staff       (20)     3420 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/loose.py
--rw-r--r--   0 lemon      (501) staff       (20)     5805 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/parsers/strict.py
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/py.typed
--rw-r--r--   0 lemon      (501) staff       (20)    23731 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/sanitizer.py
--rw-r--r--   0 lemon      (501) staff       (20)     3517 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/sgml.py
--rw-r--r--   0 lemon      (501) staff       (20)     5487 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/urls.py
--rw-r--r--   0 lemon      (501) staff       (20)     6448 2022-02-11 15:50:56.000000 reader-3.6/src/reader/_vendor/feedparser/util.py
--rw-r--r--   0 lemon      (501) staff       (20)    71461 2023-03-19 13:58:22.000000 reader-3.6/src/reader/core.py
--rw-r--r--   0 lemon      (501) staff       (20)     6149 2022-12-31 08:26:06.000000 reader-3.6/src/reader/exceptions.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.411224 reader-3.6/src/reader/plugins/
--rw-r--r--   0 lemon      (501) staff       (20)     1503 2022-12-31 08:26:13.000000 reader-3.6/src/reader/plugins/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      798 2021-03-26 12:03:04.000000 reader-3.6/src/reader/plugins/enclosure_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)    16705 2023-01-29 20:48:33.000000 reader-3.6/src/reader/plugins/entry_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)     2734 2023-03-18 22:45:04.000000 reader-3.6/src/reader/plugins/mark_as_read.py
--rw-r--r--   0 lemon      (501) staff       (20)     4678 2022-09-14 19:27:33.000000 reader-3.6/src/reader/plugins/readtime.py
--rw-r--r--   0 lemon      (501) staff       (20)     1626 2022-12-18 09:01:52.000000 reader-3.6/src/reader/plugins/ua_fallback.py
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-06-28 20:04:35.000000 reader-3.6/src/reader/py.typed
--rw-r--r--   0 lemon      (501) staff       (20)    28282 2023-03-18 22:18:25.000000 reader-3.6/src/reader/types.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.358296 reader-3.6/src/reader.egg-info/
--rw-r--r--   0 lemon      (501) staff       (20)     5410 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     6279 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/SOURCES.txt
--rw-r--r--   0 lemon      (501) staff       (20)        1 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/dependency_links.txt
--rw-r--r--   0 lemon      (501) staff       (20)      653 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/requires.txt
--rw-r--r--   0 lemon      (501) staff       (20)        7 2023-06-15 21:41:04.000000 reader-3.6/src/reader.egg-info/top_level.txt
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.455378 reader-3.6/tests/
--rw-r--r--   0 lemon      (501) staff       (20)     4829 2023-03-05 10:19:51.000000 reader-3.6/tests/conftest.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.475654 reader-3.6/tests/data/
--rw-r--r--   0 lemon      (501) staff       (20)       69 2021-10-18 18:44:15.000000 reader-3.6/tests/data/10.json
--rw-r--r--   0 lemon      (501) staff       (20)      231 2022-12-31 08:17:15.000000 reader-3.6/tests/data/10.json.py
--rw-r--r--   0 lemon      (501) staff       (20)       12 2021-01-28 12:46:50.000000 reader-3.6/tests/data/custom
--rw-r--r--   0 lemon      (501) staff       (20)      180 2020-10-28 07:20:07.000000 reader-3.6/tests/data/empty.atom
--rw-r--r--   0 lemon      (501) staff       (20)      446 2022-12-31 08:17:17.000000 reader-3.6/tests/data/empty.atom.py
--rw-r--r--   0 lemon      (501) staff       (20)      157 2021-01-28 10:55:34.000000 reader-3.6/tests/data/empty.json
--rw-r--r--   0 lemon      (501) staff       (20)      455 2022-12-31 08:17:15.000000 reader-3.6/tests/data/empty.json.py
--rw-r--r--   0 lemon      (501) staff       (20)      191 2020-10-28 07:20:07.000000 reader-3.6/tests/data/empty.rss
--rw-r--r--   0 lemon      (501) staff       (20)      326 2022-12-31 08:17:16.000000 reader-3.6/tests/data/empty.rss.py
--rw-r--r--   0 lemon      (501) staff       (20)     1551 2022-03-26 15:46:54.000000 reader-3.6/tests/data/full.atom
--rw-r--r--   0 lemon      (501) staff       (20)     2327 2022-12-31 08:17:15.000000 reader-3.6/tests/data/full.atom.py
--rw-r--r--   0 lemon      (501) staff       (20)     1743 2021-10-18 18:27:51.000000 reader-3.6/tests/data/full.json
--rw-r--r--   0 lemon      (501) staff       (20)     1760 2022-12-31 08:17:16.000000 reader-3.6/tests/data/full.json.py
--rw-r--r--   0 lemon      (501) staff       (20)     1401 2021-06-08 19:16:41.000000 reader-3.6/tests/data/full.rss
--rw-r--r--   0 lemon      (501) staff       (20)     1523 2022-12-31 08:17:15.000000 reader-3.6/tests/data/full.rss.py
--rw-r--r--   0 lemon      (501) staff       (20)     2024 2021-01-28 13:31:45.000000 reader-3.6/tests/data/invalid.json
--rw-r--r--   0 lemon      (501) staff       (20)     1290 2022-12-31 08:17:16.000000 reader-3.6/tests/data/invalid.json.py
--rw-r--r--   0 lemon      (501) staff       (20)      577 2020-10-28 07:22:29.000000 reader-3.6/tests/data/relative.atom
--rw-r--r--   0 lemon      (501) staff       (20)      906 2022-12-31 08:17:20.000000 reader-3.6/tests/data/relative.atom.py
--rw-r--r--   0 lemon      (501) staff       (20)      560 2020-10-28 07:22:29.000000 reader-3.6/tests/data/relative.rss
--rw-r--r--   0 lemon      (501) staff       (20)      907 2022-12-31 08:17:15.000000 reader-3.6/tests/data/relative.rss.py
--rw-r--r--   0 lemon      (501) staff       (20)      629 2021-01-28 18:18:08.000000 reader-3.6/tests/data/sqlite_releases.html
--rw-r--r--   0 lemon      (501) staff       (20)       72 2021-10-18 18:48:17.000000 reader-3.6/tests/data/unknown.json
--rw-r--r--   0 lemon      (501) staff       (20)      234 2022-12-31 08:17:17.000000 reader-3.6/tests/data/unknown.json.py
--rw-r--r--   0 lemon      (501) staff       (20)     4468 2023-01-17 22:12:52.000000 reader-3.6/tests/fakeparser.py
--rw-r--r--   0 lemon      (501) staff       (20)     2440 2023-03-05 10:19:51.000000 reader-3.6/tests/reader_methods.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-06-15 21:41:04.478810 reader-3.6/tests/reader_test_plugins/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2022-03-27 11:01:36.000000 reader-3.6/tests/reader_test_plugins/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)       34 2022-03-27 11:03:08.000000 reader-3.6/tests/reader_test_plugins/good.py
--rw-r--r--   0 lemon      (501) staff       (20)       59 2022-07-25 20:59:03.000000 reader-3.6/tests/reader_test_plugins/init_error.py
--rw-r--r--   0 lemon      (501) staff       (20)       73 2022-03-27 11:08:08.000000 reader-3.6/tests/reader_test_plugins/missing_dependency.py
--rw-r--r--   0 lemon      (501) staff       (20)       24 2022-03-27 11:08:24.000000 reader-3.6/tests/reader_test_plugins/missing_entry_point.py
--rw-r--r--   0 lemon      (501) staff       (20)     5534 2023-03-05 10:19:52.000000 reader-3.6/tests/test__types.py
--rw-r--r--   0 lemon      (501) staff       (20)     9097 2023-06-08 21:15:29.000000 reader-3.6/tests/test_app.py
--rw-r--r--   0 lemon      (501) staff       (20)      654 2020-10-28 07:22:21.000000 reader-3.6/tests/test_app_wsgi.py
--rw-r--r--   0 lemon      (501) staff       (20)     1028 2021-01-28 18:37:51.000000 reader-3.6/tests/test_bench.py
--rw-r--r--   0 lemon      (501) staff       (20)    11712 2023-01-23 15:26:55.000000 reader-3.6/tests/test_cli.py
--rw-r--r--   0 lemon      (501) staff       (20)     3055 2021-03-26 16:15:01.000000 reader-3.6/tests/test_config.py
--rw-r--r--   0 lemon      (501) staff       (20)     1815 2022-07-25 20:59:03.000000 reader-3.6/tests/test_exceptions.py
--rw-r--r--   0 lemon      (501) staff       (20)     2477 2021-03-19 09:00:44.000000 reader-3.6/tests/test_hash_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     2246 2022-08-21 15:09:18.000000 reader-3.6/tests/test_html_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     1319 2023-04-30 09:15:21.000000 reader-3.6/tests/test_http_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     3229 2023-04-30 09:15:21.000000 reader-3.6/tests/test_lazy_imports.py
--rw-r--r--   0 lemon      (501) staff       (20)    33547 2023-01-23 15:11:14.000000 reader-3.6/tests/test_parser.py
--rw-r--r--   0 lemon      (501) staff       (20)      702 2021-11-04 22:22:57.000000 reader-3.6/tests/test_plugins_cli_status.py
--rw-r--r--   0 lemon      (501) staff       (20)      915 2022-12-31 08:17:15.000000 reader-3.6/tests/test_plugins_enclosure_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)    22348 2023-01-29 21:01:09.000000 reader-3.6/tests/test_plugins_entry_dedupe.py
--rw-r--r--   0 lemon      (501) staff       (20)     3393 2023-01-29 20:48:19.000000 reader-3.6/tests/test_plugins_mark_as_read.py
--rw-r--r--   0 lemon      (501) staff       (20)     3159 2022-12-27 22:17:35.000000 reader-3.6/tests/test_plugins_preview_feed_list.py
--rw-r--r--   0 lemon      (501) staff       (20)     6610 2022-09-14 19:27:33.000000 reader-3.6/tests/test_plugins_readtime.py
--rw-r--r--   0 lemon      (501) staff       (20)     2467 2023-01-23 15:09:42.000000 reader-3.6/tests/test_plugins_sqlite_releases.py
--rw-r--r--   0 lemon      (501) staff       (20)      118 2020-10-28 07:22:21.000000 reader-3.6/tests/test_plugins_tumblr_gdpr.py
--rw-r--r--   0 lemon      (501) staff       (20)    34750 2022-11-06 15:48:05.000000 reader-3.6/tests/test_plugins_twitter.py
--rw-r--r--   0 lemon      (501) staff       (20)     1070 2022-12-31 08:17:15.000000 reader-3.6/tests/test_plugins_ua_fallback.py
--rw-r--r--   0 lemon      (501) staff       (20)    94505 2023-03-05 10:19:56.000000 reader-3.6/tests/test_reader.py
--rw-r--r--   0 lemon      (501) staff       (20)     8018 2022-07-30 08:23:00.000000 reader-3.6/tests/test_reader_context.py
--rw-r--r--   0 lemon      (501) staff       (20)       99 2021-07-17 15:02:59.000000 reader-3.6/tests/test_reader_deprecations.py
--rw-r--r--   0 lemon      (501) staff       (20)     8028 2022-12-31 08:17:16.000000 reader-3.6/tests/test_reader_hooks.py
--rw-r--r--   0 lemon      (501) staff       (20)     5885 2023-01-23 15:26:18.000000 reader-3.6/tests/test_reader_integration.py
--rw-r--r--   0 lemon      (501) staff       (20)     2617 2022-07-25 20:59:03.000000 reader-3.6/tests/test_reader_plugins.py
--rw-r--r--   0 lemon      (501) staff       (20)     7248 2022-12-31 08:17:15.000000 reader-3.6/tests/test_reader_private.py
--rw-r--r--   0 lemon      (501) staff       (20)    33613 2022-08-21 15:09:18.000000 reader-3.6/tests/test_reader_search.py
--rw-r--r--   0 lemon      (501) staff       (20)     7103 2022-08-29 19:45:44.000000 reader-3.6/tests/test_reader_sort.py
--rw-r--r--   0 lemon      (501) staff       (20)     5683 2022-08-21 15:09:18.000000 reader-3.6/tests/test_search.py
--rw-r--r--   0 lemon      (501) staff       (20)     4724 2021-05-21 12:10:53.000000 reader-3.6/tests/test_sql_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    11991 2022-03-16 22:01:23.000000 reader-3.6/tests/test_sqlite_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    17626 2023-03-03 21:47:06.000000 reader-3.6/tests/test_storage.py
--rw-r--r--   0 lemon      (501) staff       (20)    12402 2022-08-21 15:09:18.000000 reader-3.6/tests/test_tags.py
--rw-r--r--   0 lemon      (501) staff       (20)     1129 2020-10-28 07:23:39.000000 reader-3.6/tests/test_test_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)    11006 2022-09-09 21:29:27.000000 reader-3.6/tests/test_types.py
--rw-r--r--   0 lemon      (501) staff       (20)     2516 2022-07-19 22:03:54.000000 reader-3.6/tests/test_utils.py
--rw-r--r--   0 lemon      (501) staff       (20)     3077 2023-01-23 14:51:43.000000 reader-3.6/tests/utils.py
--rw-r--r--   0 lemon      (501) staff       (20)      698 2022-12-29 21:11:03.000000 reader-3.6/tox.ini
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.606077 reader-3.7/
+-rw-r--r--   0 lemon      (501) staff       (20)    55126 2023-07-15 15:40:20.000000 reader-3.7/CHANGES.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     1475 2021-04-07 12:51:45.000000 reader-3.7/LICENSE
+-rw-r--r--   0 lemon      (501) staff       (20)      406 2022-06-28 21:13:50.000000 reader-3.7/MANIFEST.in
+-rw-r--r--   0 lemon      (501) staff       (20)     5367 2023-07-15 15:40:43.606410 reader-3.7/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     3458 2023-07-15 08:22:17.000000 reader-3.7/README.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.352450 reader-3.7/docs/
+-rw-r--r--   0 lemon      (501) staff       (20)      604 2020-10-28 07:20:55.000000 reader-3.7/docs/Makefile
+-rw-r--r--   0 lemon      (501) staff       (20)     2956 2023-05-04 19:18:28.000000 reader-3.7/docs/api.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     3007 2023-06-08 16:51:43.000000 reader-3.7/docs/app.rst
+-rw-r--r--   0 lemon      (501) staff       (20)       29 2020-10-28 07:20:55.000000 reader-3.7/docs/changelog.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2164 2023-06-08 16:56:19.000000 reader-3.7/docs/cli.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     3368 2023-06-05 20:23:53.000000 reader-3.7/docs/conf.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1147 2020-10-28 07:23:47.000000 reader-3.7/docs/config.rst
+-rw-r--r--   0 lemon      (501) staff       (20)       33 2023-05-04 06:00:46.000000 reader-3.7/docs/contributing.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     3062 2023-04-29 12:30:57.000000 reader-3.7/docs/dev-app.rst
+-rw-r--r--   0 lemon      (501) staff       (20)    17680 2023-07-15 13:16:29.000000 reader-3.7/docs/dev.rst
+-rw-r--r--   0 lemon      (501) staff       (20)    29113 2023-05-12 22:28:36.000000 reader-3.7/docs/guide.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.353094 reader-3.7/docs/images/
+-rw-r--r--   0 lemon      (501) staff       (20)    36483 2020-10-28 07:20:31.000000 reader-3.7/docs/images/redesign-01.png
+-rw-r--r--   0 lemon      (501) staff       (20)     1595 2023-05-04 19:59:30.000000 reader-3.7/docs/index.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2920 2022-12-29 21:45:24.000000 reader-3.7/docs/install.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2240 2023-07-15 09:11:02.000000 reader-3.7/docs/internal.rst
+-rw-r--r--   0 lemon      (501) staff       (20)      810 2020-10-28 07:19:52.000000 reader-3.7/docs/make.bat
+-rw-r--r--   0 lemon      (501) staff       (20)     3158 2023-07-15 11:47:01.000000 reader-3.7/docs/plugins.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.370917 reader-3.7/docs/screenshots/
+-rw-r--r--   0 lemon      (501) staff       (20)    68106 2020-10-28 07:20:31.000000 reader-3.7/docs/screenshots/dillo.png
+-rw-r--r--   0 lemon      (501) staff       (20)   109426 2020-10-28 07:22:31.000000 reader-3.7/docs/screenshots/entries-feed.png
+-rw-r--r--   0 lemon      (501) staff       (20)    96393 2020-10-28 07:22:31.000000 reader-3.7/docs/screenshots/entries.png
+-rw-r--r--   0 lemon      (501) staff       (20)   277564 2022-07-09 07:30:35.000000 reader-3.7/docs/screenshots/entry-one.png
+-rw-r--r--   0 lemon      (501) staff       (20)   128002 2020-10-28 07:22:31.000000 reader-3.7/docs/screenshots/entry-two.png
+-rw-r--r--   0 lemon      (501) staff       (20)    48411 2020-10-28 07:22:31.000000 reader-3.7/docs/screenshots/feeds.png
+-rw-r--r--   0 lemon      (501) staff       (20)   364336 2020-10-28 07:22:31.000000 reader-3.7/docs/screenshots/lynx.png
+-rw-r--r--   0 lemon      (501) staff       (20)   111458 2020-10-28 07:22:31.000000 reader-3.7/docs/screenshots/search.png
+-rw-r--r--   0 lemon      (501) staff       (20)     9271 2023-01-16 22:55:01.000000 reader-3.7/docs/tutorial.rst
+-rw-r--r--   0 lemon      (501) staff       (20)     2238 2023-07-15 08:28:44.000000 reader-3.7/docs/why.rst
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.375290 reader-3.7/examples/
+-rw-r--r--   0 lemon      (501) staff       (20)     2710 2023-07-15 11:43:57.000000 reader-3.7/examples/config.yaml
+-rw-r--r--   0 lemon      (501) staff       (20)     1639 2023-01-16 23:03:30.000000 reader-3.7/examples/parser_only.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1596 2022-01-20 22:05:30.000000 reader-3.7/examples/podcast.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1819 2020-12-23 13:16:52.000000 reader-3.7/examples/terminal.py
+-rw-r--r--   0 lemon      (501) staff       (20)       90 2021-06-08 13:32:02.000000 reader-3.7/pyproject.toml
+-rwxr-xr-x   0 lemon      (501) staff       (20)     3831 2023-05-04 14:35:44.000000 reader-3.7/run.sh
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.391432 reader-3.7/scripts/
+-rw-r--r--   0 lemon      (501) staff       (20)    53248 2020-06-23 14:22:09.000000 reader-3.7/scripts/.coverage
+-rwxr-xr-x   0 lemon      (501) staff       (20)      559 2023-01-28 10:01:54.000000 reader-3.7/scripts/backup.sh
+-rw-r--r--   0 lemon      (501) staff       (20)    13837 2022-12-31 08:17:16.000000 reader-3.7/scripts/bench.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4340 2022-12-31 08:17:15.000000 reader-3.7/scripts/debug_storage_stats.py
+-rw-r--r--   0 lemon      (501) staff       (20)      356 2022-06-28 20:55:42.000000 reader-3.7/scripts/generate_import_all.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5021 2020-10-28 07:24:20.000000 reader-3.7/scripts/jscontrols.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1211 2020-10-28 07:24:20.000000 reader-3.7/scripts/jscontrols.py
+-rwxr-xr-x   0 lemon      (501) staff       (20)      764 2020-10-28 07:21:42.000000 reader-3.7/scripts/lines.sh
+-rw-r--r--   0 lemon      (501) staff       (20)     4600 2022-12-31 08:17:15.000000 reader-3.7/scripts/release.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3590 2023-07-15 15:40:43.610358 reader-3.7/setup.cfg
+-rw-r--r--   0 lemon      (501) staff       (20)       38 2021-04-26 16:52:55.000000 reader-3.7/setup.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.328516 reader-3.7/src/
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.433121 reader-3.7/src/reader/
+-rw-r--r--   0 lemon      (501) staff       (20)     2532 2023-07-15 15:40:20.000000 reader-3.7/src/reader/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      381 2020-10-28 07:22:22.000000 reader-3.7/src/reader/__main__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.439165 reader-3.7/src/reader/_app/
+-rw-r--r--   0 lemon      (501) staff       (20)    22629 2023-03-05 14:28:08.000000 reader-3.7/src/reader/_app/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4329 2022-12-31 08:17:16.000000 reader-3.7/src/reader/_app/api_thing.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1457 2021-10-30 11:02:39.000000 reader-3.7/src/reader/_app/cli.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.440514 reader-3.7/src/reader/_app/static/
+-rw-r--r--   0 lemon      (501) staff       (20)    14735 2022-06-23 20:50:42.000000 reader-3.7/src/reader/_app/static/controls.js
+-rw-r--r--   0 lemon      (501) staff       (20)     4194 2022-06-22 19:10:26.000000 reader-3.7/src/reader/_app/static/style.css
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.448179 reader-3.7/src/reader/_app/templates/
+-rw-r--r--   0 lemon      (501) staff       (20)      980 2021-10-27 17:55:28.000000 reader-3.7/src/reader/_app/templates/add_entry.html
+-rw-r--r--   0 lemon      (501) staff       (20)    12029 2023-03-05 14:26:36.000000 reader-3.7/src/reader/_app/templates/entries.html
+-rw-r--r--   0 lemon      (501) staff       (20)     3200 2023-02-14 22:28:37.000000 reader-3.7/src/reader/_app/templates/entry.html
+-rw-r--r--   0 lemon      (501) staff       (20)     5083 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_app/templates/feeds.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1631 2022-03-11 23:07:17.000000 reader-3.7/src/reader/_app/templates/layout.html
+-rw-r--r--   0 lemon      (501) staff       (20)     9375 2023-03-05 14:18:18.000000 reader-3.7/src/reader/_app/templates/macros.html
+-rw-r--r--   0 lemon      (501) staff       (20)     2569 2022-07-30 08:02:27.000000 reader-3.7/src/reader/_app/templates/metadata.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1515 2021-08-17 08:51:46.000000 reader-3.7/src/reader/_app/templates/tags.html
+-rw-r--r--   0 lemon      (501) staff       (20)     1150 2020-10-28 07:23:44.000000 reader-3.7/src/reader/_app/wsgi.py
+-rw-r--r--   0 lemon      (501) staff       (20)    13132 2022-12-31 08:17:16.000000 reader-3.7/src/reader/_cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4587 2022-07-16 20:45:27.000000 reader-3.7/src/reader/_config.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1531 2023-01-17 22:12:52.000000 reader-3.7/src/reader/_feedparser.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4074 2022-12-18 08:53:24.000000 reader-3.7/src/reader/_feedparser_lazy.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2980 2023-03-14 06:52:53.000000 reader-3.7/src/reader/_hash_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2220 2022-12-31 08:18:29.000000 reader-3.7/src/reader/_html_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7493 2023-06-08 21:12:49.000000 reader-3.7/src/reader/_http_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5677 2023-01-17 22:12:52.000000 reader-3.7/src/reader/_jsonfeed.py
+-rw-r--r--   0 lemon      (501) staff       (20)    24586 2023-03-19 13:56:03.000000 reader-3.7/src/reader/_parser.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.452489 reader-3.7/src/reader/_plugins/
+-rw-r--r--   0 lemon      (501) staff       (20)     1617 2022-12-29 21:54:33.000000 reader-3.7/src/reader/_plugins/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3201 2021-11-05 08:41:21.000000 reader-3.7/src/reader/_plugins/cli_status.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3065 2022-12-29 22:18:56.000000 reader-3.7/src/reader/_plugins/enclosure_tags.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4561 2023-01-01 10:20:44.000000 reader-3.7/src/reader/_plugins/preview_feed_list.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2931 2022-06-27 21:01:33.000000 reader-3.7/src/reader/_plugins/sqlite_releases.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.453393 reader-3.7/src/reader/_plugins/templates/
+-rw-r--r--   0 lemon      (501) staff       (20)      815 2022-12-27 22:01:52.000000 reader-3.7/src/reader/_plugins/templates/preview_feed_list.html
+-rw-r--r--   0 lemon      (501) staff       (20)     7785 2023-01-17 21:52:55.000000 reader-3.7/src/reader/_requests_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)      726 2023-01-01 10:22:19.000000 reader-3.7/src/reader/_requests_utils_lazy.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5623 2023-01-01 10:41:25.000000 reader-3.7/src/reader/_retrievers.py
+-rw-r--r--   0 lemon      (501) staff       (20)    34166 2023-03-03 21:46:20.000000 reader-3.7/src/reader/_search.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8256 2022-12-31 09:50:28.000000 reader-3.7/src/reader/_sql_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    24243 2022-12-31 08:26:13.000000 reader-3.7/src/reader/_sqlite_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    53646 2023-03-19 14:35:50.000000 reader-3.7/src/reader/_storage.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16419 2023-03-14 06:54:33.000000 reader-3.7/src/reader/_types.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16725 2022-12-31 08:26:13.000000 reader-3.7/src/reader/_update.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4224 2022-12-31 08:10:27.000000 reader-3.7/src/reader/_url_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     9052 2022-12-31 08:26:29.000000 reader-3.7/src/reader/_utils.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.454199 reader-3.7/src/reader/_vendor/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2020-10-28 07:24:12.000000 reader-3.7/src/reader/_vendor/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.471668 reader-3.7/src/reader/_vendor/feedparser/
+-rw-r--r--   0 lemon      (501) staff       (20)     2715 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16169 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/api.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.483292 reader-3.7/src/reader/_vendor/feedparser/datetimes/
+-rw-r--r--   0 lemon      (501) staff       (20)     2905 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2380 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/asctime.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4022 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/greek.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2945 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/hungarian.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5459 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/iso8601.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3354 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/korean.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2198 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/perforce.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5423 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/rfc822.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4506 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/datetimes/w3dtf.py
+-rw-r--r--   0 lemon      (501) staff       (20)    21181 2022-02-12 10:04:56.000000 reader-3.7/src/reader/_vendor/feedparser/encodings.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1897 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/exceptions.py
+-rw-r--r--   0 lemon      (501) staff       (20)    10791 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/html.py
+-rw-r--r--   0 lemon      (501) staff       (20)     9834 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/http.py
+-rw-r--r--   0 lemon      (501) staff       (20)    32296 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/mixin.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.489313 reader-3.7/src/reader/_vendor/feedparser/namespaces/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16998 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/_base.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2317 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/admin.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2866 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/cc.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4446 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/dc.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11399 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/georss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4115 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/itunes.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5336 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/mediarss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2839 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/namespaces/psc.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.493859 reader-3.7/src/reader/_vendor/feedparser/parsers/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/parsers/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4729 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/parsers/json.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3420 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/parsers/loose.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5805 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/parsers/strict.py
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/py.typed
+-rw-r--r--   0 lemon      (501) staff       (20)    23731 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/sanitizer.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3517 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/sgml.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5487 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/urls.py
+-rw-r--r--   0 lemon      (501) staff       (20)     6448 2022-02-11 15:50:56.000000 reader-3.7/src/reader/_vendor/feedparser/util.py
+-rw-r--r--   0 lemon      (501) staff       (20)    71461 2023-03-19 13:58:22.000000 reader-3.7/src/reader/core.py
+-rw-r--r--   0 lemon      (501) staff       (20)     6149 2022-12-31 08:26:06.000000 reader-3.7/src/reader/exceptions.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.500096 reader-3.7/src/reader/plugins/
+-rw-r--r--   0 lemon      (501) staff       (20)     1503 2022-12-31 08:26:13.000000 reader-3.7/src/reader/plugins/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      798 2021-03-26 12:03:04.000000 reader-3.7/src/reader/plugins/enclosure_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)    16705 2023-01-29 20:48:33.000000 reader-3.7/src/reader/plugins/entry_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2734 2023-03-18 22:45:04.000000 reader-3.7/src/reader/plugins/mark_as_read.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4678 2022-09-14 19:27:33.000000 reader-3.7/src/reader/plugins/readtime.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1626 2022-12-18 09:01:52.000000 reader-3.7/src/reader/plugins/ua_fallback.py
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-06-28 20:04:35.000000 reader-3.7/src/reader/py.typed
+-rw-r--r--   0 lemon      (501) staff       (20)    28282 2023-03-18 22:18:25.000000 reader-3.7/src/reader/types.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.436316 reader-3.7/src/reader.egg-info/
+-rw-r--r--   0 lemon      (501) staff       (20)     5367 2023-07-15 15:40:42.000000 reader-3.7/src/reader.egg-info/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     6083 2023-07-15 15:40:43.000000 reader-3.7/src/reader.egg-info/SOURCES.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        1 2023-07-15 15:40:42.000000 reader-3.7/src/reader.egg-info/dependency_links.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      730 2023-07-15 15:40:43.000000 reader-3.7/src/reader.egg-info/requires.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        7 2023-07-15 15:40:43.000000 reader-3.7/src/reader.egg-info/top_level.txt
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.560317 reader-3.7/tests/
+-rw-r--r--   0 lemon      (501) staff       (20)     5102 2023-06-16 19:19:37.000000 reader-3.7/tests/conftest.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.599610 reader-3.7/tests/data/
+-rw-r--r--   0 lemon      (501) staff       (20)       69 2021-10-18 18:44:15.000000 reader-3.7/tests/data/10.json
+-rw-r--r--   0 lemon      (501) staff       (20)      231 2022-12-31 08:17:15.000000 reader-3.7/tests/data/10.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)       12 2021-01-28 12:46:50.000000 reader-3.7/tests/data/custom
+-rw-r--r--   0 lemon      (501) staff       (20)      180 2020-10-28 07:20:07.000000 reader-3.7/tests/data/empty.atom
+-rw-r--r--   0 lemon      (501) staff       (20)      446 2022-12-31 08:17:17.000000 reader-3.7/tests/data/empty.atom.py
+-rw-r--r--   0 lemon      (501) staff       (20)      157 2021-01-28 10:55:34.000000 reader-3.7/tests/data/empty.json
+-rw-r--r--   0 lemon      (501) staff       (20)      455 2022-12-31 08:17:15.000000 reader-3.7/tests/data/empty.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)      191 2020-10-28 07:20:07.000000 reader-3.7/tests/data/empty.rss
+-rw-r--r--   0 lemon      (501) staff       (20)      326 2022-12-31 08:17:16.000000 reader-3.7/tests/data/empty.rss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1551 2022-03-26 15:46:54.000000 reader-3.7/tests/data/full.atom
+-rw-r--r--   0 lemon      (501) staff       (20)     2327 2022-12-31 08:17:15.000000 reader-3.7/tests/data/full.atom.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1743 2021-10-18 18:27:51.000000 reader-3.7/tests/data/full.json
+-rw-r--r--   0 lemon      (501) staff       (20)     1760 2022-12-31 08:17:16.000000 reader-3.7/tests/data/full.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1401 2021-06-08 19:16:41.000000 reader-3.7/tests/data/full.rss
+-rw-r--r--   0 lemon      (501) staff       (20)     1523 2022-12-31 08:17:15.000000 reader-3.7/tests/data/full.rss.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2024 2021-01-28 13:31:45.000000 reader-3.7/tests/data/invalid.json
+-rw-r--r--   0 lemon      (501) staff       (20)     1290 2022-12-31 08:17:16.000000 reader-3.7/tests/data/invalid.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)      577 2020-10-28 07:22:29.000000 reader-3.7/tests/data/relative.atom
+-rw-r--r--   0 lemon      (501) staff       (20)      906 2022-12-31 08:17:20.000000 reader-3.7/tests/data/relative.atom.py
+-rw-r--r--   0 lemon      (501) staff       (20)      560 2020-10-28 07:22:29.000000 reader-3.7/tests/data/relative.rss
+-rw-r--r--   0 lemon      (501) staff       (20)      907 2022-12-31 08:17:15.000000 reader-3.7/tests/data/relative.rss.py
+-rw-r--r--   0 lemon      (501) staff       (20)      629 2021-01-28 18:18:08.000000 reader-3.7/tests/data/sqlite_releases.html
+-rw-r--r--   0 lemon      (501) staff       (20)       72 2021-10-18 18:48:17.000000 reader-3.7/tests/data/unknown.json
+-rw-r--r--   0 lemon      (501) staff       (20)      234 2022-12-31 08:17:17.000000 reader-3.7/tests/data/unknown.json.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4468 2023-01-17 22:12:52.000000 reader-3.7/tests/fakeparser.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2440 2023-03-05 10:19:51.000000 reader-3.7/tests/reader_methods.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2023-07-15 15:40:43.605418 reader-3.7/tests/reader_test_plugins/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2022-03-27 11:01:36.000000 reader-3.7/tests/reader_test_plugins/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2022-03-27 11:03:08.000000 reader-3.7/tests/reader_test_plugins/good.py
+-rw-r--r--   0 lemon      (501) staff       (20)       59 2022-07-25 20:59:03.000000 reader-3.7/tests/reader_test_plugins/init_error.py
+-rw-r--r--   0 lemon      (501) staff       (20)       73 2022-03-27 11:08:08.000000 reader-3.7/tests/reader_test_plugins/missing_dependency.py
+-rw-r--r--   0 lemon      (501) staff       (20)       24 2022-03-27 11:08:24.000000 reader-3.7/tests/reader_test_plugins/missing_entry_point.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5534 2023-03-05 10:19:52.000000 reader-3.7/tests/test__types.py
+-rw-r--r--   0 lemon      (501) staff       (20)     9073 2023-06-16 18:51:44.000000 reader-3.7/tests/test_app.py
+-rw-r--r--   0 lemon      (501) staff       (20)      654 2020-10-28 07:22:21.000000 reader-3.7/tests/test_app_wsgi.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1028 2021-01-28 18:37:51.000000 reader-3.7/tests/test_bench.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11712 2023-01-23 15:26:55.000000 reader-3.7/tests/test_cli.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3055 2021-03-26 16:15:01.000000 reader-3.7/tests/test_config.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1815 2022-07-25 20:59:03.000000 reader-3.7/tests/test_exceptions.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2477 2021-03-19 09:00:44.000000 reader-3.7/tests/test_hash_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2246 2022-08-21 15:09:18.000000 reader-3.7/tests/test_html_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1319 2023-04-30 09:15:21.000000 reader-3.7/tests/test_http_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3229 2023-04-30 09:15:21.000000 reader-3.7/tests/test_lazy_imports.py
+-rw-r--r--   0 lemon      (501) staff       (20)    33547 2023-01-23 15:11:14.000000 reader-3.7/tests/test_parser.py
+-rw-r--r--   0 lemon      (501) staff       (20)      702 2021-11-04 22:22:57.000000 reader-3.7/tests/test_plugins_cli_status.py
+-rw-r--r--   0 lemon      (501) staff       (20)      915 2022-12-31 08:17:15.000000 reader-3.7/tests/test_plugins_enclosure_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)    22348 2023-01-29 21:01:09.000000 reader-3.7/tests/test_plugins_entry_dedupe.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3393 2023-01-29 20:48:19.000000 reader-3.7/tests/test_plugins_mark_as_read.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3233 2023-06-16 19:20:19.000000 reader-3.7/tests/test_plugins_preview_feed_list.py
+-rw-r--r--   0 lemon      (501) staff       (20)     6610 2022-09-14 19:27:33.000000 reader-3.7/tests/test_plugins_readtime.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2467 2023-01-23 15:09:42.000000 reader-3.7/tests/test_plugins_sqlite_releases.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1070 2022-12-31 08:17:15.000000 reader-3.7/tests/test_plugins_ua_fallback.py
+-rw-r--r--   0 lemon      (501) staff       (20)    94505 2023-03-05 10:19:56.000000 reader-3.7/tests/test_reader.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8018 2022-07-30 08:23:00.000000 reader-3.7/tests/test_reader_context.py
+-rw-r--r--   0 lemon      (501) staff       (20)       99 2021-07-17 15:02:59.000000 reader-3.7/tests/test_reader_deprecations.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8028 2022-12-31 08:17:16.000000 reader-3.7/tests/test_reader_hooks.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5885 2023-01-23 15:26:18.000000 reader-3.7/tests/test_reader_integration.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2617 2022-07-25 20:59:03.000000 reader-3.7/tests/test_reader_plugins.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7248 2022-12-31 08:17:15.000000 reader-3.7/tests/test_reader_private.py
+-rw-r--r--   0 lemon      (501) staff       (20)    33613 2022-08-21 15:09:18.000000 reader-3.7/tests/test_reader_search.py
+-rw-r--r--   0 lemon      (501) staff       (20)     7103 2022-08-29 19:45:44.000000 reader-3.7/tests/test_reader_sort.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5683 2022-08-21 15:09:18.000000 reader-3.7/tests/test_search.py
+-rw-r--r--   0 lemon      (501) staff       (20)     4724 2021-05-21 12:10:53.000000 reader-3.7/tests/test_sql_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11991 2022-03-16 22:01:23.000000 reader-3.7/tests/test_sqlite_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    17626 2023-03-03 21:47:06.000000 reader-3.7/tests/test_storage.py
+-rw-r--r--   0 lemon      (501) staff       (20)    12402 2022-08-21 15:09:18.000000 reader-3.7/tests/test_tags.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1129 2020-10-28 07:23:39.000000 reader-3.7/tests/test_test_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)    11006 2022-09-09 21:29:27.000000 reader-3.7/tests/test_types.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2516 2022-07-19 22:03:54.000000 reader-3.7/tests/test_utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3077 2023-01-23 14:51:43.000000 reader-3.7/tests/utils.py
+-rw-r--r--   0 lemon      (501) staff       (20)      752 2023-06-16 19:19:37.000000 reader-3.7/tox.ini
```

### Comparing `reader-3.6/CHANGES.rst` & `reader-3.7/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,54 @@
 Changelog
 =========
 
 .. module:: reader
   :noindex:
 
 
+Version 3.7
+-----------
+
+Released 2023-07-15
+
+.. attention::
+
+    This is the last release to support Python 3.9;
+    see :issue:`302` for details.
+
+* Support PyPy 3.10. (:issue:`302`)
+
+* Remove the :ref:`twitter` experimental plugin
+  (deprecated in `3.6 <Version 3.6_>`_).
+  (:issue:`310`)
+* Remove the :ref:`tumblr_gdpr` experimental plugin
+  (not needed since August 2020).
+  (:issue:`315`)
+
+
 Version 3.6
 -----------
 
 Released 2023-06-16
 
 * Add documentation on :doc:`contributing`. (:issue:`60`)
 * Add a detailed :ref:`roadmap`. (:issue:`60`)
 * Document the low-level
   :meth:`~reader._storage.Storage.delete_entries`
   storage method.
   (:issue:`301`, :issue:`96`)
 * Update vendored ``reader._http_utils`` to werkzeug 2.3.5.
 
-* Deprecate the (experimental) :mod:`~reader._plugins.twitter` plugin,
+* Deprecate the :ref:`twitter` experimental plugin,
   since the Twitter API does not have a (useful) free tier anymore.
   (:issue:`310`)
 
   .. attention::
 
-    The :mod:`~reader._plugins.twitter` plugin will be removed in version 3.7.
+    The :ref:`twitter` plugin will be removed in version 3.7.
 
 
 Version 3.5
 -----------
 
 Released 2023-03-19
 
@@ -118,15 +138,15 @@
         reader._parser.session_hooks.response.append(...)
 
     with::
 
         reader._parser.session_factory.request_hooks.append(...)
         reader._parser.session_factory.response_hooks.append(...)
 
-* :mod:`~reader._plugins.twitter` plugin:
+* :ref:`twitter` plugin:
   don't fail when deserializing tweets with missing ``edit_history_tweet_ids``
   (fails in tweepy 4.11, warns in tweepy >4.12).
 
 .. _5th anniversary: https://github.com/lemon24/reader/commit/73ac0bd3b8d0e5429e0bd7caf5281e4c9c74f16d
 
 
 Version 3.2
@@ -335,15 +355,15 @@
 
 
 Version 2.13
 ------------
 
 Released 2022-06-28
 
-* Add the :mod:`~reader._plugins.twitter` experimental plugin,
+* Add the :ref:`twitter` experimental plugin,
   which allows using a Twitter account as a feed.
   (:issue:`271`)
 * Skip with a warning entries that have no <guid> or <link> in an RSS feed;
   only raise :exc:`ParseError` if *all* entries have a missing id.
   (Note that both Atom and JSON Feed entries are required to have an id
   by their respective specifications.)
   Thanks to `Mirek Długosz`_ for the issue and pull request.
@@ -1649,8 +1669,8 @@
 
 Version 0.1
 -----------
 
 Released on 2018-09-15
 
 * Initial release; public API stable.
-* Support broken Tumblr feeds via the the ``tumblr_gdpr`` plugin. (:issue:`67`)
+* Support broken Tumblr feeds via the the :ref:`tumblr_gdpr` plugin. (:issue:`67`)
```

### Comparing `reader-3.6/LICENSE` & `reader-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reader-3.6/PKG-INFO` & `reader-3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reader
-Version: 3.6
+Version: 3.7
 Summary: A Python feed reader library.
 Home-page: https://github.com/lemon24/reader
 Author: lemon24
 License: BSD-3-Clause
 Project-URL: Changes, https://reader.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://reader.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/lemon24/reader/issues
@@ -84,17 +84,14 @@
 
 
 .. begin-features
 
 *reader* allows you to:
 
 * retrieve, store, and manage **Atom**, **RSS**, and **JSON** feeds
-
-  * and even follow **Twitter** accounts
-
 * mark articles as read or important
 * add arbitrary tags/metadata to feeds and articles
 * filter feeds and articles
 * full-text search articles
 * get statistics on feed and user activity
 * write plugins to extend its functionality
 * skip all the low level stuff and focus on what makes your feed reader different
```

### Comparing `reader-3.6/README.rst` & `reader-3.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,14 @@
 
 
 .. begin-features
 
 *reader* allows you to:
 
 * retrieve, store, and manage **Atom**, **RSS**, and **JSON** feeds
-
-  * and even follow **Twitter** accounts
-
 * mark articles as read or important
 * add arbitrary tags/metadata to feeds and articles
 * filter feeds and articles
 * full-text search articles
 * get statistics on feed and user activity
 * write plugins to extend its functionality
 * skip all the low level stuff and focus on what makes your feed reader different
```

### Comparing `reader-3.6/docs/Makefile` & `reader-3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/api.rst` & `reader-3.7/docs/api.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/app.rst` & `reader-3.7/docs/app.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/cli.rst` & `reader-3.7/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/conf.py` & `reader-3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/config.rst` & `reader-3.7/docs/config.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/dev-app.rst` & `reader-3.7/docs/dev-app.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/dev.rst` & `reader-3.7/docs/dev.rst`

 * *Files 12% similar despite different names*

```diff
@@ -301,14 +301,55 @@
 
 Alternative feed parsers:
 
 * the logical pipeline of parsing a feed: :issue:`264#issuecomment-973190028`
 * comparison between feedparser and Atoma: :issue:`264#issuecomment-981678120`, :issue:`263`
 
 
+Lessons learned from the :ref:`Twitter` plugin:
+
+* It is useful for a retriever to pass an arbitrary resource to the parser.
+
+  This is already codified in
+  :meth:`~reader._parser.RetrieverType` and
+  :meth:`~reader._parser.ParserType` being generic.
+
+* It is useful for a Retriever to store arbitrary caching data;
+  the plugin (mis)used
+  :attr:`~reader._parser.RetrieveResult.http_etag`
+  to store the (integer) id of the newest tweet in the thread.
+
+  It would be nice to formalize this into a single
+  "arbitrary caching data" attribute;
+  also see `this comment <https://github.com/lemon24/reader/blob/0ada24bf4e65c69c3028641bada8eaeabbe02754/src/reader/_parser.py#L569>`_.
+
+* It is useful for a Retriever to pass arbitrary data to itself;
+  the plugin (mis)used
+  :attr:`~reader._types.FeedForUpdate.http_etag` to pass from
+  :meth:`~reader._parser.FeedForUpdateRetrieverType.process_feed_for_update`
+  to :meth:`~reader._parser.RetrieverType.__call__`:
+
+  * the bearer token and the ids of recent entries (used to retrieve tweets)
+  * the ids of entries to re-render, triggered by a one-off tag (passed along to the parser)
+
+  This distinction was made so that ``process_feed_for_update()``
+  takes all the decisions upfront
+  (possibly taking advantage of ``Storage.get_feeds_for_update()``
+  future optimisations to e.g. also get tags),
+  and calling the retriever (in parallel) doesn't do any reader operations.
+
+  It would be nice to formalize this as well.
+
+* A plugin can coordinate between a custom retriever and custom parser
+  with an unregistered RetrieveResult MIME type
+  (e.g. ``application/x.twitter``).
+* A plugin can keep arbitrary data as a content with an unregistered type
+  (e.g. ``application/x.twitter+json``).
+
+
 Metrics
 ~~~~~~~
 
 Some thoughts on implementing metrics: :issue:`68#issuecomment-450025175`.
 
 
 Query builder
```

### Comparing `reader-3.6/docs/guide.rst` & `reader-3.7/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/images/redesign-01.png` & `reader-3.7/docs/images/redesign-01.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/index.rst` & `reader-3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/install.rst` & `reader-3.7/docs/install.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/internal.rst` & `reader-3.7/docs/internal.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 .. warning::
 
     As of version |version|,
     the internal API is **not** part of the public API;
     it is not stable yet and might change without any notice.
 
 
+.. _parser:
+
 Parser
 ------
 
 .. autoattribute:: reader.Reader._parser
 
 
 .. module:: reader._parser
```

### Comparing `reader-3.6/docs/make.bat` & `reader-3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/dillo.png` & `reader-3.7/docs/screenshots/dillo.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/entries-feed.png` & `reader-3.7/docs/screenshots/entries-feed.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/entries.png` & `reader-3.7/docs/screenshots/entries.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/entry-one.png` & `reader-3.7/docs/screenshots/entry-one.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/entry-two.png` & `reader-3.7/docs/screenshots/entry-two.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/feeds.png` & `reader-3.7/docs/screenshots/feeds.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/lynx.png` & `reader-3.7/docs/screenshots/lynx.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/screenshots/search.png` & `reader-3.7/docs/screenshots/search.png`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/tutorial.rst` & `reader-3.7/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `reader-3.6/docs/why.rst` & `reader-3.7/docs/why.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 Are you already working with `feedparser`_, but:
 
 * want an easier way to store, filter, sort and search feeds and entries?
 * want to get back type-annotated objects instead of dicts?
 * want to restrict or deny file-system access?
 * want to change the way feeds are retrieved by using the more familiar `requests`_ library?
 * want to also support `JSON Feed`_?
-* want to follow :ref:`Twitter <twitter>` accounts?
 * want to support custom information sources?
 
 ... while still supporting all the feed types feedparser does?
 
 If you answered yes to any of the above, *reader* can help.
```

### Comparing `reader-3.6/examples/config.yaml` & `reader-3.7/examples/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         feed_root: /path/to/feeds
 
         # Additionally, it's possible to specify reader plugins, as a
         #   <plugin import path>: <plugin options>
         # map; options are ignored at the moment.
         # Note that unlike other settings, plugins are merged, not replaced.
         plugins:
-            reader._plugins.tumblr_gdpr:tumblr_gdpr:
+            reader._plugins.sqlite_releases:init:
             reader.ua_fallback:
 
 
 # CLI context.
 
 cli:
     # When using the CLI, we want to use some additional reader plugins.
```

### Comparing `reader-3.6/examples/parser_only.py` & `reader-3.7/examples/parser_only.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/examples/podcast.py` & `reader-3.7/examples/podcast.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/examples/terminal.py` & `reader-3.7/examples/terminal.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/run.sh` & `reader-3.7/run.sh`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/.coverage` & `reader-3.7/scripts/.coverage`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/backup.sh` & `reader-3.7/scripts/backup.sh`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/bench.py` & `reader-3.7/scripts/bench.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/debug_storage_stats.py` & `reader-3.7/scripts/debug_storage_stats.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/jscontrols.html` & `reader-3.7/scripts/jscontrols.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/jscontrols.py` & `reader-3.7/scripts/jscontrols.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/lines.sh` & `reader-3.7/scripts/lines.sh`

 * *Files identical despite different names*

### Comparing `reader-3.6/scripts/release.py` & `reader-3.7/scripts/release.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/setup.cfg` & `reader-3.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 search = 
 readtime = 
 cli = 
 	click>=7
 	PyYAML
 app = 
 	flask>=0.10
-	humanize
+	humanize>=4,!=4.7.*
 	PyYAML
 unstable-plugins = 
 	
 	requests
 	mutagen
 	
 	requests
@@ -79,17 +79,17 @@
 	pytest>=4
 	pytest-randomly
 	pytest-subtests
 	flaky
 	coverage
 	pytest-cov
 	requests-mock
-	mechanicalsoup
+	mechanicalsoup; (implementation_name != "pypy" or python_version <= "3.9")
 	requests-wsgi-adapter
-	lxml
+	lxml; (implementation_name != "pypy" or python_version <= "3.9")
 	html5lib
 	werkzeug
 	mypy; implementation_name != "pypy"
 	types-requests
 docs = 
 	sphinx
 	sphinx-rtd-theme
@@ -106,14 +106,15 @@
 	build
 	twine
 
 [tool:pytest]
 markers = 
 	slow: mark a test as slow.
 	requires_lxml: mark a test to only run in places where we have lxml.
+	apptest: mark a test as a web app test (skipped sometimes).
 addopts = --no-success-flaky-report
 filterwarnings = 
 	ignore:No parser was explicitly specified::reader._html_utils
 testpaths = tests
 
 [coverage:run]
 branch = true
```

### Comparing `reader-3.6/src/reader/__init__.py` & `reader-3.7/src/reader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     for e in reader.get_entries(read=False):
         print(e.title)
 
 
 """
 
-__version__ = '3.6'
+__version__ = '3.7'
 
 from .core import (
     Reader as Reader,
     make_reader as make_reader,
 )
 
 from .types import (
```

### Comparing `reader-3.6/src/reader/_app/__init__.py` & `reader-3.7/src/reader/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/api_thing.py` & `reader-3.7/src/reader/_app/api_thing.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/cli.py` & `reader-3.7/src/reader/_app/cli.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/static/controls.js` & `reader-3.7/src/reader/_app/static/controls.js`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/static/style.css` & `reader-3.7/src/reader/_app/static/style.css`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/add_entry.html` & `reader-3.7/src/reader/_app/templates/add_entry.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/entries.html` & `reader-3.7/src/reader/_app/templates/entries.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/entry.html` & `reader-3.7/src/reader/_app/templates/entry.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/feeds.html` & `reader-3.7/src/reader/_app/templates/feeds.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/layout.html` & `reader-3.7/src/reader/_app/templates/layout.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/macros.html` & `reader-3.7/src/reader/_app/templates/macros.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/metadata.html` & `reader-3.7/src/reader/_app/templates/metadata.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/templates/tags.html` & `reader-3.7/src/reader/_app/templates/tags.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_app/wsgi.py` & `reader-3.7/src/reader/_app/wsgi.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_cli.py` & `reader-3.7/src/reader/_cli.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_config.py` & `reader-3.7/src/reader/_config.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_feedparser.py` & `reader-3.7/src/reader/_feedparser.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_feedparser_lazy.py` & `reader-3.7/src/reader/_feedparser_lazy.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_hash_utils.py` & `reader-3.7/src/reader/_hash_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_html_utils.py` & `reader-3.7/src/reader/_html_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_http_utils.py` & `reader-3.7/src/reader/_http_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_jsonfeed.py` & `reader-3.7/src/reader/_jsonfeed.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_parser.py` & `reader-3.7/src/reader/_parser.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_plugins/__init__.py` & `reader-3.7/src/reader/_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_plugins/cli_status.py` & `reader-3.7/src/reader/_plugins/cli_status.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_plugins/enclosure_tags.py` & `reader-3.7/src/reader/_plugins/enclosure_tags.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_plugins/preview_feed_list.py` & `reader-3.7/src/reader/_plugins/preview_feed_list.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_plugins/sqlite_releases.py` & `reader-3.7/src/reader/_plugins/sqlite_releases.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_plugins/templates/preview_feed_list.html` & `reader-3.7/src/reader/_plugins/templates/preview_feed_list.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_requests_utils.py` & `reader-3.7/src/reader/_requests_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_requests_utils_lazy.py` & `reader-3.7/src/reader/_requests_utils_lazy.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_retrievers.py` & `reader-3.7/src/reader/_retrievers.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_search.py` & `reader-3.7/src/reader/_search.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_sql_utils.py` & `reader-3.7/src/reader/_sql_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_sqlite_utils.py` & `reader-3.7/src/reader/_sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_storage.py` & `reader-3.7/src/reader/_storage.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_types.py` & `reader-3.7/src/reader/_types.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_update.py` & `reader-3.7/src/reader/_update.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_url_utils.py` & `reader-3.7/src/reader/_url_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_utils.py` & `reader-3.7/src/reader/_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/__init__.py` & `reader-3.7/src/reader/_vendor/feedparser/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/api.py` & `reader-3.7/src/reader/_vendor/feedparser/api.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/__init__.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/asctime.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/asctime.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/greek.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/greek.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/hungarian.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/hungarian.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/iso8601.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/iso8601.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/korean.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/korean.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/perforce.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/perforce.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/rfc822.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/rfc822.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/datetimes/w3dtf.py` & `reader-3.7/src/reader/_vendor/feedparser/datetimes/w3dtf.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/encodings.py` & `reader-3.7/src/reader/_vendor/feedparser/encodings.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/exceptions.py` & `reader-3.7/src/reader/_vendor/feedparser/exceptions.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/html.py` & `reader-3.7/src/reader/_vendor/feedparser/html.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/http.py` & `reader-3.7/src/reader/_vendor/feedparser/http.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/mixin.py` & `reader-3.7/src/reader/_vendor/feedparser/mixin.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/_base.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/_base.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/admin.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/admin.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/cc.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/cc.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/dc.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/dc.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/georss.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/georss.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/itunes.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/itunes.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/mediarss.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/mediarss.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/namespaces/psc.py` & `reader-3.7/src/reader/_vendor/feedparser/namespaces/psc.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/parsers/json.py` & `reader-3.7/src/reader/_vendor/feedparser/parsers/json.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/parsers/loose.py` & `reader-3.7/src/reader/_vendor/feedparser/parsers/loose.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/parsers/strict.py` & `reader-3.7/src/reader/_vendor/feedparser/parsers/strict.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/sanitizer.py` & `reader-3.7/src/reader/_vendor/feedparser/sanitizer.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/sgml.py` & `reader-3.7/src/reader/_vendor/feedparser/sgml.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/urls.py` & `reader-3.7/src/reader/_vendor/feedparser/urls.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/_vendor/feedparser/util.py` & `reader-3.7/src/reader/_vendor/feedparser/util.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/core.py` & `reader-3.7/src/reader/core.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/exceptions.py` & `reader-3.7/src/reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/plugins/__init__.py` & `reader-3.7/src/reader/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/plugins/enclosure_dedupe.py` & `reader-3.7/src/reader/plugins/enclosure_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/plugins/entry_dedupe.py` & `reader-3.7/src/reader/plugins/entry_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/plugins/mark_as_read.py` & `reader-3.7/src/reader/plugins/mark_as_read.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/plugins/readtime.py` & `reader-3.7/src/reader/plugins/readtime.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/plugins/ua_fallback.py` & `reader-3.7/src/reader/plugins/ua_fallback.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader/types.py` & `reader-3.7/src/reader/types.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/src/reader.egg-info/PKG-INFO` & `reader-3.7/src/reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reader
-Version: 3.6
+Version: 3.7
 Summary: A Python feed reader library.
 Home-page: https://github.com/lemon24/reader
 Author: lemon24
 License: BSD-3-Clause
 Project-URL: Changes, https://reader.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://reader.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/lemon24/reader/issues
@@ -84,17 +84,14 @@
 
 
 .. begin-features
 
 *reader* allows you to:
 
 * retrieve, store, and manage **Atom**, **RSS**, and **JSON** feeds
-
-  * and even follow **Twitter** accounts
-
 * mark articles as read or important
 * add arbitrary tags/metadata to feeds and articles
 * filter feeds and articles
 * full-text search articles
 * get statistics on feed and user activity
 * write plugins to extend its functionality
 * skip all the low level stuff and focus on what makes your feed reader different
```

### Comparing `reader-3.6/src/reader.egg-info/SOURCES.txt` & `reader-3.7/src/reader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 docs/screenshots/entries-feed.png
 docs/screenshots/entries.png
 docs/screenshots/entry-one.png
 docs/screenshots/entry-two.png
 docs/screenshots/feeds.png
 docs/screenshots/lynx.png
 docs/screenshots/search.png
-docs/screenshots/twitter-one.png
-docs/screenshots/twitter-two.png
 examples/config.yaml
 examples/parser_only.py
 examples/podcast.py
 examples/terminal.py
 scripts/.coverage
 scripts/backup.sh
 scripts/bench.py
@@ -95,16 +93,14 @@
 src/reader/_app/templates/metadata.html
 src/reader/_app/templates/tags.html
 src/reader/_plugins/__init__.py
 src/reader/_plugins/cli_status.py
 src/reader/_plugins/enclosure_tags.py
 src/reader/_plugins/preview_feed_list.py
 src/reader/_plugins/sqlite_releases.py
-src/reader/_plugins/tumblr_gdpr.py
-src/reader/_plugins/twitter.py
 src/reader/_plugins/templates/preview_feed_list.html
 src/reader/_vendor/__init__.py
 src/reader/_vendor/feedparser/__init__.py
 src/reader/_vendor/feedparser/api.py
 src/reader/_vendor/feedparser/encodings.py
 src/reader/_vendor/feedparser/exceptions.py
 src/reader/_vendor/feedparser/html.py
@@ -161,16 +157,14 @@
 tests/test_plugins_cli_status.py
 tests/test_plugins_enclosure_dedupe.py
 tests/test_plugins_entry_dedupe.py
 tests/test_plugins_mark_as_read.py
 tests/test_plugins_preview_feed_list.py
 tests/test_plugins_readtime.py
 tests/test_plugins_sqlite_releases.py
-tests/test_plugins_tumblr_gdpr.py
-tests/test_plugins_twitter.py
 tests/test_plugins_ua_fallback.py
 tests/test_reader.py
 tests/test_reader_context.py
 tests/test_reader_deprecations.py
 tests/test_reader_hooks.py
 tests/test_reader_integration.py
 tests/test_reader_plugins.py
```

### Comparing `reader-3.6/src/reader.egg-info/requires.txt` & `reader-3.7/src/reader.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 feedparser>=6
 requests>=2.18
 iso8601>=1
 beautifulsoup4>=4.5
 
 [app]
 flask>=0.10
-humanize
+humanize!=4.7.*,>=4
 PyYAML
 
 [cli]
 click>=7
 PyYAML
 
 [dev]
@@ -38,24 +38,26 @@
 pytest>=4
 pytest-randomly
 pytest-subtests
 flaky
 coverage
 pytest-cov
 requests-mock
-mechanicalsoup
 requests-wsgi-adapter
-lxml
 html5lib
 werkzeug
 types-requests
 
 [tests:implementation_name != "pypy"]
 mypy
 
+[tests:implementation_name != "pypy" or python_version <= "3.9"]
+mechanicalsoup
+lxml
+
 [unstable-plugins]
 requests
 mutagen
 beautifulsoup4
 blinker>=1.4
 tweepy
 Jinja2>=3
```

### Comparing `reader-3.6/tests/conftest.py` & `reader-3.7/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,20 +51,26 @@
 
 
 def pytest_runtest_setup(item):
     # lxml fails to build in various places,
     # see the comments in setup.cfg for details.
     for mark in item.iter_markers(name="requires_lxml"):
         no_lxml = [
-            # currently, we have lxml wheels on all supported platforms;
-            # last in bbe1deee5eee800291b5a0e83fc4ab1cb949445c
+            sys.implementation.name == 'pypy' and sys.version_info[:2] > (3, 9),
         ]
         if any(no_lxml):
             pytest.skip("test requires lxml")
 
+    # getting intermittent Flask-context-related errors on pypy:
+    #   AssertionError: Popped wrong app context.
+    #   RuntimeError: Working outside of request context.
+    for mark in item.iter_markers(name="apptest"):
+        if sys.implementation.name == 'pypy':
+            pytest.skip("flask tests are flaky on pypy")
+
 
 @pytest.fixture
 def make_reader(request):
     @wraps(original_make_reader)
     def make_reader(*args, **kwargs):
         reader = original_make_reader(*args, **kwargs)
         request.addfinalizer(reader.close)
```

### Comparing `reader-3.6/tests/data/full.atom` & `reader-3.7/tests/data/full.atom`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/full.atom.py` & `reader-3.7/tests/data/full.atom.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/full.json` & `reader-3.7/tests/data/full.json`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/full.json.py` & `reader-3.7/tests/data/full.json.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/full.rss` & `reader-3.7/tests/data/full.rss`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/full.rss.py` & `reader-3.7/tests/data/full.rss.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/invalid.json` & `reader-3.7/tests/data/invalid.json`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/invalid.json.py` & `reader-3.7/tests/data/invalid.json.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/relative.atom` & `reader-3.7/tests/data/relative.atom`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/relative.atom.py` & `reader-3.7/tests/data/relative.atom.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/relative.rss` & `reader-3.7/tests/data/relative.rss`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/relative.rss.py` & `reader-3.7/tests/data/relative.rss.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/data/sqlite_releases.html` & `reader-3.7/tests/data/sqlite_releases.html`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/fakeparser.py` & `reader-3.7/tests/fakeparser.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/reader_methods.py` & `reader-3.7/tests/reader_methods.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test__types.py` & `reader-3.7/tests/test__types.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_app.py` & `reader-3.7/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 # mechanicalsoup depends on lxml, but we don't have that everywhere.
 try:
     import mechanicalsoup
 except ImportError:
     pass
 
-# Don't run these tests if we don't have lxml.
-pytestmark = pytest.mark.requires_lxml
+pytestmark = [pytest.mark.requires_lxml, pytest.mark.apptest]
 
 
 def make_app(config):
     return create_app(make_reader_config(config))
 
 
 def make_browser(app):
```

### Comparing `reader-3.6/tests/test_app_wsgi.py` & `reader-3.7/tests/test_app_wsgi.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_bench.py` & `reader-3.7/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_cli.py` & `reader-3.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_config.py` & `reader-3.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_exceptions.py` & `reader-3.7/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_hash_utils.py` & `reader-3.7/tests/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_html_utils.py` & `reader-3.7/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_http_utils.py` & `reader-3.7/tests/test_http_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_lazy_imports.py` & `reader-3.7/tests/test_lazy_imports.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_parser.py` & `reader-3.7/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_plugins_cli_status.py` & `reader-3.7/tests/test_plugins_cli_status.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_plugins_enclosure_dedupe.py` & `reader-3.7/tests/test_plugins_enclosure_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_plugins_entry_dedupe.py` & `reader-3.7/tests/test_plugins_entry_dedupe.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_plugins_mark_as_read.py` & `reader-3.7/tests/test_plugins_mark_as_read.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_plugins_preview_feed_list.py` & `reader-3.7/tests/test_plugins_preview_feed_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import pytest
 from test_app import make_app
 from test_app import make_browser
+from test_app import pytestmark
 
 from reader._plugins.preview_feed_list import get_alternates
 
 
-pytestmark = pytest.mark.filterwarnings("ignore:No parser was explicitly specified")
+pytestmark = list(pytestmark)
+pytestmark.append(
+    pytest.mark.filterwarnings("ignore:No parser was explicitly specified")
+)
 
 
 MAIN_IN = """\
 <link rel=alternate type=rss href=1 />
 <link rel=alternate title=rss href=2 />
 <link rel=alternate type=nope title=feed href=3 />
 <link rel=alternate href=some/rss.xml />
```

### Comparing `reader-3.6/tests/test_plugins_readtime.py` & `reader-3.7/tests/test_plugins_readtime.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_plugins_sqlite_releases.py` & `reader-3.7/tests/test_plugins_sqlite_releases.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_plugins_ua_fallback.py` & `reader-3.7/tests/test_plugins_ua_fallback.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader.py` & `reader-3.7/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader_context.py` & `reader-3.7/tests/test_reader_context.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader_hooks.py` & `reader-3.7/tests/test_reader_hooks.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader_integration.py` & `reader-3.7/tests/test_reader_integration.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader_plugins.py` & `reader-3.7/tests/test_reader_plugins.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader_private.py` & `reader-3.7/tests/test_reader_private.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader_search.py` & `reader-3.7/tests/test_reader_search.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_reader_sort.py` & `reader-3.7/tests/test_reader_sort.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_search.py` & `reader-3.7/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_sql_utils.py` & `reader-3.7/tests/test_sql_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_sqlite_utils.py` & `reader-3.7/tests/test_sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_storage.py` & `reader-3.7/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_tags.py` & `reader-3.7/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_test_utils.py` & `reader-3.7/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_types.py` & `reader-3.7/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/test_utils.py` & `reader-3.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reader-3.6/tests/utils.py` & `reader-3.7/tests/utils.py`

 * *Files identical despite different names*

