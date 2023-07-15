# Comparing `tmp/vimiv-0.8.0.tar.gz` & `tmp/vimiv-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vimiv-0.8.0.tar", last modified: Mon Jan 18 15:05:54 2021, max compression
+gzip compressed data, was "vimiv-0.9.0.tar", last modified: Sat Jul 15 15:19:49 2023, max compression
```

## Comparing `vimiv-0.8.0.tar` & `vimiv-0.9.0.tar`

### file list

```diff
@@ -1,146 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.217502 vimiv-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)      444 2021-01-18 15:05:45.000000 vimiv-0.8.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-01-18 15:05:45.000000 vimiv-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      302 2021-01-18 15:05:45.000000 vimiv-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7236 2021-01-18 15:05:54.217502 vimiv-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5195 2021-01-18 15:05:45.000000 vimiv-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.209502 vimiv-0.8.0/c-extension/
--rw-r--r--   0 runner    (1001) docker     (116)     1803 2021-01-18 15:05:45.000000 vimiv-0.8.0/c-extension/brightness_contrast.h
--rw-r--r--   0 runner    (1001) docker     (116)      962 2021-01-18 15:05:45.000000 vimiv-0.8.0/c-extension/definitions.h
--rw-r--r--   0 runner    (1001) docker     (116)     1580 2021-01-18 15:05:45.000000 vimiv-0.8.0/c-extension/helper_func.h
--rw-r--r--   0 runner    (1001) docker     (116)     3645 2021-01-18 15:05:45.000000 vimiv-0.8.0/c-extension/hue_saturation_lightness.h
--rw-r--r--   0 runner    (1001) docker     (116)     2901 2021-01-18 15:05:45.000000 vimiv-0.8.0/c-extension/manipulate.c
--rw-r--r--   0 runner    (1001) docker     (116)     6563 2021-01-18 15:05:45.000000 vimiv-0.8.0/c-extension/math_func_eval.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.209502 vimiv-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      314 2021-01-18 15:05:45.000000 vimiv-0.8.0/docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4129 2021-01-18 15:05:45.000000 vimiv-0.8.0/fastentrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.209502 vimiv-0.8.0/icons/
--rw-r--r--   0 runner    (1001) docker     (116)     4421 2021-01-18 15:05:45.000000 vimiv-0.8.0/icons/vimiv.svg
--rw-r--r--   0 runner    (1001) docker     (116)     6889 2021-01-18 15:05:45.000000 vimiv-0.8.0/icons/vimiv_128x128.png
--rw-r--r--   0 runner    (1001) docker     (116)      847 2021-01-18 15:05:45.000000 vimiv-0.8.0/icons/vimiv_16x16.png
--rw-r--r--   0 runner    (1001) docker     (116)    14507 2021-01-18 15:05:45.000000 vimiv-0.8.0/icons/vimiv_256x256.png
--rw-r--r--   0 runner    (1001) docker     (116)     1700 2021-01-18 15:05:45.000000 vimiv-0.8.0/icons/vimiv_32x32.png
--rw-r--r--   0 runner    (1001) docker     (116)    32176 2021-01-18 15:05:45.000000 vimiv-0.8.0/icons/vimiv_512x512.png
--rw-r--r--   0 runner    (1001) docker     (116)     3408 2021-01-18 15:05:45.000000 vimiv-0.8.0/icons/vimiv_64x64.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.209502 vimiv-0.8.0/misc/
--rw-r--r--   0 runner    (1001) docker     (116)     1868 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     2521 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/org.karlch.vimiv.qt.metainfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.209502 vimiv-0.8.0/misc/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)       14 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       35 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_cov.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (116)       51 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_lint.txt
--rw-r--r--   0 runner    (1001) docker     (116)       34 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_mypy.txt
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_packaging.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_piexif.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_pyexiv2.txt
--rw-r--r--   0 runner    (1001) docker     (116)      100 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/requirements/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3564 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/vimiv.1
--rw-r--r--   0 runner    (1001) docker     (116)      287 2021-01-18 15:05:45.000000 vimiv-0.8.0/misc/vimiv.desktop
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-18 15:05:54.217502 vimiv-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2652 2021-01-18 15:05:45.000000 vimiv-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.209502 vimiv-0.8.0/vimiv/
--rw-r--r--   0 runner    (1001) docker     (116)      640 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      383 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.213502 vimiv-0.8.0/vimiv/api/
--rw-r--r--   0 runner    (1001) docker     (116)     2644 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12262 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/_mark.py
--rw-r--r--   0 runner    (1001) docker     (116)     7189 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/_modules.py
--rw-r--r--   0 runner    (1001) docker     (116)    12149 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/commands.py
--rw-r--r--   0 runner    (1001) docker     (116)     8546 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/completion.py
--rw-r--r--   0 runner    (1001) docker     (116)     5680 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/keybindings.py
--rw-r--r--   0 runner    (1001) docker     (116)     9179 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (116)     2999 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/objreg.py
--rw-r--r--   0 runner    (1001) docker     (116)     2007 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/prompt.py
--rw-r--r--   0 runner    (1001) docker     (116)    15113 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2592 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/signals.py
--rw-r--r--   0 runner    (1001) docker     (116)     5215 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/status.py
--rw-r--r--   0 runner    (1001) docker     (116)     9470 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/api/working_directory.py
--rw-r--r--   0 runner    (1001) docker     (116)     2892 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/app.py
--rw-r--r--   0 runner    (1001) docker     (116)     2219 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/checkversion.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.213502 vimiv-0.8.0/vimiv/commands/
--rw-r--r--   0 runner    (1001) docker     (116)     1176 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1811 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/aliases.py
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/argtypes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1825 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/delete_command.py
--rw-r--r--   0 runner    (1001) docker     (116)     5533 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/external.py
--rw-r--r--   0 runner    (1001) docker     (116)     3286 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/help_command.py
--rw-r--r--   0 runner    (1001) docker     (116)     6378 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/history.py
--rw-r--r--   0 runner    (1001) docker     (116)     1327 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/misccommands.py
--rw-r--r--   0 runner    (1001) docker     (116)     6480 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/runners.py
--rw-r--r--   0 runner    (1001) docker     (116)     5704 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/search.py
--rw-r--r--   0 runner    (1001) docker     (116)     3578 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/commands/wildcards.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.213502 vimiv-0.8.0/vimiv/completion/
--rw-r--r--   0 runner    (1001) docker     (116)      276 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3400 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/completion/completer.py
--rw-r--r--   0 runner    (1001) docker     (116)    10174 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/completion/completionmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.213502 vimiv-0.8.0/vimiv/config/
--rw-r--r--   0 runner    (1001) docker     (116)     2327 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3339 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/config/_style_options.py
--rw-r--r--   0 runner    (1001) docker     (116)     3487 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/config/configcommands.py
--rw-r--r--   0 runner    (1001) docker     (116)     5871 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/config/configfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     3416 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/config/external_configparser.py
--rw-r--r--   0 runner    (1001) docker     (116)     3107 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/config/keyfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     9634 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/config/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.217502 vimiv-0.8.0/vimiv/gui/
--rw-r--r--   0 runner    (1001) docker     (116)      262 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6529 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/commandline.py
--rw-r--r--   0 runner    (1001) docker     (116)     3741 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/commandwidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     2765 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/completionwidget.py
--rw-r--r--   0 runner    (1001) docker     (116)    10575 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/eventhandler.py
--rw-r--r--   0 runner    (1001) docker     (116)    14197 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/image.py
--rw-r--r--   0 runner    (1001) docker     (116)     6707 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/keybindings_popup.py
--rw-r--r--   0 runner    (1001) docker     (116)     3945 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/keyhintwidget.py
--rw-r--r--   0 runner    (1001) docker     (116)    21958 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/library.py
--rw-r--r--   0 runner    (1001) docker     (116)     6964 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (116)     6421 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (116)     3171 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/message.py
--rw-r--r--   0 runner    (1001) docker     (116)     6922 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/metadatawidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     3457 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/prompt.py
--rw-r--r--   0 runner    (1001) docker     (116)     3299 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/statusbar.py
--rw-r--r--   0 runner    (1001) docker     (116)     4395 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/straightenwidget.py
--rw-r--r--   0 runner    (1001) docker     (116)      578 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/synchronize.py
--rw-r--r--   0 runner    (1001) docker     (116)    18971 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (116)     3286 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/transformwidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     1489 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/gui/version_popup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.217502 vimiv-0.8.0/vimiv/imutils/
--rw-r--r--   0 runner    (1001) docker     (116)     2041 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7834 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)      952 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/current_pixmap.py
--rw-r--r--   0 runner    (1001) docker     (116)     2840 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/edit_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)    10388 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/exif.py
--rw-r--r--   0 runner    (1001) docker     (116)     8877 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/filelist.py
--rw-r--r--   0 runner    (1001) docker     (116)    20162 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/immanipulate.py
--rw-r--r--   0 runner    (1001) docker     (116)     8460 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/imtransform.py
--rw-r--r--   0 runner    (1001) docker     (116)     1776 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/imutils/slideshow.py
--rw-r--r--   0 runner    (1001) docker     (116)     4664 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.217502 vimiv-0.8.0/vimiv/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)     7380 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      882 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/plugins/demo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1877 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/plugins/imageformats.py
--rw-r--r--   0 runner    (1001) docker     (116)     6206 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/plugins/print.py
--rw-r--r--   0 runner    (1001) docker     (116)     5849 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.217502 vimiv-0.8.0/vimiv/utils/
--rw-r--r--   0 runner    (1001) docker     (116)    16316 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5469 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/crash_handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1035 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/customtypes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1702 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (116)     5706 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (116)     3872 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/imagereader.py
--rw-r--r--   0 runner    (1001) docker     (116)     2380 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (116)     7113 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (116)     4142 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/migration.py
--rw-r--r--   0 runner    (1001) docker     (116)     7212 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/thumbnail_manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     5248 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/trash_manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     4975 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/trie.py
--rw-r--r--   0 runner    (1001) docker     (116)     1645 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/utils/xdg.py
--rw-r--r--   0 runner    (1001) docker     (116)     3433 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     4831 2021-01-18 15:05:45.000000 vimiv-0.8.0/vimiv/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 15:05:54.209502 vimiv-0.8.0/vimiv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7236 2021-01-18 15:05:53.000000 vimiv-0.8.0/vimiv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3265 2021-01-18 15:05:54.000000 vimiv-0.8.0/vimiv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-18 15:05:53.000000 vimiv-0.8.0/vimiv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       42 2021-01-18 15:05:53.000000 vimiv-0.8.0/vimiv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-01-18 15:05:54.000000 vimiv-0.8.0/vimiv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-01-18 15:05:54.000000 vimiv-0.8.0/vimiv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-18 15:05:53.000000 vimiv-0.8.0/vimiv.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.053842 vimiv-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-15 15:19:35.000000 vimiv-0.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 15:19:35.000000 vimiv-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-15 15:19:35.000000 vimiv-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-15 15:19:49.053842 vimiv-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-15 15:19:35.000000 vimiv-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.045842 vimiv-0.9.0/c-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-15 15:19:35.000000 vimiv-0.9.0/c-extension/brightness_contrast.h
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-15 15:19:35.000000 vimiv-0.9.0/c-extension/definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-15 15:19:35.000000 vimiv-0.9.0/c-extension/helper_func.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-15 15:19:35.000000 vimiv-0.9.0/c-extension/hue_saturation_lightness.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-15 15:19:35.000000 vimiv-0.9.0/c-extension/manipulate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-15 15:19:35.000000 vimiv-0.9.0/c-extension/math_func_eval.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.045842 vimiv-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-15 15:19:35.000000 vimiv-0.9.0/docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-15 15:19:35.000000 vimiv-0.9.0/fastentrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.045842 vimiv-0.9.0/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-15 15:19:35.000000 vimiv-0.9.0/icons/vimiv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-15 15:19:35.000000 vimiv-0.9.0/icons/vimiv_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-15 15:19:35.000000 vimiv-0.9.0/icons/vimiv_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-07-15 15:19:35.000000 vimiv-0.9.0/icons/vimiv_256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-15 15:19:35.000000 vimiv-0.9.0/icons/vimiv_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-15 15:19:35.000000 vimiv-0.9.0/icons/vimiv_512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-15 15:19:35.000000 vimiv-0.9.0/icons/vimiv_64x64.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.045842 vimiv-0.9.0/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/org.karlch.vimiv.qt.metainfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.045842 vimiv-0.9.0/misc/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_cov.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_packaging.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_piexif.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_pyexiv2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/requirements/requirements_tox.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/vimiv.1
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 15:19:35.000000 vimiv-0.9.0/misc/vimiv.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:19:49.053842 vimiv-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-15 15:19:35.000000 vimiv-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.045842 vimiv-0.9.0/vimiv/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.049842 vimiv-0.9.0/vimiv/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/_mark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/keybindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/objreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/api/working_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/checkversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.049842 vimiv-0.9.0/vimiv/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/argtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/delete_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/misccommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/commands/wildcards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.049842 vimiv-0.9.0/vimiv/completion/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/completion/completer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/completion/completionmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.049842 vimiv-0.9.0/vimiv/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/config/_style_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/config/configcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/config/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/config/external_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/config/keyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/config/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.053842 vimiv-0.9.0/vimiv/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/commandline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/commandwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/completionwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/crop_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/eventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/keybindings_popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/keyhintwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/metadatawidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/straightenwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/synchronize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22496 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/transformwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/gui/version_popup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.053842 vimiv-0.9.0/vimiv/imutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/current_pixmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/edit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/immanipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/imtransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/imutils/slideshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.053842 vimiv-0.9.0/vimiv/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/plugins/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/plugins/imageformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/plugins/metadata_piexif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/plugins/metadata_pyexiv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/plugins/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.053842 vimiv-0.9.0/vimiv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/crash_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/customtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/imageheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/imagereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/thumbnail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/trash_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/utils/xdg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-15 15:19:35.000000 vimiv-0.9.0/vimiv/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:19:49.045842 vimiv-0.9.0/vimiv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-15 15:19:48.000000 vimiv-0.9.0/vimiv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-15 15:19:49.000000 vimiv-0.9.0/vimiv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:19:48.000000 vimiv-0.9.0/vimiv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 15:19:48.000000 vimiv-0.9.0/vimiv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 15:19:48.000000 vimiv-0.9.0/vimiv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 15:19:48.000000 vimiv-0.9.0/vimiv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:19:48.000000 vimiv-0.9.0/vimiv.egg-info/zip-safe
```

### Comparing `vimiv-0.8.0/LICENSE` & `vimiv-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/PKG-INFO` & `vimiv-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 Metadata-Version: 2.1
 Name: vimiv
-Version: 0.8.0
+Version: 0.9.0
 Summary: An image viewer with vim-like keybindings.
 Home-page: https://karlch.github.io/vimiv-qt/
 Author: Christian Karl
 Author-email: karlch@protonmail.com
 License: GPL3
 Project-URL: Source Code, https://github.com/karlch/vimiv-qt
 Project-URL: Bug Tracker, https://github.com/karlch/vimiv-qt/issues
 Project-URL: Documentation, https://karlch.github.io/vimiv-qt/documentation
