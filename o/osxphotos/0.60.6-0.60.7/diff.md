# Comparing `tmp/osxphotos-0.60.6.tar.gz` & `tmp/osxphotos-0.60.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.6.tar", last modified: Sun Jul  2 16:42:00 2023, max compression
+gzip compressed data, was "osxphotos-0.60.7.tar", last modified: Sat Jul 15 14:32:38 2023, max compression
```

## Comparing `osxphotos-0.60.6.tar` & `osxphotos-0.60.7.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.898076 osxphotos-0.60.6/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.6/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.6/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-02 16:42:00.897889 osxphotos-0.60.6/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   225720 2023-07-02 16:41:50.000000 osxphotos-0.60.6/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.6/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.868539 osxphotos-0.60.6/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.6/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15892 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-02 16:41:47.000000 osxphotos-0.60.6/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.6/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.6/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.876378 osxphotos-0.60.6/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.6/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.6/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   107303 2023-07-02 15:42:46.000000 osxphotos-0.60.6/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.6/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.6/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.6/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.6/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.6/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.6/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.876870 osxphotos-0.60.6/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.6/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1465082 2023-07-02 16:41:57.000000 osxphotos-0.60.6/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.6/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.6/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.6/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.6/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    91553 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    84853 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.879356 osxphotos-0.60.6/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10395 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149958 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.6/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.6/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-02 16:41:49.000000 osxphotos-0.60.6/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.6/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.6/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    25682 2023-07-02 16:32:35.000000 osxphotos-0.60.6/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/platform.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.6/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.884201 osxphotos-0.60.6/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.6/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.6/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.6/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.6/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.6/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.6/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.6/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.6/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.6/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.885216 osxphotos-0.60.6/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.6/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.6/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.6/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.6/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.869423 osxphotos-0.60.6/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6499 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-02 16:42:00.000000 osxphotos-0.60.6/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-02 16:42:00.898118 osxphotos-0.60.6/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.6/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.897412 osxphotos-0.60.6/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-02 16:42:00.897677 osxphotos-0.60.6/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.6/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.6/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   274105 2023-06-24 17:50:43.000000 osxphotos-0.60.6/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.6/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.6/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.6/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.6/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.6/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.6/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.6/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.6/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.6/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.6/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.6/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.6/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.6/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_photosalbum_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.6/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.6/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.6/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.6/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.6/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.6/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.6/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.6/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.6/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.6/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.6/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.6/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.6/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.6/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.750491 osxphotos-0.60.7/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.7/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.7/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-15 14:32:38.750274 osxphotos-0.60.7/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   226320 2023-07-15 14:32:27.000000 osxphotos-0.60.7/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.7/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.714928 osxphotos-0.60.7/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.7/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.7/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15892 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-15 14:32:15.000000 osxphotos-0.60.7/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.7/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.7/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.726683 osxphotos-0.60.7/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.7/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.7/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.7/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   108030 2023-07-15 14:18:05.000000 osxphotos-0.60.7/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.7/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.7/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.7/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.7/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.7/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.7/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.7/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.727202 osxphotos-0.60.7/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.7/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1477702 2023-07-15 14:32:34.000000 osxphotos-0.60.7/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.7/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.7/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.7/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.7/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    93623 2023-07-15 14:18:05.000000 osxphotos-0.60.7/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    85034 2023-07-15 14:18:05.000000 osxphotos-0.60.7/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.729480 osxphotos-0.60.7/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10395 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149958 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.7/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.7/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-15 14:32:26.000000 osxphotos-0.60.7/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.7/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.7/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    25757 2023-07-03 07:44:41.000000 osxphotos-0.60.7/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/platform.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.7/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.730713 osxphotos-0.60.7/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.7/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.7/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.7/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.7/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.7/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.7/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.7/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.731774 osxphotos-0.60.7/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.7/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.715765 osxphotos-0.60.7/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6499 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-15 14:32:38.750529 osxphotos-0.60.7/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.7/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.749369 osxphotos-0.60.7/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.749619 osxphotos-0.60.7/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.7/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.7/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   275628 2023-07-15 14:18:05.000000 osxphotos-0.60.7/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.7/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.7/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.7/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.7/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.7/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.7/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.7/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.7/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.7/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.7/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.7/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.7/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.7/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_photosalbum_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.7/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.7/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.7/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.7/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.7/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.7/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.7/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.7/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.7/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.7/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.7/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.6/LICENSE` & `osxphotos-0.60.7/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/PKG-INFO` & `osxphotos-0.60.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.6
+Version: 0.60.7
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.6/README.md` & `osxphotos-0.60.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1062,14 +1062,22 @@
                                   disk.  This will be slow and will require
                                   internet connection. This obviously only works
                                   if the Photos library is synched to iCloud.
                                   Note: --download-missing does not currently
                                   export all burst images; only the primary
                                   photo will be exported--associated burst
                                   images will be skipped.
+  --export-aae                    Also export an adjustments file detailing
+                                  edits made to the original. The resulting file
+                                  is named photoname.AAE. Note that to import
+                                  these files back to Photos succesfully, you
+                                  also need to export the edited photo and match
+                                  the filename format Photos.app expects:
+                                  --filename 'IMG_{edited_version?E,}{id:04d}'
+                                  --edited-suffix ''
   --sidecar FORMAT                Create sidecar for each photo exported; valid
                                   FORMAT values: xmp, json, exiftool; --sidecar
                                   xmp: create XMP sidecar used by Digikam, Adobe
                                   Lightroom, etc. The sidecar file is named in
                                   format photoname.ext.xmp The XMP sidecar
                                   exports the following tags: Description,
                                   Title, Keywords/Tags, Subject (set to Keywords
@@ -2106,15 +2114,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.6'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.7'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2593,15 +2601,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.6'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.7'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
```

### Comparing `osxphotos-0.60.6/README.rst` & `osxphotos-0.60.7/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/__init__.py` & `osxphotos-0.60.7/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/_constants.py` & `osxphotos-0.60.7/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.7/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/albuminfo.py` & `osxphotos-0.60.7/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/__init__.py` & `osxphotos-0.60.7/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/about.py` & `osxphotos-0.60.7/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/add_locations.py` & `osxphotos-0.60.7/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/albums.py` & `osxphotos-0.60.7/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.7/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/cli.py` & `osxphotos-0.60.7/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.7/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/cli_params.py` & `osxphotos-0.60.7/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.7/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/color_themes.py` & `osxphotos-0.60.7/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/common.py` & `osxphotos-0.60.7/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/darkmode.py` & `osxphotos-0.60.7/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.7/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/docs.py` & `osxphotos-0.60.7/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/dump.py` & `osxphotos-0.60.7/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.7/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/export.py` & `osxphotos-0.60.7/osxphotos/cli/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,22 @@
     "to interact with Photos to export the photo which will force Photos to download from iCloud if "
     "the photo does not exist on disk.  This will be slow and will require internet connection. "
     "This obviously only works if the Photos library is synched to iCloud.  "
     "Note: --download-missing does not currently export all burst images; "
     "only the primary photo will be exported--associated burst images will be skipped.",
 )
 @click.option(
+    "--export-aae",
+    is_flag=True,
+    help="Also export an adjustments file detailing edits made to the original. "
+    "The resulting file is named photoname.AAE. "
+    "Note that to import these files back to Photos succesfully, you also need to "
+    "export the edited photo and match the filename format Photos.app expects: "
+    "--filename 'IMG_{edited_version?E,}{id:04d}' --edited-suffix ''")
+@click.option(
     "--sidecar",
     default=None,
     multiple=True,
     metavar="FORMAT",
     type=click.Choice(["xmp", "json", "exiftool"], case_sensitive=False),
     help="Create sidecar for each photo exported; valid FORMAT values: xmp, json, exiftool; "
     "--sidecar xmp: create XMP sidecar used by Digikam, Adobe Lightroom, etc. "
@@ -848,14 +856,15 @@
     replace_keywords,
     report,
     retry,
     save_config,
     screenshot,
     selfie,
     shared,
+    export_aae,
     sidecar,
     sidecar_drop_ext,
     skip_bursts,
     skip_edited,
     skip_live,
     skip_original_if_edited,
     skip_raw,
@@ -1072,14 +1081,15 @@
         replace_keywords = cfg.replace_keywords
         report = cfg.report
         retry = cfg.retry
         screenshot = cfg.screenshot
         selected = cfg.selected
         selfie = cfg.selfie
         shared = cfg.shared
+        export_aae = cfg.export_aae
         sidecar = cfg.sidecar
         sidecar_drop_ext = cfg.sidecar_drop_ext
         skip_bursts = cfg.skip_bursts
         skip_edited = cfg.skip_edited
         skip_live = cfg.skip_live
         skip_original_if_edited = cfg.skip_original_if_edited
         skip_raw = cfg.skip_raw
@@ -1641,14 +1651,15 @@
         db_files = [db_file, db_file + "-wal", db_file + "-shm"]
         all_files = (
             results.exported
             + results.skipped
             + results.exif_updated
             + results.touched
             + results.converted_to_jpeg
+            + results.aae_written
             + results.sidecar_json_written
             + results.sidecar_json_skipped
             + results.sidecar_exiftool_written
             + results.sidecar_exiftool_skipped
             + results.sidecar_xmp_written
             + results.sidecar_xmp_skipped
             # include missing so a file that was already in export directory
@@ -1698,14 +1709,15 @@
 
 
 def export_photo(
     photo=None,
     dest=None,
     verbose=None,
     export_by_date=None,
+    export_aae=None,
     sidecar=None,
     sidecar_drop_ext=False,
     update=None,
     force_update=None,
     ignore_signature=None,
     export_as_hardlink=None,
     overwrite=None,
@@ -1786,14 +1798,15 @@
         overwrite: bool; overwrite dest file if it already exists
         person_keyword: bool; if True, exports person names as keywords in metadata
         photo_num: int, which number photo in total of num_photos is being exported
         preview_if_missing: bool, export preview if original is missing
         preview_suffix: str, template to use as suffix for preview images
         replace_keywords: if True, --keyword-template replaces keywords instead of adding keywords
         retry: retry up to retry # of times if there's an error
+        export_aae: bool; if True, will also save adjustments
         sidecar_drop_ext: bool; if True, drops photo extension from sidecar name
         sidecar: list zero, 1 or 2 of ["json","xmp"] of sidecar variety to export
         skip_original_if_edited: bool; if True does not export original if photo has been edited
         touch_file: bool; sets file's modification time to match photo date
         update: bool, only export updated photos
         update_errors: bool, attempt to re-export photos that previously produced errors even if they otherwise would not be exported
         use_photos_export: bool; if True forces the use of AppleScript to export even if photo not missing
@@ -1952,14 +1965,15 @@
                 overwrite=overwrite,
                 person_keyword=person_keyword,
                 photo=photo,
                 preview_if_missing=preview_if_missing,
                 preview_suffix=rendered_preview_suffix,
                 replace_keywords=replace_keywords,
                 retry=retry,
+                export_aae=export_aae,
                 sidecar_drop_ext=sidecar_drop_ext,
                 sidecar_flags=sidecar_flags,
                 touch_file=touch_file,
                 update=update,
                 update_errors=update_errors,
                 use_photos_export=use_photos_export,
                 use_photokit=use_photokit,
@@ -2068,14 +2082,15 @@
                     overwrite=overwrite,
                     person_keyword=person_keyword,
                     photo=photo,
                     preview_if_missing=preview_if_missing,
                     preview_suffix=rendered_preview_suffix,
                     replace_keywords=replace_keywords,
                     retry=retry,
+                    export_aae=export_aae,
                     sidecar_drop_ext=sidecar_drop_ext,
                     sidecar_flags=sidecar_flags if not export_original else 0,
                     touch_file=touch_file,
                     update=update,
                     update_errors=update_errors,
                     use_photos_export=use_photos_export,
                     use_photokit=use_photokit,
@@ -2155,14 +2170,15 @@
     overwrite,
     person_keyword,
     photo,
     preview_if_missing,
     preview_suffix,
     replace_keywords,
     retry,
+    export_aae,
     sidecar_drop_ext,
     sidecar_flags,
     touch_file,
     update,
     update_errors,
     use_photos_export,
     use_photokit,
@@ -2219,14 +2235,15 @@
                 overwrite=overwrite,
                 preview=export_preview or (missing and preview_if_missing),
                 preview_suffix=preview_suffix,
                 raw_photo=export_raw,
                 render_options=render_options,
                 replace_keywords=replace_keywords,
                 rich=True,
+                export_aae=export_aae,
                 sidecar=sidecar_flags,
                 sidecar_drop_ext=sidecar_drop_ext,
                 tmpdir=tmpdir,
                 touch_file=touch_file,
                 update=update,
                 update_errors=update_errors,
                 use_albums_as_keywords=album_keyword,
```

### Comparing `osxphotos-0.60.6/osxphotos/cli/exportdb.py` & `osxphotos-0.60.7/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/grep.py` & `osxphotos-0.60.7/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/help.py` & `osxphotos-0.60.7/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/import_cli.py` & `osxphotos-0.60.7/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/info.py` & `osxphotos-0.60.7/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.7/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/keywords.py` & `osxphotos-0.60.7/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/kvstore.py` & `osxphotos-0.60.7/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/labels.py` & `osxphotos-0.60.7/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/list.py` & `osxphotos-0.60.7/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/orphans.py` & `osxphotos-0.60.7/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/param_types.py` & `osxphotos-0.60.7/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/persons.py` & `osxphotos-0.60.7/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.7/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/places.py` & `osxphotos-0.60.7/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.7/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/query.py` & `osxphotos-0.60.7/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/repl.py` & `osxphotos-0.60.7/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/report_writer.py` & `osxphotos-0.60.7/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.7/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/show_command.py` & `osxphotos-0.60.7/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.7/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/sync.py` & `osxphotos-0.60.7/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/sync_results.py` & `osxphotos-0.60.7/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/theme.py` & `osxphotos-0.60.7/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/timewarp.py` & `osxphotos-0.60.7/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/tutorial.py` & `osxphotos-0.60.7/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/uuid.py` & `osxphotos-0.60.7/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/verbose.py` & `osxphotos-0.60.7/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/cli/version.py` & `osxphotos-0.60.7/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/compare_exif.py` & `osxphotos-0.60.7/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/configoptions.py` & `osxphotos-0.60.7/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/crash_reporter.py` & `osxphotos-0.60.7/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/datetime_formatter.py` & `osxphotos-0.60.7/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/datetime_utils.py` & `osxphotos-0.60.7/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/debug.py` & `osxphotos-0.60.7/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/docs/docs.zip` & `osxphotos-0.60.7/osxphotos/docs/docs.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1465082 bytes, number of entries: 99
+Zip file size: 1477702 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jul-02 16:41 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jul-15 14:32 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
--rw-r--r--  3.0 unx   324897 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photoexporter.html
+-rw-r--r--  3.0 unx   333770 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   201029 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
 -rw-r--r--  3.0 unx    52397 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   313931 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx   314708 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29242 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
 -rw-r--r--  3.0 unx   526465 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/photosdb.html
 -rw-r--r--  3.0 unx    39730 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosalbum.html
--rw-r--r--  3.0 unx    98734 tx defN 23-Jul-02 16:33 docs/_modules/osxphotos/placeinfo.html
+-rw-r--r--  3.0 unx    99009 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    61579 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
 -rw-r--r--  3.0 unx    61830 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jul-02 16:35 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jul-15 14:32 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Jul-02 16:41 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jul-15 14:32 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jul-02 16:41 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jul-15 14:32 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jul-02 16:41 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jul-15 14:32 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Jul-02 16:41 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jul-15 14:32 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jul-02 16:41 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jul-15 14:32 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   423177 tx defN 23-Jul-02 16:35 docs/cli.html
+-rw-r--r--  3.0 unx   423876 tx defN 23-Jul-15 14:32 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   251521 tx defN 23-Jul-02 16:41 docs/genindex.html
--rw-r--r--  3.0 unx   109432 tx defN 23-Jul-02 16:41 docs/index.html
+-rw-r--r--  3.0 unx   252162 tx defN 23-Jul-15 14:32 docs/genindex.html
+-rw-r--r--  3.0 unx   110079 tx defN 23-Jul-15 14:32 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9745 bx stor 23-Jul-02 16:41 docs/objects.inv
+-rw-r--r--  3.0 unx     9767 bx stor 23-Jul-15 14:32 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jul-02 16:35 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jul-02 16:35 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jul-02 16:41 docs/py-modindex.html
--rw-r--r--  3.0 unx   466218 tx defN 23-Jul-02 16:35 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jul-15 14:32 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jul-15 14:32 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jul-15 14:32 docs/py-modindex.html
+-rw-r--r--  3.0 unx   468865 tx defN 23-Jul-15 14:32 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jul-02 16:41 docs/search.html
--rw-r--r--  3.0 unx   114256 tx defN 23-Jul-02 16:41 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jul-02 16:41 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jul-02 16:41 docs/tutorial.html
-99 files, 6887161 bytes uncompressed, 1446350 bytes compressed:  79.0%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jul-15 14:32 docs/search.html
+-rw-r--r--  3.0 unx   223521 tx defN 23-Jul-15 14:32 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jul-15 14:32 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jul-15 14:32 docs/tutorial.html
+99 files, 7011007 bytes uncompressed, 1458970 bytes compressed:  79.2%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.6 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoexporter.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoexporter - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.photoexporter - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -328,14 +328,15 @@
 <span class="sd">        persons (bool): if True, include persons in exported metadata</span>
 <span class="sd">        preview_suffix (str): t.Optional string to append to end of filename for preview images</span>
 <span class="sd">        preview (bool): if True, also exports preview image</span>
 <span class="sd">        raw_photo (bool, default=False): if True, will also export the associated RAW photo</span>
 <span class="sd">        render_options (RenderOptions): t.Optional osxphotos.phototemplate.RenderOptions instance to specify options for rendering templates</span>
 <span class="sd">        replace_keywords (bool): if True, keyword_template replaces any keywords, otherwise it&#39;s additive</span>
 <span class="sd">        rich (bool): if True, will use rich markup with verbose output</span>
+<span class="sd">        export_aae (bool): if True, also exports adjustments as .AAE file</span>
 <span class="sd">        sidecar_drop_ext (bool, default=False): if True, drops the photo&#39;s extension from sidecar filename (e.g. &#39;IMG_1234.json&#39; instead of &#39;IMG_1234.JPG.json&#39;)</span>
 <span class="sd">        sidecar: bit field (int): set to one or more of `SIDECAR_XMP`, `SIDECAR_JSON`, `SIDECAR_EXIFTOOL`</span>
 <span class="sd">          - SIDECAR_JSON: if set will write a json sidecar with data in format readable by exiftool sidecar filename will be dest/filename.json;</span>
 <span class="sd">          includes exiftool tag group names (e.g. `exiftool -G -j`)</span>
 <span class="sd">          - SIDECAR_EXIFTOOL: if set will write a json sidecar with data in format readable by exiftool sidecar filename will be dest/filename.json;</span>
 <span class="sd">          does not include exiftool tag group names (e.g. `exiftool -j`)</span>
 <span class="sd">          - SIDECAR_XMP: if set will write an XMP sidecar with IPTC data sidecar filename will be dest/filename.xmp</span>
@@ -380,14 +381,15 @@
     <span class="n">persons</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
     <span class="n">preview_suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="n">DEFAULT_PREVIEW_SUFFIX</span>
     <span class="n">preview</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">raw_photo</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">render_options</span><span class="p">:</span> <span class="n">t</span><span class="o">.</span><span class="n">Optional</span><span class="p">[</span><span class="n">RenderOptions</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">replace_keywords</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">rich</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+    <span class="n">export_aae</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">sidecar_drop_ext</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">sidecar</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span>
     <span class="n">strip</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">timeout</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">120</span>
     <span class="n">touch_file</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">update</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
     <span class="n">update_errors</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
@@ -474,14 +476,15 @@
         <span class="s2">&quot;exiftool_warning&quot;</span><span class="p">,</span>
         <span class="s2">&quot;exported&quot;</span><span class="p">,</span>
         <span class="s2">&quot;exported_album&quot;</span><span class="p">,</span>
         <span class="s2">&quot;metadata_changed&quot;</span><span class="p">,</span>
         <span class="s2">&quot;missing&quot;</span><span class="p">,</span>
         <span class="s2">&quot;missing_album&quot;</span><span class="p">,</span>
         <span class="s2">&quot;new&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;aae_written&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_exiftool_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_exiftool_written&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_json_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_json_written&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_xmp_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_xmp_written&quot;</span><span class="p">,</span>
         <span class="s2">&quot;skipped&quot;</span><span class="p">,</span>
@@ -504,14 +507,15 @@
         <span class="n">exiftool_warning</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">exported</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">exported_album</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">metadata_changed</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">missing</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">missing_album</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">new</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+        <span class="n">aae_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_exiftool_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_exiftool_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_json_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_json_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_xmp_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_xmp_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
@@ -543,14 +547,15 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">exported</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">new</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">updated</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">skipped</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">exif_updated</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">touched</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">converted_to_jpeg</span>
+            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">aae_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_json_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_json_skipped</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_exiftool_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_exiftool_skipped</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_xmp_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_xmp_skipped</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">missing</span>
@@ -798,14 +803,16 @@
                 <span class="c1"># don&#39;t know what actual preview suffix would be but most likely jpeg</span>
                 <span class="n">preview_name</span> <span class="o">=</span> <span class="n">dest</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">dest</span><span class="o">.</span><span class="n">stem</span><span class="si">}{</span><span class="n">options</span><span class="o">.</span><span class="n">preview_suffix</span><span class="si">}</span><span class="s2">.jpeg&quot;</span>
                 <span class="n">all_results</span><span class="o">.</span><span class="n">missing</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">preview_name</span><span class="p">)</span>
                 <span class="n">verbose</span><span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;Skipping missing preview photo for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filename</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">original_filename</span><span class="p">)</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">uuid</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
                 <span class="p">)</span>
 
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">export_aae</span><span class="p">:</span>
+            <span class="n">all_results</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_write_aae_file</span><span class="p">(</span><span class="n">dest</span><span class="o">=</span><span class="n">dest</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="n">options</span><span class="p">)</span>
         <span class="n">all_results</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_write_sidecar_files</span><span class="p">(</span><span class="n">dest</span><span class="o">=</span><span class="n">dest</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="n">options</span><span class="p">)</span>
 
         <span class="k">return</span> <span class="n">all_results</span></div>
 
     <span class="k">def</span> <span class="nf">_init_temp_dir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Initialize (if necessary) the object&#39;s temporary directory.</span>
 
@@ -1597,14 +1604,61 @@
             <span class="k">if</span> <span class="ow">not</span> <span class="n">dry_run</span><span class="p">:</span>
                 <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">and</span> <span class="n">dest_new</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
                     <span class="n">FileUtil</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">dest_new</span><span class="p">)</span>
                 <span class="n">FileUtil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">path</span><span class="p">),</span> <span class="nb">str</span><span class="p">(</span><span class="n">dest_new</span><span class="p">))</span>
             <span class="n">exported_paths</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">dest_new</span><span class="p">))</span>
         <span class="k">return</span> <span class="n">exported_paths</span>
 
+    <span class="k">def</span> <span class="nf">_write_aae_file</span><span class="p">(</span>
+        <span class="bp">self</span><span class="p">,</span>
+        <span class="n">dest</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span>
+        <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span><span class="p">,</span>
+    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ExportResults</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Write AAE file for the photo.&quot;&quot;&quot;</span>
+
+        <span class="c1"># AAE files describe adjustments to originals, so they don&#39;t make sense</span>
+        <span class="c1"># for edited files</span>
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">edited</span><span class="p">:</span>
+            <span class="k">return</span> <span class="n">ExportResults</span><span class="p">()</span>
+
+        <span class="n">verbose</span> <span class="o">=</span> <span class="n">options</span><span class="o">.</span><span class="n">verbose</span> <span class="ow">or</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span>
+
+        <span class="n">aae_src</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">adjustments_path</span>
+        <span class="k">if</span> <span class="n">aae_src</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+            <span class="k">return</span> <span class="n">ExportResults</span><span class="p">()</span>
+        <span class="n">aae_dest</span> <span class="o">=</span> <span class="n">dest</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.AAE&quot;</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">export_as_hardlink</span><span class="p">:</span>
+            <span class="k">try</span><span class="p">:</span>
+                <span class="k">if</span> <span class="n">aae_dest</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span> <span class="ow">and</span> <span class="nb">any</span><span class="p">(</span>
+                    <span class="p">[</span><span class="n">options</span><span class="o">.</span><span class="n">overwrite</span><span class="p">,</span> <span class="n">options</span><span class="o">.</span><span class="n">update</span><span class="p">,</span> <span class="n">options</span><span class="o">.</span><span class="n">force_update</span><span class="p">]):</span>
+                    <span class="k">try</span><span class="p">:</span>
+                        <span class="n">options</span><span class="o">.</span><span class="n">fileutil</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">aae_dest</span><span class="p">)</span>
+                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+                        <span class="k">raise</span> <span class="n">ExportError</span><span class="p">(</span>
+                            <span class="sa">f</span><span class="s2">&quot;Error removing file </span><span class="si">{</span><span class="n">aae_dest</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2"> ((</span><span class="si">{</span><span class="n">lineno</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
+                        <span class="p">)</span> <span class="kn">from</span> <span class="nn">e</span>
+                <span class="n">options</span><span class="o">.</span><span class="n">fileutil</span><span class="o">.</span><span class="n">hardlink</span><span class="p">(</span><span class="n">aae_src</span><span class="p">,</span> <span class="n">aae_dest</span><span class="p">)</span>
+            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+                <span class="k">raise</span> <span class="n">ExportError</span><span class="p">(</span>
+                    <span class="sa">f</span><span class="s2">&quot;Error hardlinking </span><span class="si">{</span><span class="n">aae_src</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="n">aae_dest</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">lineno</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
+                <span class="p">)</span> <span class="kn">from</span> <span class="nn">e</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="k">try</span><span class="p">:</span>
+                <span class="n">options</span><span class="o">.</span><span class="n">fileutil</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">aae_src</span><span class="p">,</span> <span class="n">aae_dest</span><span class="p">)</span>
+                <span class="n">verbose</span><span class="p">(</span>
+                    <span class="sa">f</span><span class="s2">&quot;Exported adjustments of </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filename</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">original_filename</span><span class="p">)</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filepath</span><span class="p">(</span><span class="n">normalize_fs_path</span><span class="p">(</span><span class="n">aae_dest</span><span class="p">))</span><span class="si">}</span><span class="s2">&quot;</span>
+                <span class="p">)</span>
+            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+                <span class="k">raise</span> <span class="n">ExportError</span><span class="p">(</span>
+                    <span class="sa">f</span><span class="s2">&quot;Error copying file </span><span class="si">{</span><span class="n">aae_src</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="n">aae_dest</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">lineno</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
+                <span class="p">)</span> <span class="kn">from</span> <span class="nn">e</span>
+
+        <span class="k">return</span> <span class="n">ExportResults</span><span class="p">(</span><span class="n">aae_written</span><span class="o">=</span><span class="p">[</span><span class="n">aae_dest</span><span class="p">])</span>
+
     <span class="k">def</span> <span class="nf">_write_sidecar_files</span><span class="p">(</span>
         <span class="bp">self</span><span class="p">,</span>
         <span class="n">dest</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span>
         <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span><span class="p">,</span>
     <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ExportResults</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;Write sidecar files for the photo.&quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -202,14 +202,15 @@
 associated RAW photo
         render_options (RenderOptions): t.Optional
 osxphotos.phototemplate.RenderOptions instance to specify options for rendering
 templates
         replace_keywords (bool): if True, keyword_template replaces any
 keywords, otherwise it's additive
         rich (bool): if True, will use rich markup with verbose output
+        export_aae (bool): if True, also exports adjustments as .AAE file
         sidecar_drop_ext (bool, default=False): if True, drops the photo's
 extension from sidecar filename (e.g. 'IMG_1234.json' instead of
 'IMG_1234.JPG.json')
         sidecar: bit field (int): set to one or more of `SIDECAR_XMP`,
 `SIDECAR_JSON`, `SIDECAR_EXIFTOOL`
           - SIDECAR_JSON: if set will write a json sidecar with data in format
 readable by exiftool sidecar filename will be dest/filename.json;
@@ -273,14 +274,15 @@
     persons: bool = True
     preview_suffix: str = DEFAULT_PREVIEW_SUFFIX
     preview: bool = False
     raw_photo: bool = False
     render_options: t.Optional[RenderOptions] = None
     replace_keywords: bool = False
     rich: bool = False
+    export_aae: bool = False
     sidecar_drop_ext: bool = False
     sidecar: int = 0
     strip: bool = False
     timeout: int = 120
     touch_file: bool = False
     update: bool = False
     update_errors: bool = False
@@ -368,14 +370,15 @@
         "exiftool_warning",
         "exported",
         "exported_album",
         "metadata_changed",
         "missing",
         "missing_album",
         "new",
+        "aae_written",
         "sidecar_exiftool_skipped",
         "sidecar_exiftool_written",
         "sidecar_json_skipped",
         "sidecar_json_written",
         "sidecar_xmp_skipped",
         "sidecar_xmp_written",
         "skipped",
@@ -398,14 +401,15 @@
         exiftool_warning=None,
         exported=None,
         exported_album=None,
         metadata_changed=None,
         missing=None,
         missing_album=None,
         new=None,
+        aae_written=None,
         sidecar_exiftool_skipped=None,
         sidecar_exiftool_written=None,
         sidecar_json_skipped=None,
         sidecar_json_written=None,
         sidecar_xmp_skipped=None,
         sidecar_xmp_written=None,
         skipped=None,
@@ -437,14 +441,15 @@
             self.exported
             + self.new
             + self.updated
             + self.skipped
             + self.exif_updated
             + self.touched
             + self.converted_to_jpeg
+            + self.aae_written
             + self.sidecar_json_written
             + self.sidecar_json_skipped
             + self.sidecar_exiftool_written
             + self.sidecar_exiftool_skipped
             + self.sidecar_xmp_written
             + self.sidecar_xmp_skipped
             + self.missing
@@ -729,14 +734,16 @@
 {options.preview_suffix}.jpeg"
                 all_results.missing.append(preview_name)
                 verbose(
                     f"Skipping missing preview photo for {self._filename
 (self.photo.original_filename)} ({self._uuid(self.photo.uuid)})"
                 )
 
+        if options.export_aae:
+            all_results += self._write_aae_file(dest=dest, options=options)
         all_results += self._write_sidecar_files(dest=dest, options=options)
 
         return all_results
 
 
     def _init_temp_dir(self, options: ExportOptions):
         """Initialize (if necessary) the object's temporary directory.
@@ -1617,14 +1624,66 @@
             if not dry_run:
                 if overwrite and dest_new.exists():
                     FileUtil.unlink(dest_new)
                 FileUtil.copy(str(path), str(dest_new))
             exported_paths.append(str(dest_new))
         return exported_paths
 
+    def _write_aae_file(
+        self,
+        dest: pathlib.Path,
+        options: ExportOptions,
+    ) -> ExportResults:
+        """Write AAE file for the photo."""
+
+        # AAE files describe adjustments to originals, so they don't make sense
+        # for edited files
+        if options.edited:
+            return ExportResults()
+
+        verbose = options.verbose or self._verbose
+
+        aae_src = self.photo.adjustments_path
+        if aae_src is None:
+            return ExportResults()
+        aae_dest = dest.with_suffix(".AAE")
+
+        if options.export_as_hardlink:
+            try:
+                if aae_dest.exists() and any(
+                    [options.overwrite, options.update, options.force_update]):
+                    try:
+                        options.fileutil.unlink(aae_dest)
+                    except Exception as e:
+                        raise ExportError(
+                            f"Error removing file {aae_dest}: {e} (({lineno
+(__file__)})"
+                        ) from e
+                options.fileutil.hardlink(aae_src, aae_dest)
+            except Exception as e:
+                raise ExportError(
+                    f"Error hardlinking {aae_src} to {aae_dest}: {e} ({lineno
+(__file__)})"
+                ) from e
+        else:
+            try:
+                options.fileutil.copy(aae_src, aae_dest)
+                verbose(
+                    f"Exported adjustments of {self._filename
+(self.photo.original_filename)} to {self._filepath(normalize_fs_path
+(aae_dest))}"
+                )
+            except Exception as e:
+                raise ExportError(
+                    f"Error copying file {aae_src} to {aae_dest}: {e} ({lineno
+(__file__)})"
+                ) from e
+
+        return ExportResults(aae_written=[aae_dest])
+
     def _write_sidecar_files(
         self,
         dest: pathlib.Path,
         options: ExportOptions,
     ) -> ExportResults:
         """Write sidecar files for the photo."""
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -843,36 +843,46 @@
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">hasadjustments</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;True if picture has adjustments / edits&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;hasAdjustments&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="mi">1</span>
 
     <span class="nd">@property</span>
-    <span class="k">def</span> <span class="nf">adjustments</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Returns AdjustmentsInfo class for adjustment data or None if no adjustments; Photos 5+ only&quot;&quot;&quot;</span>
+    <span class="k">def</span> <span class="nf">adjustments_path</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Returns path to adjustments file or none if file doesn&#39;t exist&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">hasadjustments</span><span class="p">:</span>
-            <span class="k">try</span><span class="p">:</span>
-                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_adjustmentinfo</span>
-            <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-                <span class="n">library</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span>
-                <span class="n">directory</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>  <span class="c1"># first char of uuid</span>
-                <span class="n">plist_file</span> <span class="o">=</span> <span class="p">(</span>
-                    <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">library</span><span class="p">)</span>
-                    <span class="o">/</span> <span class="s2">&quot;resources&quot;</span>
-                    <span class="o">/</span> <span class="s2">&quot;renders&quot;</span>
-                    <span class="o">/</span> <span class="n">directory</span>
-                    <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="si">}</span><span class="s2">.plist&quot;</span>
-                <span class="p">)</span>
-                <span class="k">if</span> <span class="ow">not</span> <span class="n">plist_file</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-                    <span class="k">return</span> <span class="kc">None</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">_adjustmentinfo</span> <span class="o">=</span> <span class="n">AdjustmentsInfo</span><span class="p">(</span><span class="n">plist_file</span><span class="p">)</span>
-                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_adjustmentinfo</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">hasadjustments</span><span class="p">:</span>
+            <span class="k">return</span> <span class="kc">None</span>
+
+        <span class="n">library</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span>
+        <span class="n">directory</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>  <span class="c1"># first char of uuid</span>
+        <span class="n">plist_file</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">library</span><span class="p">)</span>
+            <span class="o">/</span> <span class="s2">&quot;resources&quot;</span>
+            <span class="o">/</span> <span class="s2">&quot;renders&quot;</span>
+            <span class="o">/</span> <span class="n">directory</span>
+            <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="si">}</span><span class="s2">.plist&quot;</span>
+        <span class="p">)</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="n">plist_file</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+            <span class="k">return</span> <span class="kc">None</span>
+        <span class="k">return</span> <span class="n">plist_file</span>
+
+    <span class="nd">@property</span>
+    <span class="k">def</span> <span class="nf">adjustments</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Returns AdjustmentsInfo class for adjustment data or None if no adjustments; Photos 5+ only&quot;&quot;&quot;</span>
+        <span class="k">try</span><span class="p">:</span>
+            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_adjustmentinfo</span>
+        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
+            <span class="n">plist_file</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">adjustments_path</span>
+            <span class="k">if</span> <span class="n">plist_file</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+                <span class="k">return</span> <span class="kc">None</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_adjustmentinfo</span> <span class="o">=</span> <span class="n">AdjustmentsInfo</span><span class="p">(</span><span class="n">plist_file</span><span class="p">)</span>
+            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_adjustmentinfo</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">external_edit</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns True if picture was edited outside of Photos using external editor&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;adjustmentFormatID&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;com.apple.Photos.externalEdit&quot;</span>
 
     <span class="nd">@property</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -729,37 +729,47 @@
 
     @property
     def hasadjustments(self):
         """True if picture has adjustments / edits"""
         return self._info["hasAdjustments"] == 1
 
     @property
-    def adjustments(self):
-        """Returns AdjustmentsInfo class for adjustment data or None if no
-adjustments; Photos 5+ only"""
+    def adjustments_path(self):
+        """Returns path to adjustments file or none if file doesn't exist"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return None
 
-        if self.hasadjustments:
-            try:
-                return self._adjustmentinfo
-            except AttributeError:
-                library = self._db._library_path
-                directory = self._uuid[0]  # first char of uuid
-                plist_file = (
-                    pathlib.Path(library)
-                    / "resources"
-                    / "renders"
-                    / directory
-                    / f"{self._uuid}.plist"
-                )
-                if not plist_file.is_file():
-                    return None
-                self._adjustmentinfo = AdjustmentsInfo(plist_file)
-                return self._adjustmentinfo
+        if not self.hasadjustments:
+            return None
+
+        library = self._db._library_path
+        directory = self._uuid[0]  # first char of uuid
+        plist_file = (
+            pathlib.Path(library)
+            / "resources"
+            / "renders"
+            / directory
+            / f"{self._uuid}.plist"
+        )
+        if not plist_file.is_file():
+            return None
+        return plist_file
+
+    @property
+    def adjustments(self):
+        """Returns AdjustmentsInfo class for adjustment data or None if no
+adjustments; Photos 5+ only"""
+        try:
+            return self._adjustmentinfo
+        except AttributeError:
+            plist_file = self.adjustments_path
+            if plist_file is None:
+                return None
+            self._adjustmentinfo = AdjustmentsInfo(plist_file)
+            return self._adjustmentinfo
 
     @property
     def external_edit(self):
         """Returns True if picture was edited outside of Photos using external
 editor"""
         return self._info["adjustmentFormatID"] ==
 "com.apple.Photos.externalEdit"
```

#### docs/_modules/osxphotos/placeinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.placeinfo - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.placeinfo - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -619,16 +619,17 @@
 <span class="sd">        * `street`</span>
 <span class="sd">        * `sub_administrative_area`</span>
 <span class="sd">        * `sub_locality`</span>
 <span class="sd">        * `iso_country_code`</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">pass</span>
 
-    <span class="k">def</span> <span class="nf">asdict</span><span class="p">():</span>
-        <span class="k">pass</span></div>
+<div class="viewcode-block" id="PlaceInfo.asdict"><a class="viewcode-back" href="../../reference.html#osxphotos.PlaceInfo.asdict">[docs]</a>    <span class="k">def</span> <span class="nf">asdict</span><span class="p">():</span>
+        <span class="sd">&quot;&quot;&quot;Returns a dictionary representation of the PlaceInfo object.&quot;&quot;&quot;</span>
+        <span class="k">pass</span></div></div>
 
 
 <span class="k">class</span> <span class="nc">PlaceInfo4</span><span class="p">(</span><span class="n">PlaceInfo</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;Reverse geolocation place info for a photo (Photos &lt;= 4)&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">place_names</span><span class="p">,</span> <span class="n">country_code</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;place_names: list of place name tuples in ascending order by area</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -496,15 +496,16 @@
         * `street`
         * `sub_administrative_area`
         * `sub_locality`
         * `iso_country_code`
         """
         pass
 
-    def asdict():
+[docs]    def asdict():
+        """Returns a dictionary representation of the PlaceInfo object."""
         pass
 
 
 
 class PlaceInfo4(PlaceInfo):
     """Reverse geolocation place info for a photo (Photos <= 4)"""
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.6'
+     - The osxphotos version, e.g. '0.60.7'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.6',
+    VERSION: '0.60.7',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.6 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1890,14 +1890,20 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-download-missing">
 <span class="sig-name descname"><span class="pre">--download-missing</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-download-missing" title="Permalink to this definition">#</a></dt>
 <dd><p>Attempt to download missing photos from iCloud. The current implementation uses Applescript to interact with Photos to export the photo which will force Photos to download from iCloud if the photo does not exist on disk.  This will be slow and will require internet connection. This obviously only works if the Photos library is synched to iCloud.  Note: –download-missing does not currently export all burst images; only the primary photo will be exported–associated burst images will be skipped.</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-export-aae">
+<span class="sig-name descname"><span class="pre">--export-aae</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-export-aae" title="Permalink to this definition">#</a></dt>
+<dd><p>Also export an adjustments file detailing edits made to the original. The resulting file is named photoname.AAE. Note that to import these files back to Photos succesfully, you also need to export the edited photo and match the filename format Photos.app expects: –filename ‘IMG_{edited_version?E,}{id:04d}’ –edited-suffix ‘’</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-sidecar">
 <span class="sig-name descname"><span class="pre">--sidecar</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;FORMAT&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-export-sidecar" title="Permalink to this definition">#</a></dt>
 <dd><p>Create sidecar for each photo exported; valid FORMAT values: xmp, json, exiftool; –sidecar xmp: create XMP sidecar used by Digikam, Adobe Lightroom, etc. The sidecar file is named in format photoname.ext.xmp The XMP sidecar exports the following tags: Description, Title, Keywords/Tags, Subject (set to Keywords + PersonInImage), PersonInImage, CreateDate, ModifyDate, GPSLongitude, Face Regions (Metadata Working Group and Microsoft Photo).
 –sidecar json: create JSON sidecar useable by exiftool (<a class="reference external" href="https://exiftool.org/">https://exiftool.org/</a>) The sidecar file can be used to apply metadata to the file with exiftool, for example: “exiftool -j=photoname.jpg.json photoname.jpg” The sidecar file is named in format photoname.ext.json; format includes tag groups (equivalent to running ‘exiftool -G -j’).
 –sidecar exiftool: create JSON sidecar compatible with output of ‘exiftool -j’. Unlike ‘–sidecar json’, ‘–sidecar exiftool’ does not export tag groups. Sidecar filename is in format photoname.ext.json; For a list of tags exported in the JSON and exiftool sidecar, see ‘–exiftool’. See also ‘–ignore-signature’.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Options<span class="colon">:</span></dt>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -959,14 +959,20 @@
       implementation uses Applescript to interact with Photos to export the
       photo which will force Photos to download from iCloud if the photo does
       not exist on disk. This will be slow and will require internet
       connection. This obviously only works if the Photos library is synched to
       iCloud. Note: âdownload-missing does not currently export all burst
       images; only the primary photo will be exportedâassociated burst images
       will be skipped.
+  --export-aae#
+      Also export an adjustments file detailing edits made to the original. The
+      resulting file is named photoname.AAE. Note that to import these files
+      back to Photos succesfully, you also need to export the edited photo and
+      match the filename format Photos.app expects: âfilename âIMG_
+      {edited_version?E,}{id:04d}â âedited-suffix ââ
   --sidecar <FORMAT>#
       Create sidecar for each photo exported; valid FORMAT values: xmp, json,
       exiftool; âsidecar xmp: create XMP sidecar used by Digikam, Adobe
       Lightroom, etc. The sidecar file is named in format photoname.ext.xmp The
       XMP sidecar exports the following tags: Description, Title, Keywords/
       Tags, Subject (set to Keywords + PersonInImage), PersonInImage,
       CreateDate, ModifyDate, GPSLongitude, Face Regions (Metadata Working
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.6 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.7 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -770,14 +770,21 @@
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-orphans-export">osxphotos-orphans command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-e">osxphotos-sync command line option</a>
 </li>
         </ul></li>
         <li>
+    --export-aae
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-export-export-aae">osxphotos-export command line option</a>
+</li>
+        </ul></li>
+        <li>
     --export-as-hardlink
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-export-export-as-hardlink">osxphotos-export command line option</a>
 </li>
         </ul></li>
         <li>
@@ -3032,14 +3039,16 @@
 </li>
         <li><a href="reference.html#osxphotos.PlaceInfo.address_str">address_str (osxphotos.PlaceInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExifTool.addvalues">addvalues() (osxphotos.ExifTool method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.adjustments">adjustments (osxphotos.PhotoInfo property)</a>
 </li>
+        <li><a href="reference.html#osxphotos.PhotoInfo.adjustments_path">adjustments_path (osxphotos.PhotoInfo property)</a>
+</li>
         <li><a href="reference.html#osxphotos.QueryOptions.album">album (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.FolderInfo.album_info">album_info (osxphotos.FolderInfo property)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.PhotoInfo.album_info">(osxphotos.PhotoInfo property)</a>
 </li>
@@ -3090,14 +3099,16 @@
 </li>
           <li><a href="reference.html#osxphotos.MomentInfo.asdict">(osxphotos.MomentInfo method)</a>
 </li>
           <li><a href="reference.html#osxphotos.PersonInfo.asdict">(osxphotos.PersonInfo method)</a>
 </li>
           <li><a href="reference.html#osxphotos.PhotoInfo.asdict">(osxphotos.PhotoInfo method)</a>
 </li>
+          <li><a href="reference.html#osxphotos.PlaceInfo.asdict">(osxphotos.PlaceInfo method)</a>
+</li>
           <li><a href="reference.html#osxphotos.ScoreInfo.asdict">(osxphotos.ScoreInfo method)</a>
 </li>
           <li><a href="reference.html#osxphotos.SearchInfo.asdict">(osxphotos.SearchInfo method)</a>
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.ExportResults.attributes">attributes (osxphotos.ExportResults property)</a>
 </li>
@@ -3289,22 +3300,24 @@
 </li>
         <li><a href="reference.html#osxphotos.PhotoExporter.exiftool_json_sidecar">exiftool_json_sidecar() (osxphotos.PhotoExporter method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoTemplate.expand_variables">expand_variables() (osxphotos.PhotoTemplate method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoTemplate.expand_variables_to_str">expand_variables_to_str() (osxphotos.PhotoTemplate method)</a>
 </li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.PhotoExporter.export">export() (osxphotos.PhotoExporter method)</a>
 
         <ul>
           <li><a href="reference.html#osxphotos.PhotoInfo.export">(osxphotos.PhotoInfo method)</a>
 </li>
         </ul></li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.ExportOptions.export_aae">export_aae (osxphotos.ExportOptions attribute)</a>
+</li>
         <li><a href="reference.html#osxphotos.ExportOptions.export_as_hardlink">export_as_hardlink (osxphotos.ExportOptions attribute)</a>
 </li>
         <li>
     EXPORT_DATABASE
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE">osxphotos-exportdb command line option</a>
@@ -4219,14 +4232,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-exiftool-merge-persons">--exiftool-merge-persons</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-exiftool-option">--exiftool-option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-exiftool-path">--exiftool-path</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-export-aae">--export-aae</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-export-as-hardlink">--export-as-hardlink</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-export-by-date">--export-by-date</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-exportdb">--exportdb</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-external-edit">--external-edit</a>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -41,928 +41,933 @@
 | S | T | U | V | W | Y
 
 ***** Symbols *****
     * --add-exported-to-album
           o osxphotos-export_command
             line_option
     * --add-missing-to-album
-          o osxphotos-export_command        * --not-hdr
-            line_option                           o osxphotos-add-locations
-    * --add-skipped-to-album                        command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-    * --add-to-album                              o osxphotos-query_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-timewarp_command              option
-            line_option                           o osxphotos-sync_command_line
-    * --added-after                                 option
-          o osxphotos-add-locations         * --not-hidden
-            command_line_option                   o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-sync_command_line
-    * --added-before                                option
-          o osxphotos-add-locations         * --not-in-album
-            command_line_option                   o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-sync_command_line
-    * --added-in-last                               option
-          o osxphotos-add-locations         * --not-incloud
-            command_line_option                   o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-sync_command_line
-    * --album                                       option
-          o osxphotos-add-locations         * --not-live
-            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command
+            line_option                     * --not-hdr
+    * --add-skipped-to-album                      o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
-            option                          * --not-missing
-    * --album-keyword                             o osxphotos-add-locations
-          o osxphotos-exiftool_command              command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --alt-copy                                    line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
+    * --add-to-album                                line_option
+          o osxphotos-query_command               o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-timewarp_command            o osxphotos-repl_command_line
             line_option                             option
-    * --append                                    o osxphotos-sync_command_line
-          o osxphotos-exiftool_command              option
-            line_option                     * --not-panorama
+    * --added-after                               o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --not-hidden
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-exportdb_command            o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-import_command              o osxphotos-query_command
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-query_command
+            option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --burst                                     o osxphotos-sync_command_line
+    * --added-before                              o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-portrait
+            command_line_option             * --not-in-album
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --check-signatures                          o osxphotos-sync_command_line
-          o osxphotos-exportdb_command              option
-            line_option                     * --not-reference
-    * --check-templates                           o osxphotos-add-locations
-          o osxphotos-import_command                command_line_option
-            line_option                           o osxphotos-export_command
-    * --cleanup                                     line_option
-          o osxphotos-export_command              o osxphotos-query_command
-            line_option                             line_option
-    * --clear-location                            o osxphotos-repl_command_line
-          o osxphotos-import_command                option
-            line_option                           o osxphotos-sync_command_line
-    * --clear-metadata                              option
-          o osxphotos-import_command        * --not-saved-to-library
-            line_option                           o osxphotos-add-locations
-    * --clone                                       command_line_option
-          o osxphotos-theme_command               o osxphotos-export_command
+    * --added-in-last                             o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --not-incloud
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-    * --cloudasset                                o osxphotos-query_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-repl_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-query_command                 option
-            line_option                     * --not-screenshot
-          o osxphotos-repl_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-sync_command_line           o osxphotos-export_command
+          o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
-    * --compare-exif                              o osxphotos-query_command
-          o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-repl_command_line
-    * --config                                      option
-          o osxphotos-theme_command               o osxphotos-sync_command_line
-            line_option                             option
-    * --config-only                         * --not-selfie
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --album                                     o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --not-live
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-    * --convert-to-jpeg                           o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --count                                       line_option
-          o osxphotos-query_command               o osxphotos-repl_command_line
-            line_option                             option
-    * --current-name                              o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --not-shared
-    * --date                                      o osxphotos-add-locations
-          o osxphotos-timewarp_command              command_line_option
-            line_option                           o osxphotos-export_command
-    * --date-added                                  line_option
-          o osxphotos-timewarp_command            o osxphotos-query_command
+          o osxphotos-import_command              o osxphotos-export_command
             line_option                             line_option
-    * --date-added-from-photo                     o osxphotos-repl_command_line
-          o osxphotos-timewarp_command              option
-            line_option                     * --not-slow-mo
-    * --date-delta                                o osxphotos-add-locations
-          o osxphotos-timewarp_command              command_line_option
-            line_option                           o osxphotos-export_command
-    * --db                                          line_option
-          o osxphotos-albums_command              o osxphotos-query_command
+          o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-batch-edit                  o osxphotos-repl_command_line
-            command_line_option                     option
-          o osxphotos-diff_command_line           o osxphotos-sync_command_line
+          o osxphotos-repl_command_line           o osxphotos-repl_command_line
             option                                  option
-          o osxphotos-dump_command_line     * --not-syndicated
-            option                                o osxphotos-add-locations
-          o osxphotos-exiftool_command              command_line_option
-            line_option                           o osxphotos-export_command
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --album-keyword                       * --not-missing
+          o osxphotos-exiftool_command            o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+    * --alt-copy                                  o osxphotos-query_command
           o osxphotos-export_command                line_option
+            line_option                           o osxphotos-repl_command_line
+    * --append                                      option
+          o osxphotos-exiftool_command            o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-export_command        * --not-panorama
+            line_option                           o osxphotos-add-locations
+          o osxphotos-exportdb_command              command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-import_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-info_command_line             line_option
+          o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
-          o osxphotos-inspect_command               option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-keywords_command              option
-            line_option                     * --not-time-lapse
-          o osxphotos-labels_command              o osxphotos-add-locations
+    * --burst                                       option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * --not-portrait
+            line_option                           o osxphotos-add-locations
+          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-query_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-repl_command_line
+    * --check-signatures                            option
+          o osxphotos-exportdb_command            o osxphotos-sync_command_line
+            line_option                             option
+    * --check-templates                     * --not-reference
+          o osxphotos-import_command              o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-orphans_command             o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-persons_command             o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-places_command              o osxphotos-repl_command_line
+    * --cleanup                                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-query_command
+    * --clear-location                              line_option
+          o osxphotos-import_command              o osxphotos-repl_command_line
+            line_option                             option
+    * --clear-metadata                            o osxphotos-sync_command_line
+          o osxphotos-import_command                option
+            line_option                     * --not-saved-to-library
+    * --clone                                     o osxphotos-add-locations
+          o osxphotos-theme_command                 command_line_option
+            line_option                           o osxphotos-export_command
+    * --cloudasset                                  line_option
+          o osxphotos-add-locations               o osxphotos-query_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
           o osxphotos-query_command               o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-repl_command_line     * --only-movies
+          o osxphotos-repl_command_line     * --not-screenshot
             option                                o osxphotos-add-locations
-          o osxphotos-show_command_line             command_line_option
+          o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-export_command
-          o osxphotos-snap_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --db-config                                   option
-          o osxphotos-exiftool_command            o osxphotos-sync_command_line
-            line_option                             option
-    * --default                             * --only-new
-          o osxphotos-theme_command               o osxphotos-export_command
+    * --compare-exif                                line_option
+          o osxphotos-timewarp_command            o osxphotos-query_command
+            line_option                             line_option
+    * --config                                    o osxphotos-repl_command_line
+          o osxphotos-theme_command                 option
+            line_option                           o osxphotos-sync_command_line
+    * --config-only                                 option
+          o osxphotos-export_command        * --not-selfie
+            line_option                           o osxphotos-add-locations
+    * --convert-to-jpeg                             command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --delete                              * --only-photos
-          o osxphotos-theme_command               o osxphotos-add-locations
+    * --count                                     o osxphotos-query_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-repl_command_line
+    * --current-name                                option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+    * --date                                * --not-shared
+          o osxphotos-timewarp_command            o osxphotos-add-locations
             line_option                             command_line_option
-    * --delete-file                               o osxphotos-export_command
-          o osxphotos-exportdb_command              line_option
+    * --date-added                                o osxphotos-export_command
+          o osxphotos-timewarp_command              line_option
             line_option                           o osxphotos-query_command
-    * --delete-uuid                                 line_option
-          o osxphotos-exportdb_command            o osxphotos-repl_command_line
+    * --date-added-from-photo                       line_option
+          o osxphotos-timewarp_command            o osxphotos-repl_command_line
             line_option                             option
-    * --deleted                                   o osxphotos-sync_command_line
+    * --date-delta                          * --not-slow-mo
+          o osxphotos-timewarp_command            o osxphotos-add-locations
+            line_option                             command_line_option
+    * --db                                        o osxphotos-export_command
+          o osxphotos-albums_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-diff_command_line             option
+            option                                o osxphotos-sync_command_line
           o osxphotos-dump_command_line             option
-            option                          * --original-suffix
+            option                          * --not-syndicated
+          o osxphotos-exiftool_command            o osxphotos-add-locations
+            line_option                             command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --overwrite
+          o osxphotos-info_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-inspect_command             o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-keywords_command            o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-labels_command        * --not-time-lapse
+            line_option                           o osxphotos-add-locations
+          o osxphotos-orphans_command               command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --panorama
-    * --deleted-only                              o osxphotos-add-locations
-          o osxphotos-dump_command_line             command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-export_command                line_option
+          o osxphotos-persons_command               line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-query_command                 line_option
+          o osxphotos-places_command                line_option
             line_option                           o osxphotos-repl_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
-            option                                o osxphotos-sync_command_line
-    * --description                                 option
-          o osxphotos-add-locations         * --parse-date
-            command_line_option                   o osxphotos-import_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option                   o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
-            line_option                     * --person
-          o osxphotos-import_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
+            option                          * --only-movies
+          o osxphotos-show_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-snap_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --description-template                      o osxphotos-sync_command_line
+          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                  line_option
+    * --db-config                                 o osxphotos-repl_command_line
           o osxphotos-exiftool_command              option
-            line_option                     * --person-keyword
-          o osxphotos-export_command              o osxphotos-exiftool_command
+            line_option                           o osxphotos-sync_command_line
+    * --default                                     option
+          o osxphotos-theme_command         * --only-new
+            line_option                           o osxphotos-export_command
+    * --delete                                      line_option
+          o osxphotos-theme_command         * --only-photos
+            line_option                           o osxphotos-add-locations
+    * --delete-file                                 command_line_option
+          o osxphotos-exportdb_command            o osxphotos-export_command
             line_option                             line_option
-    * --detect-text                               o osxphotos-export_command
-          o osxphotos-inspect_command               line_option
-            line_option                     * --place
-    * --directory                                 o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
+    * --delete-uuid                               o osxphotos-query_command
+          o osxphotos-exportdb_command              line_option
+            line_option                           o osxphotos-repl_command_line
+    * --deleted                                     option
+          o osxphotos-dump_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-export_command        * --original-suffix
             line_option                           o osxphotos-export_command
-    * --download-missing                            line_option
-          o osxphotos-export_command              o osxphotos-query_command
+          o osxphotos-query_command                 line_option
+            line_option                     * --overwrite
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --deleted-only                        * --panorama
+          o osxphotos-dump_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --dry-run                                   o osxphotos-repl_command_line
+          o osxphotos-query_command               o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --description                               o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-batch-edit                    option
-            command_line_option             * --plain
-          o osxphotos-exiftool_command            o osxphotos-timewarp_command
+            command_line_option             * --parse-date
+          o osxphotos-batch-edit                  o osxphotos-import_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-export_command        * --portrait
+          o osxphotos-import_command        * --person
             line_option                           o osxphotos-add-locations
-          o osxphotos-exportdb_command              command_line_option
+          o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
+          o osxphotos-repl_command_line             line_option
             option                                o osxphotos-query_command
-    * --dup-check                                   line_option
-          o osxphotos-import_command              o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-repl_command_line
+    * --description-template                        option
+          o osxphotos-exiftool_command            o osxphotos-sync_command_line
             line_option                             option
-    * --duplicate                                 o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --post-command
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-export_command        * --person-keyword
+            line_option                           o osxphotos-exiftool_command
+    * --detect-text                                 line_option
+          o osxphotos-inspect_command             o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --post-function
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --preview
-    * --edit                                      o osxphotos-export_command
-          o osxphotos-theme_command                 line_option
-            line_option                           o osxphotos-theme_command
-    * --edited                                      line_option
-          o osxphotos-add-locations         * --preview-if-missing
-            command_line_option                   o osxphotos-export_command
+    * --directory                           * --place
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+    * --download-missing                          o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                     * --preview-suffix
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line     * --print
-            option                                o osxphotos-dump_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-export_command
-    * --edited-suffix                               line_option
-          o osxphotos-export_command              o osxphotos-query_command
-            line_option                             line_option
-    * --emacs                               * --pull-exif
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+            line_option                           o osxphotos-query_command
+    * --dry-run                                     line_option
+          o osxphotos-add-locations               o osxphotos-repl_command_line
+            command_line_option                     option
+          o osxphotos-batch-edit                  o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-exiftool_command      * --plain
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * --portrait
+          o osxphotos-exportdb_command            o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --dup-check                                 o osxphotos-query_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-repl_command_line
+    * --duplicate                                   option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * --post-command
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                     * --post-function
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-import_command
             option                                  line_option
-    * --errors                              * --push-exif
-          o osxphotos-exportdb_command            o osxphotos-timewarp_command
+    * --edit                                * --preview
+          o osxphotos-theme_command               o osxphotos-export_command
             line_option                             line_option
-    * --exif                                * --query-eval
-          o osxphotos-add-locations               o osxphotos-add-locations
-            command_line_option                     command_line_option
+    * --edited                                    o osxphotos-theme_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --preview-if-missing
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+          o osxphotos-query_command         * --preview-suffix
+            line_option                           o osxphotos-export_command
+          o osxphotos-repl_command_line             line_option
+            option                          * --print
+          o osxphotos-sync_command_line           o osxphotos-dump_command_line
             option                                  option
-    * --exiftool                            * --query-function
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-import_command              o osxphotos-export_command
-            line_option                             line_option
-    * --exiftool-merge-keywords                   o osxphotos-query_command
-          o osxphotos-exiftool_command              line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-    * --exiftool-merge-persons                      option
-          o osxphotos-exiftool_command      * --quiet
-            line_option                           o osxphotos-query_command
+    * --edited-suffix                             o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                     * --ramdb
-    * --exiftool-option                           o osxphotos-export_command
-          o osxphotos-exiftool_command              line_option
-            line_option                     * --raw-output
-          o osxphotos-export_command              o osxphotos-diff_command_line
+            line_option                           o osxphotos-query_command
+    * --emacs                                       line_option
+          o osxphotos-repl_command_line     * --pull-exif
+            option                                o osxphotos-timewarp_command
+    * --errors                                      line_option
+          o osxphotos-exportdb_command      * --push-exif
+            line_option                           o osxphotos-timewarp_command
+    * --exif                                        line_option
+          o osxphotos-add-locations         * --query-eval
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --exiftool                                    option
+          o osxphotos-export_command        * --query-function
+            line_option                           o osxphotos-add-locations
+          o osxphotos-import_command                command_line_option
+            line_option                           o osxphotos-export_command
+    * --exiftool-merge-keywords                     line_option
+          o osxphotos-exiftool_command            o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
-    * --exiftool-path                       * --regex
-          o osxphotos-exiftool_command            o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+    * --exiftool-merge-persons                    o osxphotos-sync_command_line
+          o osxphotos-exiftool_command              option
+            line_option                     * --quiet
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-import_command              o osxphotos-query_command
+    * --exiftool-option                     * --ramdb
+          o osxphotos-exiftool_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-timewarp_command            o osxphotos-repl_command_line
+          o osxphotos-export_command        * --raw-output
+            line_option                           o osxphotos-diff_command_line
+    * --exiftool-path                               option
+          o osxphotos-exiftool_command      * --regex
+            line_option                           o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-timewarp_command              line_option
+            line_option                           o osxphotos-repl_command_line
+    * --export                                      option
+          o osxphotos-orphans_command             o osxphotos-sync_command_line
             line_option                             option
-    * --export                                    o osxphotos-sync_command_line
-          o osxphotos-orphans_command               option
-            line_option                     * --relative-to
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-    * --export-as-hardlink                  * --replace-keywords
-          o osxphotos-export_command              o osxphotos-batch-edit
-            line_option                             command_line_option
-    * --export-by-date                            o osxphotos-exiftool_command
+          o osxphotos-sync_command_line     * --relative-to
+            option                                o osxphotos-import_command
+    * --export-aae                                  line_option
+          o osxphotos-export_command        * --replace-keywords
+            line_option                           o osxphotos-batch-edit
+    * --export-as-hardlink                          command_line_option
+          o osxphotos-export_command              o osxphotos-exiftool_command
+            line_option                             line_option
+    * --export-by-date                            o osxphotos-export_command
           o osxphotos-export_command                line_option
+            line_option                     * --report
+    * --export-dir                                o osxphotos-exiftool_command
+          o osxphotos-exportdb_command              line_option
             line_option                           o osxphotos-export_command
-    * --export-dir                                  line_option
-          o osxphotos-exportdb_command      * --report
-            line_option                           o osxphotos-exiftool_command
     * --exportdb                                    line_option
-          o osxphotos-exiftool_command            o osxphotos-export_command
+          o osxphotos-exiftool_command            o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-export_command              o osxphotos-exportdb_command
+          o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-    * --external-edit                             o osxphotos-import_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --resume
-          o osxphotos-query_command               o osxphotos-import_command
+    * --external-edit                             o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --resume
+          o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --retry
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
+          o osxphotos-query_command         * --retry
+            line_option                           o osxphotos-export_command
+          o osxphotos-repl_command_line             line_option
             option                          * --run
-    * --favorite                                  o osxphotos-version_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --save-config
-          o osxphotos-export_command              o osxphotos-exiftool_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-exportdb_command
+          o osxphotos-sync_command_line           o osxphotos-version_command
             option                                  line_option
-          o osxphotos-sync_command_line     * --saved-to-library
-            option                                o osxphotos-add-locations
-    * --favorite-rating                             command_line_option
+    * --favorite                            * --save-config
+          o osxphotos-add-locations               o osxphotos-exiftool_command
+            command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --field                                     o osxphotos-query_command
-          o osxphotos-dump_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
-    * --filename                                    option
-          o osxphotos-export_command        * --screenshot
-            line_option                           o osxphotos-add-locations
-          o osxphotos-uuid_command_line             command_line_option
+          o osxphotos-query_command               o osxphotos-exportdb_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --saved-to-library
+            option                                o osxphotos-add-locations
+          o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-export_command
-    * --finder-tag-keywords                         line_option
+    * --favorite-rating                             line_option
           o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-    * --finder-tag-template                       o osxphotos-repl_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-    * --folder                                      option
-          o osxphotos-add-locations         * --selected
-            command_line_option                   o osxphotos-add-locations
+    * --field                                     o osxphotos-repl_command_line
+          o osxphotos-dump_command_line             option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
+            line_option                     * --screenshot
+    * --filename                                  o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
+          o osxphotos-uuid_command_line             line_option
+            option                                o osxphotos-query_command
+    * --finder-tag-keywords                         line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+    * --finder-tag-template                       o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --selected
+    * --folder                                    o osxphotos-add-locations
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-repl_command_line             option
             option                                o osxphotos-sync_command_line
-    * --force                                       option
-          o osxphotos-timewarp_command      * --selfie
-            line_option                           o osxphotos-add-locations
-    * --force-update                                command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-sync_command_line             option
+            option                          * --selfie
+    * --force                                     o osxphotos-add-locations
+          o osxphotos-timewarp_command              command_line_option
+            line_option                           o osxphotos-export_command
+    * --force-update                                line_option
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-    * --from-date                                 o osxphotos-query_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-repl_command_line
+    * --from-date                                 o osxphotos-repl_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-sync_command_line
           o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-query_command                 option
             line_option                     * --set
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-sync_command_line     * --shared
+          o osxphotos-query_command               o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-repl_command_line     * --shared
             option                                o osxphotos-add-locations
-    * --from-time                                   command_line_option
-          o osxphotos-add-locations               o osxphotos-export_command
+          o osxphotos-sync_command_line             command_line_option
+            option                                o osxphotos-export_command
+    * --from-time                                   line_option
+          o osxphotos-add-locations               o osxphotos-query_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-repl_command_line
+          o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-repl_command_line     * --sidecar
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --sidecar-drop-ext
-    * --function                                  o osxphotos-export_command
-          o osxphotos-timewarp_command              line_option
-            line_option                     * --skip-bursts
-    * --glob                                      o osxphotos-export_command
-          o osxphotos-import_command                line_option
-            line_option                     * --skip-edited
-    * --has-comment                               o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --skip-live
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-query_command         * --skip-original-if-edited
+          o osxphotos-query_command         * --sidecar
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
-            option                          * --skip-raw
+            option                          * --sidecar-drop-ext
           o osxphotos-sync_command_line           o osxphotos-export_command
             option                                  line_option
-    * --has-likes                           * --skip-uuid
+    * --function                            * --skip-bursts
+          o osxphotos-timewarp_command            o osxphotos-export_command
+            line_option                             line_option
+    * --glob                                * --skip-edited
+          o osxphotos-import_command              o osxphotos-export_command
+            line_option                             line_option
+    * --has-comment                         * --skip-live
           o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-export_command        * --skip-uuid-from-file
+          o osxphotos-export_command        * --skip-original-if-edited
             line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
+            line_option                     * --skip-raw
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * --skip-uuid
+            option                                o osxphotos-export_command
+    * --has-likes                                   line_option
+          o osxphotos-add-locations         * --skip-uuid-from-file
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                     * --slow-mo
-          o osxphotos-repl_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-sync_command_line           o osxphotos-export_command
+          o osxphotos-query_command               o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
-    * --has-raw                                   o osxphotos-query_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                  line_option
+    * --has-raw                                   o osxphotos-repl_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-sync_command_line
           o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-query_command                 option
             line_option                     * --split-folder
-          o osxphotos-repl_command_line           o osxphotos-import_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * --sql
+          o osxphotos-query_command               o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --sql
             option                                o osxphotos-exportdb_command
-    * --hdr                                         line_option
-          o osxphotos-add-locations         * --strip
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                     * --style
-          o osxphotos-query_command               o osxphotos-diff_command_line
+          o osxphotos-sync_command_line             line_option
+            option                          * --strip
+    * --hdr                                       o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --style
+          o osxphotos-export_command              o osxphotos-diff_command_line
             line_option                             option
-          o osxphotos-repl_command_line     * --syndicated
-            option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
+          o osxphotos-query_command         * --syndicated
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-query_command
     * --help                                        line_option
-          o osxphotos-run_command_line            o osxphotos-query_command
-            option                                  line_option
-    * --hidden                                    o osxphotos-repl_command_line
+          o osxphotos-run_command_line            o osxphotos-repl_command_line
+            option                                  option
+    * --hidden                                    o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --template
-          o osxphotos-query_command               o osxphotos-inspect_command
+            command_line_option             * --template
+          o osxphotos-export_command              o osxphotos-inspect_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --theme
-            option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
+          o osxphotos-query_command         * --theme
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-batch-edit
-    * --ignore-case                                 command_line_option
-          o osxphotos-add-locations               o osxphotos-exiftool_command
+          o osxphotos-sync_command_line             command_line_option
+            option                                o osxphotos-exiftool_command
+    * --ignore-case                                 line_option
+          o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-export_command              o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-exportdb_command
+          o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-import_command
+          o osxphotos-repl_command_line           o osxphotos-inspect_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-inspect_command
+          o osxphotos-sync_command_line           o osxphotos-orphans_command
             option                                  line_option
-    * --ignore-date-modified                      o osxphotos-orphans_command
-          o osxphotos-exiftool_command              line_option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-timewarp_command
-    * --ignore-signature                            line_option
-          o osxphotos-export_command        * --time
+    * --ignore-date-modified                      o osxphotos-sync_command_line
+          o osxphotos-exiftool_command              option
             line_option                           o osxphotos-timewarp_command
-    * --import                                      line_option
-          o osxphotos-sync_command_line     * --time-delta
-            option                                o osxphotos-timewarp_command
-    * --in-album                                    line_option
-          o osxphotos-add-locations         * --time-lapse
-            command_line_option                   o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
+          o osxphotos-export_command                line_option
+            line_option                     * --time
+    * --ignore-signature                          o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * --time-delta
+    * --import                                    o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --time-lapse
+    * --in-album                                  o osxphotos-add-locations
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-repl_command_line             option
             option                                o osxphotos-sync_command_line
-    * --incloud                                     option
-          o osxphotos-add-locations         * --timestamp
-            command_line_option                   o osxphotos-add-locations
+          o osxphotos-sync_command_line             option
+            option                          * --timestamp
+    * --incloud                                   o osxphotos-add-locations
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-batch-edit
           o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-batch-edit
-          o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-diff_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-exiftool_command
-          o osxphotos-sync_command_line             line_option
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-exiftool_command
+          o osxphotos-repl_command_line             line_option
             option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-exportdb_command
     * --info                                        line_option
-          o osxphotos-exportdb_command            o osxphotos-exportdb_command
+          o osxphotos-exportdb_command            o osxphotos-import_command
             line_option                             line_option
-    * --inspect                                   o osxphotos-import_command
+    * --inspect                                   o osxphotos-orphans_command
           o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-orphans_command
-    * --is-reference                                line_option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option, [1]
-          o osxphotos-query_command         * --timezone
+            line_option                           o osxphotos-sync_command_line
+    * --is-reference                                option
+          o osxphotos-add-locations               o osxphotos-timewarp_command
+            command_line_option                     line_option, [1]
+          o osxphotos-export_command        * --timezone
             line_option                           o osxphotos-timewarp_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --title
-          o osxphotos-sync_command_line           o osxphotos-add-locations
+          o osxphotos-query_command                 line_option
+            line_option                     * --title
+          o osxphotos-repl_command_line           o osxphotos-add-locations
             option                                  command_line_option
-    * --jpeg-ext                                  o osxphotos-batch-edit
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
+          o osxphotos-sync_command_line           o osxphotos-batch-edit
+            option                                  command_line_option
+    * --jpeg-ext                                  o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-import_command
     * --jpeg-quality                                line_option
-          o osxphotos-export_command              o osxphotos-import_command
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-    * --json                                      o osxphotos-query_command
-          o osxphotos-albums_command                line_option
-            line_option                           o osxphotos-repl_command_line
+    * --json                                      o osxphotos-repl_command_line
+          o osxphotos-albums_command                option
+            line_option                           o osxphotos-sync_command_line
           o osxphotos-dump_command_line             option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-info_command_line             option
             option                          * --tmpdir
-          o osxphotos-keywords_command            o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-labels_command        * --to-date
+          o osxphotos-info_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-keywords_command      * --to-date
             line_option                           o osxphotos-add-locations
-          o osxphotos-list_command_line             command_line_option
-            option                                o osxphotos-export_command
+          o osxphotos-labels_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-list_command_line             line_option
+            option                                o osxphotos-query_command
           o osxphotos-persons_command               line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-places_command                line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
+          o osxphotos-places_command                option
             line_option                           o osxphotos-sync_command_line
-    * --keep                                        option
-          o osxphotos-export_command        * --to-time
-            line_option                           o osxphotos-add-locations
-    * --keyword                                     command_line_option
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-batch-edit                  o osxphotos-query_command
+          o osxphotos-query_command                 option
+            line_option                     * --to-time
+    * --keep                                      o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+    * --keyword                                     line_option
+          o osxphotos-add-locations               o osxphotos-query_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-import_command              o osxphotos-sync_command_line
+          o osxphotos-batch-edit                  o osxphotos-repl_command_line
+            command_line_option                     option
+          o osxphotos-export_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-query_command         * --touch-file
+          o osxphotos-import_command        * --touch-file
             line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-exportdb_command
           o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-exportdb_command
-          o osxphotos-sync_command_line             line_option
             option                          * --undo
-    * --keyword-template                          o osxphotos-batch-edit
-          o osxphotos-exiftool_command              command_line_option
-            line_option                     * --unmatched
-          o osxphotos-export_command              o osxphotos-sync_command_line
+          o osxphotos-sync_command_line           o osxphotos-batch-edit
+            option                                  command_line_option
+    * --keyword-template                    * --unmatched
+          o osxphotos-exiftool_command            o osxphotos-sync_command_line
             line_option                             option
-    * --label                               * --update
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * --update-errors
+          o osxphotos-export_command        * --update
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
+    * --label                                       line_option
+          o osxphotos-add-locations         * --update-errors
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                     * --update-signatures
-          o osxphotos-repl_command_line           o osxphotos-exportdb_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * --upgrade
+          o osxphotos-query_command               o osxphotos-exportdb_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --upgrade
             option                                o osxphotos-install_command
-    * --last-errors                                 line_option
-          o osxphotos-exportdb_command      * --use-file-time
-            line_option                           o osxphotos-timewarp_command
-    * --last-run                                    line_option
-          o osxphotos-exportdb_command      * --use-photokit
-            line_option                           o osxphotos-export_command
-    * --library                                     line_option
-          o osxphotos-albums_command        * --use-photos-export
-            line_option                           o osxphotos-export_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option             * --uti
-          o osxphotos-diff_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-dump_command_line           o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --use-file-time
+    * --last-errors                               o osxphotos-timewarp_command
+          o osxphotos-exportdb_command              line_option
+            line_option                     * --use-photokit
+    * --last-run                                  o osxphotos-export_command
+          o osxphotos-exportdb_command              line_option
+            line_option                     * --use-photos-export
+    * --library                                   o osxphotos-export_command
+          o osxphotos-albums_command                line_option
+            line_option                     * --uti
+          o osxphotos-batch-edit                  o osxphotos-add-locations
+            command_line_option                     command_line_option
+          o osxphotos-diff_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-exiftool_command            o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
+          o osxphotos-dump_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-exiftool_command            o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-info_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-inspect_command       * --uuid
-            line_option                           o osxphotos-add-locations
-          o osxphotos-keywords_command              command_line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-info_command_line     * --uuid
+            option                                o osxphotos-add-locations
+          o osxphotos-inspect_command               command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-labels_command                line_option
+          o osxphotos-keywords_command              line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-orphans_command               line_option
+          o osxphotos-labels_command                line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-persons_command               option
+          o osxphotos-orphans_command               option
             line_option                           o osxphotos-sync_command_line
-          o osxphotos-places_command                option
+          o osxphotos-persons_command               option
             line_option                     * --uuid-files
-          o osxphotos-query_command               o osxphotos-exportdb_command
+          o osxphotos-places_command              o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --uuid-from-file
-            option                                o osxphotos-add-locations
-          o osxphotos-show_command_line             command_line_option
+          o osxphotos-query_command         * --uuid-from-file
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-export_command
-          o osxphotos-snap_command_line             line_option
+          o osxphotos-show_command_line             line_option
             option                                o osxphotos-query_command
-          o osxphotos-sync_command_line             line_option
+          o osxphotos-snap_command_line             line_option
             option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
           o osxphotos-timewarp_command              option
-            line_option                           o osxphotos-sync_command_line
-    * --limit                                       option
-          o osxphotos-export_command        * --uuid-info
-            line_option                           o osxphotos-exportdb_command
-    * --list                                        line_option
-          o osxphotos-theme_command         * --vacuum
-            line_option                           o osxphotos-exportdb_command
-    * --live                                        line_option
-          o osxphotos-add-locations         * --verbose
-            command_line_option                   o osxphotos-add-locations
+            line_option                     * --uuid-info
+    * --limit                                     o osxphotos-exportdb_command
+          o osxphotos-export_command                line_option
+            line_option                     * --vacuum
+    * --list                                      o osxphotos-exportdb_command
+          o osxphotos-theme_command                 line_option
+            line_option                     * --verbose
+    * --live                                      o osxphotos-add-locations
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-batch-edit
           o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-batch-edit
-          o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-diff_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-exiftool_command
-          o osxphotos-sync_command_line             line_option
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-exiftool_command
+          o osxphotos-repl_command_line             line_option
             option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-exportdb_command
     * --load-config                                 line_option
-          o osxphotos-exiftool_command            o osxphotos-exportdb_command
+          o osxphotos-exiftool_command            o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-export_command              o osxphotos-import_command
+          o osxphotos-export_command              o osxphotos-orphans_command
             line_option                             line_option
-    * --location                                  o osxphotos-orphans_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-batch-edit                    option
+    * --location                                  o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
             command_line_option                   o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
-            line_option                     * --version
-          o osxphotos-import_command              o osxphotos_command_line
+          o osxphotos-batch-edit                    line_option
+            command_line_option             * --version
+          o osxphotos-export_command              o osxphotos_command_line
             line_option                             option
-          o osxphotos-query_command               o osxphotos-exportdb_command
+          o osxphotos-import_command              o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --walk
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --window
-    * --match-time                                o osxphotos-add-locations
-          o osxphotos-timewarp_command              command_line_option
-            line_option                     * --xattr-template
-    * --max-size                                  o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --year
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --merge                                     o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
-            option                          * --yes
-    * --merge-keywords                            o osxphotos-uninstall_command
-          o osxphotos-import_command                line_option
-            line_option                     * -A
-    * --migrate                                   o osxphotos-sync_command_line
-          o osxphotos-exportdb_command              option
-            line_option                     * -a
-    * --migrate-photos-library                    o osxphotos-import_command
-          o osxphotos-exportdb_command              line_option
-            line_option                           o osxphotos-timewarp_command
-    * --min-size                                    line_option
-          o osxphotos-add-locations         * -C
-            command_line_option                   o osxphotos-import_command
-          o osxphotos-export_command                line_option
-            line_option                     * -c
-          o osxphotos-query_command               o osxphotos-timewarp_command
-            line_option                             line_option
-          o osxphotos-repl_command_line     * -D
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-timewarp_command
-    * --missing                                     line_option
-          o osxphotos-add-locations         * -d
-            command_line_option                   o osxphotos-import_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-timewarp_command
-          o osxphotos-query_command                 line_option
-            line_option                     * -e
-          o osxphotos-repl_command_line           o osxphotos-import_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-    * --name                                      o osxphotos-timewarp_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -F
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option
-          o osxphotos-query_command         * -f
-            line_option                           o osxphotos-dump_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-query_command
-    * --no-comment                                  line_option
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-uuid_command_line
-            line_option                             option
-          o osxphotos-query_command         * -g
+          o osxphotos-query_command         * --walk
             line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
-            option                          * -h
-          o osxphotos-sync_command_line           o osxphotos-run_command_line
-            option                                  option
-    * --no-description                      * -i
+            option                          * --window
+          o osxphotos-sync_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+    * --match-time                          * --xattr-template
+          o osxphotos-timewarp_command            o osxphotos-export_command
+            line_option                             line_option
+    * --max-size                            * --year
           o osxphotos-add-locations               o osxphotos-add-locations
             command_line_option                     command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-repl_command_line
             option                                  option
           o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option, [1]
-    * --no-keyword                                o osxphotos-timewarp_command
+            option                                  option
+    * --merge                               * --yes
+          o osxphotos-sync_command_line           o osxphotos-uninstall_command
+            option                                  line_option
+    * --merge-keywords                      * -A
+          o osxphotos-import_command              o osxphotos-sync_command_line
+            line_option                             option
+    * --migrate                             * -a
+          o osxphotos-exportdb_command            o osxphotos-import_command
+            line_option                             line_option
+    * --migrate-photos-library                    o osxphotos-timewarp_command
+          o osxphotos-exportdb_command              line_option
+            line_option                     * -C
+    * --min-size                                  o osxphotos-import_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * -k
-          o osxphotos-export_command              o osxphotos-import_command
+            command_line_option             * -c
+          o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-query_command         * -L
+          o osxphotos-query_command         * -D
             line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
-            option                          * -l
-    * --no-likes                                  o osxphotos-import_command
+            option                          * -d
+    * --missing                                   o osxphotos-import_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * -M
-          o osxphotos-export_command              o osxphotos-timewarp_command
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * -e
+          o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-query_command         * -m
+          o osxphotos-repl_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+    * --name                                * -F
+          o osxphotos-add-locations               o osxphotos-timewarp_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * -f
+            line_option                           o osxphotos-dump_command_line
+          o osxphotos-query_command                 option
             line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
+            option                                o osxphotos-query_command
+          o osxphotos-sync_command_line             line_option
             option                                o osxphotos-timewarp_command
-    * --no-location                                 line_option
-          o osxphotos-add-locations         * -P
-            command_line_option                   o osxphotos-import_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-timewarp_command
+    * --no-comment                                  line_option
+          o osxphotos-add-locations               o osxphotos-uuid_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * -g
+            line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
-            line_option                     * -p
-          o osxphotos-repl_command_line           o osxphotos-import_command
-            option                                  line_option
+            line_option                     * -h
+          o osxphotos-repl_command_line           o osxphotos-run_command_line
+            option                                  option
+          o osxphotos-sync_command_line     * -i
+            option                                o osxphotos-add-locations
+    * --no-description                              command_line_option
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-repl_command_line           o osxphotos-sync_command_line
+            option                                  option, [1]
           o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --no-place                            * -R
+    * --no-keyword                          * -k
           o osxphotos-add-locations               o osxphotos-import_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-query_command         * -r
-            line_option                           o osxphotos-diff_command_line
+          o osxphotos-export_command        * -L
+            line_option                           o osxphotos-import_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line             line_option
+            option                          * -l
+          o osxphotos-sync_command_line           o osxphotos-import_command
+            option                                  line_option
+    * --no-likes                            * -M
+          o osxphotos-add-locations               o osxphotos-timewarp_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * -m
+            line_option                           o osxphotos-import_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
-            option                                o osxphotos-import_command
+            option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
-            option                          * -s
-    * --no-progress                               o osxphotos-diff_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-import_command                option
-            line_option                     * -T
-    * --no-title                                  o osxphotos-inspect_command
+            option                          * -P
+    * --no-location                               o osxphotos-import_command
           o osxphotos-add-locations                 line_option
             command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
-            line_option                     * -t
+            line_option                     * -p
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-inspect_command
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+          o osxphotos-sync_command_line     * -R
+            option                                o osxphotos-import_command
+    * --no-place                                    line_option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * -r
+            line_option                           o osxphotos-diff_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-import_command
+          o osxphotos-repl_command_line             line_option
+            option                          * -s
+          o osxphotos-sync_command_line           o osxphotos-diff_command_line
+            option                                  option
+    * --no-progress                               o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * -T
+          o osxphotos-import_command              o osxphotos-inspect_command
+            line_option                             line_option
+    * --no-title                                  o osxphotos-timewarp_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -t
+          o osxphotos-export_command              o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-inspect_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --not-burst                           * -U
-          o osxphotos-add-locations               o osxphotos-install_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-query_command         * -V
+          o osxphotos-sync_command_line     * -U
+            option                                o osxphotos-install_command
+    * --not-burst                                   line_option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * -V
             line_option                           o osxphotos-add-locations
+          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-batch-edit
           o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-batch-edit
-          o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-diff_command_line
-    * --not-cloudasset                              option
-          o osxphotos-add-locations               o osxphotos-exiftool_command
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-exiftool_command
+    * --not-cloudasset                              line_option
+          o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-export_command              o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-exportdb_command
+          o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-import_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-orphans_command
+          o osxphotos-repl_command_line           o osxphotos-orphans_command
             option                                  line_option
-    * --not-edited                                o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
-            line_option                     * -v
-          o osxphotos-query_command               o osxphotos_command_line
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --not-edited                                o osxphotos-timewarp_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -v
+          o osxphotos-export_command              o osxphotos_command_line
             line_option                             option
-          o osxphotos-repl_command_line     * -w
-            option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
+          o osxphotos-query_command         * -w
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-import_command
-    * --not-favorite                                line_option
-          o osxphotos-add-locations         * -y
-            command_line_option                   o osxphotos-uninstall_command
-          o osxphotos-export_command                line_option
-            line_option                     * -z
-          o osxphotos-query_command               o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * -y
+    * --not-favorite                              o osxphotos-uninstall_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -z
+          o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
+          o osxphotos-query_command
+            line_option
           o osxphotos-repl_command_line
             option
           o osxphotos-sync_command_line
             option
 
 ***** A *****
     * activities_(osxphotos.SearchInfo
       property)
-    * added_after_                         * albums_shared_(osxphotos.PhotosDB
-      (osxphotos.QueryOptions                property)
-      attribute)                           * albums_shared_as_dict_
-    * added_before_                          (osxphotos.PhotosDB_property)
-      (osxphotos.QueryOptions              * AlbumSortOrder_(class_in
-      attribute)                             osxphotos)
-    * added_in_last_                       * all_(osxphotos.SearchInfo
-      (osxphotos.QueryOptions                property)
-      attribute)                           * all_files()_
-    * address_(osxphotos.PlaceInfo           (osxphotos.ExportResults_method)
-      property)                            * ARGS
-    * address_str_(osxphotos.PlaceInfo           o osxphotos-run_command_line
-      property)                                    option
-    * addvalues()_(osxphotos.ExifTool      * asdict()_(osxphotos.AlbumInfo
-      method)                                method)
-    * adjustments_(osxphotos.PhotoInfo           o (osxphotos.ExifTool_method)
-      property)                                  o (osxphotos.FaceInfo_method)
-    * album_(osxphotos.QueryOptions              o (osxphotos.FolderInfo
-      attribute)                                   method)
-    * album_info_(osxphotos.FolderInfo           o (osxphotos.ImportInfo
-      property)                                    method)
-          o (osxphotos.PhotoInfo                 o (osxphotos.MomentInfo
-            property)                              method)
-          o (osxphotos.PhotosDB                  o (osxphotos.PersonInfo
-            property)                              method)
-    * album_info_shared_                         o (osxphotos.PhotoInfo_method)
+    * added_after_
+      (osxphotos.QueryOptions              * albums_shared_(osxphotos.PhotosDB
+      attribute)                             property)
+    * added_before_                        * albums_shared_as_dict_
+      (osxphotos.QueryOptions                (osxphotos.PhotosDB_property)
+      attribute)                           * AlbumSortOrder_(class_in
+    * added_in_last_                         osxphotos)
+      (osxphotos.QueryOptions              * all_(osxphotos.SearchInfo
+      attribute)                             property)
+    * address_(osxphotos.PlaceInfo         * all_files()_
+      property)                              (osxphotos.ExportResults_method)
+    * address_str_(osxphotos.PlaceInfo     * ARGS
+      property)                                  o osxphotos-run_command_line
+    * addvalues()_(osxphotos.ExifTool              option
+      method)                              * asdict()_(osxphotos.AlbumInfo
+    * adjustments_(osxphotos.PhotoInfo       method)
+      property)                                  o (osxphotos.ExifTool_method)
+    * adjustments_path_                          o (osxphotos.FaceInfo_method)
+      (osxphotos.PhotoInfo_property)             o (osxphotos.FolderInfo
+    * album_(osxphotos.QueryOptions                method)
+      attribute)                                 o (osxphotos.ImportInfo
+    * album_info_(osxphotos.FolderInfo             method)
+      property)                                  o (osxphotos.MomentInfo
+          o (osxphotos.PhotoInfo                   method)
+            property)                            o (osxphotos.PersonInfo
+          o (osxphotos.PhotosDB                    method)
+            property)                            o (osxphotos.PhotoInfo_method)
+    * album_info_shared_                         o (osxphotos.PlaceInfo_method)
       (osxphotos.PhotosDB_property)              o (osxphotos.ScoreInfo_method)
     * AlbumInfo_(class_in_osxphotos)             o (osxphotos.SearchInfo
     * albums_(osxphotos.PhotoInfo                  method)
       property)                            * attributes_
           o (osxphotos.PhotosDB              (osxphotos.ExportResults_property)
             property)
     * albums_as_dict_
@@ -1031,42 +1036,45 @@
     * delete_data_for_uuid()_                 attribute)
       (osxphotos.ExportDB_method)           * duplicate_(osxphotos.QueryOptions
                                               attribute)
                                             * duplicates_(osxphotos.PhotoInfo
                                               property)
 
 ***** E *****
-    * edited_(osxphotos.ExportOptions       * export()_(osxphotos.PhotoExporter
-      attribute)                              method)
-          o (osxphotos.QueryOptions               o (osxphotos.PhotoInfo
-            attribute)                              method)
-    * end_date_(osxphotos.MomentInfo        * export_as_hardlink_
-      property)                               (osxphotos.ExportOptions
-    * execute()_(osxphotos.PhotosDB           attribute)
-      method)                               * EXPORT_DATABASE
-    * exif_(osxphotos.QueryOptions                o osxphotos-exportdb_command
-      attribute)                                    line_option
-    * exif_info_(osxphotos.PhotoInfo        * export_db_
-      property)                               (osxphotos.ExportOptions
-    * ExifInfo_(class_in_osxphotos)           attribute)
-    * ExifTool_(class_in_osxphotos)         * export_dir_(osxphotos.ExportDB
-    * exiftool_(osxphotos.ExportOptions       property)
-      attribute)                            * EXPORT_DIRECTORY
-          o (osxphotos.PhotoInfo                  o osxphotos-exiftool_command
-            property)                               line_option
-    * exiftool_flags_                       * ExportDB_(class_in_osxphotos)
-      (osxphotos.ExportOptions              * ExportDBTemp_(class_in_osxphotos)
-      attribute)                            * ExportOptions_(class_in
-    * exiftool_json_sidecar()_                osxphotos)
-      (osxphotos.PhotoExporter_method)      * ExportResults_(class_in
-    * expand_variables()_                     osxphotos)
-      (osxphotos.PhotoTemplate_method)      * external_edit_
-    * expand_variables_to_str()_              (osxphotos.PhotoInfo_property)
-      (osxphotos.PhotoTemplate_method)            o (osxphotos.QueryOptions
-                                                    attribute)
+    * edited_(osxphotos.ExportOptions
+      attribute)
+          o (osxphotos.QueryOptions         * export_aae_
+            attribute)                        (osxphotos.ExportOptions
+    * end_date_(osxphotos.MomentInfo          attribute)
+      property)                             * export_as_hardlink_
+    * execute()_(osxphotos.PhotosDB           (osxphotos.ExportOptions
+      method)                                 attribute)
+    * exif_(osxphotos.QueryOptions          * EXPORT_DATABASE
+      attribute)                                  o osxphotos-exportdb_command
+    * exif_info_(osxphotos.PhotoInfo                line_option
+      property)                             * export_db_
+    * ExifInfo_(class_in_osxphotos)           (osxphotos.ExportOptions
+    * ExifTool_(class_in_osxphotos)           attribute)
+    * exiftool_(osxphotos.ExportOptions     * export_dir_(osxphotos.ExportDB
+      attribute)                              property)
+          o (osxphotos.PhotoInfo            * EXPORT_DIRECTORY
+            property)                             o osxphotos-exiftool_command
+    * exiftool_flags_                               line_option
+      (osxphotos.ExportOptions              * ExportDB_(class_in_osxphotos)
+      attribute)                            * ExportDBTemp_(class_in_osxphotos)
+    * exiftool_json_sidecar()_              * ExportOptions_(class_in
+      (osxphotos.PhotoExporter_method)        osxphotos)
+    * expand_variables()_                   * ExportResults_(class_in
+      (osxphotos.PhotoTemplate_method)        osxphotos)
+    * expand_variables_to_str()_            * external_edit_
+      (osxphotos.PhotoTemplate_method)        (osxphotos.PhotoInfo_property)
+    * export()_(osxphotos.PhotoExporter           o (osxphotos.QueryOptions
+      method)                                       attribute)
+          o (osxphotos.PhotoInfo
+            method)
 
 ***** F *****
     * face_info_(osxphotos.PersonInfo     * fileutil_(osxphotos.ExportOptions
       property)                             attribute)
           o (osxphotos.PhotoInfo          * FileUtilNoOp_(class_in_osxphotos)
             property)                     * filter_predicate()_
     * face_rect()_(osxphotos.FaceInfo       (osxphotos.PhotoTemplate_method)
@@ -1265,229 +1273,230 @@
                                               (osxphotos.QueryOptions
                                               attribute)
                                             * not_time_lapse_
                                               (osxphotos.QueryOptions
                                               attribute)
 
 ***** O *****
-    * orientation_(osxphotos.PhotoInfo      * osxphotos-inspect command line
-      property)                               option
-    * original_filename_                          o --db
-      (osxphotos.PhotoInfo_property)              o --detect-text
-    * original_filesize_                          o --library
-      (osxphotos.PhotoInfo_property)              o --template
-    * original_height_                            o --theme
-      (osxphotos.PhotoInfo_property)              o -t
-    * original_orientation_                       o -T
-      (osxphotos.PhotoInfo_property)        * osxphotos-install command line
-    * original_width_                         option
-      (osxphotos.PhotoInfo_property)              o --upgrade
-    * osxphotos                                   o -U
-          o module                                o PACKAGES
-    * osxphotos command line option         * osxphotos-keywords command line
-          o --version                         option
-          o -v                                    o --db
-    * osxphotos-add-locations command             o --json
-      line option                                 o --library
-          o --added-after                         o PHOTOS_LIBRARY
-          o --added-before                  * osxphotos-labels command line
-          o --added-in-last                   option
-          o --album                               o --db
-          o --burst                               o --json
-          o --cloudasset                          o --library
-          o --description                         o PHOTOS_LIBRARY
-          o --dry-run                       * osxphotos-list command line
-          o --duplicate                       option
-          o --edited                              o --json
-          o --exif                          * osxphotos-orphans command line
-          o --external-edit                   option
-          o --favorite                            o --db
-          o --folder                              o --export
-          o --from-date                           o --library
-          o --from-time                           o --theme
-          o --has-comment                         o --timestamp
-          o --has-likes                           o --verbose
-          o --has-raw                             o -V
-          o --hdr                           * osxphotos-persons command line
-          o --hidden                          option
-          o --ignore-case                         o --db
-          o --in-album                            o --json
-          o --incloud                             o --library
-          o --is-reference                        o PHOTOS_LIBRARY
-          o --keyword                       * osxphotos-places command line
-          o --label                           option
-          o --live                                o --db
-          o --location                            o --json
-          o --max-size                            o --library
-          o --min-size                            o PHOTOS_LIBRARY
-          o --missing                       * osxphotos-query command line
-          o --name                            option
-          o --no-comment                          o --add-to-album
-          o --no-description                      o --added-after
-          o --no-keyword                          o --added-before
-          o --no-likes                            o --added-in-last
-          o --no-location                         o --album
-          o --no-place                            o --burst
-          o --no-title                            o --cloudasset
-          o --not-burst                           o --count
-          o --not-cloudasset                      o --db
-          o --not-edited                          o --deleted
-          o --not-favorite                        o --deleted-only
-          o --not-hdr                             o --description
-          o --not-hidden                          o --duplicate
-          o --not-in-album                        o --edited
-          o --not-incloud                         o --exif
-          o --not-live                            o --external-edit
-          o --not-missing                         o --favorite
-          o --not-panorama                        o --field
-          o --not-portrait                        o --folder
-          o --not-reference                       o --from-date
-          o --not-saved-to-library                o --from-time
-          o --not-screenshot                      o --has-comment
-          o --not-selfie                          o --has-likes
-          o --not-shared                          o --has-raw
-          o --not-slow-mo                         o --hdr
-          o --not-syndicated                      o --hidden
-          o --not-time-lapse                      o --ignore-case
-          o --only-movies                         o --in-album
-          o --only-photos                         o --incloud
-          o --panorama                            o --is-reference
-          o --person                              o --json
-          o --place                               o --keyword
-          o --portrait                            o --label
-          o --query-eval                          o --library
-          o --query-function                      o --live
-          o --regex                               o --location
-          o --saved-to-library                    o --max-size
-          o --screenshot                          o --min-size
-          o --selected                            o --missing
-          o --selfie                              o --name
-          o --shared                              o --no-comment
-          o --slow-mo                             o --no-description
-          o --syndicated                          o --no-keyword
-          o --theme                               o --no-likes
-          o --time-lapse                          o --no-location
-          o --timestamp                           o --no-place
-          o --title                               o --no-title
-          o --to-date                             o --not-burst
-          o --to-time                             o --not-cloudasset
-          o --uti                                 o --not-edited
-          o --uuid                                o --not-favorite
-          o --uuid-from-file                      o --not-hdr
-          o --verbose                             o --not-hidden
-          o --window                              o --not-in-album
-          o --year                                o --not-incloud
-          o -i                                    o --not-live
-          o -V                                    o --not-missing
-          o -w                                    o --not-panorama
-    * osxphotos-albums command line               o --not-portrait
-      option                                      o --not-reference
-          o --db                                  o --not-saved-to-library
-          o --json                                o --not-screenshot
-          o --library                             o --not-selfie
-          o PHOTOS_LIBRARY                        o --not-shared
-    * osxphotos-batch-edit command line           o --not-slow-mo
-      option                                      o --not-syndicated
-          o --db                                  o --not-time-lapse
-          o --description                         o --only-movies
-          o --dry-run                             o --only-photos
-          o --keyword                             o --panorama
-          o --library                             o --person
-          o --location                            o --place
-          o --replace-keywords                    o --portrait
-          o --theme                               o --print
-          o --timestamp                           o --query-eval
-          o --title                               o --query-function
-          o --undo                                o --quiet
-          o --verbose                             o --regex
-          o -V                                    o --saved-to-library
-    * osxphotos-diff command line                 o --screenshot
-      option                                      o --selected
-          o --db                                  o --selfie
-          o --library                             o --shared
-          o --raw-output                          o --slow-mo
-          o --style                               o --syndicated
-          o --timestamp                           o --time-lapse
-          o --verbose                             o --title
-          o -r                                    o --to-date
-          o -s                                    o --to-time
-          o -V                                    o --uti
-          o DB2                                   o --uuid
-    * osxphotos-dump command line                 o --uuid-from-file
-      option                                      o --year
-          o --db                                  o -f
-          o --deleted                             o -i
-          o --deleted-only                        o PHOTOS_LIBRARY
-          o --field                         * osxphotos-repl command line
-          o --json                            option
-          o --library                             o --added-after
-          o --print                               o --added-before
-          o -f                                    o --added-in-last
-          o PHOTOS_LIBRARY                        o --album
-    * osxphotos-exiftool command line             o --burst
-      option                                      o --cloudasset
-          o --album-keyword                       o --db
-          o --append                              o --deleted
-          o --db                                  o --deleted-only
-          o --db-config                           o --description
-          o --description-template                o --duplicate
-          o --dry-run                             o --edited
-          o --exiftool-merge-keywords             o --emacs
-          o --exiftool-merge-persons              o --exif
-          o --exiftool-option                     o --external-edit
-          o --exiftool-path                       o --favorite
-          o --exportdb                            o --folder
-          o --ignore-date-modified                o --from-date
-          o --keyword-template                    o --from-time
-          o --library                             o --has-comment
-          o --load-config                         o --has-likes
-          o --person-keyword                      o --has-raw
-          o --replace-keywords                    o --hdr
-          o --report                              o --hidden
-          o --save-config                         o --ignore-case
-          o --theme                               o --in-album
-          o --timestamp                           o --incloud
-          o --verbose                             o --is-reference
-          o -V                                    o --keyword
-          o EXPORT_DIRECTORY                      o --label
-    * osxphotos-export command line               o --library
-      option                                      o --live
-          o --add-exported-to-album               o --location
-          o --add-missing-to-album                o --max-size
-          o --add-skipped-to-album                o --min-size
-          o --added-after                         o --missing
-          o --added-before                        o --name
-          o --added-in-last                       o --no-comment
-          o --album                               o --no-description
-          o --album-keyword                       o --no-keyword
-          o --alt-copy                            o --no-likes
-          o --append                              o --no-location
-          o --burst                               o --no-place
-          o --cleanup                             o --no-title
-          o --cloudasset                          o --not-burst
-          o --config-only                         o --not-cloudasset
-          o --convert-to-jpeg                     o --not-edited
-          o --current-name                        o --not-favorite
-          o --db                                  o --not-hdr
-          o --deleted                             o --not-hidden
-          o --deleted-only                        o --not-in-album
-          o --description                         o --not-incloud
-          o --description-template                o --not-live
-          o --directory                           o --not-missing
-          o --download-missing                    o --not-panorama
-          o --dry-run                             o --not-portrait
-          o --duplicate                           o --not-reference
-          o --edited                              o --not-saved-to-library
-          o --edited-suffix                       o --not-screenshot
-          o --exif                                o --not-selfie
-          o --exiftool                            o --not-shared
-          o --exiftool-merge-keywords             o --not-slow-mo
-          o --exiftool-merge-persons              o --not-syndicated
-          o --exiftool-option                     o --not-time-lapse
-          o --exiftool-path                       o --only-movies
+    * orientation_(osxphotos.PhotoInfo
+      property)                             * osxphotos-inspect command line
+    * original_filename_                      option
+      (osxphotos.PhotoInfo_property)              o --db
+    * original_filesize_                          o --detect-text
+      (osxphotos.PhotoInfo_property)              o --library
+    * original_height_                            o --template
+      (osxphotos.PhotoInfo_property)              o --theme
+    * original_orientation_                       o -t
+      (osxphotos.PhotoInfo_property)              o -T
+    * original_width_                       * osxphotos-install command line
+      (osxphotos.PhotoInfo_property)          option
+    * osxphotos                                   o --upgrade
+          o module                                o -U
+    * osxphotos command line option               o PACKAGES
+          o --version                       * osxphotos-keywords command line
+          o -v                                option
+    * osxphotos-add-locations command             o --db
+      line option                                 o --json
+          o --added-after                         o --library
+          o --added-before                        o PHOTOS_LIBRARY
+          o --added-in-last                 * osxphotos-labels command line
+          o --album                           option
+          o --burst                               o --db
+          o --cloudasset                          o --json
+          o --description                         o --library
+          o --dry-run                             o PHOTOS_LIBRARY
+          o --duplicate                     * osxphotos-list command line
+          o --edited                          option
+          o --exif                                o --json
+          o --external-edit                 * osxphotos-orphans command line
+          o --favorite                        option
+          o --folder                              o --db
+          o --from-date                           o --export
+          o --from-time                           o --library
+          o --has-comment                         o --theme
+          o --has-likes                           o --timestamp
+          o --has-raw                             o --verbose
+          o --hdr                                 o -V
+          o --hidden                        * osxphotos-persons command line
+          o --ignore-case                     option
+          o --in-album                            o --db
+          o --incloud                             o --json
+          o --is-reference                        o --library
+          o --keyword                             o PHOTOS_LIBRARY
+          o --label                         * osxphotos-places command line
+          o --live                            option
+          o --location                            o --db
+          o --max-size                            o --json
+          o --min-size                            o --library
+          o --missing                             o PHOTOS_LIBRARY
+          o --name                          * osxphotos-query command line
+          o --no-comment                      option
+          o --no-description                      o --add-to-album
+          o --no-keyword                          o --added-after
+          o --no-likes                            o --added-before
+          o --no-location                         o --added-in-last
+          o --no-place                            o --album
+          o --no-title                            o --burst
+          o --not-burst                           o --cloudasset
+          o --not-cloudasset                      o --count
+          o --not-edited                          o --db
+          o --not-favorite                        o --deleted
+          o --not-hdr                             o --deleted-only
+          o --not-hidden                          o --description
+          o --not-in-album                        o --duplicate
+          o --not-incloud                         o --edited
+          o --not-live                            o --exif
+          o --not-missing                         o --external-edit
+          o --not-panorama                        o --favorite
+          o --not-portrait                        o --field
+          o --not-reference                       o --folder
+          o --not-saved-to-library                o --from-date
+          o --not-screenshot                      o --from-time
+          o --not-selfie                          o --has-comment
+          o --not-shared                          o --has-likes
+          o --not-slow-mo                         o --has-raw
+          o --not-syndicated                      o --hdr
+          o --not-time-lapse                      o --hidden
+          o --only-movies                         o --ignore-case
+          o --only-photos                         o --in-album
+          o --panorama                            o --incloud
+          o --person                              o --is-reference
+          o --place                               o --json
+          o --portrait                            o --keyword
+          o --query-eval                          o --label
+          o --query-function                      o --library
+          o --regex                               o --live
+          o --saved-to-library                    o --location
+          o --screenshot                          o --max-size
+          o --selected                            o --min-size
+          o --selfie                              o --missing
+          o --shared                              o --name
+          o --slow-mo                             o --no-comment
+          o --syndicated                          o --no-description
+          o --theme                               o --no-keyword
+          o --time-lapse                          o --no-likes
+          o --timestamp                           o --no-location
+          o --title                               o --no-place
+          o --to-date                             o --no-title
+          o --to-time                             o --not-burst
+          o --uti                                 o --not-cloudasset
+          o --uuid                                o --not-edited
+          o --uuid-from-file                      o --not-favorite
+          o --verbose                             o --not-hdr
+          o --window                              o --not-hidden
+          o --year                                o --not-in-album
+          o -i                                    o --not-incloud
+          o -V                                    o --not-live
+          o -w                                    o --not-missing
+    * osxphotos-albums command line               o --not-panorama
+      option                                      o --not-portrait
+          o --db                                  o --not-reference
+          o --json                                o --not-saved-to-library
+          o --library                             o --not-screenshot
+          o PHOTOS_LIBRARY                        o --not-selfie
+    * osxphotos-batch-edit command line           o --not-shared
+      option                                      o --not-slow-mo
+          o --db                                  o --not-syndicated
+          o --description                         o --not-time-lapse
+          o --dry-run                             o --only-movies
+          o --keyword                             o --only-photos
+          o --library                             o --panorama
+          o --location                            o --person
+          o --replace-keywords                    o --place
+          o --theme                               o --portrait
+          o --timestamp                           o --print
+          o --title                               o --query-eval
+          o --undo                                o --query-function
+          o --verbose                             o --quiet
+          o -V                                    o --regex
+    * osxphotos-diff command line                 o --saved-to-library
+      option                                      o --screenshot
+          o --db                                  o --selected
+          o --library                             o --selfie
+          o --raw-output                          o --shared
+          o --style                               o --slow-mo
+          o --timestamp                           o --syndicated
+          o --verbose                             o --time-lapse
+          o -r                                    o --title
+          o -s                                    o --to-date
+          o -V                                    o --to-time
+          o DB2                                   o --uti
+    * osxphotos-dump command line                 o --uuid
+      option                                      o --uuid-from-file
+          o --db                                  o --year
+          o --deleted                             o -f
+          o --deleted-only                        o -i
+          o --field                               o PHOTOS_LIBRARY
+          o --json                          * osxphotos-repl command line
+          o --library                         option
+          o --print                               o --added-after
+          o -f                                    o --added-before
+          o PHOTOS_LIBRARY                        o --added-in-last
+    * osxphotos-exiftool command line             o --album
+      option                                      o --burst
+          o --album-keyword                       o --cloudasset
+          o --append                              o --db
+          o --db                                  o --deleted
+          o --db-config                           o --deleted-only
+          o --description-template                o --description
+          o --dry-run                             o --duplicate
+          o --exiftool-merge-keywords             o --edited
+          o --exiftool-merge-persons              o --emacs
+          o --exiftool-option                     o --exif
+          o --exiftool-path                       o --external-edit
+          o --exportdb                            o --favorite
+          o --ignore-date-modified                o --folder
+          o --keyword-template                    o --from-date
+          o --library                             o --from-time
+          o --load-config                         o --has-comment
+          o --person-keyword                      o --has-likes
+          o --replace-keywords                    o --has-raw
+          o --report                              o --hdr
+          o --save-config                         o --hidden
+          o --theme                               o --ignore-case
+          o --timestamp                           o --in-album
+          o --verbose                             o --incloud
+          o -V                                    o --is-reference
+          o EXPORT_DIRECTORY                      o --keyword
+    * osxphotos-export command line               o --label
+      option                                      o --library
+          o --add-exported-to-album               o --live
+          o --add-missing-to-album                o --location
+          o --add-skipped-to-album                o --max-size
+          o --added-after                         o --min-size
+          o --added-before                        o --missing
+          o --added-in-last                       o --name
+          o --album                               o --no-comment
+          o --album-keyword                       o --no-description
+          o --alt-copy                            o --no-keyword
+          o --append                              o --no-likes
+          o --burst                               o --no-location
+          o --cleanup                             o --no-place
+          o --cloudasset                          o --no-title
+          o --config-only                         o --not-burst
+          o --convert-to-jpeg                     o --not-cloudasset
+          o --current-name                        o --not-edited
+          o --db                                  o --not-favorite
+          o --deleted                             o --not-hdr
+          o --deleted-only                        o --not-hidden
+          o --description                         o --not-in-album
+          o --description-template                o --not-incloud
+          o --directory                           o --not-live
+          o --download-missing                    o --not-missing
+          o --dry-run                             o --not-panorama
+          o --duplicate                           o --not-portrait
+          o --edited                              o --not-reference
+          o --edited-suffix                       o --not-saved-to-library
+          o --exif                                o --not-screenshot
+          o --exiftool                            o --not-selfie
+          o --exiftool-merge-keywords             o --not-shared
+          o --exiftool-merge-persons              o --not-slow-mo
+          o --exiftool-option                     o --not-syndicated
+          o --exiftool-path                       o --not-time-lapse
+          o --export-aae                          o --only-movies
           o --export-as-hardlink                  o --only-photos
           o --export-by-date                      o --panorama
           o --exportdb                            o --person
           o --external-edit                       o --place
           o --favorite                            o --portrait
           o --favorite-rating                     o --query-eval
           o --filename                            o --query-function
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.6 documentation</title>
+        <title>osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -357,14 +357,15 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.persons"><code class="docutils literal notranslate"><span class="pre">ExportOptions.persons</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.preview_suffix"><code class="docutils literal notranslate"><span class="pre">ExportOptions.preview_suffix</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.preview"><code class="docutils literal notranslate"><span class="pre">ExportOptions.preview</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.raw_photo"><code class="docutils literal notranslate"><span class="pre">ExportOptions.raw_photo</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.render_options"><code class="docutils literal notranslate"><span class="pre">ExportOptions.render_options</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.replace_keywords"><code class="docutils literal notranslate"><span class="pre">ExportOptions.replace_keywords</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.rich"><code class="docutils literal notranslate"><span class="pre">ExportOptions.rich</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.export_aae"><code class="docutils literal notranslate"><span class="pre">ExportOptions.export_aae</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.sidecar_drop_ext"><code class="docutils literal notranslate"><span class="pre">ExportOptions.sidecar_drop_ext</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.sidecar"><code class="docutils literal notranslate"><span class="pre">ExportOptions.sidecar</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.strip"><code class="docutils literal notranslate"><span class="pre">ExportOptions.strip</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.timeout"><code class="docutils literal notranslate"><span class="pre">ExportOptions.timeout</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.touch_file"><code class="docutils literal notranslate"><span class="pre">ExportOptions.touch_file</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.update"><code class="docutils literal notranslate"><span class="pre">ExportOptions.update</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ExportOptions.update_errors"><code class="docutils literal notranslate"><span class="pre">ExportOptions.update_errors</span></code></a></li>
@@ -456,14 +457,15 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoExporter.exiftool_json_sidecar"><code class="docutils literal notranslate"><span class="pre">PhotoExporter.exiftool_json_sidecar()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoExporter.export"><code class="docutils literal notranslate"><span class="pre">PhotoExporter.export()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoExporter.write_exiftool_metadata_to_file"><code class="docutils literal notranslate"><span class="pre">PhotoExporter.write_exiftool_metadata_to_file()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.adjustments"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.adjustments</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.adjustments_path"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.adjustments_path</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.album_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.album_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.albums"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.albums</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.asdict"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.asdict()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.burst"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.burst_album_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst_album_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.burst_albums"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst_albums</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.burst_default_pick"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst_default_pick</span></code></a></li>
@@ -607,14 +609,15 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.project_info"><code class="docutils literal notranslate"><span class="pre">PhotosDB.project_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.query"><code class="docutils literal notranslate"><span class="pre">PhotosDB.query()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.address"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.address_str"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address_str</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.asdict"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.asdict()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.country_code"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.country_code</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.ishome"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.ishome</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.name"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.name</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo.names"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.names</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a><ul>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -177,14 +177,15 @@
                 # ExportOptions.persons
                 # ExportOptions.preview_suffix
                 # ExportOptions.preview
                 # ExportOptions.raw_photo
                 # ExportOptions.render_options
                 # ExportOptions.replace_keywords
                 # ExportOptions.rich
+                # ExportOptions.export_aae
                 # ExportOptions.sidecar_drop_ext
                 # ExportOptions.sidecar
                 # ExportOptions.strip
                 # ExportOptions.timeout
                 # ExportOptions.touch_file
                 # ExportOptions.update
                 # ExportOptions.update_errors
@@ -258,14 +259,15 @@
                 # PersonInfo.sort_order
           o PhotoExporter
                 # PhotoExporter.exiftool_json_sidecar()
                 # PhotoExporter.export()
                 # PhotoExporter.write_exiftool_metadata_to_file()
           o PhotoInfo
                 # PhotoInfo.adjustments
+                # PhotoInfo.adjustments_path
                 # PhotoInfo.album_info
                 # PhotoInfo.albums
                 # PhotoInfo.asdict()
                 # PhotoInfo.burst
                 # PhotoInfo.burst_album_info
                 # PhotoInfo.burst_albums
                 # PhotoInfo.burst_default_pick
@@ -403,14 +405,15 @@
                 # PhotosDB.photos_by_uuid()
                 # PhotosDB.photos_version
                 # PhotosDB.project_info
                 # PhotosDB.query()
           o PlaceInfo
                 # PlaceInfo.address
                 # PlaceInfo.address_str
+                # PlaceInfo.asdict()
                 # PlaceInfo.country_code
                 # PlaceInfo.ishome
                 # PlaceInfo.name
                 # PlaceInfo.names
           o ProjectInfo
                 # ProjectInfo.folder_list
                 # ProjectInfo.folder_names
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -1,1240 +1,47 @@
 # Sphinx inventory version 2
 # Project: osxphotos
 # Version: 
 # The remainder of this file is compressed using zlib.
+#Ev|5WWxmLHudkL<ja*2ܾ	իHmp4q}%ߵQ
 
-osxphotos py:module 0 reference.html#module-$ -
-osxphotos.AlbumInfo py:class 1 reference.html#$ -
-osxphotos.AlbumInfo.asdict py:method 1 reference.html#$ -
-osxphotos.AlbumInfo.folder_list py:property 1 reference.html#$ -
-osxphotos.AlbumInfo.folder_names py:property 1 reference.html#$ -
-osxphotos.AlbumInfo.parent py:property 1 reference.html#$ -
-osxphotos.AlbumInfo.photo_index py:method 1 reference.html#$ -
-osxphotos.AlbumInfo.photos py:property 1 reference.html#$ -
-osxphotos.AlbumInfo.sort_order py:property 1 reference.html#$ -
-osxphotos.AlbumInfo.title py:property 1 reference.html#$ -
-osxphotos.AlbumSortOrder py:class 1 reference.html#$ -
-osxphotos.CommentInfo py:class 1 reference.html#$ -
-osxphotos.ExifInfo py:class 1 reference.html#$ -
-osxphotos.ExifTool py:class 1 reference.html#$ -
-osxphotos.ExifTool.addvalues py:method 1 reference.html#$ -
-osxphotos.ExifTool.asdict py:method 1 reference.html#$ -
-osxphotos.ExifTool.json py:method 1 reference.html#$ -
-osxphotos.ExifTool.pid py:property 1 reference.html#$ -
-osxphotos.ExifTool.run_commands py:method 1 reference.html#$ -
-osxphotos.ExifTool.setvalue py:method 1 reference.html#$ -
-osxphotos.ExifTool.version py:property 1 reference.html#$ -
-osxphotos.ExportDB py:class 1 reference.html#$ -
-osxphotos.ExportDB.close py:method 1 reference.html#$ -
-osxphotos.ExportDB.connection py:property 1 reference.html#$ -
-osxphotos.ExportDB.create_file_record py:method 1 reference.html#$ -
-osxphotos.ExportDB.create_or_get_file_record py:method 1 reference.html#$ -
-osxphotos.ExportDB.delete_data_for_filepath py:method 1 reference.html#$ -
-osxphotos.ExportDB.delete_data_for_uuid py:method 1 reference.html#$ -
-osxphotos.ExportDB.export_dir py:property 1 reference.html#$ -
-osxphotos.ExportDB.get_export_results py:method 1 reference.html#$ -
-osxphotos.ExportDB.get_exported_files py:method 1 reference.html#$ -
-osxphotos.ExportDB.get_file_record py:method 1 reference.html#$ -
-osxphotos.ExportDB.get_files_for_uuid py:method 1 reference.html#$ -
-osxphotos.ExportDB.get_photoinfo_for_uuid py:method 1 reference.html#$ -
-osxphotos.ExportDB.get_previous_uuids py:method 1 reference.html#$ -
-osxphotos.ExportDB.get_target_for_file py:method 1 reference.html#$ -
-osxphotos.ExportDB.get_uuid_for_file py:method 1 reference.html#$ -
-osxphotos.ExportDB.path py:property 1 reference.html#$ -
-osxphotos.ExportDB.set_config py:method 1 reference.html#$ -
-osxphotos.ExportDB.set_export_results py:method 1 reference.html#$ -
-osxphotos.ExportDB.set_photoinfo_for_uuid py:method 1 reference.html#$ -
-osxphotos.ExportDBTemp py:class 1 reference.html#$ -
-osxphotos.ExportOptions py:class 1 reference.html#$ -
-osxphotos.ExportOptions.bit_flags py:property 1 reference.html#$ -
-osxphotos.ExportOptions.convert_to_jpeg py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.description_template py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.download_missing py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.dry_run py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.edited py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.exiftool py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.exiftool_flags py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.export_as_hardlink py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.export_db py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.face_regions py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.favorite_rating py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.fileutil py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.force_update py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.ignore_date_modified py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.ignore_signature py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.increment py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.jpeg_ext py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.jpeg_quality py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.keyword_template py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.live_photo py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.location py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.merge_exif_keywords py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.merge_exif_persons py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.overwrite py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.persons py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.preview py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.preview_suffix py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.raw_photo py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.render_options py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.replace_keywords py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.rich py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.sidecar py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.sidecar_drop_ext py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.strip py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.timeout py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.tmpdir py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.touch_file py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.update py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.update_errors py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.use_albums_as_keywords py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.use_persons_as_keywords py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.use_photokit py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.use_photos_export py:attribute 1 reference.html#$ -
-osxphotos.ExportOptions.verbose py:attribute 1 reference.html#$ -
-osxphotos.ExportResults py:class 1 reference.html#$ -
-osxphotos.ExportResults.all_files py:method 1 reference.html#$ -
-osxphotos.ExportResults.attributes py:property 1 reference.html#$ -
-osxphotos.ExportResults.datetime py:property 1 reference.html#$ -
-osxphotos.FaceInfo py:class 1 reference.html#$ -
-osxphotos.FaceInfo.asdict py:method 1 reference.html#$ -
-osxphotos.FaceInfo.center py:property 1 reference.html#$ -
-osxphotos.FaceInfo.face_rect py:method 1 reference.html#$ -
-osxphotos.FaceInfo.json py:method 1 reference.html#$ -
-osxphotos.FaceInfo.mpri_reg_rect py:property 1 reference.html#$ -
-osxphotos.FaceInfo.mwg_rs_area py:property 1 reference.html#$ -
-osxphotos.FaceInfo.person_info py:property 1 reference.html#$ -
-osxphotos.FaceInfo.photo py:property 1 reference.html#$ -
-osxphotos.FaceInfo.pitch py:property 1 reference.html#$ -
-osxphotos.FaceInfo.roll py:property 1 reference.html#$ -
-osxphotos.FaceInfo.roll_pitch_yaw py:method 1 reference.html#$ -
-osxphotos.FaceInfo.size_pixels py:property 1 reference.html#$ -
-osxphotos.FaceInfo.yaw py:property 1 reference.html#$ -
-osxphotos.FileUtil py:class 1 reference.html#$ -
-osxphotos.FileUtilNoOp py:class 1 reference.html#$ -
-osxphotos.FileUtilNoOp.convert_to_jpeg py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.copy py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.file_sig py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.hardlink py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.rename py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.rmdir py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.tmpdir py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.unlink py:method 1 reference.html#$ -
-osxphotos.FileUtilNoOp.utime py:method 1 reference.html#$ -
-osxphotos.FolderInfo py:class 1 reference.html#$ -
-osxphotos.FolderInfo.album_info py:property 1 reference.html#$ -
-osxphotos.FolderInfo.asdict py:method 1 reference.html#$ -
-osxphotos.FolderInfo.parent py:property 1 reference.html#$ -
-osxphotos.FolderInfo.subfolders py:property 1 reference.html#$ -
-osxphotos.FolderInfo.title py:property 1 reference.html#$ -
-osxphotos.FolderInfo.uuid py:property 1 reference.html#$ -
-osxphotos.ImportInfo py:class 1 reference.html#$ -
-osxphotos.ImportInfo.asdict py:method 1 reference.html#$ -
-osxphotos.ImportInfo.photos py:property 1 reference.html#$ -
-osxphotos.ImportInfo.title py:property 1 reference.html#$ -
-osxphotos.LikeInfo py:class 1 reference.html#$ -
-osxphotos.MomentInfo py:class 1 reference.html#$ -
-osxphotos.MomentInfo.asdict py:method 1 reference.html#$ -
-osxphotos.MomentInfo.date py:property 1 reference.html#$ -
-osxphotos.MomentInfo.end_date py:property 1 reference.html#$ -
-osxphotos.MomentInfo.location py:property 1 reference.html#$ -
-osxphotos.MomentInfo.modification_date py:property 1 reference.html#$ -
-osxphotos.MomentInfo.photos py:property 1 reference.html#$ -
-osxphotos.MomentInfo.pk py:property 1 reference.html#$ -
-osxphotos.MomentInfo.start_date py:property 1 reference.html#$ -
-osxphotos.MomentInfo.subtitle py:property 1 reference.html#$ -
-osxphotos.MomentInfo.title py:property 1 reference.html#$ -
-osxphotos.PersonInfo py:class 1 reference.html#$ -
-osxphotos.PersonInfo.asdict py:method 1 reference.html#$ -
-osxphotos.PersonInfo.face_info py:property 1 reference.html#$ -
-osxphotos.PersonInfo.favorite py:property 1 reference.html#$ -
-osxphotos.PersonInfo.feature_less py:property 1 reference.html#$ -
-osxphotos.PersonInfo.json py:method 1 reference.html#$ -
-osxphotos.PersonInfo.photos py:property 1 reference.html#$ -
-osxphotos.PersonInfo.sort_order py:property 1 reference.html#$ -
-osxphotos.PhotoExporter py:class 1 reference.html#$ -
-osxphotos.PhotoExporter.exiftool_json_sidecar py:method 1 reference.html#$ -
-osxphotos.PhotoExporter.export py:method 1 reference.html#$ -
-osxphotos.PhotoExporter.write_exiftool_metadata_to_file py:method 1 reference.html#$ -
-osxphotos.PhotoInfo py:class 1 reference.html#$ -
-osxphotos.PhotoInfo.adjustments py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.album_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.albums py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.asdict py:method 1 reference.html#$ -
-osxphotos.PhotoInfo.burst py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.burst_album_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.burst_albums py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.burst_default_pick py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.burst_key py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.burst_photos py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.burst_selected py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.cloud_guid py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.cloud_metadata py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.cloud_owner_hashed_id py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.comments py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.date py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.date_added py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.date_modified py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.date_trashed py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.description py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.detected_text py:method 1 reference.html#$ -
-osxphotos.PhotoInfo.duplicates py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.exif_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.exiftool py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.export py:method 1 reference.html#$ -
-osxphotos.PhotoInfo.external_edit py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.face_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.favorite py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.filename py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.fingerprint py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.has_raw py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.hasadjustments py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.hdr py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.height py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.hexdigest py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.hidden py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.import_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.incloud py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.intrash py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.iscloudasset py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.ismissing py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.ismovie py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.isphoto py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.israw py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.isreference py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.json py:method 1 reference.html#$ -
-osxphotos.PhotoInfo.keywords py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.labels py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.labels_normalized py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.likes py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.live_photo py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.location py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.moment_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.orientation py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.original_filename py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.original_filesize py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.original_height py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.original_orientation py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.original_width py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.owner py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.panorama py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.path py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.path_derivatives py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.path_edited py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.path_edited_live_photo py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.path_live_photo py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.path_raw py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.person_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.persons py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.place py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.portrait py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.project_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.raw_original py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.render_template py:method 1 reference.html#$ -
-osxphotos.PhotoInfo.saved_to_library py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.score py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.screenshot py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.search_info py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.search_info_normalized py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.selfie py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.shared py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.slow_mo py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.syndicated py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.tables py:method 1 reference.html#$ -
-osxphotos.PhotoInfo.time_lapse py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.title py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.tzoffset py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.uti py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.uti_edited py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.uti_original py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.uti_raw py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.uuid py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.visible py:property 1 reference.html#$ -
-osxphotos.PhotoInfo.width py:property 1 reference.html#$ -
-osxphotos.PhotoTemplate py:class 1 reference.html#$ -
-osxphotos.PhotoTemplate.expand_variables py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.expand_variables_to_str py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.filter_predicate py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_field_values py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_filter_values py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_format_values py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_media_type py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_photo_bool_attribute py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_photo_video_type py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_template_value py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_template_value_exiftool py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_template_value_filter_function py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_template_value_function py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_template_value_multi py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.get_template_value_pathlib py:method 1 reference.html#$ -
-osxphotos.PhotoTemplate.render py:method 1 reference.html#$ -
-osxphotos.PhotosAlbum py:class 1 reference.html#$ -
-osxphotos.PhotosAlbumPhotoScript py:class 1 reference.html#$ -
-osxphotos.PhotosDB py:class 1 reference.html#$ -
-osxphotos.PhotosDB.album_info py:property 1 reference.html#$ -
-osxphotos.PhotosDB.album_info_shared py:property 1 reference.html#$ -
-osxphotos.PhotosDB.albums py:property 1 reference.html#$ -
-osxphotos.PhotosDB.albums_as_dict py:property 1 reference.html#$ -
-osxphotos.PhotosDB.albums_shared py:property 1 reference.html#$ -
-osxphotos.PhotosDB.albums_shared_as_dict py:property 1 reference.html#$ -
-osxphotos.PhotosDB.db_path py:property 1 reference.html#$ -
-osxphotos.PhotosDB.db_version py:property 1 reference.html#$ -
-osxphotos.PhotosDB.execute py:method 1 reference.html#$ -
-osxphotos.PhotosDB.folder_info py:property 1 reference.html#$ -
-osxphotos.PhotosDB.folders py:property 1 reference.html#$ -
-osxphotos.PhotosDB.get_db_connection py:method 1 reference.html#$ -
-osxphotos.PhotosDB.get_photo py:method 1 reference.html#$ -
-osxphotos.PhotosDB.import_info py:property 1 reference.html#$ -
-osxphotos.PhotosDB.keywords py:property 1 reference.html#$ -
-osxphotos.PhotosDB.keywords_as_dict py:property 1 reference.html#$ -
-osxphotos.PhotosDB.labels py:property 1 reference.html#$ -
-osxphotos.PhotosDB.labels_as_dict py:property 1 reference.html#$ -
-osxphotos.PhotosDB.labels_normalized py:property 1 reference.html#$ -
-osxphotos.PhotosDB.labels_normalized_as_dict py:property 1 reference.html#$ -
-osxphotos.PhotosDB.library_path py:property 1 reference.html#$ -
-osxphotos.PhotosDB.person_info py:property 1 reference.html#$ -
-osxphotos.PhotosDB.persons py:property 1 reference.html#$ -
-osxphotos.PhotosDB.persons_as_dict py:property 1 reference.html#$ -
-osxphotos.PhotosDB.photos py:method 1 reference.html#$ -
-osxphotos.PhotosDB.photos_by_uuid py:method 1 reference.html#$ -
-osxphotos.PhotosDB.photos_version py:property 1 reference.html#$ -
-osxphotos.PhotosDB.project_info py:property 1 reference.html#$ -
-osxphotos.PhotosDB.query py:method 1 reference.html#$ -
-osxphotos.PlaceInfo py:class 1 reference.html#$ -
-osxphotos.PlaceInfo.address py:property 1 reference.html#$ -
-osxphotos.PlaceInfo.address_str py:property 1 reference.html#$ -
-osxphotos.PlaceInfo.country_code py:property 1 reference.html#$ -
-osxphotos.PlaceInfo.ishome py:property 1 reference.html#$ -
-osxphotos.PlaceInfo.name py:property 1 reference.html#$ -
-osxphotos.PlaceInfo.names py:property 1 reference.html#$ -
-osxphotos.ProjectInfo py:class 1 reference.html#$ -
-osxphotos.ProjectInfo.folder_list py:property 1 reference.html#$ -
-osxphotos.ProjectInfo.folder_names py:property 1 reference.html#$ -
-osxphotos.QueryOptions py:class 1 reference.html#$ -
-osxphotos.QueryOptions.added_after py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.added_before py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.added_in_last py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.album py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.burst py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.burst_photos py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.cloudasset py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.deleted py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.deleted_only py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.description py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.duplicate py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.edited py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.exif py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.external_edit py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.favorite py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.folder py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.from_date py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.function py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.has_comment py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.has_likes py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.has_raw py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.hdr py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.hidden py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.ignore_case py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.in_album py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.incloud py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.is_reference py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.keyword py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.label py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.live py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.location py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.max_size py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.min_size py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.missing py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.missing_bursts py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.movies py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.name py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.no_comment py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.no_description py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.no_keyword py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.no_likes py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.no_location py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.no_place py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.no_title py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_burst py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_cloudasset py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_edited py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_favorite py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_hdr py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_hidden py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_in_album py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_incloud py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_live py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_missing py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_panorama py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_portrait py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_reference py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_saved_to_library py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_screenshot py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_selfie py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_shared py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_slow_mo py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_syndicated py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.not_time_lapse py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.panorama py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.person py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.photos py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.place py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.portrait py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.query_eval py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.regex py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.saved_to_library py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.screenshot py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.selected py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.selfie py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.shared py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.slow_mo py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.syndicated py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.time_lapse py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.title py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.to_date py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.uti py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.uuid py:attribute 1 reference.html#$ -
-osxphotos.QueryOptions.year py:attribute 1 reference.html#$ -
-osxphotos.ScoreInfo py:class 1 reference.html#$ -
-osxphotos.ScoreInfo.asdict py:method 1 reference.html#$ -
-osxphotos.SearchInfo py:class 1 reference.html#$ -
-osxphotos.SearchInfo.activities py:property 1 reference.html#$ -
-osxphotos.SearchInfo.all py:property 1 reference.html#$ -
-osxphotos.SearchInfo.asdict py:method 1 reference.html#$ -
-osxphotos.SearchInfo.bodies_of_water py:property 1 reference.html#$ -
-osxphotos.SearchInfo.camera py:property 1 reference.html#$ -
-osxphotos.SearchInfo.city py:property 1 reference.html#$ -
-osxphotos.SearchInfo.country py:property 1 reference.html#$ -
-osxphotos.SearchInfo.detected_text py:property 1 reference.html#$ -
-osxphotos.SearchInfo.holidays py:property 1 reference.html#$ -
-osxphotos.SearchInfo.labels py:property 1 reference.html#$ -
-osxphotos.SearchInfo.locality_names py:property 1 reference.html#$ -
-osxphotos.SearchInfo.media_types py:property 1 reference.html#$ -
-osxphotos.SearchInfo.month py:property 1 reference.html#$ -
-osxphotos.SearchInfo.neighborhoods py:property 1 reference.html#$ -
-osxphotos.SearchInfo.place_names py:property 1 reference.html#$ -
-osxphotos.SearchInfo.season py:property 1 reference.html#$ -
-osxphotos.SearchInfo.source py:property 1 reference.html#$ -
-osxphotos.SearchInfo.state py:property 1 reference.html#$ -
-osxphotos.SearchInfo.state_abbreviation py:property 1 reference.html#$ -
-osxphotos.SearchInfo.streets py:property 1 reference.html#$ -
-osxphotos.SearchInfo.text_found py:property 1 reference.html#$ -
-osxphotos.SearchInfo.venue_types py:property 1 reference.html#$ -
-osxphotos.SearchInfo.venues py:property 1 reference.html#$ -
-osxphotos.SearchInfo.year py:property 1 reference.html#$ -
-osxphotos._constants.AlbumSortOrder py:class -1 reference.html#osxphotos.AlbumSortOrder -
-osxphotos.albuminfo.AlbumInfo py:class -1 reference.html#osxphotos.AlbumInfo -
-osxphotos.albuminfo.FolderInfo py:class -1 reference.html#osxphotos.FolderInfo -
-osxphotos.albuminfo.ImportInfo py:class -1 reference.html#osxphotos.ImportInfo -
-osxphotos.albuminfo.ProjectInfo py:class -1 reference.html#osxphotos.ProjectInfo -
-osxphotos.exifinfo.ExifInfo py:class -1 reference.html#osxphotos.ExifInfo -
-osxphotos.exiftool.ExifTool py:class -1 reference.html#osxphotos.ExifTool -
-osxphotos.export_db.ExportDB py:class -1 reference.html#osxphotos.ExportDB -
-osxphotos.export_db.ExportDBTemp py:class -1 reference.html#osxphotos.ExportDBTemp -
-osxphotos.fileutil.FileUtil py:class -1 reference.html#osxphotos.FileUtil -
-osxphotos.fileutil.FileUtilNoOp py:class -1 reference.html#osxphotos.FileUtilNoOp -
-osxphotos.is_debug py:function 1 reference.html#$ -
-osxphotos.momentinfo.MomentInfo py:class -1 reference.html#osxphotos.MomentInfo -
-osxphotos.personinfo.FaceInfo py:class -1 reference.html#osxphotos.FaceInfo -
-osxphotos.personinfo.PersonInfo py:class -1 reference.html#osxphotos.PersonInfo -
-osxphotos.photoexporter.ExportOptions py:class -1 reference.html#osxphotos.ExportOptions -
-osxphotos.photoexporter.ExportResults py:class -1 reference.html#osxphotos.ExportResults -
-osxphotos.photoexporter.PhotoExporter py:class -1 reference.html#osxphotos.PhotoExporter -
-osxphotos.photoinfo.PhotoInfo py:class -1 reference.html#osxphotos.PhotoInfo -
-osxphotos.photosalbum.PhotosAlbum py:class -1 reference.html#osxphotos.PhotosAlbum -
-osxphotos.photosalbum.PhotosAlbumPhotoScript py:class -1 reference.html#osxphotos.PhotosAlbumPhotoScript -
-osxphotos.photosdb._photosdb_process_comments.CommentInfo py:class -1 reference.html#osxphotos.CommentInfo -
-osxphotos.photosdb._photosdb_process_comments.LikeInfo py:class -1 reference.html#osxphotos.LikeInfo -
-osxphotos.photosdb.photosdb.PhotosDB py:class -1 reference.html#osxphotos.PhotosDB -
-osxphotos.phototemplate.PhotoTemplate py:class -1 reference.html#osxphotos.PhotoTemplate -
-osxphotos.placeinfo.PlaceInfo py:class -1 reference.html#osxphotos.PlaceInfo -
-osxphotos.queryoptions.QueryOptions py:class -1 reference.html#osxphotos.QueryOptions -
-osxphotos.scoreinfo.ScoreInfo py:class -1 reference.html#osxphotos.ScoreInfo -
-osxphotos.searchinfo.SearchInfo py:class -1 reference.html#osxphotos.SearchInfo -
-osxphotos.set_debug py:function 1 reference.html#$ -
-cli std:doc -1 cli.html OSXPhotos Command Line Interface (CLI)
-genindex std:label -1 genindex.html Index
-index std:doc -1 index.html Welcome to OSXPhotos’s documentation!
-modindex std:label -1 py-modindex.html Module Index
-osxphotos-add-locations.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-added-after -
-osxphotos-add-locations.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-added-before -
-osxphotos-add-locations.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-added-in-last -
-osxphotos-add-locations.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-album -
-osxphotos-add-locations.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-burst -
-osxphotos-add-locations.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-cloudasset -
-osxphotos-add-locations.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-description -
-osxphotos-add-locations.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-dry-run -
-osxphotos-add-locations.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-duplicate -
-osxphotos-add-locations.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-edited -
-osxphotos-add-locations.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-exif -
-osxphotos-add-locations.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-external-edit -
-osxphotos-add-locations.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-favorite -
-osxphotos-add-locations.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-folder -
-osxphotos-add-locations.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-from-date -
-osxphotos-add-locations.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-from-time -
-osxphotos-add-locations.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-has-comment -
-osxphotos-add-locations.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-has-likes -
-osxphotos-add-locations.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-has-raw -
-osxphotos-add-locations.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-hdr -
-osxphotos-add-locations.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-hidden -
-osxphotos-add-locations.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-i -
-osxphotos-add-locations.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-in-album -
-osxphotos-add-locations.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-incloud -
-osxphotos-add-locations.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-is-reference -
-osxphotos-add-locations.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-keyword -
-osxphotos-add-locations.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-label -
-osxphotos-add-locations.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-live -
-osxphotos-add-locations.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-location -
-osxphotos-add-locations.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-max-size -
-osxphotos-add-locations.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-min-size -
-osxphotos-add-locations.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-missing -
-osxphotos-add-locations.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-name -
-osxphotos-add-locations.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-comment -
-osxphotos-add-locations.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-description -
-osxphotos-add-locations.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-keyword -
-osxphotos-add-locations.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-likes -
-osxphotos-add-locations.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-location -
-osxphotos-add-locations.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-place -
-osxphotos-add-locations.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-title -
-osxphotos-add-locations.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-burst -
-osxphotos-add-locations.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-cloudasset -
-osxphotos-add-locations.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-edited -
-osxphotos-add-locations.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-favorite -
-osxphotos-add-locations.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-hdr -
-osxphotos-add-locations.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-hidden -
-osxphotos-add-locations.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-in-album -
-osxphotos-add-locations.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-incloud -
-osxphotos-add-locations.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-live -
-osxphotos-add-locations.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-missing -
-osxphotos-add-locations.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-panorama -
-osxphotos-add-locations.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-portrait -
-osxphotos-add-locations.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-reference -
-osxphotos-add-locations.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-saved-to-library -
-osxphotos-add-locations.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-screenshot -
-osxphotos-add-locations.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-selfie -
-osxphotos-add-locations.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-shared -
-osxphotos-add-locations.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-slow-mo -
-osxphotos-add-locations.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-syndicated -
-osxphotos-add-locations.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-time-lapse -
-osxphotos-add-locations.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-only-movies -
-osxphotos-add-locations.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-only-photos -
-osxphotos-add-locations.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-panorama -
-osxphotos-add-locations.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-person -
-osxphotos-add-locations.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-place -
-osxphotos-add-locations.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-portrait -
-osxphotos-add-locations.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-query-eval -
-osxphotos-add-locations.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-query-function -
-osxphotos-add-locations.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-regex -
-osxphotos-add-locations.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-saved-to-library -
-osxphotos-add-locations.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-screenshot -
-osxphotos-add-locations.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-selected -
-osxphotos-add-locations.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-selfie -
-osxphotos-add-locations.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-shared -
-osxphotos-add-locations.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-slow-mo -
-osxphotos-add-locations.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-syndicated -
-osxphotos-add-locations.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-theme -
-osxphotos-add-locations.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-time-lapse -
-osxphotos-add-locations.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-timestamp -
-osxphotos-add-locations.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-title -
-osxphotos-add-locations.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-to-date -
-osxphotos-add-locations.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-to-time -
-osxphotos-add-locations.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-uti -
-osxphotos-add-locations.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-uuid -
-osxphotos-add-locations.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-uuid-from-file -
-osxphotos-add-locations.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-V -
-osxphotos-add-locations.--window std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-w -
-osxphotos-add-locations.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-year -
-osxphotos-add-locations.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-V -
-osxphotos-add-locations.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-i -
-osxphotos-add-locations.-w std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-w -
-osxphotos-albums.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-library -
-osxphotos-albums.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-json -
-osxphotos-albums.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-library -
-osxphotos-albums.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY -
-osxphotos-batch-edit.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-library -
-osxphotos-batch-edit.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-description -
-osxphotos-batch-edit.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-dry-run -
-osxphotos-batch-edit.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-keyword -
-osxphotos-batch-edit.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-library -
-osxphotos-batch-edit.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-location -
-osxphotos-batch-edit.--replace-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-replace-keywords -
-osxphotos-batch-edit.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-theme -
-osxphotos-batch-edit.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-timestamp -
-osxphotos-batch-edit.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-title -
-osxphotos-batch-edit.--undo std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-undo -
-osxphotos-batch-edit.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-V -
-osxphotos-batch-edit.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-V -
-osxphotos-diff.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-library -
-osxphotos-diff.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-library -
-osxphotos-diff.--raw-output std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-r -
-osxphotos-diff.--style std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-s -
-osxphotos-diff.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-timestamp -
-osxphotos-diff.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-V -
-osxphotos-diff.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-V -
-osxphotos-diff.-r std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-r -
-osxphotos-diff.-s std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-s -
-osxphotos-diff.DB2 std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-arg-DB2 -
-osxphotos-dump.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-library -
-osxphotos-dump.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-deleted -
-osxphotos-dump.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-deleted-only -
-osxphotos-dump.--field std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-f -
-osxphotos-dump.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-json -
-osxphotos-dump.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-library -
-osxphotos-dump.--print std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-print -
-osxphotos-dump.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-f -
-osxphotos-dump.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY -
-osxphotos-exiftool.--album-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-album-keyword -
-osxphotos-exiftool.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-append -
-osxphotos-exiftool.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-library -
-osxphotos-exiftool.--db-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-db-config -
-osxphotos-exiftool.--description-template std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-description-template -
-osxphotos-exiftool.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-dry-run -
-osxphotos-exiftool.--exiftool-merge-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-merge-keywords -
-osxphotos-exiftool.--exiftool-merge-persons std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-merge-persons -
-osxphotos-exiftool.--exiftool-option std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-option -
-osxphotos-exiftool.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-path -
-osxphotos-exiftool.--exportdb std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exportdb -
-osxphotos-exiftool.--ignore-date-modified std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-ignore-date-modified -
-osxphotos-exiftool.--keyword-template std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-keyword-template -
-osxphotos-exiftool.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-library -
-osxphotos-exiftool.--load-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-load-config -
-osxphotos-exiftool.--person-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-person-keyword -
-osxphotos-exiftool.--replace-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-replace-keywords -
-osxphotos-exiftool.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-report -
-osxphotos-exiftool.--save-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-save-config -
-osxphotos-exiftool.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-theme -
-osxphotos-exiftool.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-timestamp -
-osxphotos-exiftool.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-V -
-osxphotos-exiftool.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-V -
-osxphotos-exiftool.EXPORT_DIRECTORY std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY -
-osxphotos-export.--add-exported-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-add-exported-to-album -
-osxphotos-export.--add-missing-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-add-missing-to-album -
-osxphotos-export.--add-skipped-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-add-skipped-to-album -
-osxphotos-export.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-export-added-after -
-osxphotos-export.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-export-added-before -
-osxphotos-export.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-export-added-in-last -
-osxphotos-export.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-album -
-osxphotos-export.--album-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-album-keyword -
-osxphotos-export.--alt-copy std:cmdoption 1 cli.html#cmdoption-osxphotos-export-alt-copy -
-osxphotos-export.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-export-append -
-osxphotos-export.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-export-burst -
-osxphotos-export.--cleanup std:cmdoption 1 cli.html#cmdoption-osxphotos-export-cleanup -
-osxphotos-export.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-export-cloudasset -
-osxphotos-export.--config-only std:cmdoption 1 cli.html#cmdoption-osxphotos-export-config-only -
-osxphotos-export.--convert-to-jpeg std:cmdoption 1 cli.html#cmdoption-osxphotos-export-convert-to-jpeg -
-osxphotos-export.--current-name std:cmdoption 1 cli.html#cmdoption-osxphotos-export-current-name -
-osxphotos-export.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-export-library -
-osxphotos-export.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-export-deleted -
-osxphotos-export.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-export-deleted-only -
-osxphotos-export.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-export-description -
-osxphotos-export.--description-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-description-template -
-osxphotos-export.--directory std:cmdoption 1 cli.html#cmdoption-osxphotos-export-directory -
-osxphotos-export.--download-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-download-missing -
-osxphotos-export.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-export-dry-run -
-osxphotos-export.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-export-duplicate -
-osxphotos-export.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-edited -
-osxphotos-export.--edited-suffix std:cmdoption 1 cli.html#cmdoption-osxphotos-export-edited-suffix -
-osxphotos-export.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exif -
-osxphotos-export.--exiftool std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool -
-osxphotos-export.--exiftool-merge-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-merge-keywords -
-osxphotos-export.--exiftool-merge-persons std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-merge-persons -
-osxphotos-export.--exiftool-option std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-option -
-osxphotos-export.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-path -
-osxphotos-export.--export-as-hardlink std:cmdoption 1 cli.html#cmdoption-osxphotos-export-export-as-hardlink -
-osxphotos-export.--export-by-date std:cmdoption 1 cli.html#cmdoption-osxphotos-export-export-by-date -
-osxphotos-export.--exportdb std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exportdb -
-osxphotos-export.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-export-external-edit -
-osxphotos-export.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-export-favorite -
-osxphotos-export.--favorite-rating std:cmdoption 1 cli.html#cmdoption-osxphotos-export-favorite-rating -
-osxphotos-export.--filename std:cmdoption 1 cli.html#cmdoption-osxphotos-export-filename -
-osxphotos-export.--finder-tag-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-export-finder-tag-keywords -
-osxphotos-export.--finder-tag-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-finder-tag-template -
-osxphotos-export.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-export-folder -
-osxphotos-export.--force-update std:cmdoption 1 cli.html#cmdoption-osxphotos-export-force-update -
-osxphotos-export.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-export-from-date -
-osxphotos-export.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-export-from-time -
-osxphotos-export.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-export-has-comment -
-osxphotos-export.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-export-has-likes -
-osxphotos-export.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-export-has-raw -
-osxphotos-export.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-export-hdr -
-osxphotos-export.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-export-hidden -
-osxphotos-export.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-export-i -
-osxphotos-export.--ignore-date-modified std:cmdoption 1 cli.html#cmdoption-osxphotos-export-ignore-date-modified -
-osxphotos-export.--ignore-signature std:cmdoption 1 cli.html#cmdoption-osxphotos-export-ignore-signature -
-osxphotos-export.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-in-album -
-osxphotos-export.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-export-incloud -
-osxphotos-export.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-export-is-reference -
-osxphotos-export.--jpeg-ext std:cmdoption 1 cli.html#cmdoption-osxphotos-export-jpeg-ext -
-osxphotos-export.--jpeg-quality std:cmdoption 1 cli.html#cmdoption-osxphotos-export-jpeg-quality -
-osxphotos-export.--keep std:cmdoption 1 cli.html#cmdoption-osxphotos-export-keep -
-osxphotos-export.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-keyword -
-osxphotos-export.--keyword-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-keyword-template -
-osxphotos-export.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-export-label -
-osxphotos-export.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-library -
-osxphotos-export.--limit std:cmdoption 1 cli.html#cmdoption-osxphotos-export-limit -
-osxphotos-export.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-live -
-osxphotos-export.--load-config std:cmdoption 1 cli.html#cmdoption-osxphotos-export-load-config -
-osxphotos-export.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-export-location -
-osxphotos-export.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-export-max-size -
-osxphotos-export.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-export-min-size -
-osxphotos-export.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-missing -
-osxphotos-export.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-export-name -
-osxphotos-export.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-comment -
-osxphotos-export.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-description -
-osxphotos-export.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-keyword -
-osxphotos-export.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-likes -
-osxphotos-export.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-location -
-osxphotos-export.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-place -
-osxphotos-export.--no-progress std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-progress -
-osxphotos-export.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-title -
-osxphotos-export.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-burst -
-osxphotos-export.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-cloudasset -
-osxphotos-export.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-edited -
-osxphotos-export.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-favorite -
-osxphotos-export.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-hdr -
-osxphotos-export.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-hidden -
-osxphotos-export.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-in-album -
-osxphotos-export.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-incloud -
-osxphotos-export.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-live -
-osxphotos-export.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-missing -
-osxphotos-export.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-panorama -
-osxphotos-export.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-portrait -
-osxphotos-export.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-reference -
-osxphotos-export.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-saved-to-library -
-osxphotos-export.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-screenshot -
-osxphotos-export.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-selfie -
-osxphotos-export.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-shared -
-osxphotos-export.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-slow-mo -
-osxphotos-export.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-syndicated -
-osxphotos-export.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-time-lapse -
-osxphotos-export.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-movies -
-osxphotos-export.--only-new std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-new -
-osxphotos-export.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-photos -
-osxphotos-export.--original-suffix std:cmdoption 1 cli.html#cmdoption-osxphotos-export-original-suffix -
-osxphotos-export.--overwrite std:cmdoption 1 cli.html#cmdoption-osxphotos-export-overwrite -
-osxphotos-export.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-export-panorama -
-osxphotos-export.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-export-person -
-osxphotos-export.--person-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-person-keyword -
-osxphotos-export.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-export-place -
-osxphotos-export.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-export-portrait -
-osxphotos-export.--post-command std:cmdoption 1 cli.html#cmdoption-osxphotos-export-post-command -
-osxphotos-export.--post-function std:cmdoption 1 cli.html#cmdoption-osxphotos-export-post-function -
-osxphotos-export.--preview std:cmdoption 1 cli.html#cmdoption-osxphotos-export-preview -
-osxphotos-export.--preview-if-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-preview-if-missing -
-osxphotos-export.--preview-suffix std:cmdoption 1 cli.html#cmdoption-osxphotos-export-preview-suffix -
-osxphotos-export.--print std:cmdoption 1 cli.html#cmdoption-osxphotos-export-print -
-osxphotos-export.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-export-query-eval -
-osxphotos-export.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-export-query-function -
-osxphotos-export.--ramdb std:cmdoption 1 cli.html#cmdoption-osxphotos-export-ramdb -
-osxphotos-export.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-export-regex -
-osxphotos-export.--replace-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-export-replace-keywords -
-osxphotos-export.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-export-report -
-osxphotos-export.--retry std:cmdoption 1 cli.html#cmdoption-osxphotos-export-retry -
-osxphotos-export.--save-config std:cmdoption 1 cli.html#cmdoption-osxphotos-export-save-config -
-osxphotos-export.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-saved-to-library -
-osxphotos-export.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-export-screenshot -
-osxphotos-export.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selected -
-osxphotos-export.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selfie -
-osxphotos-export.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-export-shared -
-osxphotos-export.--sidecar std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar -
-osxphotos-export.--sidecar-drop-ext std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar-drop-ext -
-osxphotos-export.--skip-bursts std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-bursts -
-osxphotos-export.--skip-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-edited -
-osxphotos-export.--skip-live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-live -
-osxphotos-export.--skip-original-if-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-original-if-edited -
-osxphotos-export.--skip-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-raw -
-osxphotos-export.--skip-uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid -
-osxphotos-export.--skip-uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid-from-file -
-osxphotos-export.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-export-slow-mo -
-osxphotos-export.--strip std:cmdoption 1 cli.html#cmdoption-osxphotos-export-strip -
-osxphotos-export.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-export-syndicated -
-osxphotos-export.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-export-theme -
-osxphotos-export.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-export-time-lapse -
-osxphotos-export.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-export-timestamp -
-osxphotos-export.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-export-title -
-osxphotos-export.--tmpdir std:cmdoption 1 cli.html#cmdoption-osxphotos-export-tmpdir -
-osxphotos-export.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-export-to-date -
-osxphotos-export.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-export-to-time -
-osxphotos-export.--touch-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-touch-file -
-osxphotos-export.--update std:cmdoption 1 cli.html#cmdoption-osxphotos-export-update -
-osxphotos-export.--update-errors std:cmdoption 1 cli.html#cmdoption-osxphotos-export-update-errors -
-osxphotos-export.--use-photokit std:cmdoption 1 cli.html#cmdoption-osxphotos-export-use-photokit -
-osxphotos-export.--use-photos-export std:cmdoption 1 cli.html#cmdoption-osxphotos-export-use-photos-export -
-osxphotos-export.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-export-uti -
-osxphotos-export.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-export-uuid -
-osxphotos-export.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-uuid-from-file -
-osxphotos-export.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-export-V -
-osxphotos-export.--xattr-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-xattr-template -
-osxphotos-export.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-export-year -
-osxphotos-export.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-export-V -
-osxphotos-export.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-export-i -
-osxphotos-export.DEST std:cmdoption 1 cli.html#cmdoption-osxphotos-export-arg-DEST -
-osxphotos-export.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY -
-osxphotos-exportdb.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-append -
-osxphotos-exportdb.--check-signatures std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-check-signatures -
-osxphotos-exportdb.--delete-file std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-delete-file -
-osxphotos-exportdb.--delete-uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-delete-uuid -
-osxphotos-exportdb.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-dry-run -
-osxphotos-exportdb.--errors std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-errors -
-osxphotos-exportdb.--export-dir std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-export-dir -
-osxphotos-exportdb.--info std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-info -
-osxphotos-exportdb.--last-errors std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-last-errors -
-osxphotos-exportdb.--last-run std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-last-run -
-osxphotos-exportdb.--migrate std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-migrate -
-osxphotos-exportdb.--migrate-photos-library std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-migrate-photos-library -
-osxphotos-exportdb.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-report -
-osxphotos-exportdb.--save-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-save-config -
-osxphotos-exportdb.--sql std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-sql -
-osxphotos-exportdb.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-theme -
-osxphotos-exportdb.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-timestamp -
-osxphotos-exportdb.--touch-file std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-touch-file -
-osxphotos-exportdb.--update-signatures std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-update-signatures -
-osxphotos-exportdb.--uuid-files std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-uuid-files -
-osxphotos-exportdb.--uuid-info std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-uuid-info -
-osxphotos-exportdb.--vacuum std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-vacuum -
-osxphotos-exportdb.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-V -
-osxphotos-exportdb.--version std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-version -
-osxphotos-exportdb.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-V -
-osxphotos-exportdb.EXPORT_DATABASE std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE -
-osxphotos-help.SUBTOPIC std:cmdoption 1 cli.html#cmdoption-osxphotos-help-arg-SUBTOPIC -
-osxphotos-help.TOPIC std:cmdoption 1 cli.html#cmdoption-osxphotos-help-arg-TOPIC -
-osxphotos-import.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-import-a -
-osxphotos-import.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-import-append -
-osxphotos-import.--check-templates std:cmdoption 1 cli.html#cmdoption-osxphotos-import-check-templates -
-osxphotos-import.--clear-location std:cmdoption 1 cli.html#cmdoption-osxphotos-import-L -
-osxphotos-import.--clear-metadata std:cmdoption 1 cli.html#cmdoption-osxphotos-import-C -
-osxphotos-import.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-import-d -
-osxphotos-import.--dup-check std:cmdoption 1 cli.html#cmdoption-osxphotos-import-D -
-osxphotos-import.--exiftool std:cmdoption 1 cli.html#cmdoption-osxphotos-import-e -
-osxphotos-import.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-import-0 -
-osxphotos-import.--glob std:cmdoption 1 cli.html#cmdoption-osxphotos-import-g -
-osxphotos-import.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-import-k -
-osxphotos-import.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-import-l -
-osxphotos-import.--merge-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-import-m -
-osxphotos-import.--no-progress std:cmdoption 1 cli.html#cmdoption-osxphotos-import-no-progress -
-osxphotos-import.--parse-date std:cmdoption 1 cli.html#cmdoption-osxphotos-import-P -
-osxphotos-import.--post-function std:cmdoption 1 cli.html#cmdoption-osxphotos-import-post-function -
-osxphotos-import.--relative-to std:cmdoption 1 cli.html#cmdoption-osxphotos-import-r -
-osxphotos-import.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-import-report -
-osxphotos-import.--resume std:cmdoption 1 cli.html#cmdoption-osxphotos-import-R -
-osxphotos-import.--split-folder std:cmdoption 1 cli.html#cmdoption-osxphotos-import-f -
-osxphotos-import.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-import-theme -
-osxphotos-import.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-import-timestamp -
-osxphotos-import.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-import-t -
-osxphotos-import.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-import-V -
-osxphotos-import.--walk std:cmdoption 1 cli.html#cmdoption-osxphotos-import-w -
-osxphotos-import.-C std:cmdoption 1 cli.html#cmdoption-osxphotos-import-C -
-osxphotos-import.-D std:cmdoption 1 cli.html#cmdoption-osxphotos-import-D -
-osxphotos-import.-L std:cmdoption 1 cli.html#cmdoption-osxphotos-import-L -
-osxphotos-import.-P std:cmdoption 1 cli.html#cmdoption-osxphotos-import-P -
-osxphotos-import.-R std:cmdoption 1 cli.html#cmdoption-osxphotos-import-R -
-osxphotos-import.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-import-V -
-osxphotos-import.-a std:cmdoption 1 cli.html#cmdoption-osxphotos-import-a -
-osxphotos-import.-d std:cmdoption 1 cli.html#cmdoption-osxphotos-import-d -
-osxphotos-import.-e std:cmdoption 1 cli.html#cmdoption-osxphotos-import-e -
-osxphotos-import.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-import-f -
-osxphotos-import.-g std:cmdoption 1 cli.html#cmdoption-osxphotos-import-g -
-osxphotos-import.-k std:cmdoption 1 cli.html#cmdoption-osxphotos-import-k -
-osxphotos-import.-l std:cmdoption 1 cli.html#cmdoption-osxphotos-import-l -
-osxphotos-import.-m std:cmdoption 1 cli.html#cmdoption-osxphotos-import-m -
-osxphotos-import.-p std:cmdoption 1 cli.html#cmdoption-osxphotos-import-0 -
-osxphotos-import.-r std:cmdoption 1 cli.html#cmdoption-osxphotos-import-r -
-osxphotos-import.-t std:cmdoption 1 cli.html#cmdoption-osxphotos-import-t -
-osxphotos-import.-w std:cmdoption 1 cli.html#cmdoption-osxphotos-import-w -
-osxphotos-import.FILES std:cmdoption 1 cli.html#cmdoption-osxphotos-import-arg-FILES -
-osxphotos-info.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-info-library -
-osxphotos-info.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-info-json -
-osxphotos-info.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-info-library -
-osxphotos-info.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY -
-osxphotos-inspect.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-library -
-osxphotos-inspect.--detect-text std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-t -
-osxphotos-inspect.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-library -
-osxphotos-inspect.--template std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-T -
-osxphotos-inspect.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-theme -
-osxphotos-inspect.-T std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-T -
-osxphotos-inspect.-t std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-t -
-osxphotos-install.--upgrade std:cmdoption 1 cli.html#cmdoption-osxphotos-install-U -
-osxphotos-install.-U std:cmdoption 1 cli.html#cmdoption-osxphotos-install-U -
-osxphotos-install.PACKAGES std:cmdoption 1 cli.html#cmdoption-osxphotos-install-arg-PACKAGES -
-osxphotos-keywords.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-library -
-osxphotos-keywords.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-json -
-osxphotos-keywords.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-library -
-osxphotos-keywords.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY -
-osxphotos-labels.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-library -
-osxphotos-labels.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-json -
-osxphotos-labels.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-library -
-osxphotos-labels.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY -
-osxphotos-list.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-list-json -
-osxphotos-orphans.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-library -
-osxphotos-orphans.--export std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-export -
-osxphotos-orphans.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-library -
-osxphotos-orphans.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-theme -
-osxphotos-orphans.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-timestamp -
-osxphotos-orphans.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-V -
-osxphotos-orphans.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-V -
-osxphotos-persons.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-library -
-osxphotos-persons.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-json -
-osxphotos-persons.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-library -
-osxphotos-persons.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY -
-osxphotos-places.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-places-library -
-osxphotos-places.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-places-json -
-osxphotos-places.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-places-library -
-osxphotos-places.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY -
-osxphotos-query.--add-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-add-to-album -
-osxphotos-query.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-after -
-osxphotos-query.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-before -
-osxphotos-query.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-in-last -
-osxphotos-query.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-album -
-osxphotos-query.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-query-burst -
-osxphotos-query.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-query-cloudasset -
-osxphotos-query.--count std:cmdoption 1 cli.html#cmdoption-osxphotos-query-count -
-osxphotos-query.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-query-library -
-osxphotos-query.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-query-deleted -
-osxphotos-query.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-query-deleted-only -
-osxphotos-query.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-query-description -
-osxphotos-query.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-query-duplicate -
-osxphotos-query.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-query-edited -
-osxphotos-query.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-query-exif -
-osxphotos-query.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-query-external-edit -
-osxphotos-query.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-query-favorite -
-osxphotos-query.--field std:cmdoption 1 cli.html#cmdoption-osxphotos-query-f -
-osxphotos-query.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-query-folder -
-osxphotos-query.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-query-from-date -
-osxphotos-query.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-query-from-time -
-osxphotos-query.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-query-has-comment -
-osxphotos-query.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-query-has-likes -
-osxphotos-query.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-query-has-raw -
-osxphotos-query.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-query-hdr -
-osxphotos-query.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-query-hidden -
-osxphotos-query.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-query-i -
-osxphotos-query.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-in-album -
-osxphotos-query.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-query-incloud -
-osxphotos-query.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-query-is-reference -
-osxphotos-query.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-query-json -
-osxphotos-query.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-query-keyword -
-osxphotos-query.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-query-label -
-osxphotos-query.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-library -
-osxphotos-query.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-query-live -
-osxphotos-query.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-query-location -
-osxphotos-query.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-query-max-size -
-osxphotos-query.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-query-min-size -
-osxphotos-query.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-query-missing -
-osxphotos-query.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-query-name -
-osxphotos-query.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-comment -
-osxphotos-query.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-description -
-osxphotos-query.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-keyword -
-osxphotos-query.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-likes -
-osxphotos-query.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-location -
-osxphotos-query.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-place -
-osxphotos-query.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-title -
-osxphotos-query.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-burst -
-osxphotos-query.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-cloudasset -
-osxphotos-query.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-edited -
-osxphotos-query.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-favorite -
-osxphotos-query.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-hdr -
-osxphotos-query.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-hidden -
-osxphotos-query.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-in-album -
-osxphotos-query.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-incloud -
-osxphotos-query.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-live -
-osxphotos-query.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-missing -
-osxphotos-query.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-panorama -
-osxphotos-query.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-portrait -
-osxphotos-query.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-reference -
-osxphotos-query.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-saved-to-library -
-osxphotos-query.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-screenshot -
-osxphotos-query.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-selfie -
-osxphotos-query.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-shared -
-osxphotos-query.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-slow-mo -
-osxphotos-query.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-syndicated -
-osxphotos-query.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-time-lapse -
-osxphotos-query.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-query-only-movies -
-osxphotos-query.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-query-only-photos -
-osxphotos-query.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-query-panorama -
-osxphotos-query.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-query-person -
-osxphotos-query.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-query-place -
-osxphotos-query.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-query-portrait -
-osxphotos-query.--print std:cmdoption 1 cli.html#cmdoption-osxphotos-query-print -
-osxphotos-query.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-query-query-eval -
-osxphotos-query.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-query-query-function -
-osxphotos-query.--quiet std:cmdoption 1 cli.html#cmdoption-osxphotos-query-quiet -
-osxphotos-query.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-query-regex -
-osxphotos-query.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-saved-to-library -
-osxphotos-query.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-query-screenshot -
-osxphotos-query.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-query-selected -
-osxphotos-query.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-query-selfie -
-osxphotos-query.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-query-shared -
-osxphotos-query.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-query-slow-mo -
-osxphotos-query.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-query-syndicated -
-osxphotos-query.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-query-time-lapse -
-osxphotos-query.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-query-title -
-osxphotos-query.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-query-to-date -
-osxphotos-query.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-query-to-time -
-osxphotos-query.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uti -
-osxphotos-query.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uuid -
-osxphotos-query.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uuid-from-file -
-osxphotos-query.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-query-year -
-osxphotos-query.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-query-f -
-osxphotos-query.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-query-i -
-osxphotos-query.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY -
-osxphotos-repl.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-added-after -
-osxphotos-repl.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-added-before -
-osxphotos-repl.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-added-in-last -
-osxphotos-repl.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-album -
-osxphotos-repl.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-burst -
-osxphotos-repl.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-cloudasset -
-osxphotos-repl.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-library -
-osxphotos-repl.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-deleted -
-osxphotos-repl.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-deleted-only -
-osxphotos-repl.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-description -
-osxphotos-repl.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-duplicate -
-osxphotos-repl.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-edited -
-osxphotos-repl.--emacs std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-emacs -
-osxphotos-repl.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-exif -
-osxphotos-repl.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-external-edit -
-osxphotos-repl.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-favorite -
-osxphotos-repl.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-folder -
-osxphotos-repl.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-from-date -
-osxphotos-repl.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-from-time -
-osxphotos-repl.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-has-comment -
-osxphotos-repl.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-has-likes -
-osxphotos-repl.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-has-raw -
-osxphotos-repl.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-hdr -
-osxphotos-repl.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-hidden -
-osxphotos-repl.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-i -
-osxphotos-repl.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-in-album -
-osxphotos-repl.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-incloud -
-osxphotos-repl.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-is-reference -
-osxphotos-repl.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-keyword -
-osxphotos-repl.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-label -
-osxphotos-repl.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-library -
-osxphotos-repl.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-live -
-osxphotos-repl.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-location -
-osxphotos-repl.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-max-size -
-osxphotos-repl.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-min-size -
-osxphotos-repl.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-missing -
-osxphotos-repl.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-name -
-osxphotos-repl.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-comment -
-osxphotos-repl.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-description -
-osxphotos-repl.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-keyword -
-osxphotos-repl.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-likes -
-osxphotos-repl.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-location -
-osxphotos-repl.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-place -
-osxphotos-repl.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-title -
-osxphotos-repl.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-burst -
-osxphotos-repl.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-cloudasset -
-osxphotos-repl.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-edited -
-osxphotos-repl.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-favorite -
-osxphotos-repl.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-hdr -
-osxphotos-repl.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-hidden -
-osxphotos-repl.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-in-album -
-osxphotos-repl.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-incloud -
-osxphotos-repl.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-live -
-osxphotos-repl.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-missing -
-osxphotos-repl.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-panorama -
-osxphotos-repl.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-portrait -
-osxphotos-repl.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-reference -
-osxphotos-repl.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-saved-to-library -
-osxphotos-repl.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-screenshot -
-osxphotos-repl.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-selfie -
-osxphotos-repl.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-shared -
-osxphotos-repl.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-slow-mo -
-osxphotos-repl.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-syndicated -
-osxphotos-repl.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-time-lapse -
-osxphotos-repl.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-only-movies -
-osxphotos-repl.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-only-photos -
-osxphotos-repl.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-panorama -
-osxphotos-repl.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-person -
-osxphotos-repl.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-place -
-osxphotos-repl.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-portrait -
-osxphotos-repl.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-query-eval -
-osxphotos-repl.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-query-function -
-osxphotos-repl.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-regex -
-osxphotos-repl.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-saved-to-library -
-osxphotos-repl.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-screenshot -
-osxphotos-repl.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-selected -
-osxphotos-repl.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-selfie -
-osxphotos-repl.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-shared -
-osxphotos-repl.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-slow-mo -
-osxphotos-repl.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-syndicated -
-osxphotos-repl.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-time-lapse -
-osxphotos-repl.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-title -
-osxphotos-repl.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-to-date -
-osxphotos-repl.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-to-time -
-osxphotos-repl.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uti -
-osxphotos-repl.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uuid -
-osxphotos-repl.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uuid-from-file -
-osxphotos-repl.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-year -
-osxphotos-repl.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-i -
-osxphotos-run.--help std:cmdoption 1 cli.html#cmdoption-osxphotos-run-h -
-osxphotos-run.-h std:cmdoption 1 cli.html#cmdoption-osxphotos-run-h -
-osxphotos-run.ARGS std:cmdoption 1 cli.html#cmdoption-osxphotos-run-arg-ARGS -
-osxphotos-run.PYTHON_FILE std:cmdoption 1 cli.html#cmdoption-osxphotos-run-arg-PYTHON_FILE -
-osxphotos-show.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-show-library -
-osxphotos-show.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-show-library -
-osxphotos-show.UUID_OR_NAME std:cmdoption 1 cli.html#cmdoption-osxphotos-show-arg-UUID_OR_NAME -
-osxphotos-snap.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-snap-library -
-osxphotos-snap.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-snap-library -
-osxphotos-sync.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-added-after -
-osxphotos-sync.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-added-before -
-osxphotos-sync.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-added-in-last -
-osxphotos-sync.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-album -
-osxphotos-sync.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-A -
-osxphotos-sync.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-burst -
-osxphotos-sync.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-cloudasset -
-osxphotos-sync.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-library -
-osxphotos-sync.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-description -
-osxphotos-sync.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-dry-run -
-osxphotos-sync.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-duplicate -
-osxphotos-sync.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-edited -
-osxphotos-sync.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-exif -
-osxphotos-sync.--export std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-e -
-osxphotos-sync.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-external-edit -
-osxphotos-sync.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-favorite -
-osxphotos-sync.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-folder -
-osxphotos-sync.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-from-date -
-osxphotos-sync.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-from-time -
-osxphotos-sync.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-has-comment -
-osxphotos-sync.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-has-likes -
-osxphotos-sync.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-has-raw -
-osxphotos-sync.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-hdr -
-osxphotos-sync.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-hidden -
-osxphotos-sync.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-0 -
-osxphotos-sync.--import std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-i -
-osxphotos-sync.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-in-album -
-osxphotos-sync.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-incloud -
-osxphotos-sync.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-is-reference -
-osxphotos-sync.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-keyword -
-osxphotos-sync.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-label -
-osxphotos-sync.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-library -
-osxphotos-sync.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-live -
-osxphotos-sync.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-location -
-osxphotos-sync.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-max-size -
-osxphotos-sync.--merge std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-m -
-osxphotos-sync.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-min-size -
-osxphotos-sync.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-missing -
-osxphotos-sync.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-name -
-osxphotos-sync.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-comment -
-osxphotos-sync.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-description -
-osxphotos-sync.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-keyword -
-osxphotos-sync.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-likes -
-osxphotos-sync.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-location -
-osxphotos-sync.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-place -
-osxphotos-sync.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-title -
-osxphotos-sync.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-burst -
-osxphotos-sync.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-cloudasset -
-osxphotos-sync.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-edited -
-osxphotos-sync.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-favorite -
-osxphotos-sync.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-hdr -
-osxphotos-sync.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-hidden -
-osxphotos-sync.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-in-album -
-osxphotos-sync.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-incloud -
-osxphotos-sync.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-live -
-osxphotos-sync.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-missing -
-osxphotos-sync.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-panorama -
-osxphotos-sync.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-portrait -
-osxphotos-sync.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-reference -
-osxphotos-sync.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-saved-to-library -
-osxphotos-sync.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-screenshot -
-osxphotos-sync.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-selfie -
-osxphotos-sync.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-slow-mo -
-osxphotos-sync.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-syndicated -
-osxphotos-sync.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-time-lapse -
-osxphotos-sync.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-only-movies -
-osxphotos-sync.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-only-photos -
-osxphotos-sync.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-panorama -
-osxphotos-sync.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-person -
-osxphotos-sync.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-place -
-osxphotos-sync.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-portrait -
-osxphotos-sync.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-query-eval -
-osxphotos-sync.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-query-function -
-osxphotos-sync.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-regex -
-osxphotos-sync.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-R -
-osxphotos-sync.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-saved-to-library -
-osxphotos-sync.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-screenshot -
-osxphotos-sync.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-selected -
-osxphotos-sync.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-selfie -
-osxphotos-sync.--set std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-s -
-osxphotos-sync.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-slow-mo -
-osxphotos-sync.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-syndicated -
-osxphotos-sync.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-theme -
-osxphotos-sync.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-time-lapse -
-osxphotos-sync.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-timestamp -
-osxphotos-sync.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-title -
-osxphotos-sync.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-to-date -
-osxphotos-sync.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-to-time -
-osxphotos-sync.--unmatched std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-U -
-osxphotos-sync.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-uti -
-osxphotos-sync.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-uuid -
-osxphotos-sync.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-uuid-from-file -
-osxphotos-sync.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-V -
-osxphotos-sync.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-year -
-osxphotos-sync.-A std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-A -
-osxphotos-sync.-R std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-R -
-osxphotos-sync.-U std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-U -
-osxphotos-sync.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-V -
-osxphotos-sync.-e std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-e -
-osxphotos-sync.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-i -
-osxphotos-sync.-m std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-m -
-osxphotos-sync.-s std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-s -
-osxphotos-theme.--clone std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-clone -
-osxphotos-theme.--config std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-config -
-osxphotos-theme.--default std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-default -
-osxphotos-theme.--delete std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-delete -
-osxphotos-theme.--edit std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-edit -
-osxphotos-theme.--list std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-list -
-osxphotos-theme.--preview std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-preview -
-osxphotos-timewarp.--add-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-a -
-osxphotos-timewarp.--compare-exif std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-c -
-osxphotos-timewarp.--date std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-d -
-osxphotos-timewarp.--date-added std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-date-added -
-osxphotos-timewarp.--date-added-from-photo std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-date-added-from-photo -
-osxphotos-timewarp.--date-delta std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-D -
-osxphotos-timewarp.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-e -
-osxphotos-timewarp.--force std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-force -
-osxphotos-timewarp.--function std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-F -
-osxphotos-timewarp.--inspect std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-i -
-osxphotos-timewarp.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-L -
-osxphotos-timewarp.--match-time std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-0 -
-osxphotos-timewarp.--parse-date std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-M -
-osxphotos-timewarp.--plain std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-plain -
-osxphotos-timewarp.--pull-exif std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-P -
-osxphotos-timewarp.--push-exif std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-p -
-osxphotos-timewarp.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-theme -
-osxphotos-timewarp.--time std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-t -
-osxphotos-timewarp.--time-delta std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-T -
-osxphotos-timewarp.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-timestamp -
-osxphotos-timewarp.--timezone std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-z -
-osxphotos-timewarp.--use-file-time std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-1 -
-osxphotos-timewarp.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-V -
-osxphotos-timewarp.-D std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-D -
-osxphotos-timewarp.-F std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-F -
-osxphotos-timewarp.-L std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-L -
-osxphotos-timewarp.-M std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-M -
-osxphotos-timewarp.-P std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-P -
-osxphotos-timewarp.-T std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-T -
-osxphotos-timewarp.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-V -
-osxphotos-timewarp.-a std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-a -
-osxphotos-timewarp.-c std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-c -
-osxphotos-timewarp.-d std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-d -
-osxphotos-timewarp.-e std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-e -
-osxphotos-timewarp.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-1 -
-osxphotos-timewarp.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-i -
-osxphotos-timewarp.-m std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-0 -
-osxphotos-timewarp.-p std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-p -
-osxphotos-timewarp.-t std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-t -
-osxphotos-timewarp.-z std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-z -
-osxphotos-tutorial.WIDTH std:cmdoption 1 cli.html#cmdoption-osxphotos-tutorial-arg-WIDTH -
-osxphotos-uninstall.--yes std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-y -
-osxphotos-uninstall.-y std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-y -
-osxphotos-uninstall.PACKAGES std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-arg-PACKAGES -
-osxphotos-uuid.--filename std:cmdoption 1 cli.html#cmdoption-osxphotos-uuid-f -
-osxphotos-uuid.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-uuid-f -
-osxphotos-version.--run std:cmdoption 1 cli.html#cmdoption-osxphotos-version-run -
-osxphotos.--version std:cmdoption 1 cli.html#cmdoption-osxphotos-v -
-osxphotos.-v std:cmdoption 1 cli.html#cmdoption-osxphotos-v -
-overview std:doc -1 overview.html OSXPhotos
-package_overview std:doc -1 package_overview.html OSXPhotos Python Package Overview
-py-modindex std:label -1 py-modindex.html Python Module Index
-reference std:doc -1 reference.html OSXPhotos Python Reference
-search std:label -1 search.html Search Page
-template_help std:doc -1 template_help.html OSXPhotos Template System
-tutorial std:doc -1 tutorial.html OSXPhotos Tutorial
+xڵv8~
+Y,ҧzsU>jklYݽ⡒H%KL2dJV5Iwą?+R3A n~>vc7ܜ_tKn~فݳA~77w=trߔpǥam9T~l<vX_4 }wfh0¹/wO*_zz1k~6W=%Ӊo֓mpuM۲d[_usì]i=e[!_s`l"CW}؇3n2xo!"]׶l?v߳rdšnXѳ=5(Hl$*0Ϊʱ,(hr<n\j䊘ja$ѳҌpUIP@iO I.d2fq)
+(g?a|#d{asޱ9s|c߀Y}mo!<(C8edy)FT)m*N0-ׂj>tQ |VDDLwRlP˾jCSãN0.r=ub5˹uzI?CMz5n']Y˝^1l9R65>q{}_S?35'Q ݾ4581[b)jԎ[/{r8	|!?2cbKĻ 6xjz$ueO'#>BtkA]GJ !9M
+]Oy.+J6_fU %QzD`AodLz[6`j%aO|,U5pݪjk}iH6o՚}-w+}ѧn\J^uڢw)L?B}4a!u_C;NЪWNM/?o3d+h*7;Uv9TybI Ɨ/fTV?FukV:ȝ&c<\Tw Ol^k$f{4d7c^v[S^e'vqL7sLҴ !8Se?h8`/1϶X:d?}s噽@F͙S-g ych:XṊG-2ZfVS`D|04F~da/#J>d^XUb~c~zCXܰC=r|ypӂ@!TP^O{cʂ0u5oKU<fK{ӑ)e}q,#
+rTFؠܲ(
+^Dl?0e(Q>Ũ Ku97d3|lqk`jԖ|rl˦y89W6Y #}݂ߝE_63&;ǪYxD5^Տ5~^˥8q[9rF6'
+2kgp' se`jS>d/mOeSΩMNfЙOrs|+Z̊ea"2f[vRW
+Tzܘ<5z/3ڳ$eY%
+j7M v nD(Д!}W^!|oRfz"HP	enJd9b/{p;bw=CM{ځge?n Ok{6m6k[u3(>YICe}bES 񗱆Is xfanʝ3,^oĎLVsv{ёg>VNry=ֈ+;&k $qЉNYgRS"4ebyu:I<¼F*}̍8\Z{y+ӥQF<]s
+%*/z5>e#*w33NJsn^ޓSnB(|@Ik[(5g>tP
+vVtw2N-e/];1wY')˾ vMj!Dʆd?PlIy kf%23o/Bs3f) rӈ徻#!bv=hLY浶znd! /c[5z+bs>
+<Cy>@ۂ1N9fnNF1*TE6,c	#?;z>a  G}ߝt' t!bC8B򂀊p+ ^Aٗf8:F 7uyLzNʌp*&$-_'+(,L2`oWкn9vԁVO8<`(a,@l
+)O"(P`'3E!NhB<
+DF89@8eI^`B8,9-nS2u9Cn+@On$={dq:=Hݝ|.E&cmf5XP0WYq23O̚-c\un+*Z_CW+.CRf-s({vKXELUΕcU k̗vn~ƁLp0kюm+N<t*T_U<!/w>k<f_Ãd}gň6<Łw
+<HO$fJTov"N!,"= fUx*9CR@a`0".R$R
+g?d|XsxO?߁qPZPS8?P1O'Yzˬb9dq+}U6CZ:ϻDV˯I~/-Ty+ψf
+>E)r~]J5k(짃2?|c$ǎR-VH6Ycq'"U)ʣ2q'].,sx픰oaTu{+v?ݿyxnGQ[Ծ>G֪7^
+
+sB}?>O5{\8v79ooD&_3P_ԻNm]YU;xv2Empr3/w[yud=Y۝L#+PRRI+ABRN@PRbn`brN{"IG{t4!)")>-r
+Д\PJ	jRiEHiW	*%kS$$%u,@Ӈb.fMNedMJ[")S<aīD"DTnNvHK-#-2jH:
+φ1hɬ#hDJF7$DEA'LE0RBNf,#)}aT"IG!R22畠!CY^VD7ʊy޶5zYSS4-XR'4!H5Yf- җdeMlě&Ht)bUZ:5-g]59KckB.fM&,gU$RgMp'~ZQL*?V/`JkJOUQJTU1JSU{ٝ:ƬMٴTŉ&*vv*(R N#(U9|OӘUc>@QՅ^dPw'/ʺ-)%NW %5m3]9ٓ)X"NWL)rir)q<2f$%6}yǆ<Z
+"n3j R2AB'/ThR(RϬh]>)RUG
+52S@	Y-L4;&kz^AbNŧ?~yw+Pw{2~98"8\IwrEN3(;3aʹX8Urf=ȝJy$9:7c+t"پL`x>!liECC7bV p,؝4kо|u|n"ks%aC	"8F7aئ?_ H8rHfWt|C^.NV|=`ޥdyaCMRoG*;xئ(d8>r`Ąg
+8z2fݾk#cB,2n?wb#ZHvy7&&k;_Ww!1dDDd
+`<bSd:DQYQAS׵Tӕmr	$"E[0[ry.ǟP\DG":H3.!",-_`ly3KG ZX}{-~rW|ws}'I\Qe 5QGHQQvG@Q~_$CϓRB 9<So^H@g͓~3OYhLaEF>^_A6V/koam[v0~˩0|>&Q#*2c.}8LdT\@P");iȦ`F	0fA rX*F~zͬu޽vBpb`YMY`wpɮ`r3|3|4qh2
+F!vRǫVR(rsJ*X$^T=諦nH2&%
+$ͥ"!N}5X~j~KKFXnYZ}7,Y$9'!NX(mc46߳w ,1`9<?օ{X1 pg7zYfWs<<Ȇ:XfI,)1-AR-aC*x(A'-?~=
+<+c%ރ!5xJ<1mOIZLn*Rʜ
+T82:^i	w2}f 9֪xTR+[z آ2N4MF=uwiRiXݜDK.M1+4^!\Vɡ'VHi'g{ 	 υw#!.4EK3.mOWI˗P99_D
+($<Z2i!{"I3E)`L (t%DLP7Ъ>8ZɒsIރ+.0
+0~9(s<Rt*.rFLDJ Xֈ8)a&~EU]2BϬ:')d~HO8魯-=aLXy&W#XiGcM
+`ra.BѪ_)D/+G&0֭,ra	s<~0IbGUA(4D28d:蚯X5U]sѨ	^~Klsئp̃F>.@r>d[ϙo`ŅlkGs^1[D*M%vry=}qeJ[աr:,g>gsxFtjlצalgm
+%`8c+T_G;A<!K.c}na'p>%h:-ic$s53xW8"(_Rý2ya+%~vQTP(lOQyCDDl4%ȩmpJ.!-*HdtQ"1/!=%tљHy9?" ^ŊCܴq	)ZT?:738aoiZ"I4q3qJĠccK0<NR$_^(y)fsbқW+Ma# q6qGKakּ{㻯?SƐ\#ko~yTP}d}«(]!*7Ԭ{dsyΧƒk%DD85[c#m^]Ϊ 0;,·kac=@00ȧ06a&~&d8\ccV\6X56BT48bEzƇ;cI1lo`	k/apn:0p5w'(pMw!P#ȗ慗 Oz I_6y>冾d367NO͆iC⼡{o8͎/ۍ?WKuaCTfF˂$zoY8h4}$Ąv8\Q|hN331k}i4ػM/r{4M#wd|-%sHk7+XW#pG.KF/뮙2YL@]e7znPs_+5}aĚc"7N[[c"	LH[bAЊ-h(i효]p0A륌2D#<P{K&ڊ7AbmzVK!A#h3 
+bG^ @pBopG[2~Dk(nwJ2wQPDT*/@ۯ?	W²x 4rI1Yhvv\ipgC~6XI$}J8Tɂ?a<@bŃ57X;x?⠽(VX`ԇ~}8}o/Yl=r[TDȖC[|@.tY,\JWct@#nPb,PV{^iXDIYc|",SGCC!VPi	TK1\BUULv&RTՁDIUGГ#U8<_˩`BoSu@-&19` wǂx*.M8uEG©x jΰm)^R\ buM]<:`i
+x?Xo& }sBu\fJ*%MJbI3A^#.4J9~u(pG38Raš`IG!\AkL"2&F._bKgx¨5xʸPEgq39f55+hhDe)8c'\IJeB/h[CWAgeitX'dOdI0&/ĵ2i&
+^סP*1tFՌrYˎh޲؈D+MH!##_Hb@x,Uov:C¥$^h]8@%]8P΅iP`oA.	4FfFHdY0<$/BBCis(75=mXFB"4ٕA]^x
++47[X,	~"AbyLp>s $:E`ao`F{	g>HnD<̷X`_S-|s9PXSC!MTe' E49ؒXU!CaV$6`PRr,	iI#l	Mg#y,	p=a}w~,vdLZ%	͏8h<p;p:p%s0ãJ,k0sK,cA=K\<2𡨙x<Gޱ:+y&pǕ "2ʸh .3ЌF3;q`f4`$?W	*p{3
+talLh_#;`_K !zI#~Mӣ6WPl~bA|'A4{@хYtUn]Cxm[g%p7@-[p$
+%o'_Z͚#nwI-(k>GDwϻ|[!jaT(|Yp<hvKC}ۻ_~f@[VfV<vOѼp聼p#Y.o w!(ah ޑv#R+KP`#ػ5
+\fUX\~m3}-ZKvp`s4P`wu'j0!ѱ,ڏv9]hh<ȅQ#	hHA	 g`(b0!3>9PXCc2>Դe| x)M|$VPH[cf|x X,T?#襏\G"#&G&	| LhtF8XG&80d?1a]J7*-vWrLZ%G	xIqG<>1,>BQG,>	N4}dGXg`X·x(D:CaROq7# -huHWBNB@+D'9tHob}.Mpϑ@CV"pr<\819N$R㡠~A>Q!"`Hx8` r<$@pK}̀M51	q󺃣>}$Ҵ27HZ?|݈%`l]*B9-
+Em_S9Г-Mee'(2II2I;k$>Ϲ,/Fm$m~fE>'6&{xf4ՆAdG,CЊK3"TcƊUZq(ދ ]x_ Lc:Ϥ{ߝeπ	eV)JuB`UBbd5}`,A1c׉{>+ZZ1~*cXhjbXzN%#?0J/%Jnm64e#|G?cIRd`Y:]rpi=2c"bCi?Bb#O?o< xevntRnT7v$HtxX7LN;qimuټwDj[yFٻKh/7275}ݚx_(W2ĥ6'HrONh	5˙9vg(;iy?nߜSȊoۛȯV}؛fWu[HN	tեa7?_F8US_oى/>FVZnׁ3Ko
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.6 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.6 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.6 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.7 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.6 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -539,15 +539,15 @@
 <dt class="sig sig-object py" id="osxphotos.ExportDBTemp">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ExportDBTemp</span></span><a class="reference internal" href="_modules/osxphotos/export_db.html#ExportDBTemp"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportDBTemp" title="Permalink to this definition">#</a></dt>
 <dd><p>Temporary in-memory version of ExportDB</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ExportOptions">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ExportOptions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">convert_to_jpeg</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description_template</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">download_missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dry_run</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_flags</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">export_as_hardlink</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">export_db</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#osxphotos.ExportDB" title="osxphotos.export_db.ExportDB"><span class="pre">ExportDB</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">face_regions</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fileutil</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#osxphotos.FileUtil" title="osxphotos.fileutil.FileUtil"><span class="pre">FileUtil</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">force_update</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_date_modified</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_signature</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">increment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">jpeg_ext</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">jpeg_quality</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">1.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keyword_template</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">live_photo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">merge_exif_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">merge_exif_persons</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">persons</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">preview_suffix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'_preview'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">preview</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw_photo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">render_options</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">RenderOptions</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rich</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_drop_ext</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">strip</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">timeout</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">120</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">touch_file</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">update</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">update_errors</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_albums_as_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_persons_as_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_photokit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_photos_export</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">verbose</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tmpdir</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">favorite_rating</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportOptions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportOptions" title="Permalink to this definition">#</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ExportOptions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">convert_to_jpeg</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description_template</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">download_missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dry_run</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_flags</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">export_as_hardlink</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">export_db</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#osxphotos.ExportDB" title="osxphotos.export_db.ExportDB"><span class="pre">ExportDB</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">face_regions</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fileutil</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#osxphotos.FileUtil" title="osxphotos.fileutil.FileUtil"><span class="pre">FileUtil</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">force_update</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_date_modified</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_signature</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">increment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">jpeg_ext</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">jpeg_quality</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">1.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keyword_template</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">live_photo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">merge_exif_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">merge_exif_persons</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">persons</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">preview_suffix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'_preview'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">preview</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw_photo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">render_options</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">RenderOptions</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rich</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">export_aae</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_drop_ext</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">strip</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">timeout</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">120</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">touch_file</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">update</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">update_errors</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_albums_as_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_persons_as_keywords</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_photokit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_photos_export</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">verbose</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tmpdir</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">favorite_rating</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportOptions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportOptions" title="Permalink to this definition">#</a></dt>
 <dd><p>Options class for exporting photos with export</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="osxphotos.ExportOptions.convert_to_jpeg">
 <span class="sig-name descname"><span class="pre">convert_to_jpeg</span></span><a class="headerlink" href="#osxphotos.ExportOptions.convert_to_jpeg" title="Permalink to this definition">#</a></dt>
 <dd><p>if True, converts non-jpeg images to jpeg</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type<span class="colon">:</span></dt>
@@ -872,14 +872,25 @@
 <dt class="field-odd">Type<span class="colon">:</span></dt>
 <dd class="field-odd"><p>bool</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="osxphotos.ExportOptions.export_aae">
+<span class="sig-name descname"><span class="pre">export_aae</span></span><a class="headerlink" href="#osxphotos.ExportOptions.export_aae" title="Permalink to this definition">#</a></dt>
+<dd><p>if True, also exports adjustments as .AAE file</p>
+<dl class="field-list simple">
+<dt class="field-odd">Type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>bool</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="osxphotos.ExportOptions.sidecar_drop_ext">
 <span class="sig-name descname"><span class="pre">sidecar_drop_ext</span></span><a class="headerlink" href="#osxphotos.ExportOptions.sidecar_drop_ext" title="Permalink to this definition">#</a></dt>
 <dd><p>if True, drops the photo’s extension from sidecar filename (e.g. ‘IMG_1234.json’ instead of ‘IMG_1234.JPG.json’)</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type<span class="colon">:</span></dt>
 <dd class="field-odd"><p>bool, default=False</p>
 </dd>
@@ -1040,15 +1051,15 @@
 <dd><p>Return bit flags representing options that affect export</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ExportResults">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ExportResults</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">converted_to_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_directories</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_files</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif_updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_warning</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metadata_changed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">new</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_touch</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">touched</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportResults"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportResults" title="Permalink to this definition">#</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ExportResults</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">converted_to_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_directories</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_files</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif_updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_warning</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metadata_changed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">new</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">aae_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_touch</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">touched</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportResults"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportResults" title="Permalink to this definition">#</a></dt>
 <dd><p>Results class which holds export results for export</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.ExportResults.all_files">
 <span class="sig-name descname"><span class="pre">all_files</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportResults.all_files"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportResults.all_files" title="Permalink to this definition">#</a></dt>
 <dd><p>return all filenames contained in results</p>
 </dd></dl>
 
@@ -1606,14 +1617,20 @@
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.adjustments">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">adjustments</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.adjustments" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns AdjustmentsInfo class for adjustment data or None if no adjustments; Photos 5+ only</p>
 </dd></dl>
 
 <dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PhotoInfo.adjustments_path">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">adjustments_path</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.adjustments_path" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns path to adjustments file or none if file doesn’t exist</p>
+</dd></dl>
+
+<dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.album_info">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">album_info</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.album_info" title="Permalink to this definition">#</a></dt>
 <dd><p>list of AlbumInfo objects representing albums the photo is contained in</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.albums">
@@ -2771,14 +2788,20 @@
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PlaceInfo.address_str">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">address_str</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PlaceInfo.address_str" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns the full postal address as a string if defined, otherwise <cite>None</cite>.</p>
 </dd></dl>
 
+<dl class="py method">
+<dt class="sig sig-object py" id="osxphotos.PlaceInfo.asdict">
+<span class="sig-name descname"><span class="pre">asdict</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/placeinfo.html#PlaceInfo.asdict"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PlaceInfo.asdict" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns a dictionary representation of the PlaceInfo object.</p>
+</dd></dl>
+
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PlaceInfo.country_code">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">country_code</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PlaceInfo.country_code" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns the country_code of place, for example “GB”.
 Returns <cite>None</cite> if PhotoInfo contains no country code.</p>
 </dd></dl>
 
@@ -4093,14 +4116,15 @@
 <li><a class="reference internal" href="#osxphotos.ExportOptions.persons"><code class="docutils literal notranslate"><span class="pre">ExportOptions.persons</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.preview_suffix"><code class="docutils literal notranslate"><span class="pre">ExportOptions.preview_suffix</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.preview"><code class="docutils literal notranslate"><span class="pre">ExportOptions.preview</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.raw_photo"><code class="docutils literal notranslate"><span class="pre">ExportOptions.raw_photo</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.render_options"><code class="docutils literal notranslate"><span class="pre">ExportOptions.render_options</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.replace_keywords"><code class="docutils literal notranslate"><span class="pre">ExportOptions.replace_keywords</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.rich"><code class="docutils literal notranslate"><span class="pre">ExportOptions.rich</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.ExportOptions.export_aae"><code class="docutils literal notranslate"><span class="pre">ExportOptions.export_aae</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.sidecar_drop_ext"><code class="docutils literal notranslate"><span class="pre">ExportOptions.sidecar_drop_ext</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.sidecar"><code class="docutils literal notranslate"><span class="pre">ExportOptions.sidecar</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.strip"><code class="docutils literal notranslate"><span class="pre">ExportOptions.strip</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.timeout"><code class="docutils literal notranslate"><span class="pre">ExportOptions.timeout</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.touch_file"><code class="docutils literal notranslate"><span class="pre">ExportOptions.touch_file</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.update"><code class="docutils literal notranslate"><span class="pre">ExportOptions.update</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.ExportOptions.update_errors"><code class="docutils literal notranslate"><span class="pre">ExportOptions.update_errors</span></code></a></li>
@@ -4192,14 +4216,15 @@
 <li><a class="reference internal" href="#osxphotos.PhotoExporter.exiftool_json_sidecar"><code class="docutils literal notranslate"><span class="pre">PhotoExporter.exiftool_json_sidecar()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoExporter.export"><code class="docutils literal notranslate"><span class="pre">PhotoExporter.export()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoExporter.write_exiftool_metadata_to_file"><code class="docutils literal notranslate"><span class="pre">PhotoExporter.write_exiftool_metadata_to_file()</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.adjustments"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.adjustments</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PhotoInfo.adjustments_path"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.adjustments_path</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.album_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.album_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.albums"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.albums</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.asdict"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.asdict()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.burst"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.burst_album_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst_album_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.burst_albums"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst_albums</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.burst_default_pick"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.burst_default_pick</span></code></a></li>
@@ -4343,14 +4368,15 @@
 <li><a class="reference internal" href="#osxphotos.PhotosDB.project_info"><code class="docutils literal notranslate"><span class="pre">PhotosDB.project_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.query"><code class="docutils literal notranslate"><span class="pre">PhotosDB.query()</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo.address"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo.address_str"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.address_str</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PlaceInfo.asdict"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.asdict()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo.country_code"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.country_code</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo.ishome"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.ishome</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo.name"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.name</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo.names"><code class="docutils literal notranslate"><span class="pre">PlaceInfo.names</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a><ul>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -207,20 +207,20 @@
   False, ignore_signature: bool = False, increment: bool = True, jpeg_ext:
   Optional[str] = None, jpeg_quality: float = 1.0, keyword_template: Optional
   [List[str]] = None, live_photo: bool = False, location: bool = True,
   merge_exif_keywords: bool = False, merge_exif_persons: bool = False,
   overwrite: bool = False, persons: bool = True, preview_suffix: str =
   '_preview', preview: bool = False, raw_photo: bool = False, render_options:
   Optional[RenderOptions] = None, replace_keywords: bool = False, rich: bool =
-  False, sidecar_drop_ext: bool = False, sidecar: int = 0, strip: bool = False,
-  timeout: int = 120, touch_file: bool = False, update: bool = False,
-  update_errors: bool = False, use_albums_as_keywords: bool = False,
-  use_persons_as_keywords: bool = False, use_photokit: bool = False,
-  use_photos_export: bool = False, verbose: Optional[Callable] = None, tmpdir:
-  Optional[str] = None, favorite_rating: bool = False)[source]#
+  False, export_aae: bool = False, sidecar_drop_ext: bool = False, sidecar: int
+  = 0, strip: bool = False, timeout: int = 120, touch_file: bool = False,
+  update: bool = False, update_errors: bool = False, use_albums_as_keywords:
+  bool = False, use_persons_as_keywords: bool = False, use_photokit: bool =
+  False, use_photos_export: bool = False, verbose: Optional[Callable] = None,
+  tmpdir: Optional[str] = None, favorite_rating: bool = False)[source]#
       Options class for exporting photos with export
         convert_to_jpeg#
             if True, converts non-jpeg images to jpeg
               Type:
                   bool
         description_template#
             t.Optional template string that will be rendered for use as photo
@@ -356,14 +356,18 @@
             additive
               Type:
                   bool
         rich#
             if True, will use rich markup with verbose output
               Type:
                   bool
+        export_aae#
+            if True, also exports adjustments as .AAE file
+              Type:
+                  bool
         sidecar_drop_ext#
             if True, drops the photoâs extension from sidecar filename (e.g.
             âIMG_1234.jsonâ instead of âIMG_1234.JPG.jsonâ)
               Type:
                   bool, default=False
         sidecar#
             bit field (int): set to one or more
@@ -438,19 +442,19 @@
                   bool
         propertybit_flags#
             Return bit flags representing options that affect export
   classosxphotos.ExportResults(converted_to_jpeg=None,
   deleted_directories=None, deleted_files=None, error=None, exif_updated=None,
   exiftool_error=None, exiftool_warning=None, exported=None,
   exported_album=None, metadata_changed=None, missing=None, missing_album=None,
-  new=None, sidecar_exiftool_skipped=None, sidecar_exiftool_written=None,
-  sidecar_json_skipped=None, sidecar_json_written=None,
-  sidecar_xmp_skipped=None, sidecar_xmp_written=None, skipped=None,
-  skipped_album=None, to_touch=None, touched=None, updated=None,
-  xattr_skipped=None, xattr_written=None)[source]#
+  new=None, aae_written=None, sidecar_exiftool_skipped=None,
+  sidecar_exiftool_written=None, sidecar_json_skipped=None,
+  sidecar_json_written=None, sidecar_xmp_skipped=None,
+  sidecar_xmp_written=None, skipped=None, skipped_album=None, to_touch=None,
+  touched=None, updated=None, xattr_skipped=None, xattr_written=None)[source]#
       Results class which holds export results for export
         all_files() &#x2192; List[str][source]#
             return all filenames contained in results
         propertyattributes: List[str]#
             Return list of attributes tracked by ExportResults
         propertydatetime: str#
             Return datetime when ExportResults was created
@@ -711,14 +715,16 @@
   classosxphotos.PhotoInfo(db: PhotosDB, uuid: str, info: dict[str, Any])
   [source]#
       Info about a specific photo, contains all the details about the photo
       including keywords, persons, albums, uuid, path, etc.
         propertyadjustments#
             Returns AdjustmentsInfo class for adjustment data or None if no
             adjustments; Photos 5+ only
+        propertyadjustments_path#
+            Returns path to adjustments file or none if file doesnât exist
         propertyalbum_info#
             list of AlbumInfo objects representing albums the photo is
             contained in
         propertyalbums#
             list of albums picture is contained in
         asdict(shallow: bool = True) &#x2192; dict[str, Any][source]#
             Return dict representation of PhotoInfo object.
@@ -1322,14 +1328,16 @@
                 * street
                 * sub_administrative_area
                 * sub_locality
                 * iso_country_code
         propertyaddress_str: str | None#
             Returns the full postal address as a string if defined,
             otherwiseNone.
+        asdict()[source]#
+            Returns a dictionary representation of the PlaceInfo object.
         propertycountry_code: str | None#
             Returns the country_code of place, for example âGBâ.
             ReturnsNoneif PhotoInfo contains no country code.
         propertyishome: bool#
             ReturnsTrueif photo place is userâs home address, otherwiseFalse.
         propertyname: str | None#
             Returns the name of the local place as str. This is what Photos
@@ -1927,14 +1935,15 @@
                 # ExportOptions.persons
                 # ExportOptions.preview_suffix
                 # ExportOptions.preview
                 # ExportOptions.raw_photo
                 # ExportOptions.render_options
                 # ExportOptions.replace_keywords
                 # ExportOptions.rich
+                # ExportOptions.export_aae
                 # ExportOptions.sidecar_drop_ext
                 # ExportOptions.sidecar
                 # ExportOptions.strip
                 # ExportOptions.timeout
                 # ExportOptions.touch_file
                 # ExportOptions.update
                 # ExportOptions.update_errors
@@ -2008,14 +2017,15 @@
                 # PersonInfo.sort_order
           o PhotoExporter
                 # PhotoExporter.exiftool_json_sidecar()
                 # PhotoExporter.export()
                 # PhotoExporter.write_exiftool_metadata_to_file()
           o PhotoInfo
                 # PhotoInfo.adjustments
+                # PhotoInfo.adjustments_path
                 # PhotoInfo.album_info
                 # PhotoInfo.albums
                 # PhotoInfo.asdict()
                 # PhotoInfo.burst
                 # PhotoInfo.burst_album_info
                 # PhotoInfo.burst_albums
                 # PhotoInfo.burst_default_pick
@@ -2153,14 +2163,15 @@
                 # PhotosDB.photos_by_uuid()
                 # PhotosDB.photos_version
                 # PhotosDB.project_info
                 # PhotosDB.query()
           o PlaceInfo
                 # PlaceInfo.address
                 # PlaceInfo.address_str
+                # PlaceInfo.asdict()
                 # PlaceInfo.country_code
                 # PlaceInfo.ishome
                 # PlaceInfo.name
                 # PlaceInfo.names
           o ProjectInfo
                 # ProjectInfo.folder_list
                 # ProjectInfo.folder_names
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.6 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.7 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -602,15 +602,15 @@
         "destin": [0, 3, 4],
         "enclos": [0, 5],
         "quot": [0, 5, 6],
         "shell": [0, 2, 3, 5, 6],
         "expand": [0, 4, 5, 6],
         "wildcard": 0,
         "kept": 0,
-        "doesn": [0, 6],
+        "doesn": [0, 4, 6],
         "know": [0, 4],
         "well": [0, 2, 3, 4, 5, 6],
         "larg": [0, 6],
         "post": [0, 1, 3],
         "categori": [0, 6],
         "exif_upd": [0, 4],
         "converted_to_jpeg": [0, 4],
@@ -1319,15 +1319,15 @@
         "long": 4,
         "confidence_threshold": 4,
         "75": [4, 5],
         "confid": [4, 5],
         "threshold": [4, 5],
         "text_detection_confidence_threshold": 4,
         "fall": 4,
-        "back": [4, 5, 6],
+        "back": [0, 4, 5, 6],
         "earlier": 4,
         "exiftoolcach": 4,
         "log": [4, 6],
         "silent": 4,
         "boolean": [4, 5, 6],
         "outsid": 4,
         "pixel": 4,
@@ -1530,15 +1530,15 @@
         "percent": 5,
         "sign": 5,
         "escap": 5,
         "photo_or_video": 5,
         "foto": 5,
         "value_if_tru": 5,
         "value_if_fals": 5,
-        "edited_vers": 5,
+        "edited_vers": [0, 5],
         "03": 5,
         "22": 5,
         "digit": [5, 6],
         "yy": 5,
         "zero": [4, 5],
         "pad": 5,
         "mon": 5,
@@ -2262,15 +2262,21 @@
         "win32": 4,
         "wic": 4,
         "stackexchang": 4,
         "106410": 4,
         "angl": 4,
         "circl": 4,
         "drawn": 4,
-        "coreloc": 4
+        "coreloc": 4,
+        "aae": [0, 4],
+        "succesfulli": 0,
+        "04d": 0,
+        "export_aa": [1, 4],
+        "adjustments_path": [1, 4],
+        "aae_written": 4
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "osxphotos"]
         ],
         "osxphotos": [
             [4, 1, 1, "", "AlbumInfo"],
@@ -2351,14 +2357,15 @@
             [4, 4, 1, "", "convert_to_jpeg"],
             [4, 4, 1, "", "description_template"],
             [4, 4, 1, "", "download_missing"],
             [4, 4, 1, "", "dry_run"],
             [4, 4, 1, "", "edited"],
             [4, 4, 1, "", "exiftool"],
             [4, 4, 1, "", "exiftool_flags"],
+            [4, 4, 1, "", "export_aae"],
             [4, 4, 1, "", "export_as_hardlink"],
             [4, 4, 1, "", "export_db"],
             [4, 4, 1, "", "face_regions"],
             [4, 4, 1, "", "favorite_rating"],
             [4, 4, 1, "", "fileutil"],
             [4, 4, 1, "", "force_update"],
             [4, 4, 1, "", "ignore_date_modified"],
@@ -2461,14 +2468,15 @@
         "osxphotos.PhotoExporter": [
             [4, 2, 1, "", "exiftool_json_sidecar"],
             [4, 2, 1, "", "export"],
             [4, 2, 1, "", "write_exiftool_metadata_to_file"]
         ],
         "osxphotos.PhotoInfo": [
             [4, 3, 1, "", "adjustments"],
+            [4, 3, 1, "", "adjustments_path"],
             [4, 3, 1, "", "album_info"],
             [4, 3, 1, "", "albums"],
             [4, 2, 1, "", "asdict"],
             [4, 3, 1, "", "burst"],
             [4, 3, 1, "", "burst_album_info"],
             [4, 3, 1, "", "burst_albums"],
             [4, 3, 1, "", "burst_default_pick"],
@@ -2607,14 +2615,15 @@
             [4, 3, 1, "", "photos_version"],
             [4, 3, 1, "", "project_info"],
             [4, 2, 1, "", "query"]
         ],
         "osxphotos.PlaceInfo": [
             [4, 3, 1, "", "address"],
             [4, 3, 1, "", "address_str"],
+            [4, 2, 1, "", "asdict"],
             [4, 3, 1, "", "country_code"],
             [4, 3, 1, "", "ishome"],
             [4, 3, 1, "", "name"],
             [4, 3, 1, "", "names"]
         ],
         "osxphotos.ProjectInfo": [
             [4, 3, 1, "", "folder_list"],
@@ -2928,14 +2937,15 @@
             [0, 6, 1, "cmdoption-osxphotos-export-edited-suffix", "--edited-suffix"],
             [0, 6, 1, "cmdoption-osxphotos-export-exif", "--exif"],
             [0, 6, 1, "cmdoption-osxphotos-export-exiftool", "--exiftool"],
             [0, 6, 1, "cmdoption-osxphotos-export-exiftool-merge-keywords", "--exiftool-merge-keywords"],
             [0, 6, 1, "cmdoption-osxphotos-export-exiftool-merge-persons", "--exiftool-merge-persons"],
             [0, 6, 1, "cmdoption-osxphotos-export-exiftool-option", "--exiftool-option"],
             [0, 6, 1, "cmdoption-osxphotos-export-exiftool-path", "--exiftool-path"],
+            [0, 6, 1, "cmdoption-osxphotos-export-export-aae", "--export-aae"],
             [0, 6, 1, "cmdoption-osxphotos-export-export-as-hardlink", "--export-as-hardlink"],
             [0, 6, 1, "cmdoption-osxphotos-export-export-by-date", "--export-by-date"],
             [0, 6, 1, "cmdoption-osxphotos-export-exportdb", "--exportdb"],
             [0, 6, 1, "cmdoption-osxphotos-export-external-edit", "--external-edit"],
             [0, 6, 1, "cmdoption-osxphotos-export-favorite", "--favorite"],
             [0, 6, 1, "cmdoption-osxphotos-export-favorite-rating", "--favorite-rating"],
             [0, 6, 1, "cmdoption-osxphotos-export-filename", "--filename"],
@@ -4143,9 +4153,3347 @@
         "Color Themes": [
             [6, "color-themes"]
         ],
         "Conclusion": [
             [6, "conclusion"]
         ]
     },
-    "indexentries": {}
+    "indexentries": {
+        "--add-exported-to-album": [
+            [0, "cmdoption-osxphotos-export-add-exported-to-album"]
+        ],
+        "--add-missing-to-album": [
+            [0, "cmdoption-osxphotos-export-add-missing-to-album"]
+        ],
+        "--add-skipped-to-album": [
+            [0, "cmdoption-osxphotos-export-add-skipped-to-album"]
+        ],
+        "--add-to-album": [
+            [0, "cmdoption-osxphotos-query-add-to-album"],
+            [0, "cmdoption-osxphotos-timewarp-a"]
+        ],
+        "--added-after": [
+            [0, "cmdoption-osxphotos-add-locations-added-after"],
+            [0, "cmdoption-osxphotos-export-added-after"],
+            [0, "cmdoption-osxphotos-query-added-after"],
+            [0, "cmdoption-osxphotos-repl-added-after"],
+            [0, "cmdoption-osxphotos-sync-added-after"]
+        ],
+        "--added-before": [
+            [0, "cmdoption-osxphotos-add-locations-added-before"],
+            [0, "cmdoption-osxphotos-export-added-before"],
+            [0, "cmdoption-osxphotos-query-added-before"],
+            [0, "cmdoption-osxphotos-repl-added-before"],
+            [0, "cmdoption-osxphotos-sync-added-before"]
+        ],
+        "--added-in-last": [
+            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
+            [0, "cmdoption-osxphotos-export-added-in-last"],
+            [0, "cmdoption-osxphotos-query-added-in-last"],
+            [0, "cmdoption-osxphotos-repl-added-in-last"],
+            [0, "cmdoption-osxphotos-sync-added-in-last"]
+        ],
+        "--album": [
+            [0, "cmdoption-osxphotos-add-locations-album"],
+            [0, "cmdoption-osxphotos-export-album"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-query-album"],
+            [0, "cmdoption-osxphotos-repl-album"],
+            [0, "cmdoption-osxphotos-sync-album"]
+        ],
+        "--album-keyword": [
+            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
+            [0, "cmdoption-osxphotos-export-album-keyword"]
+        ],
+        "--alt-copy": [
+            [0, "cmdoption-osxphotos-export-alt-copy"]
+        ],
+        "--append": [
+            [0, "cmdoption-osxphotos-exiftool-append"],
+            [0, "cmdoption-osxphotos-export-append"],
+            [0, "cmdoption-osxphotos-exportdb-append"],
+            [0, "cmdoption-osxphotos-import-append"],
+            [0, "cmdoption-osxphotos-sync-A"]
+        ],
+        "--burst": [
+            [0, "cmdoption-osxphotos-add-locations-burst"],
+            [0, "cmdoption-osxphotos-export-burst"],
+            [0, "cmdoption-osxphotos-query-burst"],
+            [0, "cmdoption-osxphotos-repl-burst"],
+            [0, "cmdoption-osxphotos-sync-burst"]
+        ],
+        "--check-signatures": [
+            [0, "cmdoption-osxphotos-exportdb-check-signatures"]
+        ],
+        "--check-templates": [
+            [0, "cmdoption-osxphotos-import-check-templates"]
+        ],
+        "--cleanup": [
+            [0, "cmdoption-osxphotos-export-cleanup"]
+        ],
+        "--clear-location": [
+            [0, "cmdoption-osxphotos-import-L"]
+        ],
+        "--clear-metadata": [
+            [0, "cmdoption-osxphotos-import-C"]
+        ],
+        "--clone": [
+            [0, "cmdoption-osxphotos-theme-clone"]
+        ],
+        "--cloudasset": [
+            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
+            [0, "cmdoption-osxphotos-export-cloudasset"],
+            [0, "cmdoption-osxphotos-query-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-cloudasset"]
+        ],
+        "--compare-exif": [
+            [0, "cmdoption-osxphotos-timewarp-c"]
+        ],
+        "--config": [
+            [0, "cmdoption-osxphotos-theme-config"]
+        ],
+        "--config-only": [
+            [0, "cmdoption-osxphotos-export-config-only"]
+        ],
+        "--convert-to-jpeg": [
+            [0, "cmdoption-osxphotos-export-convert-to-jpeg"]
+        ],
+        "--count": [
+            [0, "cmdoption-osxphotos-query-count"]
+        ],
+        "--current-name": [
+            [0, "cmdoption-osxphotos-export-current-name"]
+        ],
+        "--date": [
+            [0, "cmdoption-osxphotos-timewarp-d"]
+        ],
+        "--date-added": [
+            [0, "cmdoption-osxphotos-timewarp-date-added"]
+        ],
+        "--date-added-from-photo": [
+            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"]
+        ],
+        "--date-delta": [
+            [0, "cmdoption-osxphotos-timewarp-D"]
+        ],
+        "--db": [
+            [0, "cmdoption-osxphotos-albums-library"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-info-library"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-keywords-library"],
+            [0, "cmdoption-osxphotos-labels-library"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-persons-library"],
+            [0, "cmdoption-osxphotos-places-library"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-show-library"],
+            [0, "cmdoption-osxphotos-snap-library"],
+            [0, "cmdoption-osxphotos-sync-library"]
+        ],
+        "--db-config": [
+            [0, "cmdoption-osxphotos-exiftool-db-config"]
+        ],
+        "--default": [
+            [0, "cmdoption-osxphotos-theme-default"]
+        ],
+        "--delete": [
+            [0, "cmdoption-osxphotos-theme-delete"]
+        ],
+        "--delete-file": [
+            [0, "cmdoption-osxphotos-exportdb-delete-file"]
+        ],
+        "--delete-uuid": [
+            [0, "cmdoption-osxphotos-exportdb-delete-uuid"]
+        ],
+        "--deleted": [
+            [0, "cmdoption-osxphotos-dump-deleted"],
+            [0, "cmdoption-osxphotos-export-deleted"],
+            [0, "cmdoption-osxphotos-query-deleted"],
+            [0, "cmdoption-osxphotos-repl-deleted"]
+        ],
+        "--deleted-only": [
+            [0, "cmdoption-osxphotos-dump-deleted-only"],
+            [0, "cmdoption-osxphotos-export-deleted-only"],
+            [0, "cmdoption-osxphotos-query-deleted-only"],
+            [0, "cmdoption-osxphotos-repl-deleted-only"]
+        ],
+        "--description": [
+            [0, "cmdoption-osxphotos-add-locations-description"],
+            [0, "cmdoption-osxphotos-batch-edit-description"],
+            [0, "cmdoption-osxphotos-export-description"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-query-description"],
+            [0, "cmdoption-osxphotos-repl-description"],
+            [0, "cmdoption-osxphotos-sync-description"]
+        ],
+        "--description-template": [
+            [0, "cmdoption-osxphotos-exiftool-description-template"],
+            [0, "cmdoption-osxphotos-export-description-template"]
+        ],
+        "--detect-text": [
+            [0, "cmdoption-osxphotos-inspect-t"]
+        ],
+        "--directory": [
+            [0, "cmdoption-osxphotos-export-directory"]
+        ],
+        "--download-missing": [
+            [0, "cmdoption-osxphotos-export-download-missing"]
+        ],
+        "--dry-run": [
+            [0, "cmdoption-osxphotos-add-locations-dry-run"],
+            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
+            [0, "cmdoption-osxphotos-exiftool-dry-run"],
+            [0, "cmdoption-osxphotos-export-dry-run"],
+            [0, "cmdoption-osxphotos-exportdb-dry-run"],
+            [0, "cmdoption-osxphotos-sync-dry-run"]
+        ],
+        "--dup-check": [
+            [0, "cmdoption-osxphotos-import-D"]
+        ],
+        "--duplicate": [
+            [0, "cmdoption-osxphotos-add-locations-duplicate"],
+            [0, "cmdoption-osxphotos-export-duplicate"],
+            [0, "cmdoption-osxphotos-query-duplicate"],
+            [0, "cmdoption-osxphotos-repl-duplicate"],
+            [0, "cmdoption-osxphotos-sync-duplicate"]
+        ],
+        "--edit": [
+            [0, "cmdoption-osxphotos-theme-edit"]
+        ],
+        "--edited": [
+            [0, "cmdoption-osxphotos-add-locations-edited"],
+            [0, "cmdoption-osxphotos-export-edited"],
+            [0, "cmdoption-osxphotos-query-edited"],
+            [0, "cmdoption-osxphotos-repl-edited"],
+            [0, "cmdoption-osxphotos-sync-edited"]
+        ],
+        "--edited-suffix": [
+            [0, "cmdoption-osxphotos-export-edited-suffix"]
+        ],
+        "--emacs": [
+            [0, "cmdoption-osxphotos-repl-emacs"]
+        ],
+        "--errors": [
+            [0, "cmdoption-osxphotos-exportdb-errors"]
+        ],
+        "--exif": [
+            [0, "cmdoption-osxphotos-add-locations-exif"],
+            [0, "cmdoption-osxphotos-export-exif"],
+            [0, "cmdoption-osxphotos-query-exif"],
+            [0, "cmdoption-osxphotos-repl-exif"],
+            [0, "cmdoption-osxphotos-sync-exif"]
+        ],
+        "--exiftool": [
+            [0, "cmdoption-osxphotos-export-exiftool"],
+            [0, "cmdoption-osxphotos-import-e"]
+        ],
+        "--exiftool-merge-keywords": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"]
+        ],
+        "--exiftool-merge-persons": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"]
+        ],
+        "--exiftool-option": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
+            [0, "cmdoption-osxphotos-export-exiftool-option"]
+        ],
+        "--exiftool-path": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
+            [0, "cmdoption-osxphotos-export-exiftool-path"],
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-timewarp-e"]
+        ],
+        "--export": [
+            [0, "cmdoption-osxphotos-orphans-export"],
+            [0, "cmdoption-osxphotos-sync-e"]
+        ],
+        "--export-aae": [
+            [0, "cmdoption-osxphotos-export-export-aae"]
+        ],
+        "--export-as-hardlink": [
+            [0, "cmdoption-osxphotos-export-export-as-hardlink"]
+        ],
+        "--export-by-date": [
+            [0, "cmdoption-osxphotos-export-export-by-date"]
+        ],
+        "--export-dir": [
+            [0, "cmdoption-osxphotos-exportdb-export-dir"]
+        ],
+        "--exportdb": [
+            [0, "cmdoption-osxphotos-exiftool-exportdb"],
+            [0, "cmdoption-osxphotos-export-exportdb"]
+        ],
+        "--external-edit": [
+            [0, "cmdoption-osxphotos-add-locations-external-edit"],
+            [0, "cmdoption-osxphotos-export-external-edit"],
+            [0, "cmdoption-osxphotos-query-external-edit"],
+            [0, "cmdoption-osxphotos-repl-external-edit"],
+            [0, "cmdoption-osxphotos-sync-external-edit"]
+        ],
+        "--favorite": [
+            [0, "cmdoption-osxphotos-add-locations-favorite"],
+            [0, "cmdoption-osxphotos-export-favorite"],
+            [0, "cmdoption-osxphotos-query-favorite"],
+            [0, "cmdoption-osxphotos-repl-favorite"],
+            [0, "cmdoption-osxphotos-sync-favorite"]
+        ],
+        "--favorite-rating": [
+            [0, "cmdoption-osxphotos-export-favorite-rating"]
+        ],
+        "--field": [
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-query-f"]
+        ],
+        "--filename": [
+            [0, "cmdoption-osxphotos-export-filename"],
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "--finder-tag-keywords": [
+            [0, "cmdoption-osxphotos-export-finder-tag-keywords"]
+        ],
+        "--finder-tag-template": [
+            [0, "cmdoption-osxphotos-export-finder-tag-template"]
+        ],
+        "--folder": [
+            [0, "cmdoption-osxphotos-add-locations-folder"],
+            [0, "cmdoption-osxphotos-export-folder"],
+            [0, "cmdoption-osxphotos-query-folder"],
+            [0, "cmdoption-osxphotos-repl-folder"],
+            [0, "cmdoption-osxphotos-sync-folder"]
+        ],
+        "--force": [
+            [0, "cmdoption-osxphotos-timewarp-force"]
+        ],
+        "--force-update": [
+            [0, "cmdoption-osxphotos-export-force-update"]
+        ],
+        "--from-date": [
+            [0, "cmdoption-osxphotos-add-locations-from-date"],
+            [0, "cmdoption-osxphotos-export-from-date"],
+            [0, "cmdoption-osxphotos-query-from-date"],
+            [0, "cmdoption-osxphotos-repl-from-date"],
+            [0, "cmdoption-osxphotos-sync-from-date"]
+        ],
+        "--from-time": [
+            [0, "cmdoption-osxphotos-add-locations-from-time"],
+            [0, "cmdoption-osxphotos-export-from-time"],
+            [0, "cmdoption-osxphotos-query-from-time"],
+            [0, "cmdoption-osxphotos-repl-from-time"],
+            [0, "cmdoption-osxphotos-sync-from-time"]
+        ],
+        "--function": [
+            [0, "cmdoption-osxphotos-timewarp-F"]
+        ],
+        "--glob": [
+            [0, "cmdoption-osxphotos-import-g"]
+        ],
+        "--has-comment": [
+            [0, "cmdoption-osxphotos-add-locations-has-comment"],
+            [0, "cmdoption-osxphotos-export-has-comment"],
+            [0, "cmdoption-osxphotos-query-has-comment"],
+            [0, "cmdoption-osxphotos-repl-has-comment"],
+            [0, "cmdoption-osxphotos-sync-has-comment"]
+        ],
+        "--has-likes": [
+            [0, "cmdoption-osxphotos-add-locations-has-likes"],
+            [0, "cmdoption-osxphotos-export-has-likes"],
+            [0, "cmdoption-osxphotos-query-has-likes"],
+            [0, "cmdoption-osxphotos-repl-has-likes"],
+            [0, "cmdoption-osxphotos-sync-has-likes"]
+        ],
+        "--has-raw": [
+            [0, "cmdoption-osxphotos-add-locations-has-raw"],
+            [0, "cmdoption-osxphotos-export-has-raw"],
+            [0, "cmdoption-osxphotos-query-has-raw"],
+            [0, "cmdoption-osxphotos-repl-has-raw"],
+            [0, "cmdoption-osxphotos-sync-has-raw"]
+        ],
+        "--hdr": [
+            [0, "cmdoption-osxphotos-add-locations-hdr"],
+            [0, "cmdoption-osxphotos-export-hdr"],
+            [0, "cmdoption-osxphotos-query-hdr"],
+            [0, "cmdoption-osxphotos-repl-hdr"],
+            [0, "cmdoption-osxphotos-sync-hdr"]
+        ],
+        "--help": [
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "--hidden": [
+            [0, "cmdoption-osxphotos-add-locations-hidden"],
+            [0, "cmdoption-osxphotos-export-hidden"],
+            [0, "cmdoption-osxphotos-query-hidden"],
+            [0, "cmdoption-osxphotos-repl-hidden"],
+            [0, "cmdoption-osxphotos-sync-hidden"]
+        ],
+        "--ignore-case": [
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-sync-0"]
+        ],
+        "--ignore-date-modified": [
+            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-export-ignore-date-modified"]
+        ],
+        "--ignore-signature": [
+            [0, "cmdoption-osxphotos-export-ignore-signature"]
+        ],
+        "--import": [
+            [0, "cmdoption-osxphotos-sync-i"]
+        ],
+        "--in-album": [
+            [0, "cmdoption-osxphotos-add-locations-in-album"],
+            [0, "cmdoption-osxphotos-export-in-album"],
+            [0, "cmdoption-osxphotos-query-in-album"],
+            [0, "cmdoption-osxphotos-repl-in-album"],
+            [0, "cmdoption-osxphotos-sync-in-album"]
+        ],
+        "--incloud": [
+            [0, "cmdoption-osxphotos-add-locations-incloud"],
+            [0, "cmdoption-osxphotos-export-incloud"],
+            [0, "cmdoption-osxphotos-query-incloud"],
+            [0, "cmdoption-osxphotos-repl-incloud"],
+            [0, "cmdoption-osxphotos-sync-incloud"]
+        ],
+        "--info": [
+            [0, "cmdoption-osxphotos-exportdb-info"]
+        ],
+        "--inspect": [
+            [0, "cmdoption-osxphotos-timewarp-i"]
+        ],
+        "--is-reference": [
+            [0, "cmdoption-osxphotos-add-locations-is-reference"],
+            [0, "cmdoption-osxphotos-export-is-reference"],
+            [0, "cmdoption-osxphotos-query-is-reference"],
+            [0, "cmdoption-osxphotos-repl-is-reference"],
+            [0, "cmdoption-osxphotos-sync-is-reference"]
+        ],
+        "--jpeg-ext": [
+            [0, "cmdoption-osxphotos-export-jpeg-ext"]
+        ],
+        "--jpeg-quality": [
+            [0, "cmdoption-osxphotos-export-jpeg-quality"]
+        ],
+        "--json": [
+            [0, "cmdoption-osxphotos-albums-json"],
+            [0, "cmdoption-osxphotos-dump-json"],
+            [0, "cmdoption-osxphotos-info-json"],
+            [0, "cmdoption-osxphotos-keywords-json"],
+            [0, "cmdoption-osxphotos-labels-json"],
+            [0, "cmdoption-osxphotos-list-json"],
+            [0, "cmdoption-osxphotos-persons-json"],
+            [0, "cmdoption-osxphotos-places-json"],
+            [0, "cmdoption-osxphotos-query-json"]
+        ],
+        "--keep": [
+            [0, "cmdoption-osxphotos-export-keep"]
+        ],
+        "--keyword": [
+            [0, "cmdoption-osxphotos-add-locations-keyword"],
+            [0, "cmdoption-osxphotos-batch-edit-keyword"],
+            [0, "cmdoption-osxphotos-export-keyword"],
+            [0, "cmdoption-osxphotos-import-k"],
+            [0, "cmdoption-osxphotos-query-keyword"],
+            [0, "cmdoption-osxphotos-repl-keyword"],
+            [0, "cmdoption-osxphotos-sync-keyword"]
+        ],
+        "--keyword-template": [
+            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
+            [0, "cmdoption-osxphotos-export-keyword-template"]
+        ],
+        "--label": [
+            [0, "cmdoption-osxphotos-add-locations-label"],
+            [0, "cmdoption-osxphotos-export-label"],
+            [0, "cmdoption-osxphotos-query-label"],
+            [0, "cmdoption-osxphotos-repl-label"],
+            [0, "cmdoption-osxphotos-sync-label"]
+        ],
+        "--last-errors": [
+            [0, "cmdoption-osxphotos-exportdb-last-errors"]
+        ],
+        "--last-run": [
+            [0, "cmdoption-osxphotos-exportdb-last-run"]
+        ],
+        "--library": [
+            [0, "cmdoption-osxphotos-albums-library"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-info-library"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-keywords-library"],
+            [0, "cmdoption-osxphotos-labels-library"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-persons-library"],
+            [0, "cmdoption-osxphotos-places-library"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-show-library"],
+            [0, "cmdoption-osxphotos-snap-library"],
+            [0, "cmdoption-osxphotos-sync-library"],
+            [0, "cmdoption-osxphotos-timewarp-L"]
+        ],
+        "--limit": [
+            [0, "cmdoption-osxphotos-export-limit"]
+        ],
+        "--list": [
+            [0, "cmdoption-osxphotos-theme-list"]
+        ],
+        "--live": [
+            [0, "cmdoption-osxphotos-add-locations-live"],
+            [0, "cmdoption-osxphotos-export-live"],
+            [0, "cmdoption-osxphotos-query-live"],
+            [0, "cmdoption-osxphotos-repl-live"],
+            [0, "cmdoption-osxphotos-sync-live"]
+        ],
+        "--load-config": [
+            [0, "cmdoption-osxphotos-exiftool-load-config"],
+            [0, "cmdoption-osxphotos-export-load-config"]
+        ],
+        "--location": [
+            [0, "cmdoption-osxphotos-add-locations-location"],
+            [0, "cmdoption-osxphotos-batch-edit-location"],
+            [0, "cmdoption-osxphotos-export-location"],
+            [0, "cmdoption-osxphotos-import-l"],
+            [0, "cmdoption-osxphotos-query-location"],
+            [0, "cmdoption-osxphotos-repl-location"],
+            [0, "cmdoption-osxphotos-sync-location"]
+        ],
+        "--match-time": [
+            [0, "cmdoption-osxphotos-timewarp-0"]
+        ],
+        "--max-size": [
+            [0, "cmdoption-osxphotos-add-locations-max-size"],
+            [0, "cmdoption-osxphotos-export-max-size"],
+            [0, "cmdoption-osxphotos-query-max-size"],
+            [0, "cmdoption-osxphotos-repl-max-size"],
+            [0, "cmdoption-osxphotos-sync-max-size"]
+        ],
+        "--merge": [
+            [0, "cmdoption-osxphotos-sync-m"]
+        ],
+        "--merge-keywords": [
+            [0, "cmdoption-osxphotos-import-m"]
+        ],
+        "--migrate": [
+            [0, "cmdoption-osxphotos-exportdb-migrate"]
+        ],
+        "--migrate-photos-library": [
+            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"]
+        ],
+        "--min-size": [
+            [0, "cmdoption-osxphotos-add-locations-min-size"],
+            [0, "cmdoption-osxphotos-export-min-size"],
+            [0, "cmdoption-osxphotos-query-min-size"],
+            [0, "cmdoption-osxphotos-repl-min-size"],
+            [0, "cmdoption-osxphotos-sync-min-size"]
+        ],
+        "--missing": [
+            [0, "cmdoption-osxphotos-add-locations-missing"],
+            [0, "cmdoption-osxphotos-export-missing"],
+            [0, "cmdoption-osxphotos-query-missing"],
+            [0, "cmdoption-osxphotos-repl-missing"],
+            [0, "cmdoption-osxphotos-sync-missing"]
+        ],
+        "--name": [
+            [0, "cmdoption-osxphotos-add-locations-name"],
+            [0, "cmdoption-osxphotos-export-name"],
+            [0, "cmdoption-osxphotos-query-name"],
+            [0, "cmdoption-osxphotos-repl-name"],
+            [0, "cmdoption-osxphotos-sync-name"]
+        ],
+        "--no-comment": [
+            [0, "cmdoption-osxphotos-add-locations-no-comment"],
+            [0, "cmdoption-osxphotos-export-no-comment"],
+            [0, "cmdoption-osxphotos-query-no-comment"],
+            [0, "cmdoption-osxphotos-repl-no-comment"],
+            [0, "cmdoption-osxphotos-sync-no-comment"]
+        ],
+        "--no-description": [
+            [0, "cmdoption-osxphotos-add-locations-no-description"],
+            [0, "cmdoption-osxphotos-export-no-description"],
+            [0, "cmdoption-osxphotos-query-no-description"],
+            [0, "cmdoption-osxphotos-repl-no-description"],
+            [0, "cmdoption-osxphotos-sync-no-description"]
+        ],
+        "--no-keyword": [
+            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
+            [0, "cmdoption-osxphotos-export-no-keyword"],
+            [0, "cmdoption-osxphotos-query-no-keyword"],
+            [0, "cmdoption-osxphotos-repl-no-keyword"],
+            [0, "cmdoption-osxphotos-sync-no-keyword"]
+        ],
+        "--no-likes": [
+            [0, "cmdoption-osxphotos-add-locations-no-likes"],
+            [0, "cmdoption-osxphotos-export-no-likes"],
+            [0, "cmdoption-osxphotos-query-no-likes"],
+            [0, "cmdoption-osxphotos-repl-no-likes"],
+            [0, "cmdoption-osxphotos-sync-no-likes"]
+        ],
+        "--no-location": [
+            [0, "cmdoption-osxphotos-add-locations-no-location"],
+            [0, "cmdoption-osxphotos-export-no-location"],
+            [0, "cmdoption-osxphotos-query-no-location"],
+            [0, "cmdoption-osxphotos-repl-no-location"],
+            [0, "cmdoption-osxphotos-sync-no-location"]
+        ],
+        "--no-place": [
+            [0, "cmdoption-osxphotos-add-locations-no-place"],
+            [0, "cmdoption-osxphotos-export-no-place"],
+            [0, "cmdoption-osxphotos-query-no-place"],
+            [0, "cmdoption-osxphotos-repl-no-place"],
+            [0, "cmdoption-osxphotos-sync-no-place"]
+        ],
+        "--no-progress": [
+            [0, "cmdoption-osxphotos-export-no-progress"],
+            [0, "cmdoption-osxphotos-import-no-progress"]
+        ],
+        "--no-title": [
+            [0, "cmdoption-osxphotos-add-locations-no-title"],
+            [0, "cmdoption-osxphotos-export-no-title"],
+            [0, "cmdoption-osxphotos-query-no-title"],
+            [0, "cmdoption-osxphotos-repl-no-title"],
+            [0, "cmdoption-osxphotos-sync-no-title"]
+        ],
+        "--not-burst": [
+            [0, "cmdoption-osxphotos-add-locations-not-burst"],
+            [0, "cmdoption-osxphotos-export-not-burst"],
+            [0, "cmdoption-osxphotos-query-not-burst"],
+            [0, "cmdoption-osxphotos-repl-not-burst"],
+            [0, "cmdoption-osxphotos-sync-not-burst"]
+        ],
+        "--not-cloudasset": [
+            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
+            [0, "cmdoption-osxphotos-export-not-cloudasset"],
+            [0, "cmdoption-osxphotos-query-not-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-not-cloudasset"]
+        ],
+        "--not-edited": [
+            [0, "cmdoption-osxphotos-add-locations-not-edited"],
+            [0, "cmdoption-osxphotos-export-not-edited"],
+            [0, "cmdoption-osxphotos-query-not-edited"],
+            [0, "cmdoption-osxphotos-repl-not-edited"],
+            [0, "cmdoption-osxphotos-sync-not-edited"]
+        ],
+        "--not-favorite": [
+            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
+            [0, "cmdoption-osxphotos-export-not-favorite"],
+            [0, "cmdoption-osxphotos-query-not-favorite"],
+            [0, "cmdoption-osxphotos-repl-not-favorite"],
+            [0, "cmdoption-osxphotos-sync-not-favorite"]
+        ],
+        "--not-hdr": [
+            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
+            [0, "cmdoption-osxphotos-export-not-hdr"],
+            [0, "cmdoption-osxphotos-query-not-hdr"],
+            [0, "cmdoption-osxphotos-repl-not-hdr"],
+            [0, "cmdoption-osxphotos-sync-not-hdr"]
+        ],
+        "--not-hidden": [
+            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
+            [0, "cmdoption-osxphotos-export-not-hidden"],
+            [0, "cmdoption-osxphotos-query-not-hidden"],
+            [0, "cmdoption-osxphotos-repl-not-hidden"],
+            [0, "cmdoption-osxphotos-sync-not-hidden"]
+        ],
+        "--not-in-album": [
+            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
+            [0, "cmdoption-osxphotos-export-not-in-album"],
+            [0, "cmdoption-osxphotos-query-not-in-album"],
+            [0, "cmdoption-osxphotos-repl-not-in-album"],
+            [0, "cmdoption-osxphotos-sync-not-in-album"]
+        ],
+        "--not-incloud": [
+            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
+            [0, "cmdoption-osxphotos-export-not-incloud"],
+            [0, "cmdoption-osxphotos-query-not-incloud"],
+            [0, "cmdoption-osxphotos-repl-not-incloud"],
+            [0, "cmdoption-osxphotos-sync-not-incloud"]
+        ],
+        "--not-live": [
+            [0, "cmdoption-osxphotos-add-locations-not-live"],
+            [0, "cmdoption-osxphotos-export-not-live"],
+            [0, "cmdoption-osxphotos-query-not-live"],
+            [0, "cmdoption-osxphotos-repl-not-live"],
+            [0, "cmdoption-osxphotos-sync-not-live"]
+        ],
+        "--not-missing": [
+            [0, "cmdoption-osxphotos-add-locations-not-missing"],
+            [0, "cmdoption-osxphotos-export-not-missing"],
+            [0, "cmdoption-osxphotos-query-not-missing"],
+            [0, "cmdoption-osxphotos-repl-not-missing"],
+            [0, "cmdoption-osxphotos-sync-not-missing"]
+        ],
+        "--not-panorama": [
+            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
+            [0, "cmdoption-osxphotos-export-not-panorama"],
+            [0, "cmdoption-osxphotos-query-not-panorama"],
+            [0, "cmdoption-osxphotos-repl-not-panorama"],
+            [0, "cmdoption-osxphotos-sync-not-panorama"]
+        ],
+        "--not-portrait": [
+            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
+            [0, "cmdoption-osxphotos-export-not-portrait"],
+            [0, "cmdoption-osxphotos-query-not-portrait"],
+            [0, "cmdoption-osxphotos-repl-not-portrait"],
+            [0, "cmdoption-osxphotos-sync-not-portrait"]
+        ],
+        "--not-reference": [
+            [0, "cmdoption-osxphotos-add-locations-not-reference"],
+            [0, "cmdoption-osxphotos-export-not-reference"],
+            [0, "cmdoption-osxphotos-query-not-reference"],
+            [0, "cmdoption-osxphotos-repl-not-reference"],
+            [0, "cmdoption-osxphotos-sync-not-reference"]
+        ],
+        "--not-saved-to-library": [
+            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-not-saved-to-library"]
+        ],
+        "--not-screenshot": [
+            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
+            [0, "cmdoption-osxphotos-export-not-screenshot"],
+            [0, "cmdoption-osxphotos-query-not-screenshot"],
+            [0, "cmdoption-osxphotos-repl-not-screenshot"],
+            [0, "cmdoption-osxphotos-sync-not-screenshot"]
+        ],
+        "--not-selfie": [
+            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
+            [0, "cmdoption-osxphotos-export-not-selfie"],
+            [0, "cmdoption-osxphotos-query-not-selfie"],
+            [0, "cmdoption-osxphotos-repl-not-selfie"],
+            [0, "cmdoption-osxphotos-sync-not-selfie"]
+        ],
+        "--not-shared": [
+            [0, "cmdoption-osxphotos-add-locations-not-shared"],
+            [0, "cmdoption-osxphotos-export-not-shared"],
+            [0, "cmdoption-osxphotos-query-not-shared"],
+            [0, "cmdoption-osxphotos-repl-not-shared"]
+        ],
+        "--not-slow-mo": [
+            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
+            [0, "cmdoption-osxphotos-export-not-slow-mo"],
+            [0, "cmdoption-osxphotos-query-not-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-not-slow-mo"]
+        ],
+        "--not-syndicated": [
+            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
+            [0, "cmdoption-osxphotos-export-not-syndicated"],
+            [0, "cmdoption-osxphotos-query-not-syndicated"],
+            [0, "cmdoption-osxphotos-repl-not-syndicated"],
+            [0, "cmdoption-osxphotos-sync-not-syndicated"]
+        ],
+        "--not-time-lapse": [
+            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
+            [0, "cmdoption-osxphotos-export-not-time-lapse"],
+            [0, "cmdoption-osxphotos-query-not-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-not-time-lapse"]
+        ],
+        "--only-movies": [
+            [0, "cmdoption-osxphotos-add-locations-only-movies"],
+            [0, "cmdoption-osxphotos-export-only-movies"],
+            [0, "cmdoption-osxphotos-query-only-movies"],
+            [0, "cmdoption-osxphotos-repl-only-movies"],
+            [0, "cmdoption-osxphotos-sync-only-movies"]
+        ],
+        "--only-new": [
+            [0, "cmdoption-osxphotos-export-only-new"]
+        ],
+        "--only-photos": [
+            [0, "cmdoption-osxphotos-add-locations-only-photos"],
+            [0, "cmdoption-osxphotos-export-only-photos"],
+            [0, "cmdoption-osxphotos-query-only-photos"],
+            [0, "cmdoption-osxphotos-repl-only-photos"],
+            [0, "cmdoption-osxphotos-sync-only-photos"]
+        ],
+        "--original-suffix": [
+            [0, "cmdoption-osxphotos-export-original-suffix"]
+        ],
+        "--overwrite": [
+            [0, "cmdoption-osxphotos-export-overwrite"]
+        ],
+        "--panorama": [
+            [0, "cmdoption-osxphotos-add-locations-panorama"],
+            [0, "cmdoption-osxphotos-export-panorama"],
+            [0, "cmdoption-osxphotos-query-panorama"],
+            [0, "cmdoption-osxphotos-repl-panorama"],
+            [0, "cmdoption-osxphotos-sync-panorama"]
+        ],
+        "--parse-date": [
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-timewarp-M"]
+        ],
+        "--person": [
+            [0, "cmdoption-osxphotos-add-locations-person"],
+            [0, "cmdoption-osxphotos-export-person"],
+            [0, "cmdoption-osxphotos-query-person"],
+            [0, "cmdoption-osxphotos-repl-person"],
+            [0, "cmdoption-osxphotos-sync-person"]
+        ],
+        "--person-keyword": [
+            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
+            [0, "cmdoption-osxphotos-export-person-keyword"]
+        ],
+        "--place": [
+            [0, "cmdoption-osxphotos-add-locations-place"],
+            [0, "cmdoption-osxphotos-export-place"],
+            [0, "cmdoption-osxphotos-query-place"],
+            [0, "cmdoption-osxphotos-repl-place"],
+            [0, "cmdoption-osxphotos-sync-place"]
+        ],
+        "--plain": [
+            [0, "cmdoption-osxphotos-timewarp-plain"]
+        ],
+        "--portrait": [
+            [0, "cmdoption-osxphotos-add-locations-portrait"],
+            [0, "cmdoption-osxphotos-export-portrait"],
+            [0, "cmdoption-osxphotos-query-portrait"],
+            [0, "cmdoption-osxphotos-repl-portrait"],
+            [0, "cmdoption-osxphotos-sync-portrait"]
+        ],
+        "--post-command": [
+            [0, "cmdoption-osxphotos-export-post-command"]
+        ],
+        "--post-function": [
+            [0, "cmdoption-osxphotos-export-post-function"],
+            [0, "cmdoption-osxphotos-import-post-function"]
+        ],
+        "--preview": [
+            [0, "cmdoption-osxphotos-export-preview"],
+            [0, "cmdoption-osxphotos-theme-preview"]
+        ],
+        "--preview-if-missing": [
+            [0, "cmdoption-osxphotos-export-preview-if-missing"]
+        ],
+        "--preview-suffix": [
+            [0, "cmdoption-osxphotos-export-preview-suffix"]
+        ],
+        "--print": [
+            [0, "cmdoption-osxphotos-dump-print"],
+            [0, "cmdoption-osxphotos-export-print"],
+            [0, "cmdoption-osxphotos-query-print"]
+        ],
+        "--pull-exif": [
+            [0, "cmdoption-osxphotos-timewarp-P"]
+        ],
+        "--push-exif": [
+            [0, "cmdoption-osxphotos-timewarp-p"]
+        ],
+        "--query-eval": [
+            [0, "cmdoption-osxphotos-add-locations-query-eval"],
+            [0, "cmdoption-osxphotos-export-query-eval"],
+            [0, "cmdoption-osxphotos-query-query-eval"],
+            [0, "cmdoption-osxphotos-repl-query-eval"],
+            [0, "cmdoption-osxphotos-sync-query-eval"]
+        ],
+        "--query-function": [
+            [0, "cmdoption-osxphotos-add-locations-query-function"],
+            [0, "cmdoption-osxphotos-export-query-function"],
+            [0, "cmdoption-osxphotos-query-query-function"],
+            [0, "cmdoption-osxphotos-repl-query-function"],
+            [0, "cmdoption-osxphotos-sync-query-function"]
+        ],
+        "--quiet": [
+            [0, "cmdoption-osxphotos-query-quiet"]
+        ],
+        "--ramdb": [
+            [0, "cmdoption-osxphotos-export-ramdb"]
+        ],
+        "--raw-output": [
+            [0, "cmdoption-osxphotos-diff-r"]
+        ],
+        "--regex": [
+            [0, "cmdoption-osxphotos-add-locations-regex"],
+            [0, "cmdoption-osxphotos-export-regex"],
+            [0, "cmdoption-osxphotos-query-regex"],
+            [0, "cmdoption-osxphotos-repl-regex"],
+            [0, "cmdoption-osxphotos-sync-regex"]
+        ],
+        "--relative-to": [
+            [0, "cmdoption-osxphotos-import-r"]
+        ],
+        "--replace-keywords": [
+            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
+            [0, "cmdoption-osxphotos-export-replace-keywords"]
+        ],
+        "--report": [
+            [0, "cmdoption-osxphotos-exiftool-report"],
+            [0, "cmdoption-osxphotos-export-report"],
+            [0, "cmdoption-osxphotos-exportdb-report"],
+            [0, "cmdoption-osxphotos-import-report"],
+            [0, "cmdoption-osxphotos-sync-R"]
+        ],
+        "--resume": [
+            [0, "cmdoption-osxphotos-import-R"]
+        ],
+        "--retry": [
+            [0, "cmdoption-osxphotos-export-retry"]
+        ],
+        "--run": [
+            [0, "cmdoption-osxphotos-version-run"]
+        ],
+        "--save-config": [
+            [0, "cmdoption-osxphotos-exiftool-save-config"],
+            [0, "cmdoption-osxphotos-export-save-config"],
+            [0, "cmdoption-osxphotos-exportdb-save-config"]
+        ],
+        "--saved-to-library": [
+            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-saved-to-library"]
+        ],
+        "--screenshot": [
+            [0, "cmdoption-osxphotos-add-locations-screenshot"],
+            [0, "cmdoption-osxphotos-export-screenshot"],
+            [0, "cmdoption-osxphotos-query-screenshot"],
+            [0, "cmdoption-osxphotos-repl-screenshot"],
+            [0, "cmdoption-osxphotos-sync-screenshot"]
+        ],
+        "--selected": [
+            [0, "cmdoption-osxphotos-add-locations-selected"],
+            [0, "cmdoption-osxphotos-export-selected"],
+            [0, "cmdoption-osxphotos-query-selected"],
+            [0, "cmdoption-osxphotos-repl-selected"],
+            [0, "cmdoption-osxphotos-sync-selected"]
+        ],
+        "--selfie": [
+            [0, "cmdoption-osxphotos-add-locations-selfie"],
+            [0, "cmdoption-osxphotos-export-selfie"],
+            [0, "cmdoption-osxphotos-query-selfie"],
+            [0, "cmdoption-osxphotos-repl-selfie"],
+            [0, "cmdoption-osxphotos-sync-selfie"]
+        ],
+        "--set": [
+            [0, "cmdoption-osxphotos-sync-s"]
+        ],
+        "--shared": [
+            [0, "cmdoption-osxphotos-add-locations-shared"],
+            [0, "cmdoption-osxphotos-export-shared"],
+            [0, "cmdoption-osxphotos-query-shared"],
+            [0, "cmdoption-osxphotos-repl-shared"]
+        ],
+        "--sidecar": [
+            [0, "cmdoption-osxphotos-export-sidecar"]
+        ],
+        "--sidecar-drop-ext": [
+            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
+        ],
+        "--skip-bursts": [
+            [0, "cmdoption-osxphotos-export-skip-bursts"]
+        ],
+        "--skip-edited": [
+            [0, "cmdoption-osxphotos-export-skip-edited"]
+        ],
+        "--skip-live": [
+            [0, "cmdoption-osxphotos-export-skip-live"]
+        ],
+        "--skip-original-if-edited": [
+            [0, "cmdoption-osxphotos-export-skip-original-if-edited"]
+        ],
+        "--skip-raw": [
+            [0, "cmdoption-osxphotos-export-skip-raw"]
+        ],
+        "--skip-uuid": [
+            [0, "cmdoption-osxphotos-export-skip-uuid"]
+        ],
+        "--skip-uuid-from-file": [
+            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"]
+        ],
+        "--slow-mo": [
+            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
+            [0, "cmdoption-osxphotos-export-slow-mo"],
+            [0, "cmdoption-osxphotos-query-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-slow-mo"]
+        ],
+        "--split-folder": [
+            [0, "cmdoption-osxphotos-import-f"]
+        ],
+        "--sql": [
+            [0, "cmdoption-osxphotos-exportdb-sql"]
+        ],
+        "--strip": [
+            [0, "cmdoption-osxphotos-export-strip"]
+        ],
+        "--style": [
+            [0, "cmdoption-osxphotos-diff-s"]
+        ],
+        "--syndicated": [
+            [0, "cmdoption-osxphotos-add-locations-syndicated"],
+            [0, "cmdoption-osxphotos-export-syndicated"],
+            [0, "cmdoption-osxphotos-query-syndicated"],
+            [0, "cmdoption-osxphotos-repl-syndicated"],
+            [0, "cmdoption-osxphotos-sync-syndicated"]
+        ],
+        "--template": [
+            [0, "cmdoption-osxphotos-inspect-T"]
+        ],
+        "--theme": [
+            [0, "cmdoption-osxphotos-add-locations-theme"],
+            [0, "cmdoption-osxphotos-batch-edit-theme"],
+            [0, "cmdoption-osxphotos-exiftool-theme"],
+            [0, "cmdoption-osxphotos-export-theme"],
+            [0, "cmdoption-osxphotos-exportdb-theme"],
+            [0, "cmdoption-osxphotos-import-theme"],
+            [0, "cmdoption-osxphotos-inspect-theme"],
+            [0, "cmdoption-osxphotos-orphans-theme"],
+            [0, "cmdoption-osxphotos-sync-theme"],
+            [0, "cmdoption-osxphotos-timewarp-theme"]
+        ],
+        "--time": [
+            [0, "cmdoption-osxphotos-timewarp-t"]
+        ],
+        "--time-delta": [
+            [0, "cmdoption-osxphotos-timewarp-T"]
+        ],
+        "--time-lapse": [
+            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
+            [0, "cmdoption-osxphotos-export-time-lapse"],
+            [0, "cmdoption-osxphotos-query-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-time-lapse"]
+        ],
+        "--timestamp": [
+            [0, "cmdoption-osxphotos-add-locations-timestamp"],
+            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
+            [0, "cmdoption-osxphotos-diff-timestamp"],
+            [0, "cmdoption-osxphotos-exiftool-timestamp"],
+            [0, "cmdoption-osxphotos-export-timestamp"],
+            [0, "cmdoption-osxphotos-exportdb-timestamp"],
+            [0, "cmdoption-osxphotos-import-timestamp"],
+            [0, "cmdoption-osxphotos-orphans-timestamp"],
+            [0, "cmdoption-osxphotos-sync-timestamp"],
+            [0, "cmdoption-osxphotos-timewarp-2"],
+            [0, "cmdoption-osxphotos-timewarp-timestamp"]
+        ],
+        "--timezone": [
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "--title": [
+            [0, "cmdoption-osxphotos-add-locations-title"],
+            [0, "cmdoption-osxphotos-batch-edit-title"],
+            [0, "cmdoption-osxphotos-export-title"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-query-title"],
+            [0, "cmdoption-osxphotos-repl-title"],
+            [0, "cmdoption-osxphotos-sync-title"]
+        ],
+        "--tmpdir": [
+            [0, "cmdoption-osxphotos-export-tmpdir"]
+        ],
+        "--to-date": [
+            [0, "cmdoption-osxphotos-add-locations-to-date"],
+            [0, "cmdoption-osxphotos-export-to-date"],
+            [0, "cmdoption-osxphotos-query-to-date"],
+            [0, "cmdoption-osxphotos-repl-to-date"],
+            [0, "cmdoption-osxphotos-sync-to-date"]
+        ],
+        "--to-time": [
+            [0, "cmdoption-osxphotos-add-locations-to-time"],
+            [0, "cmdoption-osxphotos-export-to-time"],
+            [0, "cmdoption-osxphotos-query-to-time"],
+            [0, "cmdoption-osxphotos-repl-to-time"],
+            [0, "cmdoption-osxphotos-sync-to-time"]
+        ],
+        "--touch-file": [
+            [0, "cmdoption-osxphotos-export-touch-file"],
+            [0, "cmdoption-osxphotos-exportdb-touch-file"]
+        ],
+        "--undo": [
+            [0, "cmdoption-osxphotos-batch-edit-undo"]
+        ],
+        "--unmatched": [
+            [0, "cmdoption-osxphotos-sync-U"]
+        ],
+        "--update": [
+            [0, "cmdoption-osxphotos-export-update"]
+        ],
+        "--update-errors": [
+            [0, "cmdoption-osxphotos-export-update-errors"]
+        ],
+        "--update-signatures": [
+            [0, "cmdoption-osxphotos-exportdb-update-signatures"]
+        ],
+        "--upgrade": [
+            [0, "cmdoption-osxphotos-install-U"]
+        ],
+        "--use-file-time": [
+            [0, "cmdoption-osxphotos-timewarp-1"]
+        ],
+        "--use-photokit": [
+            [0, "cmdoption-osxphotos-export-use-photokit"]
+        ],
+        "--use-photos-export": [
+            [0, "cmdoption-osxphotos-export-use-photos-export"]
+        ],
+        "--uti": [
+            [0, "cmdoption-osxphotos-add-locations-uti"],
+            [0, "cmdoption-osxphotos-export-uti"],
+            [0, "cmdoption-osxphotos-query-uti"],
+            [0, "cmdoption-osxphotos-repl-uti"],
+            [0, "cmdoption-osxphotos-sync-uti"]
+        ],
+        "--uuid": [
+            [0, "cmdoption-osxphotos-add-locations-uuid"],
+            [0, "cmdoption-osxphotos-export-uuid"],
+            [0, "cmdoption-osxphotos-query-uuid"],
+            [0, "cmdoption-osxphotos-repl-uuid"],
+            [0, "cmdoption-osxphotos-sync-uuid"]
+        ],
+        "--uuid-files": [
+            [0, "cmdoption-osxphotos-exportdb-uuid-files"]
+        ],
+        "--uuid-from-file": [
+            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-uuid-from-file"],
+            [0, "cmdoption-osxphotos-query-uuid-from-file"],
+            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
+            [0, "cmdoption-osxphotos-sync-uuid-from-file"]
+        ],
+        "--uuid-info": [
+            [0, "cmdoption-osxphotos-exportdb-uuid-info"]
+        ],
+        "--vacuum": [
+            [0, "cmdoption-osxphotos-exportdb-vacuum"]
+        ],
+        "--verbose": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-timewarp-V"]
+        ],
+        "--version": [
+            [0, "cmdoption-osxphotos-exportdb-version"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "--walk": [
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "--window": [
+            [0, "cmdoption-osxphotos-add-locations-w"]
+        ],
+        "--xattr-template": [
+            [0, "cmdoption-osxphotos-export-xattr-template"]
+        ],
+        "--year": [
+            [0, "cmdoption-osxphotos-add-locations-year"],
+            [0, "cmdoption-osxphotos-export-year"],
+            [0, "cmdoption-osxphotos-query-year"],
+            [0, "cmdoption-osxphotos-repl-year"],
+            [0, "cmdoption-osxphotos-sync-year"]
+        ],
+        "--yes": [
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "-a": [
+            [0, "cmdoption-osxphotos-sync-A"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-timewarp-a"]
+        ],
+        "-c": [
+            [0, "cmdoption-osxphotos-import-C"],
+            [0, "cmdoption-osxphotos-timewarp-c"]
+        ],
+        "-d": [
+            [0, "cmdoption-osxphotos-import-D"],
+            [0, "cmdoption-osxphotos-timewarp-D"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-timewarp-d"]
+        ],
+        "-f": [
+            [0, "cmdoption-osxphotos-timewarp-F"],
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-import-f"],
+            [0, "cmdoption-osxphotos-query-f"],
+            [0, "cmdoption-osxphotos-timewarp-1"],
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "-l": [
+            [0, "cmdoption-osxphotos-import-L"],
+            [0, "cmdoption-osxphotos-timewarp-L"],
+            [0, "cmdoption-osxphotos-import-l"]
+        ],
+        "-m": [
+            [0, "cmdoption-osxphotos-timewarp-M"],
+            [0, "cmdoption-osxphotos-import-m"],
+            [0, "cmdoption-osxphotos-sync-m"],
+            [0, "cmdoption-osxphotos-timewarp-0"]
+        ],
+        "-p": [
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-timewarp-P"],
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-timewarp-p"]
+        ],
+        "-r": [
+            [0, "cmdoption-osxphotos-import-R"],
+            [0, "cmdoption-osxphotos-sync-R"],
+            [0, "cmdoption-osxphotos-diff-r"],
+            [0, "cmdoption-osxphotos-import-r"]
+        ],
+        "-t": [
+            [0, "cmdoption-osxphotos-inspect-T"],
+            [0, "cmdoption-osxphotos-timewarp-T"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-inspect-t"],
+            [0, "cmdoption-osxphotos-timewarp-t"]
+        ],
+        "-u": [
+            [0, "cmdoption-osxphotos-install-U"],
+            [0, "cmdoption-osxphotos-sync-U"]
+        ],
+        "-v": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-timewarp-V"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "-e": [
+            [0, "cmdoption-osxphotos-import-e"],
+            [0, "cmdoption-osxphotos-sync-e"],
+            [0, "cmdoption-osxphotos-timewarp-e"]
+        ],
+        "-g": [
+            [0, "cmdoption-osxphotos-import-g"]
+        ],
+        "-h": [
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "-i": [
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-sync-0"],
+            [0, "cmdoption-osxphotos-sync-i"],
+            [0, "cmdoption-osxphotos-timewarp-i"]
+        ],
+        "-k": [
+            [0, "cmdoption-osxphotos-import-k"]
+        ],
+        "-s": [
+            [0, "cmdoption-osxphotos-diff-s"],
+            [0, "cmdoption-osxphotos-sync-s"]
+        ],
+        "-w": [
+            [0, "cmdoption-osxphotos-add-locations-w"],
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "-y": [
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "-z": [
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "args": [
+            [0, "cmdoption-osxphotos-run-arg-ARGS"]
+        ],
+        "db2": [
+            [0, "cmdoption-osxphotos-diff-arg-DB2"]
+        ],
+        "dest": [
+            [0, "cmdoption-osxphotos-export-arg-DEST"]
+        ],
+        "export_database": [
+            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"]
+        ],
+        "export_directory": [
+            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"]
+        ],
+        "files": [
+            [0, "cmdoption-osxphotos-import-arg-FILES"]
+        ],
+        "packages": [
+            [0, "cmdoption-osxphotos-install-arg-PACKAGES"],
+            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"]
+        ],
+        "photos_library": [
+            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"]
+        ],
+        "python_file": [
+            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"]
+        ],
+        "subtopic": [
+            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"]
+        ],
+        "topic": [
+            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
+        ],
+        "uuid_or_name": [
+            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"]
+        ],
+        "width": [
+            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
+        ],
+        "osxphotos command line option": [
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "osxphotos-add-locations command line option": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-add-locations-added-after"],
+            [0, "cmdoption-osxphotos-add-locations-added-before"],
+            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
+            [0, "cmdoption-osxphotos-add-locations-album"],
+            [0, "cmdoption-osxphotos-add-locations-burst"],
+            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
+            [0, "cmdoption-osxphotos-add-locations-description"],
+            [0, "cmdoption-osxphotos-add-locations-dry-run"],
+            [0, "cmdoption-osxphotos-add-locations-duplicate"],
+            [0, "cmdoption-osxphotos-add-locations-edited"],
+            [0, "cmdoption-osxphotos-add-locations-exif"],
+            [0, "cmdoption-osxphotos-add-locations-external-edit"],
+            [0, "cmdoption-osxphotos-add-locations-favorite"],
+            [0, "cmdoption-osxphotos-add-locations-folder"],
+            [0, "cmdoption-osxphotos-add-locations-from-date"],
+            [0, "cmdoption-osxphotos-add-locations-from-time"],
+            [0, "cmdoption-osxphotos-add-locations-has-comment"],
+            [0, "cmdoption-osxphotos-add-locations-has-likes"],
+            [0, "cmdoption-osxphotos-add-locations-has-raw"],
+            [0, "cmdoption-osxphotos-add-locations-hdr"],
+            [0, "cmdoption-osxphotos-add-locations-hidden"],
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-add-locations-in-album"],
+            [0, "cmdoption-osxphotos-add-locations-incloud"],
+            [0, "cmdoption-osxphotos-add-locations-is-reference"],
+            [0, "cmdoption-osxphotos-add-locations-keyword"],
+            [0, "cmdoption-osxphotos-add-locations-label"],
+            [0, "cmdoption-osxphotos-add-locations-live"],
+            [0, "cmdoption-osxphotos-add-locations-location"],
+            [0, "cmdoption-osxphotos-add-locations-max-size"],
+            [0, "cmdoption-osxphotos-add-locations-min-size"],
+            [0, "cmdoption-osxphotos-add-locations-missing"],
+            [0, "cmdoption-osxphotos-add-locations-name"],
+            [0, "cmdoption-osxphotos-add-locations-no-comment"],
+            [0, "cmdoption-osxphotos-add-locations-no-description"],
+            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
+            [0, "cmdoption-osxphotos-add-locations-no-likes"],
+            [0, "cmdoption-osxphotos-add-locations-no-location"],
+            [0, "cmdoption-osxphotos-add-locations-no-place"],
+            [0, "cmdoption-osxphotos-add-locations-no-title"],
+            [0, "cmdoption-osxphotos-add-locations-not-burst"],
+            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
+            [0, "cmdoption-osxphotos-add-locations-not-edited"],
+            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
+            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
+            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
+            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
+            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
+            [0, "cmdoption-osxphotos-add-locations-not-live"],
+            [0, "cmdoption-osxphotos-add-locations-not-missing"],
+            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
+            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
+            [0, "cmdoption-osxphotos-add-locations-not-reference"],
+            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
+            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
+            [0, "cmdoption-osxphotos-add-locations-not-shared"],
+            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
+            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
+            [0, "cmdoption-osxphotos-add-locations-only-movies"],
+            [0, "cmdoption-osxphotos-add-locations-only-photos"],
+            [0, "cmdoption-osxphotos-add-locations-panorama"],
+            [0, "cmdoption-osxphotos-add-locations-person"],
+            [0, "cmdoption-osxphotos-add-locations-place"],
+            [0, "cmdoption-osxphotos-add-locations-portrait"],
+            [0, "cmdoption-osxphotos-add-locations-query-eval"],
+            [0, "cmdoption-osxphotos-add-locations-query-function"],
+            [0, "cmdoption-osxphotos-add-locations-regex"],
+            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
+            [0, "cmdoption-osxphotos-add-locations-screenshot"],
+            [0, "cmdoption-osxphotos-add-locations-selected"],
+            [0, "cmdoption-osxphotos-add-locations-selfie"],
+            [0, "cmdoption-osxphotos-add-locations-shared"],
+            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-syndicated"],
+            [0, "cmdoption-osxphotos-add-locations-theme"],
+            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
+            [0, "cmdoption-osxphotos-add-locations-timestamp"],
+            [0, "cmdoption-osxphotos-add-locations-title"],
+            [0, "cmdoption-osxphotos-add-locations-to-date"],
+            [0, "cmdoption-osxphotos-add-locations-to-time"],
+            [0, "cmdoption-osxphotos-add-locations-uti"],
+            [0, "cmdoption-osxphotos-add-locations-uuid"],
+            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
+            [0, "cmdoption-osxphotos-add-locations-w"],
+            [0, "cmdoption-osxphotos-add-locations-year"]
+        ],
+        "osxphotos-albums command line option": [
+            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-albums-json"],
+            [0, "cmdoption-osxphotos-albums-library"]
+        ],
+        "osxphotos-batch-edit command line option": [
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-batch-edit-description"],
+            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
+            [0, "cmdoption-osxphotos-batch-edit-keyword"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-batch-edit-location"],
+            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
+            [0, "cmdoption-osxphotos-batch-edit-theme"],
+            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
+            [0, "cmdoption-osxphotos-batch-edit-title"],
+            [0, "cmdoption-osxphotos-batch-edit-undo"]
+        ],
+        "osxphotos-diff command line option": [
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-diff-arg-DB2"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-diff-r"],
+            [0, "cmdoption-osxphotos-diff-s"],
+            [0, "cmdoption-osxphotos-diff-timestamp"]
+        ],
+        "osxphotos-dump command line option": [
+            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-dump-deleted"],
+            [0, "cmdoption-osxphotos-dump-deleted-only"],
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-dump-json"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-dump-print"]
+        ],
+        "osxphotos-exiftool command line option": [
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
+            [0, "cmdoption-osxphotos-exiftool-append"],
+            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"],
+            [0, "cmdoption-osxphotos-exiftool-db-config"],
+            [0, "cmdoption-osxphotos-exiftool-description-template"],
+            [0, "cmdoption-osxphotos-exiftool-dry-run"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
+            [0, "cmdoption-osxphotos-exiftool-exportdb"],
+            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-exiftool-load-config"],
+            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
+            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-report"],
+            [0, "cmdoption-osxphotos-exiftool-save-config"],
+            [0, "cmdoption-osxphotos-exiftool-theme"],
+            [0, "cmdoption-osxphotos-exiftool-timestamp"]
+        ],
+        "osxphotos-export command line option": [
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-export-add-exported-to-album"],
+            [0, "cmdoption-osxphotos-export-add-missing-to-album"],
+            [0, "cmdoption-osxphotos-export-add-skipped-to-album"],
+            [0, "cmdoption-osxphotos-export-added-after"],
+            [0, "cmdoption-osxphotos-export-added-before"],
+            [0, "cmdoption-osxphotos-export-added-in-last"],
+            [0, "cmdoption-osxphotos-export-album"],
+            [0, "cmdoption-osxphotos-export-album-keyword"],
+            [0, "cmdoption-osxphotos-export-alt-copy"],
+            [0, "cmdoption-osxphotos-export-append"],
+            [0, "cmdoption-osxphotos-export-arg-DEST"],
+            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-export-burst"],
+            [0, "cmdoption-osxphotos-export-cleanup"],
+            [0, "cmdoption-osxphotos-export-cloudasset"],
+            [0, "cmdoption-osxphotos-export-config-only"],
+            [0, "cmdoption-osxphotos-export-convert-to-jpeg"],
+            [0, "cmdoption-osxphotos-export-current-name"],
+            [0, "cmdoption-osxphotos-export-deleted"],
+            [0, "cmdoption-osxphotos-export-deleted-only"],
+            [0, "cmdoption-osxphotos-export-description"],
+            [0, "cmdoption-osxphotos-export-description-template"],
+            [0, "cmdoption-osxphotos-export-directory"],
+            [0, "cmdoption-osxphotos-export-download-missing"],
+            [0, "cmdoption-osxphotos-export-dry-run"],
+            [0, "cmdoption-osxphotos-export-duplicate"],
+            [0, "cmdoption-osxphotos-export-edited"],
+            [0, "cmdoption-osxphotos-export-edited-suffix"],
+            [0, "cmdoption-osxphotos-export-exif"],
+            [0, "cmdoption-osxphotos-export-exiftool"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-export-exiftool-option"],
+            [0, "cmdoption-osxphotos-export-exiftool-path"],
+            [0, "cmdoption-osxphotos-export-export-aae"],
+            [0, "cmdoption-osxphotos-export-export-as-hardlink"],
+            [0, "cmdoption-osxphotos-export-export-by-date"],
+            [0, "cmdoption-osxphotos-export-exportdb"],
+            [0, "cmdoption-osxphotos-export-external-edit"],
+            [0, "cmdoption-osxphotos-export-favorite"],
+            [0, "cmdoption-osxphotos-export-favorite-rating"],
+            [0, "cmdoption-osxphotos-export-filename"],
+            [0, "cmdoption-osxphotos-export-finder-tag-keywords"],
+            [0, "cmdoption-osxphotos-export-finder-tag-template"],
+            [0, "cmdoption-osxphotos-export-folder"],
+            [0, "cmdoption-osxphotos-export-force-update"],
+            [0, "cmdoption-osxphotos-export-from-date"],
+            [0, "cmdoption-osxphotos-export-from-time"],
+            [0, "cmdoption-osxphotos-export-has-comment"],
+            [0, "cmdoption-osxphotos-export-has-likes"],
+            [0, "cmdoption-osxphotos-export-has-raw"],
+            [0, "cmdoption-osxphotos-export-hdr"],
+            [0, "cmdoption-osxphotos-export-hidden"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-export-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-export-ignore-signature"],
+            [0, "cmdoption-osxphotos-export-in-album"],
+            [0, "cmdoption-osxphotos-export-incloud"],
+            [0, "cmdoption-osxphotos-export-is-reference"],
+            [0, "cmdoption-osxphotos-export-jpeg-ext"],
+            [0, "cmdoption-osxphotos-export-jpeg-quality"],
+            [0, "cmdoption-osxphotos-export-keep"],
+            [0, "cmdoption-osxphotos-export-keyword"],
+            [0, "cmdoption-osxphotos-export-keyword-template"],
+            [0, "cmdoption-osxphotos-export-label"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-export-limit"],
+            [0, "cmdoption-osxphotos-export-live"],
+            [0, "cmdoption-osxphotos-export-load-config"],
+            [0, "cmdoption-osxphotos-export-location"],
+            [0, "cmdoption-osxphotos-export-max-size"],
+            [0, "cmdoption-osxphotos-export-min-size"],
+            [0, "cmdoption-osxphotos-export-missing"],
+            [0, "cmdoption-osxphotos-export-name"],
+            [0, "cmdoption-osxphotos-export-no-comment"],
+            [0, "cmdoption-osxphotos-export-no-description"],
+            [0, "cmdoption-osxphotos-export-no-keyword"],
+            [0, "cmdoption-osxphotos-export-no-likes"],
+            [0, "cmdoption-osxphotos-export-no-location"],
+            [0, "cmdoption-osxphotos-export-no-place"],
+            [0, "cmdoption-osxphotos-export-no-progress"],
+            [0, "cmdoption-osxphotos-export-no-title"],
+            [0, "cmdoption-osxphotos-export-not-burst"],
+            [0, "cmdoption-osxphotos-export-not-cloudasset"],
+            [0, "cmdoption-osxphotos-export-not-edited"],
+            [0, "cmdoption-osxphotos-export-not-favorite"],
+            [0, "cmdoption-osxphotos-export-not-hdr"],
+            [0, "cmdoption-osxphotos-export-not-hidden"],
+            [0, "cmdoption-osxphotos-export-not-in-album"],
+            [0, "cmdoption-osxphotos-export-not-incloud"],
+            [0, "cmdoption-osxphotos-export-not-live"],
+            [0, "cmdoption-osxphotos-export-not-missing"],
+            [0, "cmdoption-osxphotos-export-not-panorama"],
+            [0, "cmdoption-osxphotos-export-not-portrait"],
+            [0, "cmdoption-osxphotos-export-not-reference"],
+            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-not-screenshot"],
+            [0, "cmdoption-osxphotos-export-not-selfie"],
+            [0, "cmdoption-osxphotos-export-not-shared"],
+            [0, "cmdoption-osxphotos-export-not-slow-mo"],
+            [0, "cmdoption-osxphotos-export-not-syndicated"],
+            [0, "cmdoption-osxphotos-export-not-time-lapse"],
+            [0, "cmdoption-osxphotos-export-only-movies"],
+            [0, "cmdoption-osxphotos-export-only-new"],
+            [0, "cmdoption-osxphotos-export-only-photos"],
+            [0, "cmdoption-osxphotos-export-original-suffix"],
+            [0, "cmdoption-osxphotos-export-overwrite"],
+            [0, "cmdoption-osxphotos-export-panorama"],
+            [0, "cmdoption-osxphotos-export-person"],
+            [0, "cmdoption-osxphotos-export-person-keyword"],
+            [0, "cmdoption-osxphotos-export-place"],
+            [0, "cmdoption-osxphotos-export-portrait"],
+            [0, "cmdoption-osxphotos-export-post-command"],
+            [0, "cmdoption-osxphotos-export-post-function"],
+            [0, "cmdoption-osxphotos-export-preview"],
+            [0, "cmdoption-osxphotos-export-preview-if-missing"],
+            [0, "cmdoption-osxphotos-export-preview-suffix"],
+            [0, "cmdoption-osxphotos-export-print"],
+            [0, "cmdoption-osxphotos-export-query-eval"],
+            [0, "cmdoption-osxphotos-export-query-function"],
+            [0, "cmdoption-osxphotos-export-ramdb"],
+            [0, "cmdoption-osxphotos-export-regex"],
+            [0, "cmdoption-osxphotos-export-replace-keywords"],
+            [0, "cmdoption-osxphotos-export-report"],
+            [0, "cmdoption-osxphotos-export-retry"],
+            [0, "cmdoption-osxphotos-export-save-config"],
+            [0, "cmdoption-osxphotos-export-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-screenshot"],
+            [0, "cmdoption-osxphotos-export-selected"],
+            [0, "cmdoption-osxphotos-export-selfie"],
+            [0, "cmdoption-osxphotos-export-shared"],
+            [0, "cmdoption-osxphotos-export-sidecar"],
+            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
+            [0, "cmdoption-osxphotos-export-skip-bursts"],
+            [0, "cmdoption-osxphotos-export-skip-edited"],
+            [0, "cmdoption-osxphotos-export-skip-live"],
+            [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
+            [0, "cmdoption-osxphotos-export-skip-raw"],
+            [0, "cmdoption-osxphotos-export-skip-uuid"],
+            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-slow-mo"],
+            [0, "cmdoption-osxphotos-export-strip"],
+            [0, "cmdoption-osxphotos-export-syndicated"],
+            [0, "cmdoption-osxphotos-export-theme"],
+            [0, "cmdoption-osxphotos-export-time-lapse"],
+            [0, "cmdoption-osxphotos-export-timestamp"],
+            [0, "cmdoption-osxphotos-export-title"],
+            [0, "cmdoption-osxphotos-export-tmpdir"],
+            [0, "cmdoption-osxphotos-export-to-date"],
+            [0, "cmdoption-osxphotos-export-to-time"],
+            [0, "cmdoption-osxphotos-export-touch-file"],
+            [0, "cmdoption-osxphotos-export-update"],
+            [0, "cmdoption-osxphotos-export-update-errors"],
+            [0, "cmdoption-osxphotos-export-use-photokit"],
+            [0, "cmdoption-osxphotos-export-use-photos-export"],
+            [0, "cmdoption-osxphotos-export-uti"],
+            [0, "cmdoption-osxphotos-export-uuid"],
+            [0, "cmdoption-osxphotos-export-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-xattr-template"],
+            [0, "cmdoption-osxphotos-export-year"]
+        ],
+        "osxphotos-exportdb command line option": [
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-exportdb-append"],
+            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"],
+            [0, "cmdoption-osxphotos-exportdb-check-signatures"],
+            [0, "cmdoption-osxphotos-exportdb-delete-file"],
+            [0, "cmdoption-osxphotos-exportdb-delete-uuid"],
+            [0, "cmdoption-osxphotos-exportdb-dry-run"],
+            [0, "cmdoption-osxphotos-exportdb-errors"],
+            [0, "cmdoption-osxphotos-exportdb-export-dir"],
+            [0, "cmdoption-osxphotos-exportdb-info"],
+            [0, "cmdoption-osxphotos-exportdb-last-errors"],
+            [0, "cmdoption-osxphotos-exportdb-last-run"],
+            [0, "cmdoption-osxphotos-exportdb-migrate"],
+            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"],
+            [0, "cmdoption-osxphotos-exportdb-report"],
+            [0, "cmdoption-osxphotos-exportdb-save-config"],
+            [0, "cmdoption-osxphotos-exportdb-sql"],
+            [0, "cmdoption-osxphotos-exportdb-theme"],
+            [0, "cmdoption-osxphotos-exportdb-timestamp"],
+            [0, "cmdoption-osxphotos-exportdb-touch-file"],
+            [0, "cmdoption-osxphotos-exportdb-update-signatures"],
+            [0, "cmdoption-osxphotos-exportdb-uuid-files"],
+            [0, "cmdoption-osxphotos-exportdb-uuid-info"],
+            [0, "cmdoption-osxphotos-exportdb-vacuum"],
+            [0, "cmdoption-osxphotos-exportdb-version"]
+        ],
+        "osxphotos-help command line option": [
+            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"],
+            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
+        ],
+        "osxphotos-import command line option": [
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-import-C"],
+            [0, "cmdoption-osxphotos-import-D"],
+            [0, "cmdoption-osxphotos-import-L"],
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-import-R"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-import-append"],
+            [0, "cmdoption-osxphotos-import-arg-FILES"],
+            [0, "cmdoption-osxphotos-import-check-templates"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-import-e"],
+            [0, "cmdoption-osxphotos-import-f"],
+            [0, "cmdoption-osxphotos-import-g"],
+            [0, "cmdoption-osxphotos-import-k"],
+            [0, "cmdoption-osxphotos-import-l"],
+            [0, "cmdoption-osxphotos-import-m"],
+            [0, "cmdoption-osxphotos-import-no-progress"],
+            [0, "cmdoption-osxphotos-import-post-function"],
+            [0, "cmdoption-osxphotos-import-r"],
+            [0, "cmdoption-osxphotos-import-report"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-import-theme"],
+            [0, "cmdoption-osxphotos-import-timestamp"],
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "osxphotos-info command line option": [
+            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-info-json"],
+            [0, "cmdoption-osxphotos-info-library"]
+        ],
+        "osxphotos-inspect command line option": [
+            [0, "cmdoption-osxphotos-inspect-T"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-inspect-t"],
+            [0, "cmdoption-osxphotos-inspect-theme"]
+        ],
+        "osxphotos-install command line option": [
+            [0, "cmdoption-osxphotos-install-U"],
+            [0, "cmdoption-osxphotos-install-arg-PACKAGES"]
+        ],
+        "osxphotos-keywords command line option": [
+            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-keywords-json"],
+            [0, "cmdoption-osxphotos-keywords-library"]
+        ],
+        "osxphotos-labels command line option": [
+            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-labels-json"],
+            [0, "cmdoption-osxphotos-labels-library"]
+        ],
+        "osxphotos-list command line option": [
+            [0, "cmdoption-osxphotos-list-json"]
+        ],
+        "osxphotos-orphans command line option": [
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-orphans-export"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-orphans-theme"],
+            [0, "cmdoption-osxphotos-orphans-timestamp"]
+        ],
+        "osxphotos-persons command line option": [
+            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-persons-json"],
+            [0, "cmdoption-osxphotos-persons-library"]
+        ],
+        "osxphotos-places command line option": [
+            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-places-json"],
+            [0, "cmdoption-osxphotos-places-library"]
+        ],
+        "osxphotos-query command line option": [
+            [0, "cmdoption-osxphotos-query-add-to-album"],
+            [0, "cmdoption-osxphotos-query-added-after"],
+            [0, "cmdoption-osxphotos-query-added-before"],
+            [0, "cmdoption-osxphotos-query-added-in-last"],
+            [0, "cmdoption-osxphotos-query-album"],
+            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-query-burst"],
+            [0, "cmdoption-osxphotos-query-cloudasset"],
+            [0, "cmdoption-osxphotos-query-count"],
+            [0, "cmdoption-osxphotos-query-deleted"],
+            [0, "cmdoption-osxphotos-query-deleted-only"],
+            [0, "cmdoption-osxphotos-query-description"],
+            [0, "cmdoption-osxphotos-query-duplicate"],
+            [0, "cmdoption-osxphotos-query-edited"],
+            [0, "cmdoption-osxphotos-query-exif"],
+            [0, "cmdoption-osxphotos-query-external-edit"],
+            [0, "cmdoption-osxphotos-query-f"],
+            [0, "cmdoption-osxphotos-query-favorite"],
+            [0, "cmdoption-osxphotos-query-folder"],
+            [0, "cmdoption-osxphotos-query-from-date"],
+            [0, "cmdoption-osxphotos-query-from-time"],
+            [0, "cmdoption-osxphotos-query-has-comment"],
+            [0, "cmdoption-osxphotos-query-has-likes"],
+            [0, "cmdoption-osxphotos-query-has-raw"],
+            [0, "cmdoption-osxphotos-query-hdr"],
+            [0, "cmdoption-osxphotos-query-hidden"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-query-in-album"],
+            [0, "cmdoption-osxphotos-query-incloud"],
+            [0, "cmdoption-osxphotos-query-is-reference"],
+            [0, "cmdoption-osxphotos-query-json"],
+            [0, "cmdoption-osxphotos-query-keyword"],
+            [0, "cmdoption-osxphotos-query-label"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-query-live"],
+            [0, "cmdoption-osxphotos-query-location"],
+            [0, "cmdoption-osxphotos-query-max-size"],
+            [0, "cmdoption-osxphotos-query-min-size"],
+            [0, "cmdoption-osxphotos-query-missing"],
+            [0, "cmdoption-osxphotos-query-name"],
+            [0, "cmdoption-osxphotos-query-no-comment"],
+            [0, "cmdoption-osxphotos-query-no-description"],
+            [0, "cmdoption-osxphotos-query-no-keyword"],
+            [0, "cmdoption-osxphotos-query-no-likes"],
+            [0, "cmdoption-osxphotos-query-no-location"],
+            [0, "cmdoption-osxphotos-query-no-place"],
+            [0, "cmdoption-osxphotos-query-no-title"],
+            [0, "cmdoption-osxphotos-query-not-burst"],
+            [0, "cmdoption-osxphotos-query-not-cloudasset"],
+            [0, "cmdoption-osxphotos-query-not-edited"],
+            [0, "cmdoption-osxphotos-query-not-favorite"],
+            [0, "cmdoption-osxphotos-query-not-hdr"],
+            [0, "cmdoption-osxphotos-query-not-hidden"],
+            [0, "cmdoption-osxphotos-query-not-in-album"],
+            [0, "cmdoption-osxphotos-query-not-incloud"],
+            [0, "cmdoption-osxphotos-query-not-live"],
+            [0, "cmdoption-osxphotos-query-not-missing"],
+            [0, "cmdoption-osxphotos-query-not-panorama"],
+            [0, "cmdoption-osxphotos-query-not-portrait"],
+            [0, "cmdoption-osxphotos-query-not-reference"],
+            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-not-screenshot"],
+            [0, "cmdoption-osxphotos-query-not-selfie"],
+            [0, "cmdoption-osxphotos-query-not-shared"],
+            [0, "cmdoption-osxphotos-query-not-slow-mo"],
+            [0, "cmdoption-osxphotos-query-not-syndicated"],
+            [0, "cmdoption-osxphotos-query-not-time-lapse"],
+            [0, "cmdoption-osxphotos-query-only-movies"],
+            [0, "cmdoption-osxphotos-query-only-photos"],
+            [0, "cmdoption-osxphotos-query-panorama"],
+            [0, "cmdoption-osxphotos-query-person"],
+            [0, "cmdoption-osxphotos-query-place"],
+            [0, "cmdoption-osxphotos-query-portrait"],
+            [0, "cmdoption-osxphotos-query-print"],
+            [0, "cmdoption-osxphotos-query-query-eval"],
+            [0, "cmdoption-osxphotos-query-query-function"],
+            [0, "cmdoption-osxphotos-query-quiet"],
+            [0, "cmdoption-osxphotos-query-regex"],
+            [0, "cmdoption-osxphotos-query-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-screenshot"],
+            [0, "cmdoption-osxphotos-query-selected"],
+            [0, "cmdoption-osxphotos-query-selfie"],
+            [0, "cmdoption-osxphotos-query-shared"],
+            [0, "cmdoption-osxphotos-query-slow-mo"],
+            [0, "cmdoption-osxphotos-query-syndicated"],
+            [0, "cmdoption-osxphotos-query-time-lapse"],
+            [0, "cmdoption-osxphotos-query-title"],
+            [0, "cmdoption-osxphotos-query-to-date"],
+            [0, "cmdoption-osxphotos-query-to-time"],
+            [0, "cmdoption-osxphotos-query-uti"],
+            [0, "cmdoption-osxphotos-query-uuid"],
+            [0, "cmdoption-osxphotos-query-uuid-from-file"],
+            [0, "cmdoption-osxphotos-query-year"]
+        ],
+        "osxphotos-repl command line option": [
+            [0, "cmdoption-osxphotos-repl-added-after"],
+            [0, "cmdoption-osxphotos-repl-added-before"],
+            [0, "cmdoption-osxphotos-repl-added-in-last"],
+            [0, "cmdoption-osxphotos-repl-album"],
+            [0, "cmdoption-osxphotos-repl-burst"],
+            [0, "cmdoption-osxphotos-repl-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-deleted"],
+            [0, "cmdoption-osxphotos-repl-deleted-only"],
+            [0, "cmdoption-osxphotos-repl-description"],
+            [0, "cmdoption-osxphotos-repl-duplicate"],
+            [0, "cmdoption-osxphotos-repl-edited"],
+            [0, "cmdoption-osxphotos-repl-emacs"],
+            [0, "cmdoption-osxphotos-repl-exif"],
+            [0, "cmdoption-osxphotos-repl-external-edit"],
+            [0, "cmdoption-osxphotos-repl-favorite"],
+            [0, "cmdoption-osxphotos-repl-folder"],
+            [0, "cmdoption-osxphotos-repl-from-date"],
+            [0, "cmdoption-osxphotos-repl-from-time"],
+            [0, "cmdoption-osxphotos-repl-has-comment"],
+            [0, "cmdoption-osxphotos-repl-has-likes"],
+            [0, "cmdoption-osxphotos-repl-has-raw"],
+            [0, "cmdoption-osxphotos-repl-hdr"],
+            [0, "cmdoption-osxphotos-repl-hidden"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-repl-in-album"],
+            [0, "cmdoption-osxphotos-repl-incloud"],
+            [0, "cmdoption-osxphotos-repl-is-reference"],
+            [0, "cmdoption-osxphotos-repl-keyword"],
+            [0, "cmdoption-osxphotos-repl-label"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-repl-live"],
+            [0, "cmdoption-osxphotos-repl-location"],
+            [0, "cmdoption-osxphotos-repl-max-size"],
+            [0, "cmdoption-osxphotos-repl-min-size"],
+            [0, "cmdoption-osxphotos-repl-missing"],
+            [0, "cmdoption-osxphotos-repl-name"],
+            [0, "cmdoption-osxphotos-repl-no-comment"],
+            [0, "cmdoption-osxphotos-repl-no-description"],
+            [0, "cmdoption-osxphotos-repl-no-keyword"],
+            [0, "cmdoption-osxphotos-repl-no-likes"],
+            [0, "cmdoption-osxphotos-repl-no-location"],
+            [0, "cmdoption-osxphotos-repl-no-place"],
+            [0, "cmdoption-osxphotos-repl-no-title"],
+            [0, "cmdoption-osxphotos-repl-not-burst"],
+            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-not-edited"],
+            [0, "cmdoption-osxphotos-repl-not-favorite"],
+            [0, "cmdoption-osxphotos-repl-not-hdr"],
+            [0, "cmdoption-osxphotos-repl-not-hidden"],
+            [0, "cmdoption-osxphotos-repl-not-in-album"],
+            [0, "cmdoption-osxphotos-repl-not-incloud"],
+            [0, "cmdoption-osxphotos-repl-not-live"],
+            [0, "cmdoption-osxphotos-repl-not-missing"],
+            [0, "cmdoption-osxphotos-repl-not-panorama"],
+            [0, "cmdoption-osxphotos-repl-not-portrait"],
+            [0, "cmdoption-osxphotos-repl-not-reference"],
+            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-not-screenshot"],
+            [0, "cmdoption-osxphotos-repl-not-selfie"],
+            [0, "cmdoption-osxphotos-repl-not-shared"],
+            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-not-syndicated"],
+            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-only-movies"],
+            [0, "cmdoption-osxphotos-repl-only-photos"],
+            [0, "cmdoption-osxphotos-repl-panorama"],
+            [0, "cmdoption-osxphotos-repl-person"],
+            [0, "cmdoption-osxphotos-repl-place"],
+            [0, "cmdoption-osxphotos-repl-portrait"],
+            [0, "cmdoption-osxphotos-repl-query-eval"],
+            [0, "cmdoption-osxphotos-repl-query-function"],
+            [0, "cmdoption-osxphotos-repl-regex"],
+            [0, "cmdoption-osxphotos-repl-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-screenshot"],
+            [0, "cmdoption-osxphotos-repl-selected"],
+            [0, "cmdoption-osxphotos-repl-selfie"],
+            [0, "cmdoption-osxphotos-repl-shared"],
+            [0, "cmdoption-osxphotos-repl-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-syndicated"],
+            [0, "cmdoption-osxphotos-repl-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-title"],
+            [0, "cmdoption-osxphotos-repl-to-date"],
+            [0, "cmdoption-osxphotos-repl-to-time"],
+            [0, "cmdoption-osxphotos-repl-uti"],
+            [0, "cmdoption-osxphotos-repl-uuid"],
+            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
+            [0, "cmdoption-osxphotos-repl-year"]
+        ],
+        "osxphotos-run command line option": [
+            [0, "cmdoption-osxphotos-run-arg-ARGS"],
+            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"],
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "osxphotos-show command line option": [
+            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"],
+            [0, "cmdoption-osxphotos-show-library"]
+        ],
+        "osxphotos-snap command line option": [
+            [0, "cmdoption-osxphotos-snap-library"]
+        ],
+        "osxphotos-sync command line option": [
+            [0, "cmdoption-osxphotos-sync-0"],
+            [0, "cmdoption-osxphotos-sync-A"],
+            [0, "cmdoption-osxphotos-sync-R"],
+            [0, "cmdoption-osxphotos-sync-U"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-sync-added-after"],
+            [0, "cmdoption-osxphotos-sync-added-before"],
+            [0, "cmdoption-osxphotos-sync-added-in-last"],
+            [0, "cmdoption-osxphotos-sync-album"],
+            [0, "cmdoption-osxphotos-sync-burst"],
+            [0, "cmdoption-osxphotos-sync-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-description"],
+            [0, "cmdoption-osxphotos-sync-dry-run"],
+            [0, "cmdoption-osxphotos-sync-duplicate"],
+            [0, "cmdoption-osxphotos-sync-e"],
+            [0, "cmdoption-osxphotos-sync-edited"],
+            [0, "cmdoption-osxphotos-sync-exif"],
+            [0, "cmdoption-osxphotos-sync-external-edit"],
+            [0, "cmdoption-osxphotos-sync-favorite"],
+            [0, "cmdoption-osxphotos-sync-folder"],
+            [0, "cmdoption-osxphotos-sync-from-date"],
+            [0, "cmdoption-osxphotos-sync-from-time"],
+            [0, "cmdoption-osxphotos-sync-has-comment"],
+            [0, "cmdoption-osxphotos-sync-has-likes"],
+            [0, "cmdoption-osxphotos-sync-has-raw"],
+            [0, "cmdoption-osxphotos-sync-hdr"],
+            [0, "cmdoption-osxphotos-sync-hidden"],
+            [0, "cmdoption-osxphotos-sync-i"],
+            [0, "cmdoption-osxphotos-sync-in-album"],
+            [0, "cmdoption-osxphotos-sync-incloud"],
+            [0, "cmdoption-osxphotos-sync-is-reference"],
+            [0, "cmdoption-osxphotos-sync-keyword"],
+            [0, "cmdoption-osxphotos-sync-label"],
+            [0, "cmdoption-osxphotos-sync-library"],
+            [0, "cmdoption-osxphotos-sync-live"],
+            [0, "cmdoption-osxphotos-sync-location"],
+            [0, "cmdoption-osxphotos-sync-m"],
+            [0, "cmdoption-osxphotos-sync-max-size"],
+            [0, "cmdoption-osxphotos-sync-min-size"],
+            [0, "cmdoption-osxphotos-sync-missing"],
+            [0, "cmdoption-osxphotos-sync-name"],
+            [0, "cmdoption-osxphotos-sync-no-comment"],
+            [0, "cmdoption-osxphotos-sync-no-description"],
+            [0, "cmdoption-osxphotos-sync-no-keyword"],
+            [0, "cmdoption-osxphotos-sync-no-likes"],
+            [0, "cmdoption-osxphotos-sync-no-location"],
+            [0, "cmdoption-osxphotos-sync-no-place"],
+            [0, "cmdoption-osxphotos-sync-no-title"],
+            [0, "cmdoption-osxphotos-sync-not-burst"],
+            [0, "cmdoption-osxphotos-sync-not-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-not-edited"],
+            [0, "cmdoption-osxphotos-sync-not-favorite"],
+            [0, "cmdoption-osxphotos-sync-not-hdr"],
+            [0, "cmdoption-osxphotos-sync-not-hidden"],
+            [0, "cmdoption-osxphotos-sync-not-in-album"],
+            [0, "cmdoption-osxphotos-sync-not-incloud"],
+            [0, "cmdoption-osxphotos-sync-not-live"],
+            [0, "cmdoption-osxphotos-sync-not-missing"],
+            [0, "cmdoption-osxphotos-sync-not-panorama"],
+            [0, "cmdoption-osxphotos-sync-not-portrait"],
+            [0, "cmdoption-osxphotos-sync-not-reference"],
+            [0, "cmdoption-osxphotos-sync-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-not-screenshot"],
+            [0, "cmdoption-osxphotos-sync-not-selfie"],
+            [0, "cmdoption-osxphotos-sync-not-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-not-syndicated"],
+            [0, "cmdoption-osxphotos-sync-not-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-only-movies"],
+            [0, "cmdoption-osxphotos-sync-only-photos"],
+            [0, "cmdoption-osxphotos-sync-panorama"],
+            [0, "cmdoption-osxphotos-sync-person"],
+            [0, "cmdoption-osxphotos-sync-place"],
+            [0, "cmdoption-osxphotos-sync-portrait"],
+            [0, "cmdoption-osxphotos-sync-query-eval"],
+            [0, "cmdoption-osxphotos-sync-query-function"],
+            [0, "cmdoption-osxphotos-sync-regex"],
+            [0, "cmdoption-osxphotos-sync-s"],
+            [0, "cmdoption-osxphotos-sync-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-screenshot"],
+            [0, "cmdoption-osxphotos-sync-selected"],
+            [0, "cmdoption-osxphotos-sync-selfie"],
+            [0, "cmdoption-osxphotos-sync-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-syndicated"],
+            [0, "cmdoption-osxphotos-sync-theme"],
+            [0, "cmdoption-osxphotos-sync-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-timestamp"],
+            [0, "cmdoption-osxphotos-sync-title"],
+            [0, "cmdoption-osxphotos-sync-to-date"],
+            [0, "cmdoption-osxphotos-sync-to-time"],
+            [0, "cmdoption-osxphotos-sync-uti"],
+            [0, "cmdoption-osxphotos-sync-uuid"],
+            [0, "cmdoption-osxphotos-sync-uuid-from-file"],
+            [0, "cmdoption-osxphotos-sync-year"]
+        ],
+        "osxphotos-theme command line option": [
+            [0, "cmdoption-osxphotos-theme-clone"],
+            [0, "cmdoption-osxphotos-theme-config"],
+            [0, "cmdoption-osxphotos-theme-default"],
+            [0, "cmdoption-osxphotos-theme-delete"],
+            [0, "cmdoption-osxphotos-theme-edit"],
+            [0, "cmdoption-osxphotos-theme-list"],
+            [0, "cmdoption-osxphotos-theme-preview"]
+        ],
+        "osxphotos-timewarp command line option": [
+            [0, "cmdoption-osxphotos-timewarp-0"],
+            [0, "cmdoption-osxphotos-timewarp-1"],
+            [0, "cmdoption-osxphotos-timewarp-2"],
+            [0, "cmdoption-osxphotos-timewarp-D"],
+            [0, "cmdoption-osxphotos-timewarp-F"],
+            [0, "cmdoption-osxphotos-timewarp-L"],
+            [0, "cmdoption-osxphotos-timewarp-M"],
+            [0, "cmdoption-osxphotos-timewarp-P"],
+            [0, "cmdoption-osxphotos-timewarp-T"],
+            [0, "cmdoption-osxphotos-timewarp-V"],
+            [0, "cmdoption-osxphotos-timewarp-a"],
+            [0, "cmdoption-osxphotos-timewarp-c"],
+            [0, "cmdoption-osxphotos-timewarp-d"],
+            [0, "cmdoption-osxphotos-timewarp-date-added"],
+            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"],
+            [0, "cmdoption-osxphotos-timewarp-e"],
+            [0, "cmdoption-osxphotos-timewarp-force"],
+            [0, "cmdoption-osxphotos-timewarp-i"],
+            [0, "cmdoption-osxphotos-timewarp-p"],
+            [0, "cmdoption-osxphotos-timewarp-plain"],
+            [0, "cmdoption-osxphotos-timewarp-t"],
+            [0, "cmdoption-osxphotos-timewarp-theme"],
+            [0, "cmdoption-osxphotos-timewarp-timestamp"],
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "osxphotos-tutorial command line option": [
+            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
+        ],
+        "osxphotos-uninstall command line option": [
+            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"],
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "osxphotos-uuid command line option": [
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "osxphotos-version command line option": [
+            [0, "cmdoption-osxphotos-version-run"]
+        ],
+        "albuminfo (class in osxphotos)": [
+            [4, "osxphotos.AlbumInfo"]
+        ],
+        "albumsortorder (class in osxphotos)": [
+            [4, "osxphotos.AlbumSortOrder"]
+        ],
+        "commentinfo (class in osxphotos)": [
+            [4, "osxphotos.CommentInfo"]
+        ],
+        "exifinfo (class in osxphotos)": [
+            [4, "osxphotos.ExifInfo"]
+        ],
+        "exiftool (class in osxphotos)": [
+            [4, "osxphotos.ExifTool"]
+        ],
+        "exportdb (class in osxphotos)": [
+            [4, "osxphotos.ExportDB"]
+        ],
+        "exportdbtemp (class in osxphotos)": [
+            [4, "osxphotos.ExportDBTemp"]
+        ],
+        "exportoptions (class in osxphotos)": [
+            [4, "osxphotos.ExportOptions"]
+        ],
+        "exportresults (class in osxphotos)": [
+            [4, "osxphotos.ExportResults"]
+        ],
+        "faceinfo (class in osxphotos)": [
+            [4, "osxphotos.FaceInfo"]
+        ],
+        "fileutil (class in osxphotos)": [
+            [4, "osxphotos.FileUtil"]
+        ],
+        "fileutilnoop (class in osxphotos)": [
+            [4, "osxphotos.FileUtilNoOp"]
+        ],
+        "folderinfo (class in osxphotos)": [
+            [4, "osxphotos.FolderInfo"]
+        ],
+        "importinfo (class in osxphotos)": [
+            [4, "osxphotos.ImportInfo"]
+        ],
+        "likeinfo (class in osxphotos)": [
+            [4, "osxphotos.LikeInfo"]
+        ],
+        "momentinfo (class in osxphotos)": [
+            [4, "osxphotos.MomentInfo"]
+        ],
+        "personinfo (class in osxphotos)": [
+            [4, "osxphotos.PersonInfo"]
+        ],
+        "photoexporter (class in osxphotos)": [
+            [4, "osxphotos.PhotoExporter"]
+        ],
+        "photoinfo (class in osxphotos)": [
+            [4, "osxphotos.PhotoInfo"]
+        ],
+        "phototemplate (class in osxphotos)": [
+            [4, "osxphotos.PhotoTemplate"]
+        ],
+        "photosalbum (class in osxphotos)": [
+            [4, "osxphotos.PhotosAlbum"]
+        ],
+        "photosalbumphotoscript (class in osxphotos)": [
+            [4, "osxphotos.PhotosAlbumPhotoScript"]
+        ],
+        "photosdb (class in osxphotos)": [
+            [4, "osxphotos.PhotosDB"]
+        ],
+        "placeinfo (class in osxphotos)": [
+            [4, "osxphotos.PlaceInfo"]
+        ],
+        "projectinfo (class in osxphotos)": [
+            [4, "osxphotos.ProjectInfo"]
+        ],
+        "queryoptions (class in osxphotos)": [
+            [4, "osxphotos.QueryOptions"]
+        ],
+        "scoreinfo (class in osxphotos)": [
+            [4, "osxphotos.ScoreInfo"]
+        ],
+        "searchinfo (class in osxphotos)": [
+            [4, "osxphotos.SearchInfo"]
+        ],
+        "activities (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.activities"]
+        ],
+        "added_after (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.added_after"]
+        ],
+        "added_before (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.added_before"]
+        ],
+        "added_in_last (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.added_in_last"]
+        ],
+        "address (osxphotos.placeinfo property)": [
+            [4, "osxphotos.PlaceInfo.address"]
+        ],
+        "address_str (osxphotos.placeinfo property)": [
+            [4, "osxphotos.PlaceInfo.address_str"]
+        ],
+        "addvalues() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.addvalues"]
+        ],
+        "adjustments (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.adjustments"]
+        ],
+        "adjustments_path (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.adjustments_path"]
+        ],
+        "album (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.album"]
+        ],
+        "album_info (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.album_info"]
+        ],
+        "album_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.album_info"]
+        ],
+        "album_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.album_info"]
+        ],
+        "album_info_shared (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.album_info_shared"]
+        ],
+        "albums (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.albums"]
+        ],
+        "albums (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums"]
+        ],
+        "albums_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums_as_dict"]
+        ],
+        "albums_shared (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums_shared"]
+        ],
+        "albums_shared_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums_shared_as_dict"]
+        ],
+        "all (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.all"]
+        ],
+        "all_files() (osxphotos.exportresults method)": [
+            [4, "osxphotos.ExportResults.all_files"]
+        ],
+        "asdict() (osxphotos.albuminfo method)": [
+            [4, "osxphotos.AlbumInfo.asdict"]
+        ],
+        "asdict() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.asdict"]
+        ],
+        "asdict() (osxphotos.faceinfo method)": [
+            [4, "osxphotos.FaceInfo.asdict"]
+        ],
+        "asdict() (osxphotos.folderinfo method)": [
+            [4, "osxphotos.FolderInfo.asdict"]
+        ],
+        "asdict() (osxphotos.importinfo method)": [
+            [4, "osxphotos.ImportInfo.asdict"]
+        ],
+        "asdict() (osxphotos.momentinfo method)": [
+            [4, "osxphotos.MomentInfo.asdict"]
+        ],
+        "asdict() (osxphotos.personinfo method)": [
+            [4, "osxphotos.PersonInfo.asdict"]
+        ],
+        "asdict() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.asdict"]
+        ],
+        "asdict() (osxphotos.placeinfo method)": [
+            [4, "osxphotos.PlaceInfo.asdict"]
+        ],
+        "asdict() (osxphotos.scoreinfo method)": [
+            [4, "osxphotos.ScoreInfo.asdict"]
+        ],
+        "asdict() (osxphotos.searchinfo method)": [
+            [4, "osxphotos.SearchInfo.asdict"]
+        ],
+        "attributes (osxphotos.exportresults property)": [
+            [4, "osxphotos.ExportResults.attributes"]
+        ],
+        "bit_flags (osxphotos.exportoptions property)": [
+            [4, "osxphotos.ExportOptions.bit_flags"]
+        ],
+        "bodies_of_water (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.bodies_of_water"]
+        ],
+        "burst (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst"]
+        ],
+        "burst (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.burst"]
+        ],
+        "burst_album_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_album_info"]
+        ],
+        "burst_albums (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_albums"]
+        ],
+        "burst_default_pick (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_default_pick"]
+        ],
+        "burst_key (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_key"]
+        ],
+        "burst_photos (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_photos"]
+        ],
+        "burst_photos (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.burst_photos"]
+        ],
+        "burst_selected (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_selected"]
+        ],
+        "camera (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.camera"]
+        ],
+        "center (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.center"]
+        ],
+        "city (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.city"]
+        ],
+        "close() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.close"]
+        ],
+        "cloud_guid (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.cloud_guid"]
+        ],
+        "cloud_metadata (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.cloud_metadata"]
+        ],
+        "cloud_owner_hashed_id (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.cloud_owner_hashed_id"]
+        ],
+        "cloudasset (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.cloudasset"]
+        ],
+        "comments (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.comments"]
+        ],
+        "connection (osxphotos.exportdb property)": [
+            [4, "osxphotos.ExportDB.connection"]
+        ],
+        "convert_to_jpeg (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.convert_to_jpeg"]
+        ],
+        "convert_to_jpeg() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.convert_to_jpeg"]
+        ],
+        "copy() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.copy"]
+        ],
+        "country (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.country"]
+        ],
+        "country_code (osxphotos.placeinfo property)": [
+            [4, "osxphotos.PlaceInfo.country_code"]
+        ],
+        "create_file_record() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.create_file_record"]
+        ],
+        "create_or_get_file_record() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.create_or_get_file_record"]
+        ],
+        "date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.date"]
+        ],
+        "date (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date"]
+        ],
+        "date_added (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date_added"]
+        ],
+        "date_modified (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date_modified"]
+        ],
+        "date_trashed (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date_trashed"]
+        ],
+        "datetime (osxphotos.exportresults property)": [
+            [4, "osxphotos.ExportResults.datetime"]
+        ],
+        "db_path (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.db_path"]
+        ],
+        "db_version (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.db_version"]
+        ],
+        "delete_data_for_filepath() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.delete_data_for_filepath"]
+        ],
+        "delete_data_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.delete_data_for_uuid"]
+        ],
+        "deleted (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.deleted"]
+        ],
+        "deleted_only (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.deleted_only"]
+        ],
+        "description (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.description"]
+        ],
+        "description (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.description"]
+        ],
+        "description_template (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.description_template"]
+        ],
+        "detected_text (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.detected_text"]
+        ],
+        "detected_text() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.detected_text"]
+        ],
+        "download_missing (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.download_missing"]
+        ],
+        "dry_run (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.dry_run"]
+        ],
+        "duplicate (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.duplicate"]
+        ],
+        "duplicates (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.duplicates"]
+        ],
+        "edited (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.edited"]
+        ],
+        "edited (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.edited"]
+        ],
+        "end_date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.end_date"]
+        ],
+        "execute() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.execute"]
+        ],
+        "exif (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.exif"]
+        ],
+        "exif_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.exif_info"]
+        ],
+        "exiftool (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.exiftool"]
+        ],
+        "exiftool (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.exiftool"]
+        ],
+        "exiftool_flags (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.exiftool_flags"]
+        ],
+        "exiftool_json_sidecar() (osxphotos.photoexporter method)": [
+            [4, "osxphotos.PhotoExporter.exiftool_json_sidecar"]
+        ],
+        "expand_variables() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.expand_variables"]
+        ],
+        "expand_variables_to_str() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.expand_variables_to_str"]
+        ],
+        "export() (osxphotos.photoexporter method)": [
+            [4, "osxphotos.PhotoExporter.export"]
+        ],
+        "export() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.export"]
+        ],
+        "export_aae (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.export_aae"]
+        ],
+        "export_as_hardlink (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.export_as_hardlink"]
+        ],
+        "export_db (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.export_db"]
+        ],
+        "export_dir (osxphotos.exportdb property)": [
+            [4, "osxphotos.ExportDB.export_dir"]
+        ],
+        "external_edit (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.external_edit"]
+        ],
+        "external_edit (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.external_edit"]
+        ],
+        "face_info (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.face_info"]
+        ],
+        "face_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.face_info"]
+        ],
+        "face_rect() (osxphotos.faceinfo method)": [
+            [4, "osxphotos.FaceInfo.face_rect"]
+        ],
+        "face_regions (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.face_regions"]
+        ],
+        "favorite (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.favorite"]
+        ],
+        "favorite (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.favorite"]
+        ],
+        "favorite (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.favorite"]
+        ],
+        "favorite_rating (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.favorite_rating"]
+        ],
+        "feature_less (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.feature_less"]
+        ],
+        "file_sig() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.file_sig"]
+        ],
+        "filename (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.filename"]
+        ],
+        "fileutil (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.fileutil"]
+        ],
+        "filter_predicate() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.filter_predicate"]
+        ],
+        "fingerprint (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.fingerprint"]
+        ],
+        "folder (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.folder"]
+        ],
+        "folder_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.folder_info"]
+        ],
+        "folder_list (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.folder_list"]
+        ],
+        "folder_list (osxphotos.projectinfo property)": [
+            [4, "osxphotos.ProjectInfo.folder_list"]
+        ],
+        "folder_names (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.folder_names"]
+        ],
+        "folder_names (osxphotos.projectinfo property)": [
+            [4, "osxphotos.ProjectInfo.folder_names"]
+        ],
+        "folders (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.folders"]
+        ],
+        "force_update (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.force_update"]
+        ],
+        "from_date (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.from_date"]
+        ],
+        "function (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.function"]
+        ],
+        "get_db_connection() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.get_db_connection"]
+        ],
+        "get_export_results() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_export_results"]
+        ],
+        "get_exported_files() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_exported_files"]
+        ],
+        "get_field_values() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_field_values"]
+        ],
+        "get_file_record() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_file_record"]
+        ],
+        "get_files_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_files_for_uuid"]
+        ],
+        "get_filter_values() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_filter_values"]
+        ],
+        "get_format_values() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_format_values"]
+        ],
+        "get_media_type() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_media_type"]
+        ],
+        "get_photo() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.get_photo"]
+        ],
+        "get_photo_bool_attribute() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_photo_bool_attribute"]
+        ],
+        "get_photo_video_type() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_photo_video_type"]
+        ],
+        "get_photoinfo_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_photoinfo_for_uuid"]
+        ],
+        "get_previous_uuids() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_previous_uuids"]
+        ],
+        "get_target_for_file() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_target_for_file"]
+        ],
+        "get_template_value() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value"]
+        ],
+        "get_template_value_exiftool() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_exiftool"]
+        ],
+        "get_template_value_filter_function() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_filter_function"]
+        ],
+        "get_template_value_function() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_function"]
+        ],
+        "get_template_value_multi() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_multi"]
+        ],
+        "get_template_value_pathlib() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_pathlib"]
+        ],
+        "get_uuid_for_file() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_uuid_for_file"]
+        ],
+        "hardlink() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.hardlink"]
+        ],
+        "has_comment (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.has_comment"]
+        ],
+        "has_likes (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.has_likes"]
+        ],
+        "has_raw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.has_raw"]
+        ],
+        "has_raw (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.has_raw"]
+        ],
+        "hasadjustments (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hasadjustments"]
+        ],
+        "hdr (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hdr"]
+        ],
+        "hdr (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.hdr"]
+        ],
+        "height (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.height"]
+        ],
+        "hexdigest (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hexdigest"]
+        ],
+        "hidden (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hidden"]
+        ],
+        "hidden (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.hidden"]
+        ],
+        "holidays (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.holidays"]
+        ],
+        "ignore_case (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.ignore_case"]
+        ],
+        "ignore_date_modified (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.ignore_date_modified"]
+        ],
+        "ignore_signature (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.ignore_signature"]
+        ],
+        "import_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.import_info"]
+        ],
+        "import_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.import_info"]
+        ],
+        "in_album (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.in_album"]
+        ],
+        "incloud (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.incloud"]
+        ],
+        "incloud (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.incloud"]
+        ],
+        "increment (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.increment"]
+        ],
+        "intrash (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.intrash"]
+        ],
+        "is_debug() (in module osxphotos)": [
+            [4, "osxphotos.is_debug"]
+        ],
+        "is_reference (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.is_reference"]
+        ],
+        "iscloudasset (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.iscloudasset"]
+        ],
+        "ishome (osxphotos.placeinfo property)": [
+            [4, "osxphotos.PlaceInfo.ishome"]
+        ],
+        "ismissing (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.ismissing"]
+        ],
+        "ismovie (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.ismovie"]
+        ],
+        "isphoto (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.isphoto"]
+        ],
+        "israw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.israw"]
+        ],
+        "isreference (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.isreference"]
+        ],
+        "jpeg_ext (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.jpeg_ext"]
+        ],
+        "jpeg_quality (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.jpeg_quality"]
+        ],
+        "json() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.json"]
+        ],
+        "json() (osxphotos.faceinfo method)": [
+            [4, "osxphotos.FaceInfo.json"]
+        ],
+        "json() (osxphotos.personinfo method)": [
+            [4, "osxphotos.PersonInfo.json"]
+        ],
+        "json() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.json"]
+        ],
+        "keyword (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.keyword"]
+        ],
+        "keyword_template (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.keyword_template"]
+        ],
+        "keywords (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.keywords"]
+        ],
+        "keywords (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.keywords"]
+        ],
+        "keywords_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.keywords_as_dict"]
+        ],
+        "label (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.label"]
+        ],
+        "labels (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.labels"]
+        ],
+        "labels (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels"]
+        ],
+        "labels (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.labels"]
+        ],
+        "labels_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels_as_dict"]
+        ],
+        "labels_normalized (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.labels_normalized"]
+        ],
+        "labels_normalized (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels_normalized"]
+        ],
+        "labels_normalized_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels_normalized_as_dict"]
+        ],
+        "library_path (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.library_path"]
+        ],
+        "likes (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.likes"]
+        ],
+        "live (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.live"]
+        ],
+        "live_photo (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.live_photo"]
+        ],
+        "live_photo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.live_photo"]
+        ],
+        "locality_names (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.locality_names"]
+        ],
+        "location (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.location"]
+        ],
+        "location (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.location"]
+        ],
+        "location (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.location"]
+        ],
+        "location (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.location"]
+        ],
+        "max_size (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.max_size"]
+        ],
+        "media_types (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.media_types"]
+        ],
+        "merge_exif_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.merge_exif_keywords"]
+        ],
+        "merge_exif_persons (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.merge_exif_persons"]
+        ],
+        "min_size (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.min_size"]
+        ],
+        "missing (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.missing"]
+        ],
+        "missing_bursts (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.missing_bursts"]
+        ],
+        "modification_date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.modification_date"]
+        ],
+        "module": [
+            [4, "module-osxphotos"]
+        ],
+        "moment_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.moment_info"]
+        ],
+        "month (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.month"]
+        ],
+        "movies (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.movies"]
+        ],
+        "mpri_reg_rect (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.mpri_reg_rect"]
+        ],
+        "mwg_rs_area (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.mwg_rs_area"]
+        ],
+        "name (osxphotos.placeinfo property)": [
+            [4, "osxphotos.PlaceInfo.name"]
+        ],
+        "name (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.name"]
+        ],
+        "names (osxphotos.placeinfo property)": [
+            [4, "osxphotos.PlaceInfo.names"]
+        ],
+        "neighborhoods (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.neighborhoods"]
+        ],
+        "no_comment (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_comment"]
+        ],
+        "no_description (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_description"]
+        ],
+        "no_keyword (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_keyword"]
+        ],
+        "no_likes (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_likes"]
+        ],
+        "no_location (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_location"]
+        ],
+        "no_place (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_place"]
+        ],
+        "no_title (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_title"]
+        ],
+        "not_burst (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_burst"]
+        ],
+        "not_cloudasset (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_cloudasset"]
+        ],
+        "not_edited (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_edited"]
+        ],
+        "not_favorite (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_favorite"]
+        ],
+        "not_hdr (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_hdr"]
+        ],
+        "not_hidden (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_hidden"]
+        ],
+        "not_in_album (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_in_album"]
+        ],
+        "not_incloud (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_incloud"]
+        ],
+        "not_live (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_live"]
+        ],
+        "not_missing (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_missing"]
+        ],
+        "not_panorama (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_panorama"]
+        ],
+        "not_portrait (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_portrait"]
+        ],
+        "not_reference (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_reference"]
+        ],
+        "not_saved_to_library (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_saved_to_library"]
+        ],
+        "not_screenshot (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_screenshot"]
+        ],
+        "not_selfie (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_selfie"]
+        ],
+        "not_shared (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_shared"]
+        ],
+        "not_slow_mo (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_slow_mo"]
+        ],
+        "not_syndicated (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_syndicated"]
+        ],
+        "not_time_lapse (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_time_lapse"]
+        ],
+        "orientation (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.orientation"]
+        ],
+        "original_filename (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_filename"]
+        ],
+        "original_filesize (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_filesize"]
+        ],
+        "original_height (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_height"]
+        ],
+        "original_orientation (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_orientation"]
+        ],
+        "original_width (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_width"]
+        ],
+        "osxphotos": [
+            [4, "module-osxphotos"]
+        ],
+        "overwrite (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.overwrite"]
+        ],
+        "owner (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.owner"]
+        ],
+        "panorama (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.panorama"]
+        ],
+        "panorama (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.panorama"]
+        ],
+        "parent (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.parent"]
+        ],
+        "parent (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.parent"]
+        ],
+        "path (osxphotos.exportdb property)": [
+            [4, "osxphotos.ExportDB.path"]
+        ],
+        "path (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path"]
+        ],
+        "path_derivatives (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_derivatives"]
+        ],
+        "path_edited (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_edited"]
+        ],
+        "path_edited_live_photo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_edited_live_photo"]
+        ],
+        "path_live_photo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_live_photo"]
+        ],
+        "path_raw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_raw"]
+        ],
+        "person (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.person"]
+        ],
+        "person_info (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.person_info"]
+        ],
+        "person_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.person_info"]
+        ],
+        "person_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.person_info"]
+        ],
+        "persons (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.persons"]
+        ],
+        "persons (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.persons"]
+        ],
+        "persons (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.persons"]
+        ],
+        "persons_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.persons_as_dict"]
+        ],
+        "photo (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.photo"]
+        ],
+        "photo_index() (osxphotos.albuminfo method)": [
+            [4, "osxphotos.AlbumInfo.photo_index"]
+        ],
+        "photos (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.photos"]
+        ],
+        "photos (osxphotos.importinfo property)": [
+            [4, "osxphotos.ImportInfo.photos"]
+        ],
+        "photos (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.photos"]
+        ],
+        "photos (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.photos"]
+        ],
+        "photos (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.photos"]
+        ],
+        "photos() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.photos"]
+        ],
+        "photos_by_uuid() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.photos_by_uuid"]
+        ],
+        "photos_version (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.photos_version"]
+        ],
+        "pid (osxphotos.exiftool property)": [
+            [4, "osxphotos.ExifTool.pid"]
+        ],
+        "pitch (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.pitch"]
+        ],
+        "pk (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.pk"]
+        ],
+        "place (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.place"]
+        ],
+        "place (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.place"]
+        ],
+        "place_names (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.place_names"]
+        ],
+        "portrait (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.portrait"]
+        ],
+        "portrait (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.portrait"]
+        ],
+        "preview (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.preview"]
+        ],
+        "preview_suffix (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.preview_suffix"]
+        ],
+        "project_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.project_info"]
+        ],
+        "project_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.project_info"]
+        ],
+        "query() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.query"]
+        ],
+        "query_eval (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.query_eval"]
+        ],
+        "raw_original (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.raw_original"]
+        ],
+        "raw_photo (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.raw_photo"]
+        ],
+        "regex (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.regex"]
+        ],
+        "rename() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.rename"]
+        ],
+        "render() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.render"]
+        ],
+        "render_options (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.render_options"]
+        ],
+        "render_template() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.render_template"]
+        ],
+        "replace_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.replace_keywords"]
+        ],
+        "rich (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.rich"]
+        ],
+        "rmdir() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.rmdir"]
+        ],
+        "roll (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.roll"]
+        ],
+        "roll_pitch_yaw() (osxphotos.faceinfo method)": [
+            [4, "osxphotos.FaceInfo.roll_pitch_yaw"]
+        ],
+        "run_commands() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.run_commands"]
+        ],
+        "saved_to_library (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.saved_to_library"]
+        ],
+        "saved_to_library (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.saved_to_library"]
+        ],
+        "score (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.score"]
+        ],
+        "screenshot (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.screenshot"]
+        ],
+        "screenshot (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.screenshot"]
+        ],
+        "search_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.search_info"]
+        ],
+        "search_info_normalized (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.search_info_normalized"]
+        ],
+        "season (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.season"]
+        ],
+        "selected (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.selected"]
+        ],
+        "selfie (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.selfie"]
+        ],
+        "selfie (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.selfie"]
+        ],
+        "set_config() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.set_config"]
+        ],
+        "set_debug() (in module osxphotos)": [
+            [4, "osxphotos.set_debug"]
+        ],
+        "set_export_results() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.set_export_results"]
+        ],
+        "set_photoinfo_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.set_photoinfo_for_uuid"]
+        ],
+        "setvalue() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.setvalue"]
+        ],
+        "shared (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.shared"]
+        ],
+        "shared (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.shared"]
+        ],
+        "sidecar (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.sidecar"]
+        ],
+        "sidecar_drop_ext (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.sidecar_drop_ext"]
+        ],
+        "size_pixels (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.size_pixels"]
+        ],
+        "slow_mo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.slow_mo"]
+        ],
+        "slow_mo (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.slow_mo"]
+        ],
+        "sort_order (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.sort_order"]
+        ],
+        "sort_order (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.sort_order"]
+        ],
+        "source (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.source"]
+        ],
+        "start_date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.start_date"]
+        ],
+        "state (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.state"]
+        ],
+        "state_abbreviation (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.state_abbreviation"]
+        ],
+        "streets (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.streets"]
+        ],
+        "strip (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.strip"]
+        ],
+        "subfolders (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.subfolders"]
+        ],
+        "subtitle (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.subtitle"]
+        ],
+        "syndicated (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.syndicated"]
+        ],
+        "syndicated (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.syndicated"]
+        ],
+        "tables() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.tables"]
+        ],
+        "text_found (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.text_found"]
+        ],
+        "time_lapse (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.time_lapse"]
+        ],
+        "time_lapse (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.time_lapse"]
+        ],
+        "timeout (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.timeout"]
+        ],
+        "title (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.title"]
+        ],
+        "title (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.title"]
+        ],
+        "title (osxphotos.importinfo property)": [
+            [4, "osxphotos.ImportInfo.title"]
+        ],
+        "title (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.title"]
+        ],
+        "title (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.title"]
+        ],
+        "title (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.title"]
+        ],
+        "tmpdir (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.tmpdir"]
+        ],
+        "tmpdir() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.tmpdir"]
+        ],
+        "to_date (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.to_date"]
+        ],
+        "touch_file (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.touch_file"]
+        ],
+        "tzoffset (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.tzoffset"]
+        ],
+        "unlink() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.unlink"]
+        ],
+        "update (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.update"]
+        ],
+        "update_errors (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.update_errors"]
+        ],
+        "use_albums_as_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_albums_as_keywords"]
+        ],
+        "use_persons_as_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_persons_as_keywords"]
+        ],
+        "use_photokit (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_photokit"]
+        ],
+        "use_photos_export (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_photos_export"]
+        ],
+        "uti (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti"]
+        ],
+        "uti (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.uti"]
+        ],
+        "uti_edited (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti_edited"]
+        ],
+        "uti_original (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti_original"]
+        ],
+        "uti_raw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti_raw"]
+        ],
+        "utime() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.utime"]
+        ],
+        "uuid (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.uuid"]
+        ],
+        "uuid (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uuid"]
+        ],
+        "uuid (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.uuid"]
+        ],
+        "venue_types (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.venue_types"]
+        ],
+        "venues (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.venues"]
+        ],
+        "verbose (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.verbose"]
+        ],
+        "version (osxphotos.exiftool property)": [
+            [4, "osxphotos.ExifTool.version"]
+        ],
+        "visible (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.visible"]
+        ],
+        "width (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.width"]
+        ],
+        "write_exiftool_metadata_to_file() (osxphotos.photoexporter method)": [
+            [4, "osxphotos.PhotoExporter.write_exiftool_metadata_to_file"]
+        ],
+        "yaw (osxphotos.faceinfo property)": [
+            [4, "osxphotos.FaceInfo.yaw"]
+        ],
+        "year (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.year"]
+        ],
+        "year (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.year"]
+        ]
+    }
 })
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.6 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.6’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.7’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.6â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.7â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.6 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.7 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.6 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.6 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.6_documentation
+osxphotos_0.60.7_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.6/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.7/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/exifinfo.py` & `osxphotos-0.60.7/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/exiftool.py` & `osxphotos-0.60.7/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.7/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/export_db.py` & `osxphotos-0.60.7/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/export_db_utils.py` & `osxphotos-0.60.7/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/fileutil.py` & `osxphotos-0.60.7/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.7/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/imageconverter.py` & `osxphotos-0.60.7/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/momentinfo.py` & `osxphotos-0.60.7/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/path_utils.py` & `osxphotos-0.60.7/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/personinfo.py` & `osxphotos-0.60.7/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photodates.py` & `osxphotos-0.60.7/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photoexporter.py` & `osxphotos-0.60.7/osxphotos/photoexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         persons (bool): if True, include persons in exported metadata
         preview_suffix (str): t.Optional string to append to end of filename for preview images
         preview (bool): if True, also exports preview image
         raw_photo (bool, default=False): if True, will also export the associated RAW photo
         render_options (RenderOptions): t.Optional osxphotos.phototemplate.RenderOptions instance to specify options for rendering templates
         replace_keywords (bool): if True, keyword_template replaces any keywords, otherwise it's additive
         rich (bool): if True, will use rich markup with verbose output
+        export_aae (bool): if True, also exports adjustments as .AAE file
         sidecar_drop_ext (bool, default=False): if True, drops the photo's extension from sidecar filename (e.g. 'IMG_1234.json' instead of 'IMG_1234.JPG.json')
         sidecar: bit field (int): set to one or more of `SIDECAR_XMP`, `SIDECAR_JSON`, `SIDECAR_EXIFTOOL`
           - SIDECAR_JSON: if set will write a json sidecar with data in format readable by exiftool sidecar filename will be dest/filename.json;
           includes exiftool tag group names (e.g. `exiftool -G -j`)
           - SIDECAR_EXIFTOOL: if set will write a json sidecar with data in format readable by exiftool sidecar filename will be dest/filename.json;
           does not include exiftool tag group names (e.g. `exiftool -j`)
           - SIDECAR_XMP: if set will write an XMP sidecar with IPTC data sidecar filename will be dest/filename.xmp
@@ -183,14 +184,15 @@
     persons: bool = True
     preview_suffix: str = DEFAULT_PREVIEW_SUFFIX
     preview: bool = False
     raw_photo: bool = False
     render_options: t.Optional[RenderOptions] = None
     replace_keywords: bool = False
     rich: bool = False
+    export_aae: bool = False
     sidecar_drop_ext: bool = False
     sidecar: int = 0
     strip: bool = False
     timeout: int = 120
     touch_file: bool = False
     update: bool = False
     update_errors: bool = False
@@ -277,14 +279,15 @@
         "exiftool_warning",
         "exported",
         "exported_album",
         "metadata_changed",
         "missing",
         "missing_album",
         "new",
+        "aae_written",
         "sidecar_exiftool_skipped",
         "sidecar_exiftool_written",
         "sidecar_json_skipped",
         "sidecar_json_written",
         "sidecar_xmp_skipped",
         "sidecar_xmp_written",
         "skipped",
@@ -307,14 +310,15 @@
         exiftool_warning=None,
         exported=None,
         exported_album=None,
         metadata_changed=None,
         missing=None,
         missing_album=None,
         new=None,
+        aae_written=None,
         sidecar_exiftool_skipped=None,
         sidecar_exiftool_written=None,
         sidecar_json_skipped=None,
         sidecar_json_written=None,
         sidecar_xmp_skipped=None,
         sidecar_xmp_written=None,
         skipped=None,
@@ -346,14 +350,15 @@
             self.exported
             + self.new
             + self.updated
             + self.skipped
             + self.exif_updated
             + self.touched
             + self.converted_to_jpeg
+            + self.aae_written
             + self.sidecar_json_written
             + self.sidecar_json_skipped
             + self.sidecar_exiftool_written
             + self.sidecar_exiftool_skipped
             + self.sidecar_xmp_written
             + self.sidecar_xmp_skipped
             + self.missing
@@ -601,14 +606,16 @@
                 # don't know what actual preview suffix would be but most likely jpeg
                 preview_name = dest.parent / f"{dest.stem}{options.preview_suffix}.jpeg"
                 all_results.missing.append(preview_name)
                 verbose(
                     f"Skipping missing preview photo for {self._filename(self.photo.original_filename)} ({self._uuid(self.photo.uuid)})"
                 )
 
+        if options.export_aae:
+            all_results += self._write_aae_file(dest=dest, options=options)
         all_results += self._write_sidecar_files(dest=dest, options=options)
 
         return all_results
 
     def _init_temp_dir(self, options: ExportOptions):
         """Initialize (if necessary) the object's temporary directory.
 
@@ -1400,14 +1407,61 @@
             if not dry_run:
                 if overwrite and dest_new.exists():
                     FileUtil.unlink(dest_new)
                 FileUtil.copy(str(path), str(dest_new))
             exported_paths.append(str(dest_new))
         return exported_paths
 
+    def _write_aae_file(
+        self,
+        dest: pathlib.Path,
+        options: ExportOptions,
+    ) -> ExportResults:
+        """Write AAE file for the photo."""
+
+        # AAE files describe adjustments to originals, so they don't make sense
+        # for edited files
+        if options.edited:
+            return ExportResults()
+
+        verbose = options.verbose or self._verbose
+
+        aae_src = self.photo.adjustments_path
+        if aae_src is None:
+            return ExportResults()
+        aae_dest = dest.with_suffix(".AAE")
+
+        if options.export_as_hardlink:
+            try:
+                if aae_dest.exists() and any(
+                    [options.overwrite, options.update, options.force_update]):
+                    try:
+                        options.fileutil.unlink(aae_dest)
+                    except Exception as e:
+                        raise ExportError(
+                            f"Error removing file {aae_dest}: {e} (({lineno(__file__)})"
+                        ) from e
+                options.fileutil.hardlink(aae_src, aae_dest)
+            except Exception as e:
+                raise ExportError(
+                    f"Error hardlinking {aae_src} to {aae_dest}: {e} ({lineno(__file__)})"
+                ) from e
+        else:
+            try:
+                options.fileutil.copy(aae_src, aae_dest)
+                verbose(
+                    f"Exported adjustments of {self._filename(self.photo.original_filename)} to {self._filepath(normalize_fs_path(aae_dest))}"
+                )
+            except Exception as e:
+                raise ExportError(
+                    f"Error copying file {aae_src} to {aae_dest}: {e} ({lineno(__file__)})"
+                ) from e
+
+        return ExportResults(aae_written=[aae_dest])
+
     def _write_sidecar_files(
         self,
         dest: pathlib.Path,
         options: ExportOptions,
     ) -> ExportResults:
         """Write sidecar files for the photo."""
```

### Comparing `osxphotos-0.60.6/osxphotos/photoinfo.py` & `osxphotos-0.60.7/osxphotos/photoinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,36 +646,46 @@
 
     @property
     def hasadjustments(self):
         """True if picture has adjustments / edits"""
         return self._info["hasAdjustments"] == 1
 
     @property
-    def adjustments(self):
-        """Returns AdjustmentsInfo class for adjustment data or None if no adjustments; Photos 5+ only"""
+    def adjustments_path(self):
+        """Returns path to adjustments file or none if file doesn't exist"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return None
 
-        if self.hasadjustments:
-            try:
-                return self._adjustmentinfo
-            except AttributeError:
-                library = self._db._library_path
-                directory = self._uuid[0]  # first char of uuid
-                plist_file = (
-                    pathlib.Path(library)
-                    / "resources"
-                    / "renders"
-                    / directory
-                    / f"{self._uuid}.plist"
-                )
-                if not plist_file.is_file():
-                    return None
-                self._adjustmentinfo = AdjustmentsInfo(plist_file)
-                return self._adjustmentinfo
+        if not self.hasadjustments:
+            return None
+
+        library = self._db._library_path
+        directory = self._uuid[0]  # first char of uuid
+        plist_file = (
+            pathlib.Path(library)
+            / "resources"
+            / "renders"
+            / directory
+            / f"{self._uuid}.plist"
+        )
+        if not plist_file.is_file():
+            return None
+        return plist_file
+
+    @property
+    def adjustments(self):
+        """Returns AdjustmentsInfo class for adjustment data or None if no adjustments; Photos 5+ only"""
+        try:
+            return self._adjustmentinfo
+        except AttributeError:
+            plist_file = self.adjustments_path
+            if plist_file is None:
+                return None
+            self._adjustmentinfo = AdjustmentsInfo(plist_file)
+            return self._adjustmentinfo
 
     @property
     def external_edit(self):
         """Returns True if picture was edited outside of Photos using external editor"""
         return self._info["adjustmentFormatID"] == "com.apple.Photos.externalEdit"
 
     @property
```

### Comparing `osxphotos-0.60.6/osxphotos/photokit.py` & `osxphotos-0.60.7/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosalbum.py` & `osxphotos-0.60.7/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photoscript_utils.py` & `osxphotos-0.60.7/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/_photosdb_process_syndicationinfo.py` & `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_syndicationinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.7/osxphotos/photosdb/photosdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.7/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/phototables.py` & `osxphotos-0.60.7/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.7/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/phototemplate.md` & `osxphotos-0.60.7/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/phototemplate.py` & `osxphotos-0.60.7/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/phototemplate.tx` & `osxphotos-0.60.7/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/phototz.py` & `osxphotos-0.60.7/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/placeinfo.py` & `osxphotos-0.60.7/osxphotos/placeinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,14 +423,15 @@
         * `sub_administrative_area`
         * `sub_locality`
         * `iso_country_code`
         """
         pass
 
     def asdict():
+        """Returns a dictionary representation of the PlaceInfo object."""
         pass
 
 
 class PlaceInfo4(PlaceInfo):
     """Reverse geolocation place info for a photo (Photos <= 4)"""
 
     def __init__(self, place_names, country_code):
```

### Comparing `osxphotos-0.60.6/osxphotos/platform.py` & `osxphotos-0.60.7/osxphotos/platform.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/pyrepl.py` & `osxphotos-0.60.7/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.7/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/query_builder.py` & `osxphotos-0.60.7/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/queryoptions.py` & `osxphotos-0.60.7/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/scoreinfo.py` & `osxphotos-0.60.7/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/searchinfo.py` & `osxphotos-0.60.7/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/sqlgrep.py` & `osxphotos-0.60.7/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/sqlite_utils.py` & `osxphotos-0.60.7/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.7/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/template_counter.py` & `osxphotos-0.60.7/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.7/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.7/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/text_detection.py` & `osxphotos-0.60.7/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/timeutils.py` & `osxphotos-0.60.7/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/timezones.py` & `osxphotos-0.60.7/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/tutorial.md` & `osxphotos-0.60.7/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/unicode.py` & `osxphotos-0.60.7/osxphotos/unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/uti.py` & `osxphotos-0.60.7/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos/utils.py` & `osxphotos-0.60.7/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.7/osxphotos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.6
+Version: 0.60.7
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.6/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.7/osxphotos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.7/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/setup.py` & `osxphotos-0.60.7/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_10_12_6.py` & `osxphotos-0.60.7/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.7/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.7/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.7/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.7/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli.py` & `osxphotos-0.60.7/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,14 +600,21 @@
     [
         "Pumkins2.jpg",
         "Pumkins2.json",
         "Pumkins2.xmp",
     ]
 )
 
+CLI_EXPORT_AAE_UUID = "E9BC5C36-7CD1-40A1-A72B-8B8FAC227D51"
+CLI_EXPORT_AAE_FILENAMES = [
+    "wedding.jpg",
+    "wedding.AAE",
+    "wedding_edited.jpeg",
+]
+
 CLI_EXPORT_LIVE = [
     "51F2BEF7-431A-4D31-8AC1-3284A57826AE.jpeg",
     "51F2BEF7-431A-4D31-8AC1-3284A57826AE.mov",
 ]
 
 CLI_EXPORT_LIVE_ORIGINAL = _normalize_fs_paths(
     [
@@ -3353,14 +3360,61 @@
     )
     assert result.exit_code == 0
     json_got = json.loads(result.output)
     assert len(json_got) == PHOTOS_IN_TRASH_LEN_15_7
     assert json_got[0]["intrash"]
 
 
+def test_export_aae():
+    """Test export with --export-aae"""
+
+    runner = CliRunner()
+    cwd = os.getcwd()
+    # pylint: disable=not-context-manager
+    with runner.isolated_filesystem():
+        result = runner.invoke(
+            cli_main,
+            [
+                "export",
+                "--db",
+                os.path.join(cwd, CLI_PHOTOS_DB),
+                ".",
+                "--export-aae",
+                f"--uuid={CLI_EXPORT_AAE_UUID}",
+                "-V",
+            ],
+        )
+        assert result.exit_code == 0
+        files = glob.glob("*.*")
+        assert sorted(files) == sorted(CLI_EXPORT_AAE_FILENAMES)
+
+def test_export_aae_as_hardlink():
+    """Test export with --export-aae and --export-as-hardlink"""
+
+    runner = CliRunner()
+    cwd = os.getcwd()
+    # pylint: disable=not-context-manager
+    with isolated_filesystem_here():
+        result = runner.invoke(
+            cli_main,
+            [
+                "export",
+                "--db",
+                os.path.join(cwd, CLI_PHOTOS_DB),
+                ".",
+                "--export-aae",
+                "--export-as-hardlink",
+                f"--uuid={CLI_EXPORT_AAE_UUID}",
+                "-V",
+            ],
+        )
+        assert result.exit_code == 0
+        files = glob.glob("*.*")
+        assert sorted(files) == sorted(CLI_EXPORT_AAE_FILENAMES)
+
 def test_export_sidecar():
     """test --sidecar"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
```

### Comparing `osxphotos-0.60.6/tests/test_cli_add_locations.py` & `osxphotos-0.60.7/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_add_to_album.py` & `osxphotos-0.60.7/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_all_commands.py` & `osxphotos-0.60.7/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_batch_edit.py` & `osxphotos-0.60.7/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_dump.py` & `osxphotos-0.60.7/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_exiftool.py` & `osxphotos-0.60.7/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_export_cloud.py` & `osxphotos-0.60.7/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_export_projects.py` & `osxphotos-0.60.7/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_exportdb.py` & `osxphotos-0.60.7/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_import.py` & `osxphotos-0.60.7/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_orphans.py` & `osxphotos-0.60.7/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_param_types.py` & `osxphotos-0.60.7/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_sync.py` & `osxphotos-0.60.7/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_timewarp.py` & `osxphotos-0.60.7/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_utils.py` & `osxphotos-0.60.7/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cli_verbose.py` & `osxphotos-0.60.7/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.7/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_comments.py` & `osxphotos-0.60.7/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_concurrent_export.py` & `osxphotos-0.60.7/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_configoptions.py` & `osxphotos-0.60.7/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_datetime_formatter.py` & `osxphotos-0.60.7/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_datetime_utils.py` & `osxphotos-0.60.7/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_debug.py` & `osxphotos-0.60.7/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_empty_library_4_0.py` & `osxphotos-0.60.7/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_exif_info.py` & `osxphotos-0.60.7/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_exiftool.py` & `osxphotos-0.60.7/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_exiftool_caching.py` & `osxphotos-0.60.7/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.7/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.7/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.7/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_export_db.py` & `osxphotos-0.60.7/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.7/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_exportresults.py` & `osxphotos-0.60.7/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_faceinfo.py` & `osxphotos-0.60.7/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_fileutil.py` & `osxphotos-0.60.7/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_highsierra.py` & `osxphotos-0.60.7/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_image_converter.py` & `osxphotos-0.60.7/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.7/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.7/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.7/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.7/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.7/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.7/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.7/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.7/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_movies_4_0.py` & `osxphotos-0.60.7/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_movies_5_0.py` & `osxphotos-0.60.7/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_path_utils.py` & `osxphotos-0.60.7/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_personinfo.py` & `osxphotos-0.60.7/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_photokit.py` & `osxphotos-0.60.7/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_photosalbum_unicode.py` & `osxphotos-0.60.7/tests/test_photosalbum_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_photosdb_utils.py` & `osxphotos-0.60.7/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_placeinfo.py` & `osxphotos-0.60.7/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.7/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.7/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_projects_catalina.py` & `osxphotos-0.60.7/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_projects_sierra.py` & `osxphotos-0.60.7/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_score_info.py` & `osxphotos-0.60.7/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.7/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.7/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.7/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.7/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.7/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_sidecar_xmp.py` & `osxphotos-0.60.7/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.7/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.7/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.7/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.7/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_sqlitekvstore.py` & `osxphotos-0.60.7/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_template.py` & `osxphotos-0.60.7/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_template_counter.py` & `osxphotos-0.60.7/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_template_today.py` & `osxphotos-0.60.7/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_unicode.py` & `osxphotos-0.60.7/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_uti.py` & `osxphotos-0.60.7/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_utils.py` & `osxphotos-0.60.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.7/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.6/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.7/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