-Description: <img src="https://karlch.github.io/vimiv-qt/_images/vimiv_banner_800.png" alt="vimiv banner" width="400"/>
-        
-        [![Build Status](https://github.com/karlch/vimiv-qt/workflows/CI/badge.svg)](https://github.com/karlch/vimiv-qt/actions)
-        [![Codecov](https://codecov.io/github/karlch/vimiv-qt/coverage.svg?branch=master)](https://codecov.io/github/karlch/vimiv-qt?branch=master)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        
-        [website](https://karlch.github.io/vimiv-qt/) |
-        [docs](https://karlch.github.io/vimiv-qt/documentation/index.html) |
-        [install](https://karlch.github.io/vimiv-qt/documentation/install.html) |
-        [screenshots](https://karlch.github.io/vimiv-qt/screenshots.html) |
-        [changelog](https://karlch.github.io/vimiv-qt/changelog.html) |
-        [contributing](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
-        
-        <img src="https://i.postimg.cc/VkcPgcbR/vimiv.gif" alt="vimiv screencast" width="440"/>
-        
-        ---
-        > :information_source: This Qt port is the future of vimiv. New features will
-        > only be implemented here and there are already many improvements compared to the
-        > [deprecated gtk version](https://github.com/karlch/vimiv). The old version is only
-        > recommended if you require a more stable software. In case there is anything you miss
-        > here, please [open an issue](https://github.com/karlch/vimiv-qt/issues). Check the
-        > [roadmap](https://karlch.github.io/vimiv-qt/roadmap.html) for more details.
-        ---
-        
-        Vimiv is an image viewer with vim-like keybindings. It is written in python3
-        using the Qt5 toolkit and is free software, licensed under the GPL.
-        
-        ### Features
-        
-        * Basic image operations and navigation
-        * [ranger](https://github.com/ranger/ranger)-like library to browse your images
-        * Thumbnail mode: navigable grid of image previews
-        * Command mode with tab-completion
-        * Search with pattern matching
-        * Simple mark and tag system
-        * Customization of keybindings, settings and style via configuration files,
-          [base-16 support](https://github.com/karlch/base16-vimiv), ...
-        
-        ### Install
-        
-        To learn how to get vimiv running on various platforms, please check out the
-        [installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html).
-        
-        ### Documentation
-        
-        Much more details on vimiv are available on the
-        [website](https://karlch.github.io/vimiv-qt/). Here are some hints to get you started:
-        * [The installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html)
-           includes instructions on how to get vimiv running on various platforms.
-        * [Getting started](https://karlch.github.io/vimiv-qt/documentation/getting\_started.html)
-          starts with the basic concepts and keybindings to later show some more advanced
-          features.
-        * [Commands](https://karlch.github.io/vimiv-qt/documentation/commands.html)
-          gives a complete overview and description of all commands.
-        * [Keybindings](https://karlch.github.io/vimiv-qt/documentation/configuration/keybindings.html)
-          lists the default keybindings and describes how to configure them.
-        * [Settings](https://karlch.github.io/vimiv-qt/documentation/configuration/settings.html)
-          describes the available settings and how to change them.
-        * [Style](https://karlch.github.io/vimiv-qt/documentation/configuration/style.html)
-          explains how to configure the look and colorscheme of vimiv.
-        * [Plugins](https://karlch.github.io/vimiv-qt/documentation/configuration/plugins.html)
-          illustrates vimiv's python plugin system: a great way to extend the functionality
-          beyond the defaults and to start delving into the source code.
-        
-        ### Contributing
-        
-        You want to contribute to vimiv? Great! :tada:
-        
-        Every little help counts and is appreciated!  Feel free to read the
-        [contributing guidelines](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
-        for some useful tips and tricks.
-        
-        There are many ways to contribute, including:
-        * [giving feedback and requesting new features](https://karlch.github.io/vimiv-qt/documentation/contributing.html#feedback-and-feature-requests),
-        * [reporting bugs](https://karlch.github.io/vimiv-qt/documentation/contributing.html#reporting-bugs),
-        * [writing code](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-code)
-          and
-        * [extending the documentation](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-documentation).
-        * spreading the word in an article, blog, reddit post, ...
-        
-        Need help? Feel free to
-        [contact me directly](mailto:karlch@protonmail.com)
-        or, even better,
-        open an [issue on github](https://github.com/karlch/vimiv-qt/issues/).
-        
-        ### License
-        
-        This program is free software: you can redistribute it and/or modify it under
-        the terms of the GNU General Public License as published by the Free Software
-        Foundation, either version 3 of the License, or (at your option) any later
-        version.
-        
-        This program is distributed in the hope that it will be useful, but WITHOUT ANY
-        WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-        PARTICULAR PURPOSE. See the GNU General Public License for more details.
-        
-        You should have received a copy of the GNU General Public License along with
-        this program. If not, see <http://www.gnu.org/licenses/>.
-        
 Keywords: pyqt,image viewer,vim
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+<img src="https://karlch.github.io/vimiv-qt/_images/vimiv_banner_800.png" alt="vimiv banner" width="400"/>
+
+[![Build Status](https://github.com/karlch/vimiv-qt/workflows/CI/badge.svg)](https://github.com/karlch/vimiv-qt/actions)
+[![Codecov](https://codecov.io/github/karlch/vimiv-qt/coverage.svg?branch=master)](https://codecov.io/github/karlch/vimiv-qt?branch=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+[website](https://karlch.github.io/vimiv-qt/) |
+[docs](https://karlch.github.io/vimiv-qt/documentation/index.html) |
+[install](https://karlch.github.io/vimiv-qt/documentation/install.html) |
+[screenshots](https://karlch.github.io/vimiv-qt/screenshots.html) |
+[changelog](https://karlch.github.io/vimiv-qt/changelog.html) |
+[contributing](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
+
+<img src="https://i.postimg.cc/VkcPgcbR/vimiv.gif" alt="vimiv screencast" width="440"/>
+
+---
+> :information_source: This Qt port is the future of vimiv. New features will
+> only be implemented here and there are already many improvements compared to the
+> [deprecated gtk version](https://github.com/karlch/vimiv). The old version is only
+> recommended if you require a more stable software. In case there is anything you miss
+> here, please [open an issue](https://github.com/karlch/vimiv-qt/issues). Check the
+> [roadmap](https://karlch.github.io/vimiv-qt/roadmap.html) for more details.
+---
+
+Vimiv is an image viewer with vim-like keybindings. It is written in python3
+using the Qt5 toolkit and is free software, licensed under the GPL.
+
+### Features
+
+* Basic image operations and navigation
+* [ranger](https://github.com/ranger/ranger)-like library to browse your images
+* Thumbnail mode: navigable grid of image previews
+* Command mode with tab-completion
+* Search with pattern matching
+* Simple mark and tag system
+* Customization of keybindings, settings and style via configuration files,
+  [base-16 support](https://github.com/karlch/base16-vimiv), ...
+
+### Install
+
+To learn how to get vimiv running on various platforms, please check out the
+[installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html).
+
+### Documentation
+
+Much more details on vimiv are available on the
+[website](https://karlch.github.io/vimiv-qt/). Here are some hints to get you started:
+* [The installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html)
+   includes instructions on how to get vimiv running on various platforms.
+* [Getting started](https://karlch.github.io/vimiv-qt/documentation/getting\_started.html)
+  starts with the basic concepts and keybindings to later show some more advanced
+  features.
+* [Commands](https://karlch.github.io/vimiv-qt/documentation/commands.html)
+  gives a complete overview and description of all commands.
+* [Keybindings](https://karlch.github.io/vimiv-qt/documentation/configuration/keybindings.html)
+  lists the default keybindings and describes how to configure them.
+* [Settings](https://karlch.github.io/vimiv-qt/documentation/configuration/settings.html)
+  describes the available settings and how to change them.
+* [Style](https://karlch.github.io/vimiv-qt/documentation/configuration/style.html)
+  explains how to configure the look and colorscheme of vimiv.
+* [Plugins](https://karlch.github.io/vimiv-qt/documentation/configuration/plugins.html)
+  illustrates vimiv's python plugin system: a great way to extend the functionality
+  beyond the defaults and to start delving into the source code.
+
+### Contributing
+
+You want to contribute to vimiv? Great! :tada:
+
+Every little help counts and is appreciated!  Feel free to read the
+[contributing guidelines](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
+for some useful tips and tricks.
+
+There are many ways to contribute, including:
+* [giving feedback and requesting new features](https://karlch.github.io/vimiv-qt/documentation/contributing.html#feedback-and-feature-requests)
+* [reporting bugs](https://karlch.github.io/vimiv-qt/documentation/contributing.html#reporting-bugs)
+* [writing code](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-code)
+* [extending the documentation](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-documentation)
+* spreading the word in an article, blog, reddit post, ...
+
+Need help? Feel free to
+[contact me directly](mailto:karlch@protonmail.com)
+or, even better,
+open an [issue on github](https://github.com/karlch/vimiv-qt/issues/).
+
+### License
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+This program is distributed in the hope that it will be useful, but WITHOUT ANY
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `vimiv-0.8.0/README.md` & `vimiv-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,18 @@
 You want to contribute to vimiv? Great! :tada:
 
 Every little help counts and is appreciated!  Feel free to read the
 [contributing guidelines](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
 for some useful tips and tricks.
 
 There are many ways to contribute, including:
-* [giving feedback and requesting new features](https://karlch.github.io/vimiv-qt/documentation/contributing.html#feedback-and-feature-requests),
-* [reporting bugs](https://karlch.github.io/vimiv-qt/documentation/contributing.html#reporting-bugs),
+* [giving feedback and requesting new features](https://karlch.github.io/vimiv-qt/documentation/contributing.html#feedback-and-feature-requests)
+* [reporting bugs](https://karlch.github.io/vimiv-qt/documentation/contributing.html#reporting-bugs)
 * [writing code](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-code)
-  and
-* [extending the documentation](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-documentation).
+* [extending the documentation](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-documentation)
 * spreading the word in an article, blog, reddit post, ...
 
 Need help? Feel free to
 [contact me directly](mailto:karlch@protonmail.com)
 or, even better,
 open an [issue on github](https://github.com/karlch/vimiv-qt/issues/).
```

### Comparing `vimiv-0.8.0/c-extension/brightness_contrast.h` & `vimiv-0.9.0/c-extension/brightness_contrast.h`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/c-extension/definitions.h` & `vimiv-0.9.0/c-extension/definitions.h`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/c-extension/helper_func.h` & `vimiv-0.9.0/c-extension/helper_func.h`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/c-extension/hue_saturation_lightness.h` & `vimiv-0.9.0/c-extension/hue_saturation_lightness.h`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/c-extension/manipulate.c` & `vimiv-0.9.0/c-extension/manipulate.c`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/c-extension/math_func_eval.h` & `vimiv-0.9.0/c-extension/math_func_eval.h`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/fastentrypoints.py` & `vimiv-0.9.0/fastentrypoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,23 +91,23 @@
 
     for dst in dests:
         shutil.copy(filename, dst)
         manifest_path = os.path.join(dst, "MANIFEST.in")
         setup_path = os.path.join(dst, "setup.py")
 
         # Insert the include statement to MANIFEST.in if not present
-        with open(manifest_path, "a+") as manifest:
+        with open(manifest_path, "a+", encoding="utf-8") as manifest:
             manifest.seek(0)
             manifest_content = manifest.read()
             if "include fastentrypoints.py" not in manifest_content:
                 manifest.write(
                     ("\n" if manifest_content else "") + "include fastentrypoints.py"
                 )
 
         # Insert the import statement to setup.py if not present
-        with open(setup_path, "a+") as setup:
+        with open(setup_path, "a+", encoding="utf-8") as setup:
             setup.seek(0)
             setup_content = setup.read()
             if "import fastentrypoints" not in setup_content:
                 setup.seek(0)
                 setup.truncate()
                 setup.write("import fastentrypoints\n" + setup_content)
```

### Comparing `vimiv-0.8.0/icons/vimiv.svg` & `vimiv-0.9.0/icons/vimiv.svg`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/icons/vimiv_128x128.png` & `vimiv-0.9.0/icons/vimiv_128x128.png`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/icons/vimiv_16x16.png` & `vimiv-0.9.0/icons/vimiv_16x16.png`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/icons/vimiv_256x256.png` & `vimiv-0.9.0/icons/vimiv_256x256.png`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/icons/vimiv_32x32.png` & `vimiv-0.9.0/icons/vimiv_32x32.png`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/icons/vimiv_512x512.png` & `vimiv-0.9.0/icons/vimiv_512x512.png`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/icons/vimiv_64x64.png` & `vimiv-0.9.0/icons/vimiv_64x64.png`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/misc/Makefile` & `vimiv-0.9.0/misc/Makefile`

 * *Files identical despite different names*

### Comparing `vimiv-0.8.0/misc/org.karlch.vimiv.qt.metainfo.xml` & `vimiv-0.9.0/misc/org.karlch.vimiv.qt.metainfo.xml`

 * *Files 7% similar despite different names*

#### Comparing `vimiv-0.8.0/misc/org.karlch.vimiv.qt.metainfo.xml` & `vimiv-0.9.0/misc/org.karlch.vimiv.qt.metainfo.xml`

```diff
@@ -39,14 +39,16 @@
   </screenshots>
   <url type="homepage">https://karlch.github.io/vimiv-qt</url>
   <url type="bugtracker">https://github.com/karlch/vimiv-qt/issues</url>
   <url type="help">https://karlch.github.io/vimiv-qt/documentation</url>
   <update_contact>ankursinha AT fedoraproject.org</update_contact>
   <releases>
     <!-- Add new releases here -->
+    <release version="0.9.0" date="2023-07-15"/>
+    <release version="0.8.0" date="2021-01-18"/>
     <release version="0.7.0" date="2020-05-17"/>
     <release version="0.6.1" date="2020-03-07"/>
     <release version="0.6.0" date="2020-03-07"/>
     <release version="0.5.0" date="2020-01-05"/>
     <release version="0.4.0" date="2019-12-01"/>
     <release version="0.3.0" date="2019-11-01"/>
     <release version="0.2.0" date="2019-10-01"/>
```

### Comparing `vimiv-0.8.0/misc/vimiv.1` & `vimiv-0.9.0/misc/vimiv.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "VIMIV" "1" "Jan 18, 2021" "" "vimiv"
-.SH NAME
-vimiv \- an image viewer with vim-like keybindings
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,17 +23,20 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "VIMIV" "1" "Jan 08, 2022" "" "vimiv"
+.SH NAME
+vimiv \- an image viewer with vim-like keybindings
 .SH SYNOPSIS
 .sp
-\fBvimiv\fP [\fBPATH\fP] [\fB\-h\fP] [\fB\-\-help\fP] [\fB\-f\fP] [\fB\-\-fullscreen\fP] [\fB\-v\fP] [\fB\-\-version\fP] [\fB\-g\fP \fIWIDTHxHEIGHT\fP] [\fB\-\-geometry\fP \fIWIDTHxHEIGHT\fP] [\fB\-\-temp\-basedir\fP] [\fB\-\-config\fP \fIFILE\fP] [\fB\-\-keyfile\fP \fIFILE\fP] [\fB\-s\fP \fIOPTION\fP \fIVALUE\fP] [\fB\-\-set\fP \fIOPTION\fP \fIVALUE\fP] [\fB\-\-log\-level\fP \fILEVEL\fP] [\fB\-\-command\fP \fICOMMAND\fP] [\fB\-b\fP \fIDIRECTORY\fP] [\fB\-\-basedir\fP \fIDIRECTORY\fP] [\fB\-\-debug\fP \fIMODULE\fP]
+\fBvimiv\fP [\fBPATH\fP] [\fB\-\-help\fP|\fB\-h\fP] [\fB\-\-fullscreen\fP|\fB\-f\fP] [\fB\-\-version\fP|\fB\-v\fP] [\fB\-\-geometry\fP \fIWIDTHxHEIGHT\fP|\fB\-g\fP \fIWIDTHxHEIGHT\fP] [\fB\-\-temp\-basedir\fP] [\fB\-\-config\fP \fIFILE\fP] [\fB\-\-keyfile\fP \fIFILE\fP] [\fB\-\-set\fP \fIOPTION\fP \fIVALUE\fP|\fB\-s\fP \fIOPTION\fP \fIVALUE\fP] [\fB\-\-log\-level\fP \fILEVEL\fP] [\fB\-\-command\fP \fICOMMAND\fP] [\fB\-\-basedir\fP \fIDIRECTORY\fP|\fB\-b\fP \fIDIRECTORY\fP] [\fB\-\-output\fP \fITEXT\fP|\fB\-o\fP \fITEXT\fP] [\fB\-\-input\fP|\fB\-i\fP] [\fB\-\-debug\fP \fIMODULE\fP] [\fB\-\-qt\-args\fP \fIARGS\fP]
 .SH DESCRIPTION
 .sp
 Vimiv is an image viewer with vim\-like keybindings. It is written in python3
 using the Qt5 toolkit and is free software, licensed under the GPL. Some of the
 features are:
 .INDENT 0.0
 .IP \(bu 2
@@ -50,46 +50,46 @@
 .IP \(bu 2
 Complete customization with style sheets
 .UNINDENT
 .sp
 A much more complete documentation can be found under
 \fI\%https://karlch.github.io/vimiv\-qt/\fP\&.
 .SH OPTIONS
-.SS positional arguments
+.SS POSITIONAL ARGUMENTS
 .sp
 \fBPATH\fP
 .INDENT 0.0
 .INDENT 3.5
 Paths to open
 .UNINDENT
 .UNINDENT
-.SS optional arguments
+.SS OPTIONS
 .sp
-\fB\-h\fP, \fB\-\-help\fP
+\fB\-\-help\fP, \fB\-h\fP
 .INDENT 0.0
 .INDENT 3.5
 show this help message and exit
 .UNINDENT
 .UNINDENT
 .sp
-\fB\-f\fP, \fB\-\-fullscreen\fP
+\fB\-\-fullscreen\fP, \fB\-f\fP
 .INDENT 0.0
 .INDENT 3.5
 Start fullscreen
 .UNINDENT
 .UNINDENT
 .sp
-\fB\-v\fP, \fB\-\-version\fP
+\fB\-\-version\fP, \fB\-v\fP
 .INDENT 0.0
 .INDENT 3.5
 Print version information and exit
 .UNINDENT
 .UNINDENT
 .sp
-\fB\-g\fP \fIWIDTHxHEIGHT\fP, \fB\-\-geometry\fP \fIWIDTHxHEIGHT\fP
+\fB\-\-geometry\fP \fIWIDTHxHEIGHT\fP, \fB\-g\fP \fIWIDTHxHEIGHT\fP
 .INDENT 0.0
 .INDENT 3.5
 Set the starting geometry
 .UNINDENT
 .UNINDENT
 .sp
 \fB\-\-temp\-basedir\fP
@@ -109,15 +109,15 @@
 \fB\-\-keyfile\fP \fIFILE\fP
 .INDENT 0.0
 .INDENT 3.5
 Use FILE as keybinding file
 .UNINDENT
 .UNINDENT
 .sp
-\fB\-s\fP \fIOPTION\fP \fIVALUE\fP, \fB\-\-set\fP \fIOPTION\fP \fIVALUE\fP
+\fB\-\-set\fP \fIOPTION\fP \fIVALUE\fP, \fB\-s\fP \fIOPTION\fP \fIVALUE\fP
 .INDENT 0.0
 .INDENT 3.5
 Set a temporary setting
 .UNINDENT
 .UNINDENT
 .sp
 \fB\-\-log\-level\fP \fILEVEL\fP
@@ -130,30 +130,51 @@
 \fB\-\-command\fP \fICOMMAND\fP
 .INDENT 0.0
 .INDENT 3.5
 Run COMMAND on startup, usable multiple times
 .UNINDENT
 .UNINDENT
 .sp
-\fB\-b\fP \fIDIRECTORY\fP, \fB\-\-basedir\fP \fIDIRECTORY\fP
+\fB\-\-basedir\fP \fIDIRECTORY\fP, \fB\-b\fP \fIDIRECTORY\fP
 .INDENT 0.0
 .INDENT 3.5
 Directory to use for all storage
 .UNINDENT
 .UNINDENT
-.SS development arguments
+.sp
+\fB\-\-output\fP \fITEXT\fP, \fB\-o\fP \fITEXT\fP
+.INDENT 0.0
+.INDENT 3.5
+Wildcard expanded string to print to standard output upon quit
+.UNINDENT
+.UNINDENT
+.sp
+\fB\-\-input\fP, \fB\-i\fP
+.INDENT 0.0
+.INDENT 3.5
+Read paths to open from standard input
+.UNINDENT
+.UNINDENT
+.SS DEVELOPMENT ARGUMENTS
 .sp
 \fB\-\-debug\fP \fIMODULE\fP
 .INDENT 0.0
 .INDENT 3.5
 Force showing debug log messages of MODULE
 .UNINDENT
 .UNINDENT
+.sp
+\fB\-\-qt\-args\fP \fIARGS\fP
+.INDENT 0.0
+.INDENT 3.5
+Arguments to pass to qt directly, use quotes to pass multiple arguments
+.UNINDENT
+.UNINDENT
 .SH WEBSITE
 .sp
 \fI\%https://karlch.github.io/vimiv\-qt/\fP
 .SH AUTHOR
 Christian Karl
 .SH COPYRIGHT
-2017-2020, Christian Karl
+2017-2022, Christian Karl
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `vimiv-0.8.0/setup.py` & `vimiv-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 import ast
 import os
 import re
 import setuptools
 
@@ -21,29 +21,29 @@
     BASEDIR = os.path.dirname(os.path.realpath(__file__))
 except NameError:
     BASEDIR = None
 
 
 def read_file(filename):
     """Read content of filename into string and return it."""
-    with open(filename) as f:
+    with open(filename, encoding="utf-8") as f:
         return f.read()
 
 
 def read_from_init(name):
     """Read value of a __magic__ value from the __init__.py file."""
     field_re = re.compile(r"__{}__\s+=\s+(.*)".format(re.escape(name)))
     path = os.path.join(BASEDIR, "vimiv", "__init__.py")
     line = field_re.search(read_file(path)).group(1)
     return ast.literal_eval(line)
 
 
 setuptools.setup(
-    python_requires=">=3.6",
-    install_requires=["PyQt5>=5.9.2"],
+    python_requires=">=3.8",
+    install_requires=["PyQt5>=5.13.2"],
     packages=setuptools.find_packages(),
     ext_modules=[manipulate_module],
     entry_points={"gui_scripts": ["vimiv = vimiv.startup:main"]},
     name="vimiv",
     version=".".join(str(num) for num in read_from_init("version_info")),
     description=read_from_init("description"),
     long_description=read_file(os.path.join(BASEDIR, "README.md")),
@@ -63,16 +63,16 @@
         "Development Status :: 4 - Beta",
         "Environment :: X11 Applications :: Qt",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: GNU General Public License v3 or later " "(GPLv3+)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Multimedia",
         "Topic :: Multimedia :: Graphics",
         "Topic :: Multimedia :: Graphics :: Viewers",
     ],
 )
```

### Comparing `vimiv-0.8.0/vimiv/__init__.py` & `vimiv-0.9.0/vimiv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """An image viewer with vim-like keybindings based on PyQt5."""
 
 import vimiv.checkversion
 
 __license__ = "GPL3"
-__version_info__ = (0, 8, 0)
+__version_info__ = (0, 9, 0)
 __version__ = ".".join(str(num) for num in __version_info__)
 __author__ = "Christian Karl"
 __maintainer__ = __author__
 __email__ = "karlch@protonmail.com"
 __description__ = "An image viewer with vim-like keybindings."
 __url__ = "https://karlch.github.io/vimiv-qt/"
```

### Comparing `vimiv-0.8.0/vimiv/api/__init__.py` & `vimiv-0.9.0/vimiv/api/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """`Utilities to interact with the application`."""
 
 import os
 from typing import List, Iterable, Callable, BinaryIO
 from PyQt5.QtGui import QPixmap
 
-from vimiv.utils import files, imagereader
+from vimiv.utils import files, imagereader, imageheader
 
 from vimiv.api import (
     commands,
     completion,
     keybindings,
     modes,
     objreg,
@@ -60,14 +60,17 @@
     """Open one or more paths.
 
     **syntax:** ``:open path [path ...]``
 
     If any path given is an image, all valid images are opened in image mode. Otherwise
     the first valid directory is opened. If both fails, an error is displayed.
 
+    .. hint:: Passing a single directory therefore changes the directory in the library,
+        think ``cd``.
+
     positional arguments:
         * ``paths``: The path(s) to open.
     """
     images, directories = files.supported(paths)
     if images:
         working_directory.handler.chdir(os.path.dirname(images[0]))
         signals.load_images.emit(images)
@@ -77,19 +80,21 @@
         modes.LIBRARY.enter()
     else:
         raise commands.CommandError("No valid paths")
 
 
 def add_external_format(
     file_format: str,
-    test_func: Callable[[bytes, BinaryIO], bool],
+    test_func: imageheader.CheckFuncT,
     load_func: Callable[[str], QPixmap],
 ) -> None:
     """Add support for new fileformat.
 
     Args:
         file_format: String value of the file type
         test_func: Function returning True if load_func supports this type.
         load_func: Function to load a QPixmap from the passed path.
     """
-    files.add_image_format(file_format, test_func)
+    # Prioritize external formats over all default formats, to ensure that on signature
+    # collision, the explicitly registered handler is used.
+    imageheader.register(file_format, test_func, priority=True)
     imagereader.external_handler[file_format] = load_func
```

### Comparing `vimiv-0.8.0/vimiv/api/_mark.py` & `vimiv-0.9.0/vimiv/api/_mark.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Mark and tag images."""
 
 
+import enum
 import os
 import shutil
 from typing import Any, Callable, List, Optional
 
 from PyQt5.QtCore import QObject, pyqtSignal, QFileSystemWatcher, QDateTime
 
 from vimiv.api import commands, keybindings, objreg, status, settings, modes
@@ -32,25 +33,37 @@
     Attributes:
         _indicator: Attribute to cache the evaluated mark indicator string.
         _marked: List of all currently marked images.
         _last_marked: List of images that were marked before clearing.
         _watcher: QFileSystemWatcher to monitor marked paths.
     """
 
+    class Action(enum.Enum):
+        """Valid action options for the mark command."""
+
+        Toggle = "toggle"
+        Mark = "mark"
+        Unmark = "unmark"
+
     marked = pyqtSignal(str)
     unmarked = pyqtSignal(str)
     markdone = pyqtSignal()
 
     @objreg.register
     def __init__(self) -> None:
         super().__init__()
         self._indicator: Optional[str] = None
         self._marked: List[str] = []
         self._last_marked: List[str] = []
         self._watcher: Optional[QFileSystemWatcher] = None
+        self._actions = {
+            Mark.Action.Toggle: self._toggle_mark,
+            Mark.Action.Mark: self._mark,
+            Mark.Action.Unmark: self._unmark,
+        }
 
     @property
     def tagdir(self) -> str:
         """Path to the tag directory."""
         return Tag.dirname()
 
     @property
@@ -58,35 +71,46 @@
         """The QFileSystemWatcher to monitor marked paths.
 
         This is required as during __init__ the QApplication is not created yet.
         """
         if self._watcher is None:
             _logger.debug("Creating watcher to monitor marked paths")
             self._watcher = QFileSystemWatcher()
-            self._watcher.fileChanged.connect(self._on_file_changed)  # type: ignore
+            self._watcher.fileChanged.connect(self._on_file_changed)
         return self._watcher
 
+    def is_marked(self, path: str) -> bool:
+        """Return True if the passed path is marked."""
+        return path in self._marked
+
     @keybindings.register("m", "mark %")
     @commands.register()
-    def mark(self, paths: List[str]) -> None:
+    def mark(self, paths: List[str], action: Action = Action.Toggle) -> None:
         """Mark one or more paths.
 
-        **syntax:** ``:mark path [path ...]``
-
-        If a path is currently marked, it is unmarked instead.
+        **syntax:** ``:mark path [path ...] [--action=ACTION]``
 
         .. hint:: ``:mark %`` marks the current path.
 
         positional arguments:
             * ``paths``: The path(s) to mark.
+
+        optional arguments:
+            * ``--action``: One of toggle/mark/unmark. Toggle, the default, inverses the
+              mark status of the path(s). Mark forces marking while unmark forces
+              removing the mark.
         """
-        _logger.debug("Marking %d paths", len(paths))
+        _logger.debug("Calling %s on %d paths", action.value, len(paths))
+        function = self._actions[action]
         for path in paths:
             if files.is_image(path):
-                self._toggle_mark(path)
+                try:
+                    function(path)
+                except ValueError:
+                    _logger.debug("Calling %s on '%s' failed", action.value, path)
         self.markdone.emit()
 
     @commands.register()
     def mark_clear(self) -> None:
         """Clear all marks.
 
         .. hint::
@@ -260,14 +284,16 @@
     def _on_file_changed(self, path: str) -> None:
         """Unmark deleted paths."""
         if not os.path.exists(path):
             self._unmark(path)
 
     def _mark(self, path: str) -> None:
         """Mark the given path."""
+        if self.is_marked(path):
+            raise ValueError(f"Path '{path}' is already marked")
         self._marked.append(path)
         self.marked.emit(path)
         self.watcher.addPath(path)
         _logger.debug("Marked '%s'", path)
 
     def _unmark(self, path: str) -> None:
         """Unmark the given path."""
@@ -306,15 +332,17 @@
         self.name = name
         abspath = Tag.path(name)
         exists = os.path.isfile(abspath)
         self._mode = "r" if read_only else ("r+" if exists else "a+")
         _logger.debug("Opened tag object: '%s'", self)
         xdg.makedirs(os.path.dirname(abspath))
         try:
-            self._file = open(abspath, self._mode)
+            # We are writing our own context-manager here
+            # pylint: disable=consider-using-with
+            self._file = open(abspath, self._mode, encoding="utf-8")
         except FileNotFoundError:  # For read-only if the file does not exist
             raise commands.CommandError(f"No tag called '{name}'")
         except OSError as e:
             raise commands.CommandError(f"Error reading '{name}': {e}")
 
         if read_only:
             _logger.debug("%s: Reading tag file", self)
```

### Comparing `vimiv-0.8.0/vimiv/api/commands.py` & `vimiv-0.9.0/vimiv/api/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """`Command storage and initialization`.
 
 The user interacts with vimiv using commands. Creating a new command is done
 using the :func:`register` decorator. The command name is directly inferred from
 the function name, the functions docstring is used to document the command. The
@@ -45,15 +45,16 @@
     @commands.register()
     def hello_planet(name: str = "earth", count: int = 1):
         for i in range(count):
             print("hello", name)
 
 Another special argument is the ``paths`` argument. It will perform unix-style pattern
 matching using the ``glob`` module on each path given and return a list of matched
-paths. An example of this in action is the ``:open`` command defined in ``vimiv.app``.
+paths. An example of this in action is the ``:open`` command defined in ``vimiv.api`` in
+the ``open_paths`` function.
 
 Each command is valid for a specific mode, the default being global. To supply
 the mode, add it to the register decorator::
 
     @commands.register(mode=Modes.IMAGE)
     def ...
 
@@ -72,15 +73,15 @@
 import argparse
 import contextlib
 import glob
 import inspect
 import os
 import typing
 
-from vimiv.api import modes, objreg
+from vimiv.api import modes, objreg, settings
 from vimiv.utils import (
     flatten,
     log,
     customtypes,
     escape_glob,
     is_optional_type,
     type_of_optional,
@@ -90,27 +91,29 @@
 _logger = log.module_logger(__name__)
 
 
 def register(
     mode: modes.Mode = modes.GLOBAL,
     hide: bool = False,
     store: bool = True,
+    edit: bool = False,
     name: str = None,
 ) -> typing.Callable[[customtypes.FuncT], customtypes.FuncT]:
     """Decorator to store a command in the registry.
 
     Args:
         mode: Mode in which the command can be executed.
         hide: Hide command from command line.
         store: Save command to allow repeating with '.'.
+        edit: Command may make changes on disk.
         name: Name of the command if it should not be inferred from the function name.
     """
 
     def decorator(func: customtypes.FuncT) -> customtypes.FuncT:
-        _Command(func, mode=mode, hide=hide, store=store, name=name)
+        _Command(func, mode=mode, hide=hide, store=store, name=name, edit=edit)
         return func
 
     return decorator
 
 
 def get(name: str, mode: modes.Mode = modes.GLOBAL) -> "_Command":
     """Get one command object.
@@ -196,19 +199,19 @@
             self._add_argument(argument, annotations.get(argument.name, None))
 
     def print_help(self, _file: typing.IO = None) -> typing.NoReturn:
         """Override help message to display in statusbar."""
         raise CommandInfo(self.description)
 
     def parse_args(self, args: typing.List[str]) -> argparse.Namespace:  # type: ignore
-        """Override parse_args to sort and flatten paths list in addition."""
+        """Override parse_args to flatten paths list in addition."""
         parsed_args = super().parse_args(args)
         with contextlib.suppress(AttributeError):
             parsed_args.paths = [
-                os.path.abspath(path) for path in sorted(flatten(parsed_args.paths))
+                os.path.abspath(path) for path in flatten(parsed_args.paths)
             ]
         return parsed_args
 
     def error(self, message: str) -> typing.NoReturn:
         """Override error to raise an exception instead of calling sys.exit."""
         if message.startswith("argument"):  # Remove argument argname:
             message = " ".join(message.split(":")[1:])
@@ -273,31 +276,34 @@
         func: Corresponding executable to call.
         mode: Mode in which the command can be executed.
         hide: Hide command from command line.
         store: Save command to allow repeating with '.'.
         description: Brief command description.
 
         _argparser: Argument parser used when the command is called.
+        _edit: The command may make changes on disk.
         _long_description: Full command description.
     """
 
     def __init__(
         self,
         func: typing.Callable,
         mode: modes.Mode = modes.GLOBAL,
         hide: bool = False,
         store: bool = True,
+        edit: bool = False,
         name: str = None,
     ):
         self._argparser: typing.Optional[_CommandArguments] = None
         self.name = _get_command_name(func) if name is None else name
         self.func = func
         self.mode = mode
         self.hide = hide
         self.store = store
+        self._edit = edit
         # Retrieve description from docstring
         docstr = inspect.getdoc(func)
         if docstr is None:
             _logger.error("Command %s for %s is missing docstring.", self.name, func)
             self.description = self.long_description = ""
         else:
             self.description = docstr.split("\n", maxsplit=1)[0]
@@ -308,14 +314,16 @@
     def __call__(self, args: typing.List[str], count: str) -> None:
         """Parse arguments and call func.
 
         Args:
             args: List of arguments for argparser to parse.
             count: Count passed to the command.
         """
+        if self._edit and settings.read_only:
+            raise CommandError("Disabled due to read-only being active")
         parsed_args = self.argparser.parse_args(args)
         kwargs = vars(parsed_args)
         self._parse_count(count, kwargs)
         objreg._call_with_instance(self.func, **kwargs)
 
     @property
     def argparser(self) -> _CommandArguments:
```

### Comparing `vimiv-0.8.0/vimiv/api/completion.py` & `vimiv-0.9.0/vimiv/api/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """*Utilities to work with completion modules*.
 
 A completion module offers a model with options for command line completion and a filter
 that decides which results are filtered depending on the text in the command line. All
 completion models inherit from the :class:`BaseModel` class.
```

### Comparing `vimiv-0.8.0/vimiv/api/keybindings.py` & `vimiv-0.9.0/vimiv/api/keybindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """`Utilities to map commands to a sequence of keys`.
 
 Adding a new default keybinding is done using the :func:`register` decorator.
 This decorator requires the sequence of keys to bind to as first argument, the
 command as second argument and, similar to :func:`vimiv.api.commands.register`
```

### Comparing `vimiv-0.8.0/vimiv/api/modes.py` & `vimiv-0.9.0/vimiv/api/modes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """`Default modes and utility functions for mode handling`.
 
 Similar to vim, vimiv has the concept of ``modes``. The same command or
 keybinding can perform different actions depending on the mode it is executed
 in. Each mode is assigned to a ``QWidget`` class which is focused when this
@@ -30,14 +30,15 @@
 
 import abc
 from typing import cast, Any, Callable, List, Tuple
 
 from PyQt5.QtCore import pyqtSignal, QObject
 from PyQt5.QtWidgets import QWidget
 
+from vimiv.api import settings
 from vimiv.utils import AbstractQObjectMeta, log
 
 
 _logger = log.module_logger(__name__)
 
 
 class InvalidMode(Exception):
@@ -198,26 +199,23 @@
     for mode in ALL:
         if mode.name.lower() == name.lower():
             return mode
     raise InvalidMode(f"'{name.upper()}' is not a valid mode")
 
 
 class _ModeWidget(QWidget):
-    """Helper class defining the requirements for mode widgets.
-
-    This should in principle be solved using protocols, but these are only available
-    starting from python 3.8 and we still support python 3.6.
-    See https://docs.python.org/3/library/typing.html#typing.Protocol for more details.
-    """
+    """Helper class defining the requirements for mode widgets."""
 
     def current(self) -> str:
         """Return the current path valid for this mode."""
+        raise NotImplementedError("Do not use _ModeWidget directly")
 
     def pathlist(self) -> List[str]:
         """Return the current list of paths valid for this mode."""
+        raise NotImplementedError("Do not use _ModeWidget directly")
 
 
 def widget(mode: Mode) -> Callable:
     """Decorator to assign a widget to a mode.
 
     The decorator decorates the __init__ function of a QWidget class storing
     the created component as the widget associated to the mode. This is used
@@ -267,22 +265,33 @@
 
     def _set_last(self, mode: Mode) -> None:
         """Store any mode except for command."""
         if mode != self:
             self._last = mode
 
 
+class _ManipulateMode(_MainMode):
+    """Manipulate mode class."""
+
+    def enter(self) -> None:
+        """Override enter to ensure we are not in read-only mode when manipulating."""
+        if settings.read_only:
+            log.error("Manipulate mode is disabled due to read-only being active")
+        else:
+            super().enter()
+
+
 # Create all modes
 GLOBAL = _MainMode("global")
 IMAGE = _MainMode("image")
 Mode.active = IMAGE
 LIBRARY = _MainMode("library", last=IMAGE)
 THUMBNAIL = _MainMode("thumbnail", last=IMAGE)
 COMMAND = _CommandMode("command", last=IMAGE)
-MANIPULATE = _MainMode("manipulate", last=IMAGE)
+MANIPULATE = _ManipulateMode("manipulate", last=IMAGE)
 # This cannot be done in the constructor as the constructor of LIBRARY requires IMAGE
 # and vice-versa
 IMAGE.last = IMAGE.last_fallback = LIBRARY
 
 # Utility tuples to allow iterating
 ALL: Tuple[Mode, ...] = (GLOBAL, IMAGE, LIBRARY, THUMBNAIL, COMMAND, MANIPULATE)
 GLOBALS: Tuple[Mode, ...] = (IMAGE, LIBRARY, THUMBNAIL)
```

### Comparing `vimiv-0.8.0/vimiv/api/objreg.py` & `vimiv-0.9.0/vimiv/api/objreg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """*Storage system for objects*.
 
 The object registry is a storage system for long-lived objects. These objects are stored
 and identified using their type. Therefore every stored object must be unique in its
 type and only one instance of each type can be stored. Purpose of this registry is to
```

### Comparing `vimiv-0.8.0/vimiv/api/prompt.py` & `vimiv-0.9.0/vimiv/api/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Prompt the user for a question."""
 
 import typing
 
 from PyQt5.QtCore import QObject, pyqtSignal
```

### Comparing `vimiv-0.8.0/vimiv/api/settings.py` & `vimiv-0.9.0/vimiv/api/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Store and change settings.
 
 Module attributes:
     _storage: Initialized Storage object to store settings globally.
 """
 
 import abc
 import contextlib
 import enum
-from typing import Any, Dict, ItemsView, List
+import os
+from typing import Any, Dict, ItemsView, List, Callable, Iterable
 
 from PyQt5.QtCore import QObject, pyqtSignal
 
 from vimiv.api import prompt
-from vimiv.utils import clamp, AbstractQObjectMeta, log, customtypes
+from vimiv.utils import clamp, AbstractQObjectMeta, log, customtypes, natural_sort
 
 
 _storage: Dict[str, "Setting"] = {}
 _logger = log.module_logger(__name__)
 
 
 def get(name: str) -> "Setting":
@@ -311,29 +312,85 @@
 
     typ = str
 
     def __str__(self) -> str:
         return "String"
 
 
-# Initialize all settings
+class OrderSetting(Setting):
+    """Stores an ordering setting."""
+
+    typ = str
+
+    ORDER_TYPES: Dict[str, Callable[..., Any]] = {
+        "alphabetical": str,
+        "natural": natural_sort,
+        "recently-modified": os.path.getmtime,
+        "none": lambda x: 0,
+    }
+
+    STR_ORDER_TYPES = "alphabetical", "natural"
+
+    def __init__(
+        self,
+        *args: Any,
+        additional_order_types: Dict[str, Callable[..., Any]] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(*args, **kwargs)
+        self.order_types = dict(self.ORDER_TYPES)
+        if additional_order_types:
+            self.order_types.update(additional_order_types)
+
+    def convert(self, value: str) -> str:
+        if value not in self.order_types:
+            raise ValueError(f"Option must be one of {', '.join(self.order_types)}")
+        return value
+
+    def sort(self, values: Iterable[str]) -> List[str]:
+        """Sort values according to the current ordering."""
+        ordering = self._get_ordering()
+        return sorted(values, key=ordering, reverse=sort.reverse.value)
+
+    def suggestions(self) -> List[str]:
+        return list(self.order_types)
+
+    def _get_ordering(self) -> Callable[..., Any]:
+        """Retrieve current ordering function.
+
+        Respects the sort.ignore_case setting and applies os.path.basename to
+        string-like orderings.
+        """
+        ordering = self.order_types[self.value]
+        if self.value not in self.STR_ORDER_TYPES:
+            return ordering
+        if sort.ignore_case.value:
+            return lambda s: ordering(os.path.basename(s).lower())
+        return lambda s: ordering(os.path.basename(s))
+
+    def __str__(self) -> str:
+        return "Order"
+
 
+# Initialize all settings
 monitor_fs = BoolSetting(
     "monitor_filesystem",
     True,
     desc="Monitor current directory for changes and reload widgets automatically",
 )
-shuffle = BoolSetting("shuffle", False, desc="Randomly shuffle images")
 startup_library = BoolSetting(
     "startup_library",
     True,
     desc="Enter library at startup if there are no images to show",
     hidden=True,
 )
 style = StrSetting("style", "default", hidden=True)
+read_only = BoolSetting(
+    "read_only", False, desc="Disable any commands that are able to edit files on disk"
+)
 
 
 class command:  # pylint: disable=invalid-name
     """Namespace for command related settings."""
 
     history_limit = IntSetting(
         "command.history_limit",
@@ -382,14 +439,19 @@
     overzoom = FloatSetting(
         "image.overzoom",
         1.0,
         desc="Maximum scale to apply trying to fit image to window",
         suggestions=["1.0", "1.5", "2.0", "5.0"],
         min_value=1.0,
     )
+    zoom_wheel_ctrl = BoolSetting(
+        "image.zoom_wheel_ctrl",
+        True,
+        desc="Require holding the control modifier for zooming with the mouse wheel",
+    )
 
 
 class library:  # pylint: disable=invalid-name
     """Namespace for library related settings."""
 
     width = FloatSetting(
         "library.width",
@@ -404,14 +466,19 @@
     )
 
 
 class thumbnail:  # pylint: disable=invalid-name
     """Namespace for thumbnail related settings."""
 
     size = ThumbnailSizeSetting("thumbnail.size", 128, desc="Size of thumbnails")
+    save = BoolSetting(
+        "thumbnail.save",
+        True,
+        desc="Save new thumbnails to disk in the shared icon cache for later use",
+    )
 
 
 class slideshow:  # pylint: disable=invalid-name
     """Namespace for slideshow related settings."""
 
     delay = FloatSetting(
         "slideshow.delay", 2.0, desc="Delay to next image in slideshow", min_value=0.5
@@ -438,19 +505,21 @@
     )
     mark_indicator = StrSetting(
         "statusbar.mark_indicator",
         "<b>*</b>",
         desc="Text to display if the current image is marked",
     )
     # Statusbar module strings, these are not retrieved by their type
-    StrSetting("statusbar.left", "{pwd}")
-    StrSetting("statusbar.left_image", "{index}/{total} {basename} [{zoomlevel}]")
+    StrSetting("statusbar.left", "{pwd}{read-only}")
+    StrSetting(
+        "statusbar.left_image", "{index}/{total} {basename}{read-only} [{zoomlevel}]"
+    )
     StrSetting(
         "statusbar.left_thumbnail",
-        "{thumbnail-index}/{thumbnail-total} {thumbnail-name}",
+        "{thumbnail-index}/{thumbnail-total} {thumbnail-basename}{read-only}",
     )
     StrSetting(
         "statusbar.left_manipulate",
         "{basename}   {image-size}   Modified: {modified}   {processing}",
     )
     StrSetting("statusbar.center_thumbnail", "{thumbnail-size}")
     StrSetting(
@@ -491,21 +560,59 @@
 
 
 class metadata:  # pylint: disable=invalid-name
     """Namespace for metadata related settings."""
 
     # Default sets
     defaults = [
-        "Exif.Image.Make, Exif.Image.Model, Exif.Image.DateTime, Exif.Photo.ExposureTime, Exif.Photo.FNumber, Exif.Photo.IsoSpeedRatings, Exif.Photo.FocalLength, Exif.Photo.LensMake, Exif.Photo.LensModel, Exif.Photo.ExposureBiasValue",  # pylint: disable=line-too-long,useless-suppression
-        "Exif.Photo.ExposureTime, Exif.Photo.FNumber, Exif.Photo.IsoSpeedRatings, Exif.Photo.FocalLength",  # pylint: disable=line-too-long,useless-suppression
-        "Exif.Image.Artist, Exif.Image.Copyright",
+        "Exif.Image.Make,Exif.Image.Model,Exif.Photo.LensModel,Exif.Image.DateTime,Exif.Image.Artist,Exif.Image.Copyright",  # pylint: disable=line-too-long,useless-suppression
+        "Exif.Photo.ExposureTime,Exif.Photo.FNumber,Exif.Photo.ISOSpeedRatings,Exif.Photo.ApertureValue,Exif.Photo.ExposureBiasValue,Exif.Photo.FocalLength,Exif.Photo.ExposureProgram",  # pylint: disable=line-too-long,useless-suppression
+        "Exif.GPSInfo.GPSLatitudeRef,Exif.GPSInfo.GPSLatitude,Exif.GPSInfo.GPSLongitudeRef,Exif.GPSInfo.GPSLongitude,Exif.GPSInfo.GPSAltitudeRef,Exif.GPSInfo.GPSAltitude",  # pylint: disable=line-too-long,useless-suppression
+        "Iptc.Application2.Caption,Iptc.Application2.Keywords,Iptc.Application2.City,Iptc.Application2.SubLocation,Iptc.Application2.ProvinceState,Iptc.Application2.CountryName,Iptc.Application2.Source,Iptc.Application2.Credit,Iptc.Application2.Copyright,Iptc.Application2.Contact",  # pylint: disable=line-too-long,useless-suppression
+        "Exif.Image.ImageWidth,Exif.Image.ImageLength,Exif.Photo.PixelXDimension,Exif.Photo.PixelYDimension,Exif.Image.BitsPerSample,Exif.Image.Compression,Exif.Photo.ColorSpace",  # pylint: disable=line-too-long,useless-suppression
     ]
 
     # Store the keys as a comma separated string
     current_keyset = StrSetting(
         "metadata.current_keyset",
         defaults[0],
         desc="Currently displayed metadata keyset",
         suggestions=defaults,
     )
 
     keysets: Dict[int, str] = dict(enumerate(defaults, start=1))
+
+
+class sort:  # pylint: disable=invalid-name
+    """Namespace for sorting related settings."""
+
+    image_order = OrderSetting(
+        "sort.image_order",
+        "alphabetical",
+        desc="Ordering of images, e.g. in the library",
+        additional_order_types={
+            "size": os.path.getsize,
+        },
+    )
+    directory_order = OrderSetting(
+        "sort.directory_order",
+        "alphabetical",
+        desc="Ordering of directories, e.g. in the library",
+        additional_order_types={
+            "size": lambda d: len(os.listdir(d)),
+        },
+    )
+    reverse = BoolSetting(
+        "sort.reverse",
+        False,
+        desc="Reverse the order of sorting, i.e. z before a, largest first, etc.",
+    )
+    ignore_case = BoolSetting(
+        "sort.ignore_case",
+        False,
+        desc="Ignore case when sorting, i.e. 'A' and 'a' are equal",
+    )
+    shuffle = BoolSetting(
+        "sort.shuffle",
+        False,
+        desc="Randomly shuffle images and ignoring all other sort settings",
+    )
```

### Comparing `vimiv-0.8.0/vimiv/api/signals.py` & `vimiv-0.9.0/vimiv/api/signals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Namespace for signals exposed via the api."""
 
 from PyQt5.QtCore import QObject, pyqtSignal
 from PyQt5.QtGui import QPixmap, QMovie
 
@@ -31,14 +31,16 @@
             arg2: True if it is only reloaded.
         movie_loaded: Emitted when the file handler loaded a new animation.
             arg1: The QMovie loaded.
             arg2: True if it is only reloaded.
         svg_loaded: Emitted when the file handler loaded a new vector graphic.
             arg1: The path as the VectorGraphic class is constructed directly.
             arg2: True if it is only reloaded.
+
+        plugins_loaded: Emitted when the user plugins have been loaded.
     """
 
     # Emitted when new images should be loaded
     load_images = pyqtSignal(list)
 
     # Emitted when new image path(s) were opened
     new_image_opened = pyqtSignal(str, bool)
@@ -49,19 +51,23 @@
     image_changed = pyqtSignal()
 
     # Tell the image to get a new object to display
     pixmap_loaded = pyqtSignal(QPixmap, bool)
     movie_loaded = pyqtSignal(QMovie, bool)
     svg_loaded = pyqtSignal(str, bool)
 
+    # Plugins loaded
+    plugins_loaded = pyqtSignal()
+
 
 _signal_handler = _SignalHandler()  # Instance of Qt signal handler to work with
 
 # Convenience access to the signals
 load_images = _signal_handler.load_images
 new_image_opened = _signal_handler.new_image_opened
 new_images_opened = _signal_handler.new_images_opened
 all_images_cleared = _signal_handler.all_images_cleared
 image_changed = _signal_handler.image_changed
 pixmap_loaded = _signal_handler.pixmap_loaded
 movie_loaded = _signal_handler.movie_loaded
 svg_loaded = _signal_handler.svg_loaded
+plugins_loaded = _signal_handler.plugins_loaded
```

### Comparing `vimiv-0.8.0/vimiv/api/status.py` & `vimiv-0.9.0/vimiv/api/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """*Utilities to add status modules and retrieve status text*.
 
 Status objects in vimiv, e.g. the statusbar displayed at the bottom, are
 configurable using so called status modules. These are created using the
 :func:`module` decorator.  As an example let's create a module that returns the
```

### Comparing `vimiv-0.8.0/vimiv/api/working_directory.py` & `vimiv-0.9.0/vimiv/api/working_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 r"""Handler to take care of the current working directory.
 
 The handler stores the current working directory and provides the :func:`chdir` method
 to change it::
 
@@ -105,27 +105,32 @@
     def __init__(self) -> None:
         super().__init__()
         self._dir = ""
         self._images: List[str] = []
         self._directories: List[str] = []
 
         settings.monitor_fs.changed.connect(self._on_monitor_fs_changed)
-        # TODO Fix upstream and open PR
-        self.directoryChanged.connect(self._reload_directory)  # type: ignore
-        self.fileChanged.connect(self._on_file_changed)  # type: ignore
+        settings.sort.image_order.changed.connect(self._reorder_directory)
+        settings.sort.directory_order.changed.connect(self._reorder_directory)
+        settings.sort.reverse.changed.connect(self._reorder_directory)
+        settings.sort.ignore_case.changed.connect(self._reorder_directory)
+
+        self.directoryChanged.connect(self._reload_directory)
+        self.fileChanged.connect(self._on_file_changed)
+
         signals.new_image_opened.connect(self._on_new_image)
 
     @property
     def images(self) -> List[str]:
         """List of images in the current working directory."""
         return self._images
 
     def chdir(self, directory: str, reload_current: bool = False) -> None:
         """Change the current working directory to directory."""
-        directory = os.path.abspath(directory)
+        directory = os.path.realpath(directory)
         if directory != self._dir or reload_current:
             _logger.debug("Changing directory to '%s'", directory)
             if self.directories():  # Unmonitor old directories
                 self.removePaths(self.directories())
             try:
                 os.chdir(directory)
                 self._load_directory(directory)
@@ -215,20 +220,34 @@
             self._directories = directories
             self.changed.emit(images, directories)
 
     def _get_content(self, directory: str) -> Tuple[List[str], List[str]]:
         """Get supported content of directory.
 
         Returns:
-            images: List of images inside the directory.
-            directories: List of directories inside the directory.
+            images: Ordered list of images inside the directory.
+            directories: Ordered list of directories inside the directory.
         """
         show_hidden = settings.library.show_hidden.value
         paths = files.listdir(directory, show_hidden=show_hidden)
-        return files.supported(paths)
+        return self._order_paths(*files.supported(paths))
+
+    @slot
+    def _reorder_directory(self) -> None:
+        """Reorder current files / directories."""
+        _logger.debug("Reloading working directory")
+        self._emit_changes(*self._order_paths(self._images, self._directories))
+
+    @staticmethod
+    def _order_paths(images: List[str], dirs: List[str]) -> Tuple[List[str], List[str]]:
+        """Order images and directories according to the current ordering setting."""
+        return (
+            settings.sort.image_order.sort(images),
+            settings.sort.directory_order.sort(dirs),
+        )
 
 
 handler = cast(WorkingDirectoryHandler, None)
 
 
 def init() -> None:
     """Initialize handler.
```

### Comparing `vimiv-0.8.0/vimiv/app.py` & `vimiv-0.9.0/vimiv/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Main application class using QApplication."""
 
 import os
 
 from PyQt5.QtGui import QIcon
@@ -18,17 +18,22 @@
 _logger = utils.log.module_logger(__name__)
 
 
 class Application(QApplication):
     """Main application class."""
 
     @api.objreg.register
-    def __init__(self) -> None:
-        """Initialize the main Qt application."""
-        super().__init__([vimiv.__name__])  # Only pass program name to Qt
+    def __init__(self, *qtargs: str) -> None:
+        """Initialize the main Qt application.
+
+        Args:
+            qtargs: Arguments passed directly to the QApplication.
+        """
+        _logger.debug("Passing %s to qt", utils.quotedjoin(qtargs))
+        super().__init__([vimiv.__name__, *qtargs])
         self.setApplicationVersion(vimiv.__version__)
         self.setDesktopFileName(vimiv.__name__)
         self._set_icon()
 
     @staticmethod
     @api.keybindings.register("q", "quit")
     @api.commands.register()
```

### Comparing `vimiv-0.8.0/vimiv/checkversion.py` & `vimiv-0.9.0/vimiv/checkversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Check version and availability of required software upon import.
 
 This module is imported first in the top-level __init__.py to ensure we are running with
 the correct python and PyQt versions. In case this fails, error messages are written to
 stderr and we exit with returncode ERR_CODE.
@@ -24,16 +24,16 @@
 
     PYQT_VERSION = tuple(map(int, PYQT_VERSION_STR.split(".")))
 except ImportError:  # pragma: no cover  # PyQt is there in tests, using None is tested
     # We check explicitly for None before using the tuple version
     PYQT_VERSION = None  # type: ignore
 
 
-PYTHON_REQUIRED_VERSION = (3, 6)
-PYQT_REQUIRED_VERSION = (5, 9, 2)
+PYTHON_REQUIRED_VERSION = (3, 8)
+PYQT_REQUIRED_VERSION = (5, 13, 2)
 ERR_CODE = 2
 
 
 def check_python_version():
     """Ensure the python version is new enough."""
     if sys.version_info < PYTHON_REQUIRED_VERSION:
         _exit_version("python", PYTHON_REQUIRED_VERSION, sys.version_info[:3])
@@ -49,14 +49,16 @@
 
 def join_version_tuple(version):
     return ".".join(map(str, version))
 
 
 def _exit_version(software, required, installed):
     """Call exit for out-of-date software."""
+    # This module needs to work for python < 3.6
+    # pylint: disable=consider-using-f-string
     _exit(
         "At least %s %s is required to run vimiv. Using %s.\n"
         % (software, join_version_tuple(required), join_version_tuple(installed))
     )
 
 
 def _exit(message):
```

### Comparing `vimiv-0.8.0/vimiv/commands/__init__.py` & `vimiv-0.9.0/vimiv/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions to store and run commands."""
 
 from typing import cast
```

### Comparing `vimiv-0.8.0/vimiv/commands/aliases.py` & `vimiv-0.9.0/vimiv/commands/aliases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Class and functions to add and get aliases.
 
 Module Attribute:
     _aliases: Dictionary storing aliases initialized with defaults.
 """
@@ -15,15 +15,15 @@
 from vimiv import api
 
 Aliases = Dict[str, str]
 
 
 _aliases: Dict[api.modes.Mode, Aliases] = {mode: {} for mode in api.modes.ALL}
 # Add default aliases
-_aliases[api.modes.GLOBAL].update(q="quit")
+_aliases[api.modes.GLOBAL].update({"q": "quit", "mark-print": "print-stdout %m"})
 _aliases[api.modes.IMAGE].update(w="write", wq="write && quit")
 
 
 def get(mode: api.modes.Mode) -> Aliases:
     """Return all aliases for the mode 'mode'."""
     if mode in api.modes.GLOBALS:
         return {**_aliases[api.modes.GLOBAL], **_aliases[mode]}
```

### Comparing `vimiv-0.8.0/vimiv/commands/external.py` & `vimiv-0.9.0/vimiv/commands/external.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Runner for external commands."""
 
 import os
 import glob
 import shlex
```

### Comparing `vimiv-0.8.0/vimiv/commands/help_command.py` & `vimiv-0.9.0/vimiv/commands/help_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions to format and retrieve text for the :help command."""
 
 import contextlib
 
 import vimiv
@@ -46,17 +46,16 @@
         f"<br>Website: {vimiv.__url__}<br><br>"
         "For an overview of keybindings, run :keybindings.<br>"
         "To retrieve help on a command, setting or other topic run :help topic."
     )
     _format_help(title=vimiv.__name__, description=vimiv.__description__, text=text)
 
 
-# TODO Expose a public command class so the pylint suppression is no longer required
 def _command_help(
-    command: api.commands._Command,  # pylint: disable=protected-access
+    command: api.commands._Command,
 ) -> None:
     """Display information on this command."""
     description = command.long_description.replace("\n", "<br>")
     _format_help(title=command.name, description=description)
 
 
 def _setting_help(setting: api.settings.Setting) -> None:
```

### Comparing `vimiv-0.8.0/vimiv/commands/history.py` & `vimiv-0.9.0/vimiv/commands/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions to read and write command history."""
 
 import collections
 import enum
 import json
@@ -47,24 +47,24 @@
     def reset(self):
         """Reset history deque of each mode."""
         for history_deque in self.values():
             history_deque.reset()
 
     def write(self):
         """Write history of each mode to the json file."""
-        with open(self.filename(), "w") as f:
+        with open(self.filename(), "w", encoding="utf-8") as f:
             json.dump(
                 {mode.name: list(value) for mode, value in self.items()}, f, indent=4
             )
 
     def migrate_nonmode_based_history(self):
         """Backup and read history from the old text-file history."""
         old_path = self.filename().replace(".json", "")
         if os.path.isfile(old_path):
-            with open(old_path, "r") as f:
+            with open(old_path, "r", encoding="utf-8") as f:
                 old_commands = [line.strip() for line in f]
             backup_name = old_path + ".bak"
             _logger.info(
                 "Transferring old non-mode based history file. "
                 "A backup is kept at '%s'.",
                 backup_name,
             )
@@ -79,15 +79,15 @@
 
     @classmethod
     def _read(cls, path: str) -> DefaultDict[str, list]:
         """Read command history from file located at path."""
         history: DefaultDict[str, list] = collections.defaultdict(list)
 
         try:
-            with open(path, "r") as f:
+            with open(path, "r", encoding="utf-8") as f:
                 history.update(json.load(f))
             _logger.debug("Loaded history from '%s'", path)
         except FileNotFoundError:
             _logger.debug("No history file to read")
         except (OSError, json.JSONDecodeError) as e:
             _logger.error("Failed loading history from '%s': %s", path, e)
```

### Comparing `vimiv-0.8.0/vimiv/commands/misccommands.py` & `vimiv-0.9.0/vimiv/commands/misccommands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Miscellaneous commands that don't really fit anywhere."""
 
 import logging
 import time
 from typing import List
```

### Comparing `vimiv-0.8.0/vimiv/commands/runners.py` & `vimiv-0.9.0/vimiv/commands/runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Classes and functions to run commands.
 
 Module Attributes:
     SEPARATOR: String used to separate chained commands.
```

### Comparing `vimiv-0.8.0/vimiv/commands/search.py` & `vimiv-0.9.0/vimiv/commands/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Search class implementing functions to search.
 
 Module Attributes:
     search: Instance of the Search class used.
 """
```

### Comparing `vimiv-0.8.0/vimiv/commands/wildcards.py` & `vimiv-0.9.0/vimiv/commands/wildcards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Module to store and expand wildcards.
 
 Module Attributes:
     INTERNAL: List of all special vimiv-internal wildcards such as % or %m.
 """
 
 import re
 import shlex
 import typing
 
 from vimiv import api, utils
 
-WildcardReturnT = typing.Union[str, typing.Iterable[str]]
-WildcardCallbackT = typing.Callable[..., WildcardReturnT]
+WildcardReturn = typing.Union[str, typing.Iterable[str]]
+WildcardCallbackT = typing.Callable[..., WildcardReturn]
 
 
 class Wildcard:
     """Storage class for a wildcard.
 
     Wildcards are called with the current mode to retrieve a single path or a list of
     paths the wildcard corresponds to. The current mode is required as many wildcards,
@@ -35,15 +35,15 @@
     """
 
     def __init__(self, wildcard: str, description: str, callback: WildcardCallbackT):
         self.wildcard = wildcard
         self.description = description
         self._callback = callback
 
-    def __call__(self, mode: api.modes.Mode) -> WildcardReturnT:
+    def __call__(self, mode: api.modes.Mode) -> WildcardReturn:
         return self._callback(mode)
 
 
 INTERNAL = [
     Wildcard("%", "currently focused path or image", api.current_path),
     Wildcard("%f", "all paths in the current file list", api.pathlist),
     Wildcard("%m", "all marked paths", lambda _mode: api.mark.paths),
```

### Comparing `vimiv-0.8.0/vimiv/completion/completer.py` & `vimiv-0.9.0/vimiv/completion/completer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Completer class as man-in-the-middle between command line and completion."""
 
 from PyQt5.QtCore import QObject
 
 from vimiv import api, utils
```

### Comparing `vimiv-0.8.0/vimiv/completion/completionmodels.py` & `vimiv-0.9.0/vimiv/completion/completionmodels.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Various completion models for command line completion."""
 
 import functools
 import os
 import re
@@ -35,15 +35,15 @@
             for name, command in api.commands.items(mode)
             if not command.hide
         ]
 
     def formatted_aliases(self, mode: api.modes.Mode) -> List[Tuple[str, str]]:
         """Return list of aliases with explanation for this mode."""
         return [
-            (alias, f"Alias for '{command}'")
+            (f":{alias}", f"Alias for '{command}'")
             for alias, command in aliases.get(mode).items()
         ]
 
 
 class ExternalCommandModel(api.completion.BaseModel):
     """Completion model filled with shell executables for :!."""
 
@@ -112,15 +112,18 @@
         if not os.path.isdir(os.path.expanduser(directory)):
             return
         # Retrieve supported paths
         images, directories = files.supported(files.listdir(directory))
         # Format data
         self.set_data(
             self._create_row(os.path.join(directory, os.path.basename(path)))
-            for path in images + directories
+            for path in (
+                api.settings.sort.image_order.sort(images)
+                + api.settings.sort.directory_order.sort(directories)
+            )
         )
 
     def _create_row(self, path):
         return (f":{self._command} {api.completion.escape(path)}",)
 
     def _get_directory(self, text: str) -> str:
         """Retrieve directory for which the path completion is created."""
@@ -152,15 +155,16 @@
 
     Attributes:
         _setting: The corresponding settings object.
     """
 
     def __init__(self, setting: api.settings.Setting):
         super().__init__(
-            f":set {setting.name}", column_widths=(0.5, 0.5),
+            f":set {setting.name}",
+            column_widths=(0.5, 0.5),
         )
         self._setting = setting
         self.setSortRole(3)
         setting.changed.connect(self._on_changed)
         self._update_data()
 
     def _update_data(self):
@@ -192,15 +196,16 @@
         )
         self._old_date_re = re.compile(r"(\d{4})(\d{2})(\d{2})T(\d{2})(\d{2})(\d{2})")
         self._date_re = re.compile(r"(\d{4})-(\d{2})-(\d{2})T(\d{2}):(\d{2}):(\d{2})")
 
     def on_enter(self, text: str) -> None:
         """Update trash model on enter to include any newly un-/deleted paths."""
         data = []
-        for path in files.listdir(trash_manager.files_directory()):
+        paths = files.listdir(trash_manager.files_directory())
+        for path in api.settings.sort.image_order.sort(paths):
             cmd = f":undelete {api.completion.escape(os.path.basename(path))}"
             # Get info and format it neatly
             original, date = trash_manager.trash_info(path)
             original = original.replace(os.path.expanduser("~"), "~")
             original = os.path.dirname(original)
             date_match = self._date_re.match(date)
             if date_match is None:
@@ -223,15 +228,16 @@
     Attributes:
         _command: Tag command for which the completion model is valid.
     """
 
     def __init__(self, suffix):
         self._command = f"tag-{suffix}"
         super().__init__(
-            f":{self._command} ", valid_modes=api.modes.GLOBALS,
+            f":{self._command} ",
+            valid_modes=api.modes.GLOBALS,
         )
 
     def on_enter(self, text: str) -> None:
         """Update tag model on enter to include any new/deleted tags."""
         self.set_data(
             (f":{self._command} {api.completion.escape(fname)}",)
             for fname in files.listfiles(api.mark.tagdir)
@@ -263,20 +269,30 @@
         """Return list of commands with description for this mode."""
         return [
             (f":help :{name}", command.description)
             for name, command in api.commands.items(mode)
         ]
 
 
+class CropModel(api.completion.BaseModel):
+    """Completion model filled with aspectratio options for :crop."""
+
+    def __init__(self):
+        super().__init__(":crop ")
+        options = ("", "--aspectratio=keep", "--aspectratio=16:9", "--aspectratio=4:3")
+        self.set_data((f":crop {option}",) for option in options)
+
+
 def init():
     """Create completion models."""
     CommandModel()
     ExternalCommandModel()
     SettingsModel()
     for _, setting in api.settings.items():
         SettingsOptionModel(setting)
     for command in ("open", "delete", "mark"):
         PathModel(command)
     for suffix in ("delete", "load", "write", "open"):
         TagModel(suffix)
     TrashModel()
     HelpModel()
+    CropModel()
```

### Comparing `vimiv-0.8.0/vimiv/config/__init__.py` & `vimiv-0.9.0/vimiv/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions to store, read and change configurations."""
 
 import configparser
 import os
 import sys
```

### Comparing `vimiv-0.8.0/vimiv/config/_style_options.py` & `vimiv-0.9.0/vimiv/config/_style_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Style dictionary storing default options."""
 
 DEFAULT_OPTIONS = {
     # Image
     "image.bg": "{base00}",
@@ -83,8 +83,15 @@
     "prompt.font": "{statusbar.font}",
     "prompt.fg": "{statusbar.fg}",
     "prompt.bg": "{statusbar.bg}",
     "prompt.padding": "{keyhint.padding}",
     "prompt.border_radius": "{keyhint.border_radius}",
     "prompt.border": "{statusbar.message_border}",
     "prompt.border.color": "{statusbar.info}",
+    # Crop
+    "crop.shading": "#88000000",
+    "crop.border": "{manipulate.image.border}",
+    "crop.border.color": "#88AAAAAA",
+    "crop.grip.color": "#88FFFFFF",
+    "crop.grip.border": "{manipulate.image.border}",
+    "crop.grip.border.color": "{crop.border.color}",
 }
```

### Comparing `vimiv-0.8.0/vimiv/config/configcommands.py` & `vimiv-0.9.0/vimiv/config/configcommands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Commands dealing with settings and configuration."""
 
 from typing import List
 
 from vimiv import api
 
 
+@api.keybindings.register("zh", "set library.show_hidden!")
 @api.keybindings.register("sl", "set slideshow.delay +0.5", mode=api.modes.IMAGE)
 @api.keybindings.register("sh", "set slideshow.delay -0.5", mode=api.modes.IMAGE)
 @api.keybindings.register("H", "set library.width -0.05", mode=api.modes.LIBRARY)
 @api.keybindings.register("L", "set library.width +0.05", mode=api.modes.LIBRARY)
 @api.keybindings.register("b", "set statusbar.show!", mode=api.modes.MANIPULATE)
 @api.keybindings.register("b", "set statusbar.show!")
 @api.commands.register(mode=api.modes.MANIPULATE, name="set")
 @api.commands.register(name="set")
 def set_command(name: str, value: List[str]):
     """Set an option.
 
-    **syntax:** ``:set name [value]``
+    **syntax:** ``:set name[!] [[+|-]value]``
 
     positional arguments:
         * ``name``: Name of the setting to set.
-        * ``value``: Value to set the setting to. If not given, set to default.
+          Append a ``!`` to toggle the value of boolean settings.
+        * ``value``: Value to set the setting to.
+          Prepend with ``+`` / ``-`` to increment/decrement the value of numerical
+          settings.
+          If not given, set to default.
     """
     strvalue = " ".join(value)  # List comes from nargs='*'
     try:
         setting = api.settings.get(name.rstrip("!"))
         # Toggle boolean settings
         if name.endswith("!"):
             operation = "toggling"
-            setting.toggle()
+            setting.toggle()  # type: ignore  # We catch the AttributeError later
         # Set default
         elif not strvalue:
             operation = "resetting"
             setting.set_to_default()
         # Add to number settings
         elif strvalue.startswith("+") or strvalue.startswith("-"):
             operation = "adding"
             setting += strvalue  # type: ignore  # We catch the AttributeError later
         else:
             operation = "setting"
             setting.value = strvalue
     except KeyError:
         raise api.commands.CommandError(f"unknown setting '{name}'")
     except (AttributeError, TypeError):
+        # The string is always assigned, the exception can only be raised later-on when
+        # performing the operation
+        # pylint: disable=used-before-assignment
         raise api.commands.CommandError(
             f"'{setting.name}' does not support {operation}"
         )
     except ValueError as e:
         raise api.commands.CommandError(str(e))
```

### Comparing `vimiv-0.8.0/vimiv/config/configfile.py` & `vimiv-0.9.0/vimiv/config/configfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions to read configurations from config file and update settings."""
 
 import configparser
 import re
 
@@ -21,15 +21,15 @@
 def parse(cli_path: str) -> None:
     """Parse settings from the vimiv.conf into the settings api."""
     parse_config(cli_path, "vimiv.conf", read, dump)
 
 
 def dump(path: str) -> None:
     """Write default configurations to config file at path."""
-    with open(path, "w") as f:
+    with open(path, "w", encoding="utf-8") as f:
         get_default_parser().write(f)
     _logger.debug("Created default configuration file '%s'", path)
 
 
 def get_default_parser() -> configparser.ConfigParser:
     """Retrieve configparser with default values."""
     parser = configparser.ConfigParser()
```

### Comparing `vimiv-0.8.0/vimiv/config/external_configparser.py` & `vimiv-0.9.0/vimiv/config/external_configparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Custom configparser able to retrieve variables from external resources.
 
 Values in the configuration file with the syntax ${PREFIX:variable} are updated with the
 value of the variable in the context corresponding to PREFIX. A valid example is
 ${env:variable} where the value of the environment variable $variable is retrieved.
```

### Comparing `vimiv-0.8.0/vimiv/config/keyfile.py` & `vimiv-0.9.0/vimiv/config/keyfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Methods to read keybindings from file and store them."""
 
 import configparser
 from typing import Iterable, Tuple
 
@@ -22,15 +22,15 @@
     """Parse keybindings from the keys.conf into the keybindings registry."""
     config.parse_config(cli_path, "keys.conf", read, dump)
     api.keybindings.check()
 
 
 def dump(path: str):
     """Write default keybindings to keys file at path."""
-    with open(path, "w") as f:
+    with open(path, "w", encoding="utf-8") as f:
         get_default_parser().write(f)
     _logger.debug("Created default keys file '%s'", path)
 
 
 def get_default_parser() -> configparser.ConfigParser:
     """Retrieve configparser with default keybindings."""
     parser = KeyfileParser(delimiters=":")
```

### Comparing `vimiv-0.8.0/vimiv/config/styles.py` & `vimiv-0.9.0/vimiv/config/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions dealing with the stylesheet of the Qt widgets.
 
 Module Attributes:
     NAME_DEFAULT: Name of the default theme.
     NAME_DEFAULT_DARK: Name of the dark default theme.
@@ -152,15 +152,15 @@
         sheet = sheet.replace(option, value)
     obj.setStyleSheet(sheet)
 
 
 def get(name: str) -> str:
     """Return style option for a given name."""
     try:
-        return _style["{%s}" % (name)]
+        return _style[f"{{{name}}}"]
     except KeyError:
         log.error("Style option '%s' not found, falling back to default", name)
         return ""
 
 
 def create_default(dark: bool = False, save_to_file: bool = True) -> Style:
     """Create the default style.
@@ -260,15 +260,15 @@
     xdg.makedirs(os.path.dirname(filename))
     _logger.debug("Dumping style to file '%s'", filename)
     parser = configparser.ConfigParser()
     parser.add_section("STYLE")
     for option, value in style.items():
         option = option.strip("{}")
         parser["STYLE"][option] = value
-    with open(filename, "w") as f:
+    with open(filename, "w", encoding="utf-8") as f:
         f.write(
             "; This file is a reference for creating own styles."
             " It will never be read.\n"
             "; To change values, copy this file using a new name and"
             " set the style setting\n; in vimiv.conf to that name.\n"
         )
         parser.write(f)
```

### Comparing `vimiv-0.8.0/vimiv/gui/commandline.py` & `vimiv-0.9.0/vimiv/gui/commandline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """CommandLine widget in the bar."""
 
 import contextlib
 from typing import cast, TYPE_CHECKING
 
@@ -58,15 +58,16 @@
         api.modes.COMMAND.first_entered.connect(self.init)
 
     def init(self) -> None:
         """Lazy-initialize command-line when first entering command mode."""
         from vimiv.commands import history
 
         self._history = history.History(
-            self.PREFIXES, max_items=api.settings.command.history_limit.value,
+            self.PREFIXES,
+            max_items=api.settings.command.history_limit.value,
         )
 
         self.returnPressed.connect(self._on_return_pressed)
         self.textEdited.connect(self._on_text_edited)
         self.textChanged.connect(self._incremental_search)
         self.cursorPositionChanged.connect(self._on_cursor_position_changed)
         QCoreApplication.instance().aboutToQuit.connect(  # type: ignore
```

### Comparing `vimiv-0.8.0/vimiv/gui/commandwidget.py` & `vimiv-0.9.0/vimiv/gui/commandwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Command widget at the bottom including commandline and completion widget."""
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QWidget, QSizePolicy, QVBoxLayout
```

### Comparing `vimiv-0.8.0/vimiv/gui/completionwidget.py` & `vimiv-0.9.0/vimiv/gui/completionwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Completion widget in the bar."""
 
 from PyQt5.QtCore import pyqtSignal, Qt
 
 from vimiv import api, widgets
```

### Comparing `vimiv-0.8.0/vimiv/gui/eventhandler.py` & `vimiv-0.9.0/vimiv/gui/eventhandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Handles key and mouse events."""
 
 import string
 from typing import Union, Tuple, List, cast
 
@@ -243,19 +243,15 @@
     """Return the names of all modifiers pressed in the event."""
     modmask2str = {
         Qt.ControlModifier: "<ctrl>",
         Qt.AltModifier: "<alt>",
         Qt.MetaModifier: "<meta>",
     }
     modifiers = event.modifiers()
-    return [
-        mod_name
-        for mask, mod_name in modmask2str.items()
-        if modifiers & mask  # type: ignore
-    ]
+    return [mod_name for mask, mod_name in modmask2str.items() if modifiers & mask]
 
 
 def _get_base_keysequence(event: QKeyEvent) -> SequenceT:
     """Get main keyname part of QKeyEvent.
 
     Converts special keys to usable names and uses event.text() otherwise. Is a sequence
     to allow prepending <shift> to special keys.
@@ -277,25 +273,23 @@
         Qt.Key_Right: "<right>",
         Qt.Key_Up: "<up>",
         Qt.Key_Down: "<down>",
         Qt.Key_Home: "<home>",
         Qt.Key_End: "<end>",
         Qt.Key_PageUp: "<page-up>",
         Qt.Key_PageDown: "<page-down>",
-        Qt.Key_Home: "<home>",
-        Qt.Key_End: "<end>",
     }
     separator_keys = {
         Qt.Key_Colon: "<colon>",
         Qt.Key_Equal: "<equal>",
     }
     if event.key() in special_keys:
         # Parse shift here as the key does not support it otherwise
         text = special_keys[event.key()]  # type: ignore
-        if event.modifiers() & Qt.ShiftModifier:  # type: ignore
+        if event.modifiers() & Qt.ShiftModifier:
             return "<shift>", text
         return (text,)
     if event.key() in separator_keys:  # Required as configparser crashes otherwise
         return (separator_keys[event.key()],)  # type: ignore
     if event.text().isprintable():
         return (event.text(),)
     return (QKeySequence(event.key()).toString().lower(),)
```

### Comparing `vimiv-0.8.0/vimiv/gui/image.py` & `vimiv-0.9.0/vimiv/gui/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """QtWidgets for IMAGE mode."""
 
 import contextlib
 from typing import List, Union, Optional, Callable
 
@@ -18,26 +18,36 @@
     QGraphicsPixmapItem,
     QLabel,
 )
 from PyQt5.QtGui import QMovie, QPixmap
 
 from vimiv import api, imutils, utils
 from vimiv.imutils import slideshow
-from vimiv.commands.argtypes import Direction, ImageScale, ImageScaleFloat, Zoom
+from vimiv.commands.argtypes import (
+    Direction,
+    ImageScale,
+    ImageScaleFloat,
+    Zoom,
+    AspectRatio,
+)
 from vimiv.config import styles
 from vimiv.gui import eventhandler
-from vimiv.utils import lazy
+from vimiv.utils import lazy, log
 
 QtSvg = lazy.import_module("PyQt5.QtSvg", optional=True)
 
 
 INF = float("inf")
 
+_logger = log.module_logger(__name__)
+
 
 class ScrollableImage(eventhandler.EventHandlerMixin, QGraphicsView):
+    # pylint: disable=too-many-public-methods
+    # TODO consider refactoring
     """QGraphicsView to display Image or Animation.
 
     Connects to the *_loaded signals to create the appropriate child widget.
     Commands used in image mode are defined here.
 
     Class Attributes:
         MIN_SCALE: Minimum scale to scale an image to.
@@ -120,14 +130,15 @@
         """Load new movie into the graphics scene."""
         movie.jumpToFrame(0)
         if api.settings.image.autoplay.value:
             movie.start()
         widget = QLabel()
         widget.setMovie(movie)
         self._update_scene(widget, QRectF(movie.currentPixmap().rect()), keep_zoom)
+        widget.resize(movie.currentPixmap().size())
 
     def _load_svg(self, path: str, keep_zoom: bool) -> None:
         """Load new vector graphic into the graphics scene."""
         item = QtSvg.QGraphicsSvgItem(path)
         self._update_scene(item, item.boundingRect(), keep_zoom)
 
     def _update_scene(
@@ -210,15 +221,15 @@
         **syntax:** ``:zoom direction``
 
         positional arguments:
             * ``direction``: The direction to zoom in (in/out).
 
         **count:** multiplier
         """
-        scale = 1.25 ** count if direction == Zoom.In else 1 / 1.25 ** count
+        scale = 1.25**count if direction == Zoom.In else 1 / 1.25**count
         self._scale_to_float(self.zoom_level * scale)
         self._scale = ImageScaleFloat(self.zoom_level)
 
     @api.keybindings.register(
         ("w", "<equal>"), "scale --level=fit", mode=api.modes.IMAGE
     )
     @api.keybindings.register("W", "scale --level=1", mode=api.modes.IMAGE)
@@ -314,59 +325,120 @@
     def play_or_pause(self):
         """Toggle between play and pause of animation."""
         with contextlib.suppress(IndexError, AttributeError):  # No items, not a movie
             widget = self.items()[0].widget()
             movie = widget.movie()
             movie.setPaused(not movie.state() == QMovie.Paused)
 
-    @api.commands.register(mode=api.modes.IMAGE)
+    @api.commands.register(mode=api.modes.IMAGE, edit=True)
     def straighten(self):
         """Display a grid to straighten the current image.
 
         The image can then be straightened clockwise using the ``l``, ``>`` and ``L``
         keys and counter-clockwise with ``h``, ``<`` and ``H``. Accept the changes with
         ``<return>`` and reject them with ``<escape>``.
         """
         from vimiv.gui.straightenwidget import StraightenWidget
 
         StraightenWidget(self)
 
+    @api.commands.register(mode=api.modes.IMAGE)
+    def crop(self, aspectratio: AspectRatio = None):
+        """Display a widget to crop the current image.
+
+        **syntax:** ``crop [--aspectratio=ASPECTRATIO]``
+
+        optional arguments:
+            * ``--aspectratio``: Fix the cropping to the given aspectratio. Valid
+              options are two integers separated by ``:`` or the special ``keep`` to
+              keep the aspectratio of the current image.
+        """
+        from .crop_widget import CropWidget
+
+        self.scale(level=ImageScale.Fit)  # type: ignore
+        if aspectratio is not None and aspectratio.keep:
+            aspectratio.setWidth(int(self.sceneRect().width()))
+            aspectratio.setHeight(int(self.sceneRect().height()))
+        CropWidget(self, aspectratio=aspectratio)
+
     @api.status.module("{transformation-info}")
     def transformation_info(self) -> str:
         """Additional information on image transformations such as straightening."""
         if self.transformation_module is None:
             return ""
         return self.transformation_module()  # pylint: disable=not-callable
 
+    @api.status.module("{cursor-position}")
+    def cursor_position(self) -> str:
+        """Current cursor position in image coordinates."""
+        # Initialize mouse tracking on first call
+        if not self.hasMouseTracking():
+            _logger.debug("Activating mouse tracking for {cursor-position} module")
+            self.setMouseTracking(True)
+            # We only want to override leaveEvent if we really have to
+            # pylint: disable=invalid-name
+            self.leaveEvent = self._leave_event  # type: ignore[method-assign]
+
+        rect = self.sceneRect().toRect()
+        if rect.width() == 1:  # Empty
+            return ""
+
+        cursor_pos = self.mapToScene(self.mapFromGlobal(self.cursor().pos())).toPoint()
+
+        if not 0 < cursor_pos.x() <= rect.width():
+            return ""
+        if not 0 < cursor_pos.y() <= rect.height():
+            return ""
+        return f"({cursor_pos.x()}, {cursor_pos.y()})"
+
     def resizeEvent(self, event):
         """Rescale the child image and update statusbar on resize event."""
         super().resizeEvent(event)
         if self.items():
             self.scale(self._scale)
             api.status.update("image zoom level changed")
             self.resized.emit()
 
+    def mouseMoveEvent(self, event):
+        """Override mouse move event to also update the status.
+
+        Needed by the cursor position related status module and only applied in case it
+        is used at all to avoid unnecessary updates.
+        """
+        api.status.update("mouse position changed")
+        super().mouseMoveEvent(event)
+
+    def _leave_event(self, event):
+        """Override leave event to also update the status.
+
+        Needed by the cursor position related status module and only applied in case it
+        is used at all to avoid unnecessary updates.
+        """
+        api.status.update("mouse position changed")
+        super().leaveEvent(event)
+
     def mousePressEvent(self, event):
         """Update mouse press event to start panning on left button."""
         if event.button() == Qt.LeftButton:
             self.setDragMode(QGraphicsView.ScrollHandDrag)
         super().mousePressEvent(event)
 
     def mouseReleaseEvent(self, event):
         """Update mouse release event to stop any panning."""
         self.setDragMode(QGraphicsView.NoDrag)
         super().mouseReleaseEvent(event)
 
     def wheelEvent(self, event):
         """Update mouse wheel to zoom with control."""
-        if event.modifiers() & Qt.ControlModifier:
+        require_ctrl = api.settings.image.zoom_wheel_ctrl
+        if not require_ctrl or event.modifiers() & Qt.ControlModifier:
             # We divide by 120 as this is the regular delta multiple
             # See https://doc.qt.io/qt-5/qwheelevent.html#angleDelta
             steps = event.angleDelta().y() / 120
-            scale = 1.03 ** steps
+            scale = 1.03**steps
             self._scale_to_float(self.zoom_level * scale)
             self._scale = ImageScaleFloat(self.zoom_level)
             api.status.update("image zoom level changed")
         else:
             super().wheelEvent(event)
 
     def focusOutEvent(self, event):
```

### Comparing `vimiv-0.8.0/vimiv/gui/keybindings_popup.py` & `vimiv-0.9.0/vimiv/gui/keybindings_popup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Pop-up window to display keybindings of current mode."""
 
 from typing import List, Tuple, Iterator, Set
 
 from PyQt5.QtWidgets import QLabel, QHBoxLayout, QVBoxLayout, QLayout, QLineEdit
```

### Comparing `vimiv-0.8.0/vimiv/gui/keyhintwidget.py` & `vimiv-0.9.0/vimiv/gui/keyhintwidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Widget to display partial matches above the statusbar."""
 
 from typing import Iterator, Tuple
 
 from PyQt5.QtCore import QTimer, Qt
```

### Comparing `vimiv-0.8.0/vimiv/gui/library.py` & `vimiv-0.9.0/vimiv/gui/library.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Library widget with model and delegate."""
 
 import contextlib
+import math
 import os
-from typing import List, Optional, Dict, NamedTuple
+from typing import List, Optional, Dict, NamedTuple, cast
 
 from PyQt5.QtCore import Qt, pyqtSlot
-from PyQt5.QtWidgets import QStyledItemDelegate, QSizePolicy, QStyle
+from PyQt5.QtWidgets import QStyledItemDelegate, QSizePolicy, QStyle, QWidget
 from PyQt5.QtGui import QStandardItemModel, QColor, QTextDocument, QStandardItem
 
 from vimiv import api, utils, widgets
 from vimiv.commands import argtypes, search, number_for_command
 from vimiv.config import styles
 from vimiv.gui import eventhandler, synchronize
 from vimiv.utils import files, strip_html, clamp, wrap_style_span, log
@@ -32,15 +33,20 @@
         row: Row of the stored position used in case the path is no longer available.
     """
 
     path: str
     row: int = 0
 
 
-class Library(eventhandler.EventHandlerMixin, widgets.FlatTreeView):
+class Library(
+    eventhandler.EventHandlerMixin,
+    widgets.GetNumVisibleMixin,
+    widgets.ScrollWheelCumulativeMixin,
+    widgets.FlatTreeView,
+):
     """Library widget.
 
     Attributes:
         _last_selected: Name of the path that was selected last.
         _positions: Dictionary that stores positions in directories.
     """
 
@@ -77,16 +83,18 @@
         border: none;
         background: none;
     }
     """
 
     @api.modes.widget(api.modes.LIBRARY)
     @api.objreg.register
-    def __init__(self, mainwindow):
-        super().__init__(parent=mainwindow)
+    def __init__(self, mainwindow: QWidget):
+        widgets.ScrollWheelCumulativeMixin.__init__(self, self._scroll_wheel_callback)
+        widgets.FlatTreeView.__init__(self, parent=mainwindow)
+
         self._last_selected = ""
         self._positions: Dict[str, Position] = {}
 
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Ignored)
 
         self.setModel(LibraryModel(self))
@@ -120,14 +128,15 @@
         """
         if mode == api.modes.LIBRARY:
             _logger.debug("Updating library due to new search")
             self._select_row(index)
             self.repaint()
 
     def _on_show_hidden_changed(self, _value: bool):
+        self.store_position()
         self._open_directory(".", reload_current=True)
 
     @utils.slot
     def _on_enter(self):
         """Update widths and ensure that the current path is visible at the center."""
         self.update_width()
 
@@ -176,40 +185,52 @@
         # Update image if a new image was selected
         if path != self._last_selected:
             api.signals.load_images.emit([path])
         self._last_selected = path
         if close:
             api.modes.LIBRARY.close()
 
-    @api.keybindings.register("p", "scroll up --open-selected", mode=api.modes.LIBRARY)
+    @api.keybindings.register("<ctrl>b", "scroll page-up", mode=api.modes.LIBRARY)
+    @api.keybindings.register("<ctrl>f", "scroll page-down", mode=api.modes.LIBRARY)
+    @api.keybindings.register("<ctrl>u", "scroll half-page-up", mode=api.modes.LIBRARY)
+    @api.keybindings.register(
+        "<ctrl>d", "scroll half-page-down", mode=api.modes.LIBRARY
+    )
+    @api.keybindings.register(
+        ("p", "<button-back>"), "scroll up --open-selected", mode=api.modes.LIBRARY
+    )
     @api.keybindings.register("k", "scroll up", mode=api.modes.LIBRARY)
     @api.keybindings.register(
-        "n", "scroll down --open-selected", mode=api.modes.LIBRARY
+        ("n", "<button-forward>"), "scroll down --open-selected", mode=api.modes.LIBRARY
     )
     @api.keybindings.register("j", "scroll down", mode=api.modes.LIBRARY)
-    @api.keybindings.register(  # No idea why this has to go in this weird location
-        "h", "scroll left", mode=api.modes.LIBRARY  # type: ignore[override]
+    @api.keybindings.register(
+        ("h", "<button-right>"), "scroll left", mode=api.modes.LIBRARY
     )
     @api.keybindings.register("l", "scroll right", mode=api.modes.LIBRARY)
     @api.commands.register(mode=api.modes.LIBRARY)
-    def scroll(
-        self, direction: argtypes.Direction, open_selected: bool = False, count=1
+    def scroll(  # type: ignore[override]
+        self,
+        direction: argtypes.DirectionWithPage,
+        open_selected: bool = False,
+        count=1,
     ):
         """Scroll the library in the given direction.
 
         **syntax:** ``:scroll direction``
 
         The behaviour is similar to the file manager ranger.
 
         * Scrolling right selects the current file.
         * Scrolling left selects the parent directory.
         * Scrolling up and down moves the cursor.
 
         positional arguments:
-            * ``direction``: The direction to scroll in (left/right/up/down).
+            * ``direction``: The direction to scroll in
+              (left/right/up/down/page-up/page-down/half-page-up/half-page-down).
 
         optional arguments:
             * ``--open-selected``: Automatically open any selected image.
 
         **count:** multiplier
         """
         _logger.debug("Scrolling in direction '%s'", direction)
@@ -222,18 +243,23 @@
             parent = os.path.abspath(os.pardir)
             self._positions[parent] = Position(os.getcwd())
             api.working_directory.handler.chdir(parent)
         else:
             row = self.row()
             if row == -1:  # Directory is empty
                 raise api.commands.CommandWarning("Directory is empty")
-            if direction == direction.Up:
-                row -= count
-            else:
-                row += count
+            if direction.is_page_step:
+                n_items = self._n_visible_items()
+                factor = 0.5 if direction.is_half_page_step else 1
+                stepsize = math.ceil(n_items * factor)
+                count *= stepsize
+            if direction.is_reverse:
+                count *= -1
+            _logger.debug("Scrolling %d rows", count)
+            row += count
             self._select_row(clamp(row, 0, self.model().rowCount() - 1), open_selected)
 
     @api.keybindings.register("go", "goto 1 --open-selected", mode=api.modes.LIBRARY)
     @api.keybindings.register("gg", "goto 1", mode=api.modes.LIBRARY)
     @api.keybindings.register("G", "goto -1", mode=api.modes.LIBRARY)
     @api.commands.register(mode=api.modes.LIBRARY)
     def goto(
@@ -322,14 +348,24 @@
         _logger.debug("Selecting library row %d", row)
         current = self.current()
         if emit:
             synchronize.signals.new_library_path_selected.emit(current)
         if open_selected_image and not os.path.isdir(current):
             self.open_selected(close=False)
 
+    def _scroll_wheel_callback(self, _steps_x, steps_y):
+        """Callback function used by the scroll wheel mixin for mouse scrolling."""
+        if steps_y < 0:
+            self.scroll(argtypes.DirectionWithPage.Down, count=abs(steps_y))
+        elif steps_y > 0:
+            self.scroll(argtypes.DirectionWithPage.Up, count=steps_y)
+
+    def model(self) -> "LibraryModel":
+        return cast(LibraryModel, super().model())
+
 
 class LibraryModel(QStandardItemModel):
     """Model used for the library.
 
     The model stores the rows and populates the row content when the working directory
     has changed.
 
@@ -439,15 +475,15 @@
             if are_directories:
                 name = utils.add_html(name + "/", "b")
             if path in api.mark.paths:
                 name = mark_prefix + name
             with contextlib.suppress(FileNotFoundError):  # Deleted in the meantime
                 size = get_size(path)
                 self.appendRow(
-                    (QStandardItem(str(i)), QStandardItem(name), QStandardItem(size),)
+                    (QStandardItem(str(i)), QStandardItem(name), QStandardItem(size))
                 )
                 self.paths.append(path)
 
 
 class LibraryDelegate(QStyledItemDelegate):
     """Delegate used for the library.
```

### Comparing `vimiv-0.8.0/vimiv/gui/mainwindow.py` & `vimiv-0.9.0/vimiv/gui/mainwindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """QMainWindow which groups all the other widgets."""
 
 from typing import List
 
 from PyQt5.QtWidgets import QWidget, QStackedWidget, QGridLayout
@@ -16,29 +16,28 @@
 # Import all GUI widgets used to create the full main window
 from vimiv.gui.commandwidget import CommandWidget
 from vimiv.gui.image import ScrollableImage
 from vimiv.gui.keyhintwidget import KeyhintWidget
 from vimiv.gui.library import Library
 from vimiv.gui.thumbnail import ThumbnailView
 from vimiv.gui.message import Message
-from vimiv.gui.metadatawidget import MetadataWidget
 from vimiv.gui.statusbar import StatusBar
 
 
 class MainWindow(QWidget):
     """QMainWindow which groups all the other widgets.
 
     Attributes:
         _library: Library object at the left of the grid.
         _overlays: List of overlay widgets.
         _statusbar: Statusbar object displayed at the bottom.
     """
 
     @api.objreg.register
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self._overlays: List[QWidget] = []
         # Create main widgets and add them to the grid layout
         self._statusbar = StatusBar()
         grid = QGridLayout(self)
         grid.setSpacing(0)
         grid.setContentsMargins(0, 0, 0, 0)
@@ -46,30 +45,39 @@
         self._library = Library(self)
         grid.addWidget(self._library, 0, 0, 1, 1)
         grid.addWidget(self._statusbar, 1, 0, 1, 2)
         # Add overlay widgets
         self._overlays.append(KeyhintWidget(self))
         self._overlays.append(Message(self))
         self._overlays.append(CommandWidget(self))
-        if MetadataWidget is not None:  # Not defined if there is no exif support
-            self._overlays.append(MetadataWidget(self))
         # Connect signals
         api.status.signals.update.connect(self._set_title)
         api.settings.statusbar.show.changed.connect(self._update_overlay_geometry)
         api.modes.MANIPULATE.first_entered.connect(self._init_manipulate)
         api.prompt.question_asked.connect(self._run_prompt)
+        api.signals.plugins_loaded.connect(self._init_metadata)
 
     @utils.slot
     def _init_manipulate(self):
         """Create UI widgets related to manipulate mode."""
         from vimiv.gui.manipulate import Manipulate
 
         manipulate_widget = Manipulate(self)
         self.add_overlay(manipulate_widget)
 
+    @utils.slot
+    def _init_metadata(self):
+        """Initialize metadata widget in case we have metadata support."""
+        from vimiv.imutils import metadata
+
+        if metadata.has_metadata_support():
+            from vimiv.gui.metadatawidget import MetadataWidget
+
+            self._overlays.append(MetadataWidget(self))
+
     @api.keybindings.register("f", "fullscreen", mode=api.modes.MANIPULATE)
     @api.keybindings.register("f", "fullscreen")
     @api.commands.register(mode=api.modes.MANIPULATE)
     @api.commands.register()
     def fullscreen(self):
         """Toggle fullscreen mode."""
         if self.isFullScreen():
```

### Comparing `vimiv-0.8.0/vimiv/gui/manipulate.py` & `vimiv-0.9.0/vimiv/gui/manipulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Manipulate widget."""
 
 from typing import List, Optional
 
 from PyQt5.QtCore import Qt, QSize, QPoint
```

### Comparing `vimiv-0.8.0/vimiv/gui/message.py` & `vimiv-0.9.0/vimiv/gui/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Message widget to display temporary information to the user."""
 
 from PyQt5.QtCore import Qt, QTimer
 from PyQt5.QtWidgets import QLabel, QSizePolicy
```

### Comparing `vimiv-0.8.0/vimiv/gui/metadatawidget.py` & `vimiv-0.9.0/vimiv/gui/metadatawidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,182 +1,181 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Overlay widget to display image metadata."""
 
 import itertools
 from typing import Optional
 
 from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QLabel, QSizePolicy
+from PyQt5.QtWidgets import QLabel, QSizePolicy, QWidget
 
 from vimiv import api, utils
-from vimiv.imutils import exif
+from vimiv.imutils import metadata
 from vimiv.config import styles
 
 _logger = utils.log.module_logger(__name__)
 
 
-if exif.has_exif_support:
+class MetadataWidget(QLabel):
+    """Overlay widget to display image metadata.
 
-    class MetadataWidget(QLabel):
-        """Overlay widget to display image metadata.
+    The display of the widget can be toggled by command. It is filled with
+    metadata information of the current image.
 
-        The display of the widget can be toggled by command. It is filled with exif
-        metadata information of the current image.
 
+    Attributes:
+        _mainwindow_bottom: y-coordinate of the bottom of the mainwindow.
+        _mainwindow_width: width of the mainwindow.
+        _path: Absolute path of the current image to load metadata of.
+        _current_set: Holds a string of the currently selected keyset.
+        _handler: MetadataHandler for _path or None. Use its property for access.
+    """
+
+    STYLESHEET = """
+    QLabel {
+        font: {statusbar.font};
+        color: {statusbar.fg};
+        background: {metadata.bg};
+        padding: {metadata.padding};
+        border-top-left-radius: {metadata.border_radius};
+    }
+    """
+
+    @api.objreg.register
+    def __init__(self, parent: QWidget):
+        super().__init__(parent=parent)
+        styles.apply(self)
+
+        self.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Minimum)
+        self.setTextFormat(Qt.RichText)
+
+        self._mainwindow_bottom = 0
+        self._mainwindow_width = 0
+        self._path = ""
+        self._current_set = ""
+        self._handler: Optional[metadata.MetadataHandler] = None
+
+        api.signals.new_image_opened.connect(self._on_image_opened)
+        api.settings.metadata.current_keyset.changed.connect(self._update_text)
+
+        self.hide()
+
+    @property
+    def handler(self) -> metadata.MetadataHandler:
+        """Return the MetadataHandler for the current path."""
+        if self._handler is None:
+            self._handler = metadata.MetadataHandler(self._path)
+        return self._handler
+
+    @api.keybindings.register("i", "metadata", mode=api.modes.IMAGE)
+    @api.commands.register(mode=api.modes.IMAGE)
+    def metadata(self, count: Optional[int] = None):
+        """Toggle display of metadata of current image.
+
+        **count:** Select the key set to display instead.
+
+        .. hint::
+            5 default key sets are provided and mapped to the counts 1-5. To
+            override them or add your own, extend the METADATA section in your
+            configfile like this::
 
-        Attributes:
-            _mainwindow_bottom: y-coordinate of the bottom of the mainwindow.
-            _mainwindow_width: width of the mainwindow.
-            _path: Absolute path of the current image to load exif metadata of.
-            _current_set: Holds a string of the currently selected keyset.
-            _handler: ExifHandler for _path or None. Use the handler property to access.
-        """
+                keys2 = Override,Second,Set
+                keys4 = New,Fourth,Set
 
-        STYLESHEET = """
-        QLabel {
-            font: {statusbar.font};
-            color: {statusbar.fg};
-            background: {metadata.bg};
-            padding: {metadata.padding};
-            border-top-left-radius: {metadata.border_radius};
-        }
+            where the values must be a comma-separated list of valid metadata keys.
         """
 
-        @api.objreg.register
-        def __init__(self, parent):
-            super().__init__(parent=parent)
-            styles.apply(self)
-
-            self.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Minimum)
-            self.setTextFormat(Qt.RichText)
-
-            self._mainwindow_bottom = 0
-            self._mainwindow_width = 0
-            self._path = ""
-            self._current_set = ""
-            self._handler: Optional[exif.ExifHandler] = None
-
-            api.signals.new_image_opened.connect(self._on_image_opened)
-            api.settings.metadata.current_keyset.changed.connect(self._update_text)
-
+        if count is not None:
+            try:
+                _logger.debug("Switch keyset")
+                new_keyset = api.settings.metadata.keysets[count]
+                api.settings.metadata.current_keyset.value = new_keyset
+                if not self.isVisible():
+                    _logger.debug("Showing widget")
+                    self.raise_()
+                    self.show()
+            except KeyError:
+                raise api.commands.CommandError(f"Invalid key set option {count}")
+        elif self.isVisible():
+            _logger.debug("Hiding widget")
             self.hide()
+        else:
+            _logger.debug("Showing widget")
+            self._update_text()
+            self.raise_()
+            self.show()
+
+    @api.commands.register(mode=api.modes.IMAGE)
+    def metadata_list_keys(self, n_cols: int = 3, to_term: bool = False):
+        """Display a list of all valid metadata keys for the current image.
+
+        **syntax:** ``:metadata-list-keys [--n-cols=NUMBER] [--to-term]``
+
+        optional arguments:
+            * ``--n-cols``: Number of columns used to display the keys.
+            * ``--to-term``: Print the keys to the terminal instead.
+        """
 
-        @property
-        def handler(self) -> exif.ExifHandler:
-            """Return the ExifHandler for the current path."""
-            if self._handler is None:
-                self._handler = exif.ExifHandler(self._path)
-            return self._handler
-
-        @api.keybindings.register("i", "metadata", mode=api.modes.IMAGE)
-        @api.commands.register(mode=api.modes.IMAGE)
-        def metadata(self, count: Optional[int] = None):
-            """Toggle display of exif metadata of current image.
-
-            **count:** Select the key set to display instead.
-
-            .. hint::
-                3 default key sets are provided and mapped to the counts 1-3. To
-                override them or add your own, extend the METADATA section in your
-                configfile like this::
-
-                    keys2 = Override,Second,Set
-                    keys4 = New,Fourth,Set
-
-                where the values must be a comma-separated list of valid metadata keys.
-            """
-
-            if count is not None:
-                try:
-                    _logger.debug("Switch keyset")
-                    new_keyset = api.settings.metadata.keysets[count]
-                    api.settings.metadata.current_keyset.value = new_keyset
-                    if not self.isVisible():
-                        _logger.debug("Showing widget")
-                        self.raise_()
-                        self.show()
-                except KeyError:
-                    raise api.commands.CommandError(f"Invalid key set option {count}")
-            elif self.isVisible():
-                _logger.debug("Hiding widget")
-                self.hide()
-            else:
-                _logger.debug("Showing widget")
-                self._update_text()
-                self.raise_()
-                self.show()
-
-        @api.commands.register(mode=api.modes.IMAGE)
-        def metadata_list_keys(self, n_cols: int = 3, to_term: bool = False):
-            """Display a list of all valid metadata keys for the current image.
-
-            **syntax:** ``:metadata-list-keys [--n-cols=NUMBER] [--to-term]``
-
-            optional arguments:
-                * ``--n-cols``: Number of columns used to display the keys.
-                * ``--to-term``: Print the keys to the terminal instead.
-            """
-
-            keys = sorted(set(self.handler.get_keys()))
-            if to_term:
-                print(*keys, sep="\n")
-            elif n_cols < 1:
-                raise api.commands.CommandError("Number of columns must be positive")
-            else:
-                columns = list(utils.split(keys, n_cols))
-                table = utils.format_html_table(
-                    itertools.zip_longest(*columns, fillvalue="")
-                )
-                self.setText(table)
-                self._update_geometry()
-                self.show()
-
-        def update_geometry(self, window_width, window_bottom):
-            """Adapt location when main window geometry changes."""
-            self._mainwindow_width = window_width
-            self._mainwindow_bottom = window_bottom
-            self._update_geometry()
-
-        def _update_geometry(self):
-            """Update geometry according to current text content and window location."""
-            self.adjustSize()
-            y = self._mainwindow_bottom - self.height()
-            self.setGeometry(
-                self._mainwindow_width - self.width(), y, self.width(), self.height()
+        keys = sorted(set(self.handler.get_keys()))
+        if to_term:
+            print(*keys, sep="\n")
+        elif n_cols < 1:
+            raise api.commands.CommandError("Number of columns must be positive")
+        else:
+            columns = list(utils.split(keys, n_cols))
+            table = utils.format_html_table(
+                itertools.zip_longest(*columns, fillvalue="")
             )
+            self.setText(table)
+            self._update_geometry()
+            self.show()
 
-        def _update_text(self):
-            """Update the metadata text if the current image has not been loaded."""
-            if self._current_set == api.settings.metadata.current_keyset.value:
-                return
-            _logger.debug(
-                "%s: reading exif of %s", self.__class__.__qualname__, self._path
-            )
-            keys = [
-                e.strip() for e in api.settings.metadata.current_keyset.value.split(",")
-            ]
-            _logger.debug(f"Read metadata.current_keys {keys}")
-            formatted_exif = self.handler.get_formatted_exif(keys)
-            if formatted_exif:
-                self.setText(utils.format_html_table(formatted_exif.values()))
+    def update_geometry(self, window_width, window_bottom):
+        """Adapt location when main window geometry changes."""
+        self._mainwindow_width = window_width
+        self._mainwindow_bottom = window_bottom
+        self._update_geometry()
+
+    def _update_geometry(self):
+        """Update geometry according to current text content and window location."""
+        self.adjustSize()
+        y = self._mainwindow_bottom - self.height()
+        self.setGeometry(
+            self._mainwindow_width - self.width(), y, self.width(), self.height()
+        )
+
+    def _update_text(self):
+        """Update the metadata text if the current image has not been loaded."""
+        if self._current_set == api.settings.metadata.current_keyset.value:
+            return
+        _logger.debug(
+            "%s: reading metadata of %s", self.__class__.__qualname__, self._path
+        )
+        keys = [
+            e.strip() for e in api.settings.metadata.current_keyset.value.split(",")
+        ]
+        _logger.debug(f"Extracting metadata for keys: {keys}")
+        try:
+            data = self.handler.get_metadata(keys)
+            if data:
+                # Sort data according to order provided in config
+                sorted_data = [data[key] for key in keys if key in data]
+                self.setText(utils.format_html_table(sorted_data))
             else:
                 self.setText("No matching metadata found")
-            self._update_geometry()
-            self._current_set = api.settings.metadata.current_keyset.value
-
-        @utils.slot
-        def _on_image_opened(self, path: str):
-            """Load new image and update text if the widget is currently visible."""
-            self._path = path
-            self._current_set = ""
-            self._handler = None
-            if self.isVisible():
-                self._update_text()
-
-
-else:  # No exif support  # pragma: no cover  # Covered in another CI
-    MetadataWidget = None  # type: ignore
+        except metadata.MetadataError as e:
+            self.setText(str(e))
+        self._update_geometry()
+        self._current_set = api.settings.metadata.current_keyset.value
+
+    @utils.slot
+    def _on_image_opened(self, path: str):
+        """Load new image and update text if the widget is currently visible."""
+        self._path = path
+        self._current_set = ""
+        self._handler = None
+        if self.isVisible():
+            self._update_text()
```

### Comparing `vimiv-0.8.0/vimiv/gui/prompt.py` & `vimiv-0.9.0/vimiv/gui/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Blocking prompt widget asking the user a question."""
 
 from PyQt5.QtCore import Qt, QEventLoop
 from PyQt5.QtWidgets import QLabel
```

### Comparing `vimiv-0.8.0/vimiv/gui/statusbar.py` & `vimiv-0.9.0/vimiv/gui/statusbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Statusbar widget in the bar to display information.
 
 The statusbar is one of the status objects in vimiv. It therefore connects to
 the api.status.signals.update signal and updates its content when this signal
 was emitted.
```

### Comparing `vimiv-0.8.0/vimiv/gui/straightenwidget.py` & `vimiv-0.9.0/vimiv/gui/straightenwidget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Widget to display a grid for straightening and interact with image and transform."""
 
 import functools
 
 from PyQt5.QtCore import Qt
@@ -44,14 +44,17 @@
         self._add_rotate_binding("h", "<", counter_clockwise=True, angle=0.2)
         self._add_rotate_binding("H", counter_clockwise=True, angle=1.0)
 
         self.color = QColor(styles.get("image.straighten.color"))
         self.angle = 0.0
         self._init_size = self.transform.size
 
+        self.update_geometry()
+        self.show()
+
     def _add_rotate_binding(
         self, *keys: str, counter_clockwise: bool = False, angle: float
     ) -> None:
         """Add keybindings for the rotate command.
 
         Args:
             keys: Tuple of keys to bind to this command.
@@ -83,25 +86,15 @@
         """
         self.reset_transformations()
         self.transform.straighten(angle=self.angle, original_size=self._init_size)
         self.update_geometry()
 
     def update_geometry(self):
         """Update geometry of the grid to overlay the image."""
-        image_size = self.parent().sceneRect()
-        width = min(
-            int(image_size.width() * self.parent().zoom_level), self.parent().width()
-        )
-        height = min(
-            int(image_size.height() * self.parent().zoom_level), self.parent().height()
-        )
-        self.setFixedSize(width, height)
-        x = (self.parent().width() - width) // 2
-        y = (self.parent().height() - height) // 2
-        self.move(x, y)
+        self.setGeometry(self.image_rect)
 
     def status_info(self):
         """Display current rotation angle in the status bar."""
         return f"angle: {self.angle:+.1f}°"
 
     def paintEvent(self, _event):
         """Paint a grid of helper lines."""
```

### Comparing `vimiv-0.8.0/vimiv/gui/synchronize.py` & `vimiv-0.9.0/vimiv/gui/synchronize.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Helper module to synchronize selection of library and thumbnail mode.
 
 Module Attributes:
     signals: Signals used as synchronization method.
 """
```

### Comparing `vimiv-0.8.0/vimiv/gui/thumbnail.py` & `vimiv-0.9.0/vimiv/gui/thumbnail.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Thumbnail widget."""
 
 import contextlib
+import math
 import os
 from typing import List, Optional, Iterator, cast
 
 from PyQt5.QtCore import Qt, QSize, QRect, pyqtSlot
 from PyQt5.QtWidgets import QListWidget, QListWidgetItem, QStyle, QStyledItemDelegate
 from PyQt5.QtGui import QColor, QIcon
 
@@ -20,16 +21,26 @@
 from vimiv.gui import eventhandler, synchronize
 from vimiv.utils import create_pixmap, thumbnail_manager, log
 
 
 _logger = log.module_logger(__name__)
 
 
+# The class is certainly very border-line in size, much like the corresponding classes
+# image.ScrollableImage and library.Library.
+# TODO consider refactoring if this improves code-clarity
+# pylint: disable=too-many-public-methods
+
+
 class ThumbnailView(
-    eventhandler.EventHandlerMixin, widgets.ScrollToCenterMixin, QListWidget
+    eventhandler.EventHandlerMixin,
+    widgets.GetNumVisibleMixin,
+    widgets.ScrollToCenterMixin,
+    widgets.ScrollWheelCumulativeMixin,
+    QListWidget,
 ):
     """Thumbnail widget.
 
     Attributes:
         _manager: ThumbnailManager class to create thumbnails asynchronously.
         _paths: Last paths loaded to avoid duplicate loading.
     """
@@ -64,16 +75,18 @@
         border: none;
         background: none;
     }
     """
 
     @api.modes.widget(api.modes.THUMBNAIL)
     @api.objreg.register
-    def __init__(self):
-        super().__init__()
+    def __init__(self) -> None:
+        widgets.ScrollWheelCumulativeMixin.__init__(self, self._scroll_wheel_callback)
+        QListWidget.__init__(self)
+
         self._paths: List[str] = []
 
         fail_pixmap = create_pixmap(
             color=styles.get("thumbnail.error.bg"),
             frame_color=styles.get("thumbnail.frame.fg"),
             size=256,
             frame_size=10,
@@ -105,14 +118,35 @@
 
         styles.apply(self)
 
     def __iter__(self) -> Iterator["ThumbnailItem"]:
         for index in range(self.count()):
             yield self.item(index)
 
+    def current_index(self) -> int:
+        """Return the index of the currently selected item."""
+        return self.currentRow()
+
+    def current_column(self) -> int:
+        """Return the column of the currently selected item."""
+        return self.current_index() % self.n_columns()
+
+    def current_row(self) -> int:
+        """Return the row of the currently selected item."""
+        return self.current_index() // self.n_columns()
+
+    def n_columns(self) -> int:
+        """Return the number of columns."""
+        sb_width = int(styles.get("image.scrollbar.width").replace("px", ""))
+        return (self.width() - sb_width) // self.item_size()
+
+    def n_rows(self) -> int:
+        """Return the number of rows."""
+        return math.ceil(self.count() / self.n_columns())
+
     def item(self, index: int) -> "ThumbnailItem":
         return cast(ThumbnailItem, super().item(index))
 
     def clear(self):
         """Override clear to also empty paths."""
         self._paths = []
         super().clear()
@@ -200,53 +234,71 @@
     @api.commands.register(mode=api.modes.THUMBNAIL)
     def open_selected(self):
         """Open the currently selected thumbnail in image mode."""
         _logger.debug("Opening selected thumbnail '%s'", self.current())
         api.signals.load_images.emit([self.current()])
         api.modes.IMAGE.enter()
 
+    @api.keybindings.register("<ctrl>b", "scroll page-up", mode=api.modes.THUMBNAIL)
+    @api.keybindings.register("<ctrl>f", "scroll page-down", mode=api.modes.THUMBNAIL)
+    @api.keybindings.register(
+        "<ctrl>u", "scroll half-page-up", mode=api.modes.THUMBNAIL
+    )
+    @api.keybindings.register(
+        "<ctrl>d", "scroll half-page-down", mode=api.modes.THUMBNAIL
+    )
     @api.keybindings.register("k", "scroll up", mode=api.modes.THUMBNAIL)
     @api.keybindings.register("j", "scroll down", mode=api.modes.THUMBNAIL)
-    @api.keybindings.register("h", "scroll left", mode=api.modes.THUMBNAIL)
-    @api.keybindings.register("l", "scroll right", mode=api.modes.THUMBNAIL)
+    @api.keybindings.register(
+        ("h", "<button-back>"), "scroll left", mode=api.modes.THUMBNAIL
+    )
+    @api.keybindings.register(
+        ("l", "<button-forward>"), "scroll right", mode=api.modes.THUMBNAIL
+    )
     @api.commands.register(mode=api.modes.THUMBNAIL)
-    def scroll(self, direction: argtypes.Direction, count=1):  # type: ignore[override]
+    def scroll(  # type: ignore[override]
+        self, direction: argtypes.DirectionWithPage, count=1
+    ):
         """Scroll to another thumbnail in the given direction.
 
         **syntax:** ``:scroll direction``
 
         positional arguments:
-            * ``direction``: The direction to scroll in (left/right/up/down).
+            * ``direction``: The direction to scroll in
+              (left/right/up/down/page-up/page-down/half-page-up/half-page-down).
 
         **count:** multiplier
         """
         _logger.debug("Scrolling in direction '%s'", direction)
-        current = self.currentRow()
-        column = current % self.columns()
-        if direction == argtypes.Direction.Right:
-            current += 1 * count
-            current = min(current, self.count() - 1)
-        elif direction == argtypes.Direction.Left:
-            current -= 1 * count
-            current = max(0, current)
-        elif direction == argtypes.Direction.Down:
-            # Do not jump between columns
-            current += self.columns() * count
-            elems_in_last_row = self.count() % self.columns()
-            if not elems_in_last_row:
-                elems_in_last_row = self.columns()
-            if column < elems_in_last_row:
-                current = min(self.count() - (elems_in_last_row - column), current)
-            else:
-                current = min(self.count() - 1, current)
+        current = self.current_index()
+        if direction == direction.Right:
+            current += count
+        elif direction == direction.Left:
+            current -= count
         else:
-            current -= self.columns() * count
-            current = max(column, current)
+            current = self._scroll_updown(current, direction, count)
         self._select_index(current)
 
+    def _scroll_updown(
+        self, current: int, direction: argtypes.DirectionWithPage, step: int
+    ) -> int:
+        """Helper function bundling the logic required to scroll up/down."""
+        if direction.is_page_step:
+            n_items = self._n_visible_items(contains=True)
+            factor = 0.5 if direction.is_half_page_step else 1
+            n_rows = int(n_items / self.n_columns() * factor)
+            step *= n_rows
+        if direction.is_reverse:  # Upwards
+            return max(self.current_column(), current - self.n_columns() * step)
+        # Do not jump between columns
+        last_in_col = (self.n_rows() - 1) * self.n_columns() + self.current_column()
+        if last_in_col > self.count() - 1:
+            last_in_col -= self.n_columns()
+        return min(current + self.n_columns() * step, last_in_col)
+
     @api.keybindings.register("gg", "goto 1", mode=api.modes.THUMBNAIL)
     @api.keybindings.register("G", "goto -1", mode=api.modes.THUMBNAIL)
     @api.commands.register(mode=api.modes.THUMBNAIL)
     def goto(self, index: Optional[int], count: Optional[int] = None):
         """Select specific thumbnail in current filelist.
 
         **syntax:** ``:goto index``
@@ -263,14 +315,27 @@
             index = number_for_command(
                 index, count, max_count=self.count(), elem_name="thumbnail"
             )
         except ValueError as e:
             raise api.commands.CommandError(str(e))
         self._select_index(index)
 
+    @api.keybindings.register("$", "end-of-line", mode=api.modes.THUMBNAIL)
+    @api.commands.register(mode=api.modes.THUMBNAIL)
+    def end_of_line(self):
+        """Select the last thumbnail in the current row."""
+        first_in_next_row = (self.current_row() + 1) * self.n_columns()
+        self._select_index(first_in_next_row - 1)
+
+    @api.keybindings.register("^", "first-of-line", mode=api.modes.THUMBNAIL)
+    @api.commands.register(mode=api.modes.THUMBNAIL)
+    def first_of_line(self):
+        """Select the first thumbnail in the current row."""
+        self._select_index(self.current_row() * self.n_columns())
+
     @api.keybindings.register("-", "zoom out", mode=api.modes.THUMBNAIL)
     @api.keybindings.register("+", "zoom in", mode=api.modes.THUMBNAIL)
     @api.commands.register(mode=api.modes.THUMBNAIL)
     def zoom(self, direction: argtypes.Zoom):
         """Zoom the current widget.
 
         **syntax:** ``:zoom direction``
@@ -302,49 +367,61 @@
         Args:
             index: Number of the current item to select.
             emit: Emit the new_thumbnail_path_selected signal.
         """
         if not self._paths:
             raise api.commands.CommandWarning("Thumbnail list is empty")
         _logger.debug("Selecting thumbnail number %d", index)
-        model_index = self.model().index(index, 0)
-        self.setCurrentIndex(model_index)
+        index = utils.clamp(index, 0, self.count() - 1)
+        self.setCurrentRow(index)
         if emit:
             synchronize.signals.new_thumbnail_path_selected.emit(self._paths[index])
 
     def _on_size_changed(self, value: int):
         _logger.debug("Setting size to %d", value)
         self.setIconSize(QSize(value, value))
         self.rescale_items()
 
-    def columns(self):
-        """Return the number of columns."""
-        sb_width = int(styles.get("image.scrollbar.width").replace("px", ""))
-        return (self.width() - sb_width) // self.item_size()
-
     def item_size(self):
         """Return the size of one icon including padding."""
         padding = int(styles.get("thumbnail.padding").replace("px", ""))
         return self.iconSize().width() + 2 * padding
 
+    @api.status.module("{thumbnail-basename}")
+    def _thumbnail_basename(self):
+        """Basename of the currently selected thumbnail."""
+        try:
+            abspath = self._paths[self.current_index()]
+            basename = os.path.basename(abspath)
+            return basename
+        except IndexError:
+            return ""
+
     @api.status.module("{thumbnail-name}")
     def _thumbnail_name(self):
-        """Name of the currently selected thumbnail."""
+        """Name without extension of the currently selected thumbnail."""
         try:
-            abspath = self._paths[self.currentRow()]
-            basename = os.path.basename(abspath)
-            name, _ = os.path.splitext(basename)
+            name, _ = os.path.splitext(self._thumbnail_basename())
             return name
         except IndexError:
             return ""
 
+    @api.status.module("{thumbnail-extension}")
+    def _thumbnail_extension(self):
+        """Extension of the currently selected thumbnail."""
+        try:
+            _, extension = os.path.splitext(self._thumbnail_basename())
+            return extension.replace(".", "")
+        except IndexError:
+            return ""
+
     def current(self):
         """Current path for thumbnail mode."""
         try:
-            return self._paths[self.currentRow()]
+            return self._paths[self.current_index()]
         except IndexError:
             return ""
 
     @staticmethod
     def pathlist() -> List[str]:
         """List of current paths for thumbnail mode."""
         return imutils.pathlist()
@@ -352,28 +429,39 @@
     @api.status.module("{thumbnail-size}")
     def size(self):
         """Current thumbnail size (small/normal/large/x-large)."""
         sizes = {64: "small", 128: "normal", 256: "large", 512: "x-large"}
         return sizes[self.iconSize().width()]
 
     @api.status.module("{thumbnail-index}")
-    def current_index(self):
+    def current_index_statusbar(self) -> str:
         """Index of the currently selected thumbnail."""
-        return str(self.currentRow() + 1)
+        return str(self.current_index() + 1).zfill(len(self.total()))
 
     @api.status.module("{thumbnail-total}")
     def total(self):
         """Total number of thumbnails."""
         return str(self.model().rowCount())
 
     def resizeEvent(self, event):
         """Update resize event to keep selected thumbnail centered."""
         super().resizeEvent(event)
         self.scrollTo(self.currentIndex())
 
+    def _scroll_wheel_callback(self, steps_x, steps_y):
+        """Callback function used by the scroll wheel mixin for mouse scrolling."""
+        if steps_y < 0:
+            self.scroll(argtypes.DirectionWithPage.Down, count=abs(steps_y))
+        elif steps_y > 0:
+            self.scroll(argtypes.DirectionWithPage.Up, count=steps_y)
+        if steps_x < 0:
+            self.scroll(argtypes.DirectionWithPage.Right, count=abs(steps_x))
+        elif steps_x > 0:
+            self.scroll(argtypes.DirectionWithPage.Left, count=steps_x)
+
 
 class ThumbnailDelegate(QStyledItemDelegate):
     """Delegate used for the thumbnail widget.
 
     The delegate draws the items.
     """
```

### Comparing `vimiv-0.8.0/vimiv/gui/transformwidget.py` & `vimiv-0.9.0/vimiv/gui/transformwidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Base class for widgets which provide a gui for more complex transformations."""
 
 import abc
 import contextlib
 import functools
+from typing import cast
 
-from PyQt5.QtCore import Qt
+from PyQt5.QtCore import Qt, QRect
 from PyQt5.QtWidgets import QWidget
 
 from vimiv.imutils import imtransform
 
 from vimiv import api, utils
 from vimiv.gui import eventhandler
+from .image import ScrollableImage
 
 
 class TransformWidget(QWidget, metaclass=utils.AbstractQObjectMeta):
     """Base class for widgets which provide a gui for more complex transformations.
 
     The child class must implement update_geometry to adapt to a resized image and
     should provide additional keybindings which implement the actual transformation.
@@ -43,16 +45,18 @@
         }
         self.transform = imtransform.Transform.instance
         self.previous_matrix = self.transform.matrix
 
         image.transformation_module = self.status_info
 
         image.resized.connect(self.update_geometry)
-        self.update_geometry()
-        self.show()
+
+    @property
+    def image(self) -> ScrollableImage:
+        return cast(ScrollableImage, self.parent())
 
     @abc.abstractmethod
     def update_geometry(self):
         """Update geometry of the widget."""
 
     def status_info(self) -> str:
         """Can be overridden by the child to display information in the status bar."""
@@ -63,22 +67,27 @@
 
         Args:
             accept: If True, keep the straightening as transformation.
         """
         if not accept:
             self.reset_transformations()
             self.transform.apply()
-        self.parent().transformation_module = None  # type: ignore
-        self.parent().setFocus()
+        self.image.transformation_module = None
+        self.image.setFocus()
         self.deleteLater()
         api.status.update("transform widget left")
 
     def reset_transformations(self):
         self.transform.setMatrix(*self.previous_matrix)
 
+    @property
+    def image_rect(self) -> QRect:
+        """Rectangle occupied by the image within the parent widget."""
+        return self.image.mapFromScene(self.image.sceneRect()).boundingRect()
+
     def keyPressEvent(self, event):
         """Run binding from bindings dictionary."""
         with contextlib.suppress(ValueError, KeyError):
             keysequence = eventhandler.keyevent_to_sequence(event)
             binding = self.bindings[keysequence]
             api.status.clear("transform binding")
             binding()
```

### Comparing `vimiv-0.8.0/vimiv/gui/version_popup.py` & `vimiv-0.9.0/vimiv/gui/version_popup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Pop-up window to display version information."""
 
 from PyQt5.QtWidgets import QLabel, QVBoxLayout, QPushButton
 from PyQt5.QtGui import QGuiApplication
```

### Comparing `vimiv-0.8.0/vimiv/imutils/__init__.py` & `vimiv-0.9.0/vimiv/imutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """`Utilities to load, edit, navigate and save images`.
 
 The Image Loading Process
 ,,,,,,,,,,,,,,,,,,,,,,,,,
 
@@ -34,15 +34,15 @@
 * ``movie_loaded`` for animated Gifs
 * ``svg_loaded`` for vector graphics
 
 The image widget in ``vimiv.gui.image`` connects to these signals and displays
 the appropriate Qt widget.
 """
 
-from vimiv.imutils import exif
+from vimiv.imutils import metadata
 from vimiv.imutils.edit_handler import EditHandler
 from vimiv.imutils.filelist import current, pathlist
 from vimiv.imutils.filelist import SignalHandler as _FilelistSignalHandler
 from vimiv.imutils._file_handler import ImageFileHandler as _ImageFileHandler
 
 
 def init():
```

### Comparing `vimiv-0.8.0/vimiv/imutils/_file_handler.py` & `vimiv-0.9.0/vimiv/imutils/_file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Classes to deal with the actual image file."""
 
 import os
 import shutil
 import tempfile
@@ -120,15 +120,15 @@
             except ValueError as e:
                 log.error("%s", e)
                 return
             self._edit_handler.pixmap = pixmap
             api.signals.pixmap_loaded.emit(pixmap, keep_zoom)
         self._path = path
 
-    @api.commands.register(mode=api.modes.IMAGE)
+    @api.commands.register(mode=api.modes.IMAGE, edit=True)
     def write(self, path: List[str]):
         """Save the current image to disk.
 
         **syntax:** ``:write [path]``.
 
         positional arguments:
             * ``path``: Save to this path instead of the current one.
@@ -147,14 +147,15 @@
             pixmap: The QPixmap to write.
             path: The path to save the pixmap to.
             original_path: Original path of the opened pixmap.
             parallel: Perform operation in parallel.
         """
         if not path:
             path = original_path = self._path
+        path = os.path.abspath(os.path.expanduser(path))
         if parallel:
             asyncrun(write_pixmap, pixmap, path, original_path)
         else:
             write_pixmap(pixmap, path, original_path)
         self._edit_handler.reset()
 
 
@@ -167,15 +168,15 @@
     temporary file if possible and finally rename the temporary file to the
     final path. The renaming is done as it is an atomic operation and we may be
     overriding the existing file.
 
     Args:
         pixmap: The QPixmap to write.
         path: Path to write the pixmap to.
-        original_path: Original path of the opened pixmap to retrieve exif information.
+        original_path: Original path of the opened pixmap to retrieve metadata.
     """
     try:
         _can_write(pixmap, path)
         _logger.debug("Image is writable")
         _write(pixmap, path, original_path)
         log.info("Saved %s", path)
     except WriteError as e:
@@ -205,18 +206,18 @@
     """
     # Get pixmap type
     _, ext = os.path.splitext(path)
     # First create temporary file and then move it to avoid race conditions
     handle, filename = tempfile.mkstemp(suffix=ext)
     os.close(handle)
     pixmap.save(filename)
-    # Copy exif info from original file to new file
+    # Best-effort copy metadata info from original file to new file
     try:
-        imutils.exif.ExifHandler(original_path).copy_exif(filename)
-    except imutils.exif.UnsupportedExifOperation:
+        imutils.metadata.MetadataHandler(original_path).copy_metadata(filename)
+    except imutils.metadata.MetadataError:
         pass
     shutil.move(filename, path)
     # Check if valid image was created
     if not os.path.isfile(path):
         raise WriteError("File not written, unknown exception")
     if not files.is_image(path):
         os.remove(path)
```

### Comparing `vimiv-0.8.0/vimiv/imutils/current_pixmap.py` & `vimiv-0.9.0/vimiv/imutils/current_pixmap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Storage class for the current pixmap."""
 
 from PyQt5.QtGui import QPixmap
```

### Comparing `vimiv-0.8.0/vimiv/imutils/edit_handler.py` & `vimiv-0.9.0/vimiv/imutils/edit_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Handler class as man-in-the-middle between file handler and the edit classes."""
 
 from PyQt5.QtCore import QObject
 from PyQt5.QtGui import QPixmap
```

### Comparing `vimiv-0.8.0/vimiv/imutils/filelist.py` & `vimiv-0.9.0/vimiv/imutils/filelist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Filelist of images.
 
 The module provides methods to navigate and update the current image filelist. Once a
 new image in the filelist is selected, it is passed on to the file handler to open it.
 """
@@ -25,15 +25,17 @@
 _paths: List[str] = []
 _index = 0
 _logger = log.module_logger(__name__)
 
 
 # We want to use the name next here as it is the best name for the command
 @api.keybindings.register("<ctrl>n", "next --keep-zoom", mode=api.modes.IMAGE)
-@api.keybindings.register(["n", "<page-down>"], "next", mode=api.modes.IMAGE)
+@api.keybindings.register(
+    ("n", "<page-down>", "<button-forward>"), "next", mode=api.modes.IMAGE
+)
 @api.commands.register(name="next")
 def next_path(count: int = 1, keep_zoom: bool = False) -> None:
     """Select next image.
 
     **syntax:** ``:next [--keep-zoom]``
 
     optional arguments:
@@ -42,15 +44,17 @@
     **count:** multiplier
     """
     if _paths:
         _set_index((_index + count) % len(_paths), keep_zoom=keep_zoom)
 
 
 @api.keybindings.register("<ctrl>p", "prev --keep-zoom", mode=api.modes.IMAGE)
-@api.keybindings.register(["p", "<page-up>"], "prev", mode=api.modes.IMAGE)
+@api.keybindings.register(
+    ("p", "<page-up>", "<button-back>"), "prev", mode=api.modes.IMAGE
+)
 @api.commands.register(name="prev")
 def prev_path(count: int = 1, keep_zoom: bool = False) -> None:
     """Select previous image.
 
     **syntax:** ``:prev [--keep-zoom]``
 
     optional arguments:
@@ -96,14 +100,28 @@
 
 @api.status.module("{basename}")
 def basename() -> str:
     """Basename of the current image."""
     return os.path.basename(current())
 
 
+@api.status.module("{name}")
+def name() -> str:
+    """Name without extension of the current image."""
+    filename, _ = os.path.splitext(basename())
+    return filename
+
+
+@api.status.module("{extension}")
+def extension() -> str:
+    """File extension of the current image."""
+    _, fileextension = os.path.splitext(basename())
+    return fileextension.replace(".", "")
+
+
 @api.status.module("{index}")
 def get_index() -> str:  # Needs to be called get as we use index as variable often
     """Index of the current image."""
     if _paths:
         return str(_index + 1).zfill(len(total()))
     return "0"
 
@@ -119,16 +137,16 @@
     """Exif creation date and time of the current image.
 
     This is meant as an example api.status.module to show how to display exif
     data in the statusbar. If there are any requests/ideas for more, this can
     be used as basis to work with.
     """
     try:
-        return imutils.exif.ExifHandler(current()).exif_date_time()
-    except imutils.exif.UnsupportedExifOperation:
+        return imutils.metadata.MetadataHandler(current()).get_date_time()
+    except imutils.metadata.MetadataError:
         return ""
 
 
 def pathlist() -> List[str]:
     """Return the currently loaded list of paths."""
     return _paths
 
@@ -148,14 +166,15 @@
         search.search.new_search.connect(self._on_new_search)
         # The slideshow object is created here as it is not required by anything else
         # It stays around as it is part of the global object registry
         slideshow.event.connect(self._on_slideshow_event)
 
         api.signals.load_images.connect(self._on_load_images)
         api.working_directory.handler.images_changed.connect(self._on_images_changed)
+        api.settings.sort.shuffle.changed.connect(self._on_shuffle)
 
     @pyqtSlot(list)
     def _on_load_images(self, paths: List[str]):
         """Load new paths into the filelist.
 
         This function is used from outside to interact with the filelist. For example by
         the library to update the current selection or by the app to open image paths.
@@ -168,15 +187,15 @@
         if not paths:
             _logger.debug("Image filelist: no paths to load")
         elif len(paths) == 1:
             _logger.debug("Image filelist: loading single path %s", paths[0])
             _load_single(*paths)
         else:
             _logger.debug("Image filelist: loading %d paths", len(paths))
-            _load_paths(paths, paths[0])
+            _load_paths(paths)
 
     @pyqtSlot(int, list, api.modes.Mode, bool)
     def _on_new_search(
         self, index: int, _matches: List[str], mode: api.modes.Mode, incremental: bool
     ):
         """Select search result after new search.
 
@@ -214,14 +233,20 @@
         if not paths:
             _clear()
             api.status.update("Image filelist cleared")
         else:
             _load_paths(paths, current())
             api.status.update("Image filelist changed")
 
+    @utils.slot
+    def _on_shuffle(self):
+        """Reload paths to force shuffling."""
+        if _paths:
+            _load_paths(_paths, current())
+
 
 def _set_index(index: int, previous: str = None, *, keep_zoom: bool = False) -> None:
     """Set the global _index to index."""
     global _index
     _index = index
     if previous != current():
         api.signals.new_image_opened.emit(current(), keep_zoom)
@@ -240,25 +265,27 @@
         goto(_paths.index(path) + 1)  # goto is indexed from 1
     elif path not in api.working_directory.handler.images and files.is_image(path):
         _load_paths([path, *api.working_directory.handler.images], path)
     else:
         _load_paths(api.working_directory.handler.images, path)
 
 
-def _load_paths(paths: Iterable[str], focused_path: str) -> None:
+def _load_paths(paths: Iterable[str], focused_path: str = None) -> None:
     """Populate imstorage with a new list of paths.
 
     Args:
         paths: List of paths to load.
-        focused_path: The path to display.
+        focused_path: The path to display if defined.
     """
     paths = [os.path.abspath(path) for path in paths]
-    focused_path = os.path.abspath(focused_path)
-    if api.settings.shuffle.value:
+    if api.settings.sort.shuffle.value:
         random.shuffle(paths)
+    else:
+        paths = api.settings.sort.image_order.sort(paths)
+    focused_path = os.path.abspath(focused_path) if focused_path else paths[0]
     previous = current()
     _set_paths(paths)
     index = (
         paths.index(focused_path)
         if focused_path in paths
         else min(len(paths) - 1, _index)
     )
```

### Comparing `vimiv-0.8.0/vimiv/imutils/immanipulate.py` & `vimiv-0.9.0/vimiv/imutils/immanipulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """*immanipulate - more complex image manipulations like brightness and contrast*.
 
 The module includes classes in a hierarchical structure where each following class
 includes components of the previous class in the hierarchy.
 
@@ -352,15 +352,15 @@
     pool = utils.Pool.get(globalinstance=False)
     pool.setMaxThreadCount(1)  # Only one manipulation is run in parallel
 
     accepted = pyqtSignal(QPixmap)
     updated = pyqtSignal(QPixmap)
 
     @api.objreg.register
-    def __init__(self, current_pixmap):
+    def __init__(self, current_pixmap: QPixmap):
         super().__init__()
 
         self.manipulations = Manipulations()
 
         self._changes: List[ManipulationChange] = []
         self._current_manipulation = self.manipulations[0]  # Default manipulation
         self._current_manipulation.focus()
```

### Comparing `vimiv-0.8.0/vimiv/imutils/imtransform.py` & `vimiv-0.9.0/vimiv/imutils/imtransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """*imtransform - transformations such as rotate and flip*."""
 
 import functools
 import math
 from typing import Optional
@@ -28,15 +28,15 @@
         def inner(self, *args, **kwargs):
             # Only used to wrap methods of transform
             # pylint: disable=protected-access
             self._ensure_editable()
             func(self, *args, **kwargs)
             self.apply()
 
-        return api.commands.register(mode=api.modes.IMAGE, **kwargs)(inner)
+        return api.commands.register(mode=api.modes.IMAGE, edit=True, **kwargs)(inner)
 
     return decorator
 
 
 class Transform(QTransform):
     """Apply transformations to an image.
 
@@ -165,14 +165,17 @@
         self.rotate(angle)
         transformed = self.original.transformed(self, mode=Qt.SmoothTransformation)
         rect = self.largest_rect_in_rotated(
             original=original_size, rotated=transformed.size(), angle=angle
         )
         self._apply(transformed.copy(rect))
 
+    def crop(self, rect):
+        self._apply(self.current.copy(rect))
+
     def _apply(self, transformed):
         """Check the transformed pixmap for validity and apply it to the handler."""
         if transformed.isNull():
             raise api.commands.CommandError(
                 "Error transforming image, ignoring transformation.\n"
                 "Is the resulting image too large? Zero?."
             )
@@ -181,15 +184,21 @@
     def _ensure_editable(self):
         if not self._current.editable:
             raise api.commands.CommandError("File format does not support transform")
 
     @property
     def changed(self):
         """True if transformations have been applied."""
-        return not self.isIdentity()
+        if self.current.rect().isNull():
+            return False
+        transformed = not self.isIdentity()
+        if self._original is None:
+            return transformed
+        cropped = self.current.rect() != self._original.rect()
+        return transformed or cropped
 
     @property
     def matrix(self):
         """Tuple of matrix elements defining the current transformation matrix."""
         # fmt: off
         return (
             self.m11(), self.m12(), self.m13(),
@@ -199,15 +208,15 @@
         # fmt: on
 
     @property
     def size(self) -> QSize:
         """Size of the transformed image."""
         return self.current.size()
 
-    @api.commands.register(mode=api.modes.IMAGE)
+    @register_transform_command()
     def undo_transformations(self):
         """Undo any transformation applied to the current image."""
         self.reset()
         self.transformed.emit(self.original)
 
     @classmethod
     def largest_rect_in_rotated(
@@ -234,15 +243,15 @@
         sin_a = abs(math.sin(rad))
         cos_a = abs(math.cos(rad))
 
         if short <= 2.0 * sin_a * cos_a * long or abs(sin_a - cos_a) < 1e-10:
             s = 0.5 * short
             wr, hr = (s / cos_a, s / sin_a) if is_portrait else (s / sin_a, s / cos_a)
         else:
-            cos_2a = cos_a ** 2 - sin_a ** 2
+            cos_2a = cos_a**2 - sin_a**2
             wr = (original.width() * cos_a - original.height() * sin_a) / cos_2a
             hr = (original.height() * cos_a - original.width() * sin_a) / cos_2a
 
         x = (rotated.width() - wr) // 2
         y = (rotated.height() - hr) // 2
 
         return QRect(int(x), int(y), int(wr), int(hr))
```

### Comparing `vimiv-0.8.0/vimiv/imutils/slideshow.py` & `vimiv-0.9.0/vimiv/imutils/slideshow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Module to play a slideshow."""
 
 from typing import Optional
 
 from PyQt5.QtCore import QTimer
```

### Comparing `vimiv-0.8.0/vimiv/parser.py` & `vimiv-0.9.0/vimiv/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """The commandline argument parser and related functions."""
 
 import argparse
 import contextlib
 import logging
 import os
+import shlex
+from typing import List
 
 from PyQt5.QtCore import QSize
 
 import vimiv
 
 
 def get_argparser() -> argparse.ArgumentParser:
@@ -52,15 +54,15 @@
         metavar="FILE",
         help="Use FILE as keybinding file",
     )
     parser.add_argument(
         "-s",
         "--set",
         nargs=2,
-        default=[],  # List is required for action="append"
+        default=[],  # List is required for iterating
         action="append",
         dest="cmd_settings",
         metavar=("OPTION", "VALUE"),
         help="Set a temporary setting",
     )
     parser.add_argument(
         "--log-level",
@@ -77,23 +79,41 @@
     )
     parser.add_argument(
         "-b", "--basedir", metavar="DIRECTORY", help="Directory to use for all storage"
     )
     parser.add_argument(
         "paths", nargs="*", type=existing_path, metavar="PATH", help="Paths to open"
     )
+    parser.add_argument(
+        "-o",
+        "--output",
+        metavar="TEXT",
+        help="Wildcard expanded string to print to standard output upon quit",
+    )
+    parser.add_argument(
+        "-i",
+        "--input",
+        action="store_true",
+        help="Read paths to open from standard input",
+        dest="stdinput",
+    )
 
     devel = parser.add_argument_group("development arguments")
     devel.add_argument(
         "--debug",
         nargs="+",
         metavar="MODULE",
         default=(),
         help="Force showing debug log messages of MODULE",
     )
+    devel.add_argument(
+        "--qt-args",
+        metavar="ARGS",
+        help="Arguments to pass to qt directly, use quotes to pass multiple arguments",
+    )
     return parser
 
 
 def positive_int(value: str) -> int:
     """Check if an argument value is a positive int.
 
     Args:
@@ -161,7 +181,14 @@
         value: Value given to command option as string.
     Returns:
         value as logging level.
     """
     with contextlib.suppress(AttributeError):
         return getattr(logging, value.upper())
     raise argparse.ArgumentTypeError(f"Invalid log level '{value}'")
+
+
+def get_qt_args(args: argparse.Namespace) -> List[str]:
+    """Retrieve list of arguments to pass to qt from argparse namespace."""
+    if args.qt_args:
+        return shlex.split(args.qt_args)
+    return []
```

### Comparing `vimiv-0.8.0/vimiv/plugins/__init__.py` & `vimiv-0.9.0/vimiv/plugins/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """`Interface to load and initialize plugins`.
 
 Plugins are python modules that are either in ``vimiv/plugins/`` (app plugins) or
 ``$XDG_DATA_HOME/vimiv/plugins/`` (user plugins). A possible path is to write a plugin
 in its own git repository and let the user to clone that repository into
@@ -65,20 +65,22 @@
 import importlib
 import os
 import sys
 import types
 from typing import Dict, List
 
 from vimiv.utils import xdg, log, quotedjoin
+from vimiv import api
 
 
 _app_plugin_directory = os.path.dirname(__file__)
 _user_plugin_directory = xdg.vimiv_data_dir("plugins")
 _plugins: Dict[str, str] = {
-    "print": "default"
+    "print": "default",
+    "metadata": "default",
 }  # key: name, value: additional information
 _loaded_plugins: Dict[str, types.ModuleType] = {}  # key:name, value: loaded module
 _logger = log.module_logger(__name__)
 
 
 def load() -> None:
     """Load plugins defined.
@@ -108,40 +110,47 @@
                 "    User plugin directory: '%s'",
                 plugin,
                 quotedjoin(app_plugins),
                 quotedjoin(user_plugins),
                 _user_plugin_directory,
             )
     _logger.debug("Plugin loading completed")
+    api.signals.plugins_loaded.emit()
 
 
 def cleanup() -> None:
     """Clean up all loaded plugins.
 
     This calls the cleanup function for all loaded plugins and is called before vimiv is
     closed.
     """
     _logger.debug("Cleaning up plugins")
     for name, module in _loaded_plugins.items():
         try:
-            # AttributeError is caught afterwards, the module may or may not define
-            # cleanup
-            module.cleanup()  # type: ignore
+            module.cleanup()
             _logger.debug("Cleaned up '%s'", name)
         except AttributeError:
             _logger.debug("Plugin '%s' does not define cleanup()", name)
 
 
 def add_plugins(**plugins: str) -> None:
     """Add plugins to the dictionary of plugins.
 
+    Note that the plugins are prepended, and take precedence above the existing plugins.
+
     Args:
         plugins: Dictionary of plugin names with metadata to add to plugins.
     """
-    _plugins.update(plugins)
+    global _plugins
+
+    for plugin, info in _plugins.items():
+        if plugin not in plugins:
+            plugins[plugin] = info
+
+    _plugins = plugins
 
 
 def get_plugins() -> Dict[str, str]:
     """Retrieve dictionary containing active plugin names and additional information."""
     return dict(_plugins)
 
 
@@ -156,16 +165,15 @@
     _logger.debug("Loading plugin '%s' from '%s'", name, directory)
     try:
         module = importlib.import_module(name, directory)
     except (ImportError, SyntaxError) as e:
         log.error("Importing plugin '%s': %s", name, str(e))
         return
     try:
-        # AttributeError is caught afterwards, the module may or may not define init
-        module.init(info)  # type: ignore
+        module.init(info)
         _logger.debug("Initialized '%s'", name)
     except AttributeError:
         _logger.debug("Plugin '%s' does not define init()", name)
     _logger.debug("Loaded '%s' successfully", name)
     _loaded_plugins[name] = module
```

### Comparing `vimiv-0.8.0/vimiv/plugins/demo.py` & `vimiv-0.9.0/vimiv/plugins/demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Simple hello world greeting as example plugin.
 
 The plugin defines a new command :hello-world which simply prints a message to the
 terminal. The init and cleanup functions also print messages to the terminal without
 further usage for demonstration purposes.
```

### Comparing `vimiv-0.8.0/vimiv/plugins/print.py` & `vimiv-0.9.0/vimiv/plugins/print.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Plugin enabling print support."""
 
 import abc
 from typing import Optional, Any, Union
 
-from PyQt5.QtCore import QObject, Qt, QSize, pyqtSignal
+from PyQt5.QtCore import QObject, Qt, QSize, pyqtBoundSignal
 from PyQt5.QtGui import QPixmap, QMovie, QPainter
 from PyQt5.QtPrintSupport import QPrintDialog, QPrintPreviewDialog, QPrinter
 
 from vimiv import api
 from vimiv.utils import slot, log, lazy
 
 QtSvg = lazy.import_module("PyQt5.QtSvg", optional=True)
@@ -63,15 +63,15 @@
             _logger.debug("Starting print dialog")
             self.handle_print(self._widget, QPrintDialog(), auto_apply_orientation=True)
 
     @staticmethod
     def handle_print(
         widget: "PrintWidget",
         dialog: Union[QPrintPreviewDialog, QPrintDialog],
-        *signals: pyqtSignal,
+        *signals: pyqtBoundSignal,
         auto_apply_orientation: bool = False,
     ) -> None:
         """Handle a print request of widget for a specific dialog."""
 
         def handler() -> None:
             widget.print(dialog.printer(), auto_apply_orientation)
```

### Comparing `vimiv-0.8.0/vimiv/startup.py` & `vimiv-0.9.0/vimiv/startup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Main function and startup utilities for vimiv.
 
 Module Attributes:
     _tmpdir: TemporaryDirectory when running with ``--temp-basedir``. The
         object must exist until vimiv exits.
 """
 
 import argparse
 import os
 import sys
 import tempfile
-from typing import List
+from typing import cast, List
 
-from PyQt5.QtCore import QSize
+from PyQt5.QtCore import QSize, QCoreApplication
 from PyQt5.QtWidgets import QApplication
 
 from vimiv import app, api, parser, imutils, plugins
-from vimiv.commands import runners, search
+from vimiv.commands import runners, search, wildcards
 from vimiv.config import configfile, keyfile, styles
 from vimiv.gui import mainwindow
 from vimiv.utils import xdg, crash_handler, log, trash_manager, customtypes, migration
 
 # Must be imported to create the commands using the decorators
 from vimiv.commands import (  # pylint: disable=unused-import
     misccommands,
@@ -38,15 +38,16 @@
 _tmpdir = None
 _logger = log.module_logger(__name__)
 
 
 def main() -> int:
     """Run startup and the Qt main loop."""
     args = setup_pre_app(sys.argv[1:])
-    qapp = app.Application()
+    qt_args = parser.get_qt_args(args)
+    qapp = app.Application(*qt_args)
     crash_handler.CrashHandler(qapp)
     setup_post_app(args)
     _logger.debug("Startup completed, starting Qt main loop")
     returncode = qapp.exec_()
     plugins.cleanup()
     _logger.debug("Exiting with status %d", returncode)
     return returncode
@@ -84,39 +85,55 @@
     # Must be done after UI so the search signals are processed after the widgets have
     # been updated
     search.search.connect_signals()
     plugins.load()
     init_paths(args)
     if args.command:
         run_startup_commands(*args.command)
+    if args.output:
+
+        def print_output() -> None:
+            print(wildcards.expand_internal(args.output, api.modes.current()))
+
+        # We are sure we have an application here
+        qapp = cast(QApplication, QCoreApplication.instance())
+        qapp.aboutToQuit.connect(print_output)
 
 
 def init_directories(args: argparse.Namespace) -> None:
     """Create vimiv cache, config and data directories.
 
     The directories are either the directories defined in the freedesktop
     standard or located in a temporary base directory.
 
     Args:
         args: Arguments returned from parser.parse_args().
     """
     if args.temp_basedir:
         global _tmpdir
+        # We want the temporary directory to stick around until the end
+        # pylint: disable=consider-using-with
         _tmpdir = tempfile.TemporaryDirectory(prefix="vimiv-tempdir-")
         args.basedir = _tmpdir.name
     if args.basedir is not None:
         xdg.basedir = args.basedir
     xdg.makedirs(xdg.vimiv_cache_dir(), xdg.vimiv_config_dir(), xdg.vimiv_data_dir())
 
 
 def init_paths(args: argparse.Namespace) -> None:
     """Open paths given from commandline or fallback to library if set."""
     _logger.debug("Opening paths")
+    read_stdin = args.stdinput and not sys.stdin.isatty()
+    paths = (
+        [os.path.realpath(line.strip()) for line in sys.stdin]
+        if read_stdin
+        else args.paths
+    )
     try:
-        api.open_paths(args.paths)
+        api.open_paths(paths)
     except api.commands.CommandError:
         _logger.debug("init_paths: No valid paths retrieved")
         if api.settings.startup_library.value:
             api.open_paths([os.getcwd()])
     api.status.update("startup paths initialized")
```

### Comparing `vimiv-0.8.0/vimiv/utils/__init__.py` & `vimiv-0.9.0/vimiv/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Various utility functions."""
 
 import abc
 import functools
 import inspect
@@ -201,15 +201,15 @@
         @slot
         def function(self, x: int, y: int) -> None:
         ...
     """
     annotations = typing.get_type_hints(function)
     args = _slot_args(function, annotations)
     kwargs = _slot_kwargs(annotations)
-    return pyqtSlot(*args, **kwargs)(function)
+    return pyqtSlot(*args, **kwargs)(function)  # type: ignore[return-value]
 
 
 def _slot_args(function, annotations):
     """Create arguments for pyqtSlot from function arguments.
 
     Args:
         function: The python function for which the arguments are created.
@@ -522,7 +522,19 @@
             throttle.setInterval(0)
 
     @classmethod
     def stop_all(cls):
         """Stop all running throttles."""
         for throttle in cls.throttles:
             throttle.stop()
+
+
+def natural_sort(text: str) -> typing.List[typing.Union[str, int]]:
+    """Key function for natural sort.
+
+    Credits to https://stackoverflow.com/a/5967539/5464989
+    """
+
+    def convert(t: str) -> typing.Union[str, int]:
+        return int(t) if t.isdigit() else t
+
+    return [convert(c) for c in re.split(r"(\d+)", text)]
```

### Comparing `vimiv-0.8.0/vimiv/utils/crash_handler.py` & `vimiv-0.9.0/vimiv/utils/crash_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Handler for uncaught exceptions and signals."""
 
 import functools
 import os
 import signal
 import sys
 import types
-from typing import Callable, Type
+from typing import Callable, Optional, Type
 
 from PyQt5.QtCore import QTimer, QSocketNotifier, QObject
 from PyQt5.QtWidgets import QApplication
 
 from vimiv.utils import log, customtypes
 
 # Fails on windows
@@ -26,18 +26,15 @@
     # Mypy does not approve that we assign None to a module but that is exactly what we
     # want to do for the optional import
     fcntl = None  # type: ignore
 
 ExceptionHandler = Callable[
     [Type[BaseException], BaseException, types.TracebackType], None
 ]
-# See https://github.com/PyCQA/pylint/issues/2804
-SignalHandler = Callable[
-    [signal.Signals, types.FrameType], None  # pylint: disable=no-member
-]
+SignalHandler = Callable[[int, Optional[types.FrameType]], None]
 
 _logger = log.module_logger(__name__)
 
 
 class CrashHandler(QObject):
     """Handler for uncaught exceptions and signals.
 
@@ -67,16 +64,15 @@
         """
         _logger.debug("Setting up wakeup filedescriptor for unix-like systems")
         read_fd, write_fd = os.pipe()
         for fd in (read_fd, write_fd):
             flags = fcntl.fcntl(fd, fcntl.F_GETFL)
             fcntl.fcntl(fd, fcntl.F_SETFL, flags | os.O_NONBLOCK)
         notifier = QSocketNotifier(read_fd, QSocketNotifier.Read, self)  # type: ignore
-        # Signal misinterpreted as a callable
-        notifier.activated.connect(lambda: None)  # type: ignore
+        notifier.activated.connect(lambda: None)
         signal.set_wakeup_fd(write_fd)
 
     def _setup_timer(self, timeout: int = 1000) -> None:
         """Set up a timer for signal handling.
 
         The timer gets called every timeout ms and returns the control from the Qt main
         loop in C++ back to python and allows signal handling in python. Available on
@@ -109,29 +105,31 @@
         # We exit immediately by killing the application if an error in the graceful
         # exit occurs
         except Exception as e:  # pylint: disable=broad-except
             log.fatal("Uncaught exception in graceful exit... Committing suicide :(")
             log.fatal("Exception: %r", e)
             sys.exit(customtypes.Exit.err_suicide)
 
-    def handle_interrupt(self, signum: int, _frame: types.FrameType) -> None:
+    def handle_interrupt(self, signum: int, _frame: Optional[types.FrameType]) -> None:
         """Initial handler for interrupt signals to exit gracefully.
 
         Args:
             signum: Signal number of the interrupt signal retrieved.
         """
         _logger.debug("Interrupt handler called with signal %d", signum)
         _assign_interrupt_handler(self.handle_interrupt_forcefully)
         log.info("SIGINT/SIGTERM received, exiting gracefully...")
         log.info("To kill the process repeat the signal")
         QTimer.singleShot(
             0, functools.partial(self._app.exit, customtypes.Exit.signal + signum)
         )
 
-    def handle_interrupt_forcefully(self, signum: int, _frame: types.FrameType) -> None:
+    def handle_interrupt_forcefully(
+        self, signum: int, _frame: Optional[types.FrameType]
+    ) -> None:
         """Second handler for interrupt signals to exit forcefully.
 
         Args:
             signum: Signal number of the interrupt signal retrieved.
         """
         _logger.debug("Interrupt handler called a second time with %d", signum)
         log.fatal("Forceful kill signal retrieved... Hello darkness my old friend")
```

### Comparing `vimiv-0.8.0/vimiv/utils/customtypes.py` & `vimiv-0.9.0/vimiv/utils/customtypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Custom data types."""
 
 import enum
 import typing
```

### Comparing `vimiv-0.8.0/vimiv/utils/debug.py` & `vimiv-0.9.0/vimiv/utils/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Various utility functions for debugging and profiling."""
 
 import contextlib
 import cProfile
 import functools
```

### Comparing `vimiv-0.8.0/vimiv/utils/imagereader.py` & `vimiv-0.9.0/vimiv/utils/imagereader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Image reader classes to read images from file to Qt objects."""
 
 import abc
 from typing import Dict, Callable
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QImageReader, QPixmap, QImage
 
-from .files import imghdr
+from vimiv.utils import imageheader
 
 external_handler: Dict[str, Callable[[str], QPixmap]] = {}
 
 
 class BaseReader(abc.ABC):
     """Base class for image readers.
 
@@ -45,28 +45,27 @@
 
     def get_image(self, size: int) -> QImage:
         """Read self.path from disk and return a scaled QImage."""
         pixmap = self.get_pixmap().scaled(size, size, Qt.KeepAspectRatio)
         return pixmap.toImage()
 
     @classmethod
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def supports(cls, file_format: str) -> bool:
         """Return True if the file_format is supported."""
 
 
 class QtReader(BaseReader):
     """Image reader using Qt's QImageReader implementation under the hood."""
 
     def __init__(self, path: str, file_format: str):
         super().__init__(path, file_format)
         self._handler = QImageReader(path, file_format.encode())
         self._handler.setAutoTransform(True)
         if not self._handler.canRead():
-            # TODO
             raise ValueError(f"'{path}' cannot be read as image")
 
     @classmethod
     def supports(cls, file_format: str) -> bool:
         return file_format in QImageReader.supportedImageFormats()
 
     @property
@@ -98,25 +97,28 @@
         return file_format in external_handler
 
     def get_pixmap(self) -> QPixmap:
         handler = external_handler[self.file_format]
         return handler(self.path)
 
 
-READERS = [QtReader, ExternalReader]
-
-
 def get_reader(path: str) -> BaseReader:
     """Retrieve the appropriate image reader class for path."""
     error = ValueError(f"'{path}' cannot be read as image")
     try:
-        file_format = imghdr.what(path)
+        file_format = imageheader.detect(path)
     except OSError:
         raise error
     if file_format is None:
         raise error
 
-    for readercls in READERS:
-        if readercls.supports(file_format):
-            return readercls(path, file_format)
+    # Prioritize external reader over qt reader to ensure that a external reader can
+    # overwrite a default reader for the same image format.
+    # Used when one wants to use a different methods for generating the QPixmap than how
+    # Qt does it, for a given format.
+    if ExternalReader.supports(file_format):
+        return ExternalReader(path, file_format)
+
+    if QtReader.supports(file_format):
+        return QtReader(path, file_format)
 
     raise error
```

### Comparing `vimiv-0.8.0/vimiv/utils/lazy.py` & `vimiv-0.9.0/vimiv/utils/lazy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Provides the import_module function for lazy importing."""
 
 import functools
 import sys
 import types
```

### Comparing `vimiv-0.8.0/vimiv/utils/log.py` & `vimiv-0.9.0/vimiv/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """`Utilities related to logging`.
 
 There are two different types of loggers: the application-wide logger and module
 specific loggers.
 
@@ -43,15 +43,15 @@
 
     _logger.debug("Something happened, and may now happen very often", once=True)
 """
 
 import logging
 from typing import Dict, List, Optional, Any, Set
 
-from PyQt5.QtCore import pyqtSignal, QObject
+from PyQt5.QtCore import pyqtSignal, QObject, QLoggingCategory
 
 import vimiv
 
 from vimiv.utils import xdg
 
 
 _module_loggers: Dict[str, "LazyLogger"] = {}
@@ -107,14 +107,19 @@
     # mode=w creates a new file for every new vimiv process
     file_handler = logging.FileHandler(xdg.vimiv_data_dir("vimiv.log"), mode="w")
     file_handler.setFormatter(formatter)
     # Configure app logger
     _app_logger.level = level
     _app_logger.handlers = [file_handler, console_handler, statusbar_loghandler]
     LazyLogger.handlers = [console_handler, file_handler]
+    # Disable qt logging at higher log levels
+    if level > logging.ERROR:
+        QLoggingCategory.setFilterRules("*.warning=false\n*.critical=false")
+    elif level > logging.WARNING:
+        QLoggingCategory.setFilterRules("*.warning=false")
     # Setup debug logging for specific module loggers
     _debug_loggers.extend(debug_modules)
     for name, logger in _module_loggers.items():
         logger.level = logging.DEBUG if name in debug_modules else level
 
 
 def module_logger(name: str) -> "LazyLogger":
@@ -193,15 +198,17 @@
 
     Signals:
         message: Emitted with severity and message on log message.
     """
 
     message = pyqtSignal(str, str)
 
-    def handle(self, record: logging.LogRecord) -> None:
+    def handle(self, record: logging.LogRecord) -> bool:
         if record.levelno >= logging.INFO:  # Debug in the statusbar makes no sense
             self.message.emit(record.levelname.lower(), record.message)
+            return True
+        return False
 
 
 _app_logger = LazyLogger(f"{vimiv.__name__}")
 log = _app_logger.log
 statusbar_loghandler = StatusbarLogHandler()
```

### Comparing `vimiv-0.8.0/vimiv/utils/migration.py` & `vimiv-0.9.0/vimiv/utils/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Tools to help with migration from the deprecated gtk version."""
 
 import os
 import shutil
 from typing import NamedTuple, Optional, List
```

### Comparing `vimiv-0.8.0/vimiv/utils/thumbnail_manager.py` & `vimiv-0.9.0/vimiv/utils/thumbnail_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """ThumbnailManager to create thumbnails asynchronously.
 
 The ThumbnailManager class uses the Creator classes to create thumbnails for a
 list of paths. When one thumbnail was created, the 'created' signal is emitted
 with the index and the QPixmap of the generated thumbnail for the thumbnail
@@ -18,14 +18,15 @@
 import tempfile
 from typing import Dict, List
 
 from PyQt5.QtCore import QRunnable, pyqtSignal, QObject
 from PyQt5.QtGui import QIcon, QPixmap, QImage
 
 import vimiv
+from vimiv import api
 from vimiv.utils import xdg, imagereader, Pool
 
 
 KEY_URI = "Thumb::URI"
 KEY_MTIME = "Thumb::MTime"
 KEY_SIZE = "Thumb::Size"
 KEY_WIDTH = "Thumb::Image::Width"
@@ -127,14 +128,32 @@
         uri = self._get_source_uri(path)
         return hashlib.md5(uri.encode()).hexdigest() + ".png"
 
     @staticmethod
     def _get_source_mtime(path: str) -> int:
         return int(os.path.getmtime(path))
 
+    def _save_thumbnail(self, image: QImage, thumbnail_path: str) -> None:
+        """Save the thumbnail file to the disk.
+
+        Args:
+            image: The QImage representing the thumbnail.
+            thumbnail_path: Path to which the thumbnail is stored.
+        Returns:
+            None.
+        """
+        # First create temporary file and then move it. This avoids
+        # problems with concurrent access of the thumbnail cache, since
+        # "move" is an atomic operation
+        handle, tmp_filename = tempfile.mkstemp(dir=self._manager.directory)
+        os.close(handle)
+        os.chmod(tmp_filename, 0o600)
+        image.save(tmp_filename, format="png")
+        os.replace(tmp_filename, thumbnail_path)
+
     def _create_thumbnail(self, path: str, thumbnail_path: str) -> QPixmap:
         """Create thumbnail for an image.
 
         Args:
             path: Path to the image for which the thumbnail is created.
             thumbnail_path: Path to which the thumbnail is stored.
         Returns:
@@ -149,22 +168,16 @@
         # Image was deleted in the time between reader.read() and now
         try:
             attributes = self._get_thumbnail_attributes(path, image)
         except FileNotFoundError:
             return self._manager.fail_pixmap
         for key, value in attributes.items():
             image.setText(key, value)
-        # First create temporary file and then move it. This avoids
-        # problems with concurrent access of the thumbnail cache, since
-        # "move" is an atomic operation
-        handle, tmp_filename = tempfile.mkstemp(dir=self._manager.directory)
-        os.close(handle)
-        os.chmod(tmp_filename, 0o600)
-        image.save(tmp_filename, format="png")
-        os.replace(tmp_filename, thumbnail_path)
+        if api.settings.thumbnail.save:
+            self._save_thumbnail(image, thumbnail_path)
         return QPixmap(image)
 
     def _get_thumbnail_attributes(self, path: str, image: QImage) -> Dict[str, str]:
         """Return a dictionary filled with thumbnail attributes.
 
         Args:
             path: Path to the original image to get attributes from.
```

### Comparing `vimiv-0.8.0/vimiv/utils/trash_manager.py` & `vimiv-0.9.0/vimiv/utils/trash_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Provides functions and signals to handle a shared trash directory.
 
 The functions delete and undeletes images from the user's Trash directory
 in $XDG_DATA_HOME/Trash according to the freedesktop.org trash specification.
 
@@ -59,15 +59,17 @@
     Args:
         basename: Basename of the file in the trash directory.
     Returns:
         The path to the restored file.
     """
     trash_filename = os.path.join(_files_directory, basename)
     info_filename = _get_info_filename(basename)
-    if not os.path.exists(info_filename) or not os.path.exists(trash_filename):
+    if not os.path.exists(info_filename) or (
+        not os.path.exists(trash_filename) and not os.path.islink(trash_filename)
+    ):
         raise FileNotFoundError(f"File for '{basename}' does not exist")
     original_filename, _ = trash_info(basename)
     if not os.path.isdir(os.path.dirname(original_filename)):
         raise FileNotFoundError(f"Original directory of '{basename}' is not accessible")
     shutil.move(trash_filename, original_filename)
     os.remove(info_filename)
     return original_filename
@@ -134,24 +136,26 @@
         trash_filename: The name of the file in self.files_directory.
         original_filename: The original name of the file.
     """
     from urllib.parse import quote
 
     # Write to temporary file and use shutil.move to make sure the
     # operation is an atomic operation as specified by the standard
-    temp_file = tempfile.NamedTemporaryFile(dir=_info_directory, delete=False, mode="w")
-    info = TrashInfoParser()
-    info["Trash Info"] = {
-        "Path": quote(original_filename),
-        "DeletionDate": time.strftime("%Y-%m-%dT%H:%M:%S"),
-    }
-    info.write(temp_file, space_around_delimiters=False)
-    # Move to proper filename
-    info_filename = _get_info_filename(trash_filename)
-    shutil.move(temp_file.name, info_filename)
+    with tempfile.NamedTemporaryFile(
+        dir=_info_directory, delete=False, mode="w"
+    ) as temp_file:
+        info = TrashInfoParser()
+        info["Trash Info"] = {
+            "Path": quote(original_filename),
+            "DeletionDate": time.strftime("%Y-%m-%dT%H:%M:%S"),
+        }
+        info.write(temp_file, space_around_delimiters=False)
+        # Move to proper filename
+        info_filename = _get_info_filename(trash_filename)
+        shutil.move(temp_file.name, info_filename)
 
 
 class TrashInfoParser(configparser.ConfigParser):
     """Case-sensitive configparser without interpolation."""
 
     def __init__(self) -> None:
         super().__init__(interpolation=None)
```

### Comparing `vimiv-0.8.0/vimiv/utils/trie.py` & `vimiv-0.9.0/vimiv/utils/trie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Implementation of a trie datastructure.
 
 See e.g. https://en.wikipedia.org/wiki/Trie for more details.
 """
 
@@ -122,16 +122,16 @@
     def check(self) -> None:
         """Checks for possible clashes and logs warnings."""
         if self.key and self.children:
             hidden: List[str] = []
             for child in self.children.values():
                 hidden.extend(key for key, _ in child)
             _logger.warning("%s hides longer keys: %s", self.key, quotedjoin(hidden))
-        for elem in self.children:
-            self.children[elem].check()
+        for child in self.children.values():
+            child.check()
 
 
 class TrieMatch(NamedTuple):
     """Helper class as result for Trie.match, see Trie.match for details."""
 
     value: Optional[str] = None
     partial: Optional[IterResultT] = None
```

### Comparing `vimiv-0.8.0/vimiv/utils/xdg.py` & `vimiv-0.9.0/vimiv/utils/xdg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions to help with XDG_USER_* settings."""
 
 import os
 
 from PyQt5.QtCore import QStandardPaths
```

### Comparing `vimiv-0.8.0/vimiv/version.py` & `vimiv-0.9.0/vimiv/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
 """Functions to retrieve various version information.
 
 Module Attributes:
     _license_str: GPL boilerplate including the licensing information.
 """
@@ -14,15 +14,14 @@
 import os
 import sys
 from typing import Optional
 
 from PyQt5.QtCore import QT_VERSION_STR, PYQT_VERSION_STR
 
 import vimiv
-from vimiv.imutils import exif
 from vimiv.utils import xdg, run_qprocess, lazy
 
 QtSvg = lazy.import_module("PyQt5.QtSvg", optional=True)
 
 
 def info() -> str:
     """Retrieve version information.
@@ -38,16 +37,14 @@
     )
     return (
         f"{vimiv_version}\n\n"
         f"Python: {_python_version()}\n"
         f"Qt: {QT_VERSION_STR}\n"
         f"PyQt: {PYQT_VERSION_STR}\n\n"
         f"Svg Support: {bool(QtSvg)}\n"
-        f"Pyexiv2: {exif.pyexiv2.__version__ if exif.pyexiv2 is not None else None}\n"
-        f"Piexif: {exif.piexif.VERSION if exif.piexif is not None else None}"
     )
 
 
 def paths() -> str:
     """Retrieve information on relevant paths."""
     return (
         "Paths:\n"
```

### Comparing `vimiv-0.8.0/vimiv/widgets.py` & `vimiv-0.9.0/vimiv/plugins/metadata_pyexiv2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,162 +1,133 @@
 # vim: ft=python fileencoding=utf-8 sw=4 et sts=4
 
 # This file is part of vimiv.
-# Copyright 2017-2021 Christian Karl (karlch) <karlch at protonmail dot com>
+# Copyright 2017-2023 Christian Karl (karlch) <karlch at protonmail dot com>
 # License: GNU GPL v3, see the "LICENSE" and "AUTHORS" files for details.
 
-"""Miscellaneous QtWidgets."""
+"""Metadata plugin based on pyexiv2 (https://pypi.org/project/py3exiv2/) backend.
 
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QPainter, QFontMetrics
-from PyQt5.QtWidgets import QTreeView, QAbstractItemView, QSlider, QDialog
-
-from vimiv.config import styles
-from vimiv.utils import cached_method
-
-
-class ScrollToCenterMixin:
-    """Mixin class to ensure the selected index stays at the center when scrolling."""
-
-    def scrollTo(self, index, _hint=None):
-        super().scrollTo(index, self.PositionAtCenter)
-
-
-class FlatTreeView(ScrollToCenterMixin, QTreeView):
-    """QTreeView without expandable items."""
-
-    def __init__(self, parent=None):
-        super().__init__(parent=parent)
-
-        self.setSelectionBehavior(QAbstractItemView.SelectRows)
-        self.setSelectionMode(QAbstractItemView.SingleSelection)
-
-        self.setUniformRowHeights(True)
-        self.setIndentation(0)
-        self.setHeaderHidden(True)
-        self.setAlternatingRowColors(True)
-        self.setItemsExpandable(False)
-        self.setExpandsOnDoubleClick(False)
-        self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
-
-    def _select_row(self, row):
-        """Select a specific row in the library.
-
-        Args:
-            row: Number of the row to select.
-        """
-        index = self.model().index(row, 0)
-        self._select_index(index)
-
-    def _select_index(self, index):
-        """Select a specific index in the library.
-
-        Args:
-            index: QModelIndex to select.
-        """
-        self.setCurrentIndex(index)
-
-    def row(self):
-        """Return the currently selected row."""
-        return self.currentIndex().row()
-
-
-class SliderWithValue(QSlider):
-    """QSlider displaying the current value at the center.
-
-    Attributes:
-        _padding: Vertical padding in pixels between text and slider bar.
-        _handle_margin: Vertical size the handle goes over the slider bar in pixels.
-        _handle_width: Width of the handle in pixels.
-    """
-
-    STYLESHEET = ""  # Dummy that gets extended by custom dynamic styling
-
-    PADDING = 2
-    HANDLE_MARGIN = 5
-
-    def __init__(self, left_color, handle_color, right_color, *args, parent=None):
-        super().__init__(*args, parent=parent)
-        self._left_color = left_color
-        self._handle_color = handle_color
-        self._right_color = right_color
-
-    def paintEvent(self, event):
-        """Override paint event to additionally paint the current value."""
-        super().paintEvent(event)
-        self._init_style()
-
-        text = str(self.value())
-        rect = self.geometry()
-        painter = QPainter(self)
-        font_metrics = QFontMetrics(self.font())
-
-        x = (rect.width() - font_metrics.width(text)) // 2
-        y = rect.height() - (rect.height() - font_metrics.capHeight()) // 2
-        painter.drawText(x, y, text)
-
-    @cached_method
-    def _init_style(self):
-        """Initialize the stylesheet.
-
-        This is called on the first paintEvent to ensure all sizes and fonts are
-        correct.
-        """
-        font_height = QFontMetrics(self.font()).capHeight()
-        groove_height = font_height + 2 * self.PADDING
-        total_height = groove_height + 2 * self.HANDLE_MARGIN
-        sheet = f"""
-        QSlider {{
-            height: {total_height:d}px;
-        }}
-
-        QSlider::sub-page {{
-            background-color: {self._left_color};
-        }}
-
-        QSlider::handle {{
-            width: 24px;
-            background-color: {self._handle_color};
-            margin: -{SliderWithValue.HANDLE_MARGIN}px 0px;
-        }}
-
-        QSlider::groove {{
-            background-color: {self._right_color};
-            height: {groove_height}px;
-        }}
-        """
-        styles.apply(self, append=sheet)
-
-
-class PopUp(QDialog):
-    """Base class for pop-up windows to ensure consistent styling and behaviour."""
-
-    STYLESHEET = """
-    QDialog {
-        background: {image.bg};
-    }
-    QLabel {
-        color: {statusbar.fg};
-        font: {library.font}
-    }
-    QPushButton {
-        font: {statusbar.font};
-        background-color: {statusbar.bg};
-        border: 0px;
-        padding: 4px;
-        color: {statusbar.fg};
-    }
-    QPushButton:pressed {
-        background-color: {library.selected.bg};
-    }
-    """
-
-    def __init__(self, title: str, parent=None):
-        super().__init__(parent=parent)
-        self.setWindowTitle(title)
-        self.setWindowFlags(self.windowFlags() | Qt.Tool)  # type: ignore
-        styles.apply(self)
-
-    def reject(self):
-        """Override reject to additionally delete the QObject."""
-        super().reject()
-        self.deleteLater()
+Properties:
+- Shared libraries as dependencies.
+- Formatted Metadata.
+- Reads Exif, IPTC and XMP.
+"""
+
+import contextlib
+import itertools
+from typing import Any, Sequence, Iterable
+
+from vimiv.imutils import metadata
+from vimiv.utils import log, is_hex, lazy
+
+pyexiv2 = lazy.import_module("pyexiv2", optional=True)
+
+_logger = log.module_logger(__name__)
+
+
+class MetadataPyexiv2(metadata.MetadataPlugin):
+    """Provides metadata support based on pyexiv2."""
+
+    def __init__(self, path: str) -> None:
+        self._path = path
+
+        try:
+            self._metadata = pyexiv2.ImageMetadata(path)
+            self._metadata.read()
+        except FileNotFoundError:
+            _logger.debug("File %s not found", path)
+            self._metadata = None
+
+    @staticmethod
+    def name() -> str:
+        """Get the name of the used backend."""
+        return "pyexiv2"
+
+    @staticmethod
+    def version() -> str:
+        """Get the version of the used backend."""
+        return pyexiv2.__version__
+
+    def get_metadata(self, desired_keys: Sequence[str]) -> metadata.MetadataDictT:
+        """Get value of all desired keys for the current image."""
+
+        out = {}
+
+        if self._metadata is None:
+            return {}
+
+        for key in desired_keys:
+            try:
+                key_name = self._metadata[key].name
+
+                try:
+                    key_value = self._metadata[key].human_value
+
+                # Not all metadata (i.e. IPTC) provide human_value, take raw_value
+                except AttributeError:
+                    value = self._metadata[key].raw_value
+
+                    # For IPTC the raw_value is a list of strings
+                    if isinstance(value, list):
+                        key_value = ", ".join(value)
+                    else:
+                        key_value = value
+
+                out[key] = (key_name, key_value)
+
+            except KeyError:
+                _logger.debug("Key %s is invalid for the current image", key)
+
+        return out
+
+    def get_keys(self) -> Iterable[str]:
+        """Get the keys for all metadata values available for the current image."""
+        if self._metadata is None:
+            return iter([])
+
+        return (key for key in self._metadata if not is_hex(key.rpartition(".")[2]))
+
+    def copy_metadata(self, dest: str, reset_orientation: bool = True) -> bool:
+        """Copy metadata from the current image to dest image."""
+        if self._metadata is None:
+            return False
+
+        if reset_orientation:
+            with contextlib.suppress(KeyError):
+                self._metadata[
+                    "Exif.Image.Orientation"
+                ] = metadata.ExifOrientation.Normal
+
+        try:
+            dest_image = pyexiv2.ImageMetadata(dest)
+            dest_image.read()
+
+            # File types restrict the metadata type they can store.
+            # Try copying all types one by one and skip if it fails.
+            for copy_args in set(itertools.permutations((True, False, False, False))):
+                with contextlib.suppress(ValueError):
+                    self._metadata.copy(dest_image, *copy_args)
+
+            dest_image.write()
+            return True
+        except FileNotFoundError:
+            _logger.debug("Failed to write metadata. Destination '%s' not found", dest)
+        except OSError as e:
+            _logger.debug("Failed to write metadata for '%s': '%s'", dest, str(e))
+        return False
+
+    def get_date_time(self) -> str:
+        """Get creation date and time of the current image as formatted string."""
+        if self._metadata is None:
+            return ""
+
+        with contextlib.suppress(KeyError):
+            return self._metadata["Exif.Image.DateTime"].raw_value
+        return ""
+
+
+def init(*_args: Any, **_kwargs: Any) -> None:
+    """Initialize pyexiv2 handler if pyexiv2 is available."""
+    if pyexiv2 is not None:
+        metadata.register(MetadataPyexiv2)
+    else:
+        _logger.warning("Please install py3exiv2 to use this plugin")
```

### Comparing `vimiv-0.8.0/vimiv.egg-info/PKG-INFO` & `vimiv-0.9.0/vimiv.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 Metadata-Version: 2.1
 Name: vimiv
-Version: 0.8.0
+Version: 0.9.0
 Summary: An image viewer with vim-like keybindings.
 Home-page: https://karlch.github.io/vimiv-qt/
 Author: Christian Karl
 Author-email: karlch@protonmail.com
 License: GPL3
 Project-URL: Source Code, https://github.com/karlch/vimiv-qt
 Project-URL: Bug Tracker, https://github.com/karlch/vimiv-qt/issues
 Project-URL: Documentation, https://karlch.github.io/vimiv-qt/documentation
-Description: <img src="https://karlch.github.io/vimiv-qt/_images/vimiv_banner_800.png" alt="vimiv banner" width="400"/>
-        
-        [![Build Status](https://github.com/karlch/vimiv-qt/workflows/CI/badge.svg)](https://github.com/karlch/vimiv-qt/actions)
-        [![Codecov](https://codecov.io/github/karlch/vimiv-qt/coverage.svg?branch=master)](https://codecov.io/github/karlch/vimiv-qt?branch=master)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        
-        [website](https://karlch.github.io/vimiv-qt/) |
-        [docs](https://karlch.github.io/vimiv-qt/documentation/index.html) |
-        [install](https://karlch.github.io/vimiv-qt/documentation/install.html) |
-        [screenshots](https://karlch.github.io/vimiv-qt/screenshots.html) |
-        [changelog](https://karlch.github.io/vimiv-qt/changelog.html) |
-        [contributing](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
-        
-        <img src="https://i.postimg.cc/VkcPgcbR/vimiv.gif" alt="vimiv screencast" width="440"/>
-        
-        ---
-        > :information_source: This Qt port is the future of vimiv. New features will
-        > only be implemented here and there are already many improvements compared to the
-        > [deprecated gtk version](https://github.com/karlch/vimiv). The old version is only
-        > recommended if you require a more stable software. In case there is anything you miss
-        > here, please [open an issue](https://github.com/karlch/vimiv-qt/issues). Check the
-        > [roadmap](https://karlch.github.io/vimiv-qt/roadmap.html) for more details.
-        ---
-        
-        Vimiv is an image viewer with vim-like keybindings. It is written in python3
-        using the Qt5 toolkit and is free software, licensed under the GPL.
-        
-        ### Features
-        
-        * Basic image operations and navigation
-        * [ranger](https://github.com/ranger/ranger)-like library to browse your images
-        * Thumbnail mode: navigable grid of image previews
-        * Command mode with tab-completion
-        * Search with pattern matching
-        * Simple mark and tag system
-        * Customization of keybindings, settings and style via configuration files,
-          [base-16 support](https://github.com/karlch/base16-vimiv), ...
-        
-        ### Install
-        
-        To learn how to get vimiv running on various platforms, please check out the
-        [installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html).
-        
-        ### Documentation
-        
-        Much more details on vimiv are available on the
-        [website](https://karlch.github.io/vimiv-qt/). Here are some hints to get you started:
-        * [The installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html)
-           includes instructions on how to get vimiv running on various platforms.
-        * [Getting started](https://karlch.github.io/vimiv-qt/documentation/getting\_started.html)
-          starts with the basic concepts and keybindings to later show some more advanced
-          features.
-        * [Commands](https://karlch.github.io/vimiv-qt/documentation/commands.html)
-          gives a complete overview and description of all commands.
-        * [Keybindings](https://karlch.github.io/vimiv-qt/documentation/configuration/keybindings.html)
-          lists the default keybindings and describes how to configure them.
-        * [Settings](https://karlch.github.io/vimiv-qt/documentation/configuration/settings.html)
-          describes the available settings and how to change them.
-        * [Style](https://karlch.github.io/vimiv-qt/documentation/configuration/style.html)
-          explains how to configure the look and colorscheme of vimiv.
-        * [Plugins](https://karlch.github.io/vimiv-qt/documentation/configuration/plugins.html)
-          illustrates vimiv's python plugin system: a great way to extend the functionality
-          beyond the defaults and to start delving into the source code.
-        
-        ### Contributing
-        
-        You want to contribute to vimiv? Great! :tada:
-        
-        Every little help counts and is appreciated!  Feel free to read the
-        [contributing guidelines](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
-        for some useful tips and tricks.
-        
-        There are many ways to contribute, including:
-        * [giving feedback and requesting new features](https://karlch.github.io/vimiv-qt/documentation/contributing.html#feedback-and-feature-requests),
-        * [reporting bugs](https://karlch.github.io/vimiv-qt/documentation/contributing.html#reporting-bugs),
-        * [writing code](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-code)
-          and
-        * [extending the documentation](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-documentation).
-        * spreading the word in an article, blog, reddit post, ...
-        
-        Need help? Feel free to
-        [contact me directly](mailto:karlch@protonmail.com)
-        or, even better,
-        open an [issue on github](https://github.com/karlch/vimiv-qt/issues/).
-        
-        ### License
-        
-        This program is free software: you can redistribute it and/or modify it under
-        the terms of the GNU General Public License as published by the Free Software
-        Foundation, either version 3 of the License, or (at your option) any later
-        version.
-        
-        This program is distributed in the hope that it will be useful, but WITHOUT ANY
-        WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-        PARTICULAR PURPOSE. See the GNU General Public License for more details.
-        
-        You should have received a copy of the GNU General Public License along with
-        this program. If not, see <http://www.gnu.org/licenses/>.
-        
 Keywords: pyqt,image viewer,vim
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+<img src="https://karlch.github.io/vimiv-qt/_images/vimiv_banner_800.png" alt="vimiv banner" width="400"/>
+
+[![Build Status](https://github.com/karlch/vimiv-qt/workflows/CI/badge.svg)](https://github.com/karlch/vimiv-qt/actions)
+[![Codecov](https://codecov.io/github/karlch/vimiv-qt/coverage.svg?branch=master)](https://codecov.io/github/karlch/vimiv-qt?branch=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+[website](https://karlch.github.io/vimiv-qt/) |
+[docs](https://karlch.github.io/vimiv-qt/documentation/index.html) |
+[install](https://karlch.github.io/vimiv-qt/documentation/install.html) |
+[screenshots](https://karlch.github.io/vimiv-qt/screenshots.html) |
+[changelog](https://karlch.github.io/vimiv-qt/changelog.html) |
+[contributing](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
+
+<img src="https://i.postimg.cc/VkcPgcbR/vimiv.gif" alt="vimiv screencast" width="440"/>
+
+---
+> :information_source: This Qt port is the future of vimiv. New features will
+> only be implemented here and there are already many improvements compared to the
+> [deprecated gtk version](https://github.com/karlch/vimiv). The old version is only
+> recommended if you require a more stable software. In case there is anything you miss
+> here, please [open an issue](https://github.com/karlch/vimiv-qt/issues). Check the
+> [roadmap](https://karlch.github.io/vimiv-qt/roadmap.html) for more details.
+---
+
+Vimiv is an image viewer with vim-like keybindings. It is written in python3
+using the Qt5 toolkit and is free software, licensed under the GPL.
+
+### Features
+
+* Basic image operations and navigation
+* [ranger](https://github.com/ranger/ranger)-like library to browse your images
+* Thumbnail mode: navigable grid of image previews
+* Command mode with tab-completion
+* Search with pattern matching
+* Simple mark and tag system
+* Customization of keybindings, settings and style via configuration files,
+  [base-16 support](https://github.com/karlch/base16-vimiv), ...
+
+### Install
+
+To learn how to get vimiv running on various platforms, please check out the
+[installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html).
+
+### Documentation
+
+Much more details on vimiv are available on the
+[website](https://karlch.github.io/vimiv-qt/). Here are some hints to get you started:
+* [The installation guide](https://karlch.github.io/vimiv-qt/documentation/install.html)
+   includes instructions on how to get vimiv running on various platforms.
+* [Getting started](https://karlch.github.io/vimiv-qt/documentation/getting\_started.html)
+  starts with the basic concepts and keybindings to later show some more advanced
+  features.
+* [Commands](https://karlch.github.io/vimiv-qt/documentation/commands.html)
+  gives a complete overview and description of all commands.
+* [Keybindings](https://karlch.github.io/vimiv-qt/documentation/configuration/keybindings.html)
+  lists the default keybindings and describes how to configure them.
+* [Settings](https://karlch.github.io/vimiv-qt/documentation/configuration/settings.html)
+  describes the available settings and how to change them.
+* [Style](https://karlch.github.io/vimiv-qt/documentation/configuration/style.html)
+  explains how to configure the look and colorscheme of vimiv.
+* [Plugins](https://karlch.github.io/vimiv-qt/documentation/configuration/plugins.html)
+  illustrates vimiv's python plugin system: a great way to extend the functionality
+  beyond the defaults and to start delving into the source code.
+
+### Contributing
+
+You want to contribute to vimiv? Great! :tada:
+
+Every little help counts and is appreciated!  Feel free to read the
+[contributing guidelines](https://karlch.github.io/vimiv-qt/documentation/contributing.html)
+for some useful tips and tricks.
+
+There are many ways to contribute, including:
+* [giving feedback and requesting new features](https://karlch.github.io/vimiv-qt/documentation/contributing.html#feedback-and-feature-requests)
+* [reporting bugs](https://karlch.github.io/vimiv-qt/documentation/contributing.html#reporting-bugs)
+* [writing code](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-code)
+* [extending the documentation](https://karlch.github.io/vimiv-qt/documentation/contributing.html#writing-documentation)
+* spreading the word in an article, blog, reddit post, ...
+
+Need help? Feel free to
+[contact me directly](mailto:karlch@protonmail.com)
+or, even better,
+open an [issue on github](https://github.com/karlch/vimiv-qt/issues/).
+
+### License
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+This program is distributed in the hope that it will be useful, but WITHOUT ANY
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `vimiv-0.8.0/vimiv.egg-info/SOURCES.txt` & `vimiv-0.9.0/vimiv.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 misc/requirements/requirements_docs.txt
 misc/requirements/requirements_lint.txt
 misc/requirements/requirements_mypy.txt
 misc/requirements/requirements_packaging.txt
 misc/requirements/requirements_piexif.txt
 misc/requirements/requirements_pyexiv2.txt
 misc/requirements/requirements_tests.txt
+misc/requirements/requirements_tox.txt
 vimiv/__init__.py
 vimiv/__main__.py
 vimiv/app.py
 vimiv/checkversion.py
 vimiv/parser.py
 vimiv/startup.py
 vimiv/version.py
@@ -80,48 +81,54 @@
 vimiv/config/external_configparser.py
 vimiv/config/keyfile.py
 vimiv/config/styles.py
 vimiv/gui/__init__.py
 vimiv/gui/commandline.py
 vimiv/gui/commandwidget.py
 vimiv/gui/completionwidget.py
+vimiv/gui/crop_widget.py
 vimiv/gui/eventhandler.py
 vimiv/gui/image.py
 vimiv/gui/keybindings_popup.py
 vimiv/gui/keyhintwidget.py
 vimiv/gui/library.py
 vimiv/gui/mainwindow.py
 vimiv/gui/manipulate.py
 vimiv/gui/message.py
 vimiv/gui/metadatawidget.py
 vimiv/gui/prompt.py
+vimiv/gui/resize.py
 vimiv/gui/statusbar.py
 vimiv/gui/straightenwidget.py
 vimiv/gui/synchronize.py
 vimiv/gui/thumbnail.py
 vimiv/gui/transformwidget.py
 vimiv/gui/version_popup.py
 vimiv/imutils/__init__.py
 vimiv/imutils/_file_handler.py
 vimiv/imutils/current_pixmap.py
 vimiv/imutils/edit_handler.py
-vimiv/imutils/exif.py
 vimiv/imutils/filelist.py
 vimiv/imutils/immanipulate.py
 vimiv/imutils/imtransform.py
+vimiv/imutils/metadata.py
 vimiv/imutils/slideshow.py
 vimiv/plugins/__init__.py
 vimiv/plugins/demo.py
 vimiv/plugins/imageformats.py
+vimiv/plugins/metadata.py
+vimiv/plugins/metadata_piexif.py
+vimiv/plugins/metadata_pyexiv2.py
 vimiv/plugins/print.py
 vimiv/utils/__init__.py
 vimiv/utils/crash_handler.py
 vimiv/utils/customtypes.py
 vimiv/utils/debug.py
 vimiv/utils/files.py
+vimiv/utils/imageheader.py
 vimiv/utils/imagereader.py
 vimiv/utils/lazy.py
 vimiv/utils/log.py
 vimiv/utils/migration.py
 vimiv/utils/thumbnail_manager.py
 vimiv/utils/trash_manager.py
 vimiv/utils/trie.py
```

