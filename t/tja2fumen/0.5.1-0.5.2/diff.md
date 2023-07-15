# Comparing `tmp/tja2fumen-0.5.1.tar.gz` & `tmp/tja2fumen-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.5.1.tar", last modified: Tue Jul 11 12:16:47 2023, max compression
+gzip compressed data, was "tja2fumen-0.5.2.tar", last modified: Sat Jul 15 16:07:50 2023, max compression
```

## Comparing `tja2fumen-0.5.1.tar` & `tja2fumen-0.5.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/
--rw-rw-rw-   0        0        0     1083 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4388 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/README.md
--rw-rw-rw-   0        0        0      897 2023-07-11 12:16:33.000000 tja2fumen-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.407547 tja2fumen-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.423106 tja2fumen-0.5.1/src/tja2fumen/
--rw-rw-rw-   0        0        0     1732 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    18157 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    19863 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    20989 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-1.csv
--rw-rw-rw-   0        0        0    20505 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-2-3.csv
--rw-rw-rw-   0        0        0    21140 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-4-5.csv
--rw-rw-rw-   0        0        0    20349 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-1-2.csv
--rw-rw-rw-   0        0        0    20328 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-3.csv
--rw-rw-rw-   0        0        0    20390 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-4.csv
--rw-rw-rw-   0        0        0    20545 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-5-8.csv
--rw-rw-rw-   0        0        0    20516 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-1-2.csv
--rw-rw-rw-   0        0        0    20482 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-3.csv
--rw-rw-rw-   0        0        0    20393 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-4.csv
--rw-rw-rw-   0        0        0    21000 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-5-7.csv
--rw-rw-rw-   0        0        0    20458 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-1-7.csv
--rw-rw-rw-   0        0        0    20435 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-8.csv
--rw-rw-rw-   0        0        0    20464 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-9-10.csv
--rw-rw-rw-   0        0        0    20661 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-1.csv
--rw-rw-rw-   0        0        0    20385 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-2-3.csv
--rw-rw-rw-   0        0        0    20976 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-4-5.csv
--rw-rw-rw-   0        0        0    20222 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-1-2.csv
--rw-rw-rw-   0        0        0    20145 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-3.csv
--rw-rw-rw-   0        0        0    20136 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-4.csv
--rw-rw-rw-   0        0        0    20182 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-5-8.csv
--rw-rw-rw-   0        0        0    20294 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-1-2.csv
--rw-rw-rw-   0        0        0    20289 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-3.csv
--rw-rw-rw-   0        0        0    20245 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-4.csv
--rw-rw-rw-   0        0        0    20715 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-5-7.csv
--rw-rw-rw-   0        0        0    19707 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-1-7.csv
--rw-rw-rw-   0        0        0    19785 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-8.csv
--rw-rw-rw-   0        0        0    19777 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-9-10.csv
--rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-9-10.csv
--rw-rw-rw-   0        0        0     4363 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2910 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.423106 tja2fumen-0.5.1/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4388 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2559 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 16:07:50.542768 tja2fumen-0.5.2/
+-rw-rw-rw-   0        0        0     1083 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4484 2023-07-15 16:07:50.542768 tja2fumen-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2765 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-15 16:07:37.000000 tja2fumen-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:07:50.542768 tja2fumen-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:07:50.480224 tja2fumen-0.5.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 16:07:50.495848 tja2fumen-0.5.2/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1715 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     4031 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    18753 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    19840 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:07:50.527098 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/
+-rw-rw-rw-   0        0        0    20989 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-1.csv
+-rw-rw-rw-   0        0        0    20505 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-2-3.csv
+-rw-rw-rw-   0        0        0    21140 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-4-5.csv
+-rw-rw-rw-   0        0        0    20349 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-1-2.csv
+-rw-rw-rw-   0        0        0    20328 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-3.csv
+-rw-rw-rw-   0        0        0    20390 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-4.csv
+-rw-rw-rw-   0        0        0    20545 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-5-8.csv
+-rw-rw-rw-   0        0        0    20516 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-1-2.csv
+-rw-rw-rw-   0        0        0    20482 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-3.csv
+-rw-rw-rw-   0        0        0    20393 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-4.csv
+-rw-rw-rw-   0        0        0    21000 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-5-7.csv
+-rw-rw-rw-   0        0        0    20458 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-1-7.csv
+-rw-rw-rw-   0        0        0    20435 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-8.csv
+-rw-rw-rw-   0        0        0    20464 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-9-10.csv
+-rw-rw-rw-   0        0        0    20661 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-1.csv
+-rw-rw-rw-   0        0        0    20385 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-2-3.csv
+-rw-rw-rw-   0        0        0    20976 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-4-5.csv
+-rw-rw-rw-   0        0        0    20222 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-1-2.csv
+-rw-rw-rw-   0        0        0    20145 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-3.csv
+-rw-rw-rw-   0        0        0    20136 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-4.csv
+-rw-rw-rw-   0        0        0    20182 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-5-8.csv
+-rw-rw-rw-   0        0        0    20294 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-1-2.csv
+-rw-rw-rw-   0        0        0    20289 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-3.csv
+-rw-rw-rw-   0        0        0    20245 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-4.csv
+-rw-rw-rw-   0        0        0    20715 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-5-7.csv
+-rw-rw-rw-   0        0        0    19707 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-1-7.csv
+-rw-rw-rw-   0        0        0    19785 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-8.csv
+-rw-rw-rw-   0        0        0    19777 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-9-10.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-1.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-2-3.csv
+-rw-rw-rw-   0        0        0    23890 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-4-5.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-1-2.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-3.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-4.csv
+-rw-rw-rw-   0        0        0    23883 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-5-8.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-1-2.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-3.csv
+-rw-rw-rw-   0        0        0    23887 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-4.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-5-7.csv
+-rw-rw-rw-   0        0        0    23880 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-1-7.csv
+-rw-rw-rw-   0        0        0    23872 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-8.csv
+-rw-rw-rw-   0        0        0    23869 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-9-10.csv
+-rw-rw-rw-   0        0        0     4950 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/types.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2829 2023-07-15 16:06:49.000000 tja2fumen-0.5.2/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:07:50.495848 tja2fumen-0.5.2/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4484 2023-07-15 16:07:50.000000 tja2fumen-0.5.2/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-07-15 16:07:50.000000 tja2fumen-0.5.2/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 16:07:50.000000 tja2fumen-0.5.2/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-15 16:07:50.000000 tja2fumen-0.5.2/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-15 16:07:50.000000 tja2fumen-0.5.2/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 16:07:50.000000 tja2fumen-0.5.2/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.5.1/LICENSE.txt` & `tja2fumen-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/PKG-INFO` & `tja2fumen-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.5.1
+Version: 0.5.2
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -38,14 +38,15 @@
 
 This project attempts to replace/complement the existing closed-source [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter packaged alongside TakoTako. 
 
 ## Goals
 
 - Act as a drop-in replacement for `tja2bin.exe` in TakoTako.
 - Fix https://github.com/Fluto/TakoTako/issues/16. (The original `tjabin.exe` doesn't properly handle `#BPMCHANGE` commands.)
+- Better handle commands that `tjabin.exe` fails for (`#SECTION`, `#NEXTSONG`, `#LYRIC`, etc.)
 - Provide open source code to act as a reference for parsing and writing both the TJA and Fumen file formats.
 - Stick to the Python stdlib, i.e. no external dependencies if possible.
 
 ## Usage
 
 ### Option 1: Standalone Python installation
```

### Comparing `tja2fumen-0.5.1/README.md` & `tja2fumen-0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 This project attempts to replace/complement the existing closed-source [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter packaged alongside TakoTako. 
 
 ## Goals
 
 - Act as a drop-in replacement for `tja2bin.exe` in TakoTako.
 - Fix https://github.com/Fluto/TakoTako/issues/16. (The original `tjabin.exe` doesn't properly handle `#BPMCHANGE` commands.)
+- Better handle commands that `tjabin.exe` fails for (`#SECTION`, `#NEXTSONG`, `#LYRIC`, etc.)
 - Provide open source code to act as a reference for parsing and writing both the TJA and Fumen file formats.
 - Stick to the Python stdlib, i.e. no external dependencies if possible.
 
 ## Usage
 
 ### Option 1: Standalone Python installation
```

### Comparing `tja2fumen-0.5.1/pyproject.toml` & `tja2fumen-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.5.1"
+version = "0.5.2"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.5.1/src/tja2fumen/__init__.py` & `tja2fumen-0.5.2/src/tja2fumen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         help="Path to a Taiko no Tatsujin TJA file.",
     )
     args = parser.parse_args(argv)
     fnameTJA = getattr(args, "file.tja")
     baseName = os.path.splitext(fnameTJA)[0]
 
     # Parse lines in TJA file
-    parsedTJACourses = parseTJA(fnameTJA)
+    parsedTJA = parseTJA(fnameTJA)
 
     # Convert parsed TJA courses to Fumen data, and write each course to `.bin` files
-    for parsedCourse in parsedTJACourses.items():
-        convert_and_write(parsedCourse, baseName, singleCourse=(len(parsedTJACourses) == 1))
+    for course in parsedTJA.courses.items():
+        convert_and_write(course, baseName, singleCourse=(len(parsedTJA.courses) == 1))
 
 
 def convert_and_write(parsedCourse, baseName, singleCourse=False):
     courseName, tjaData = parsedCourse
     fumenData = convertTJAToFumen(tjaData)
     # Add course ID (e.g. '_x', '_x_1', '_x_2') to the output file's base name
     outputName = baseName
```

### Comparing `tja2fumen-0.5.1/src/tja2fumen/constants.py` & `tja2fumen-0.5.2/src/tja2fumen/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,14 +88,19 @@
 sampleHeaderMetadata[68] = 30
 sampleHeaderMetadata[72] = 20
 sampleHeaderMetadata[76] = 78
 sampleHeaderMetadata[77] = 97
 sampleHeaderMetadata[78] = 188
 # Certain other bytes (8+9, 20) will need to be filled in on a song-by-song basis
 
+TJA_COURSE_NAMES = []
+for difficulty in ['Ura', 'Oni', 'Hard', 'Normal', 'Easy']:
+    for player in ['', 'P1', 'P2']:
+        TJA_COURSE_NAMES.append(difficulty+player)
+
 NORMALIZE_COURSE = {
     '0': 'Easy',
     'Easy': 'Easy',
     '1': 'Normal',
     'Normal': 'Normal',
     '2': 'Hard',
     'Hard': 'Hard',
```

### Comparing `tja2fumen-0.5.1/src/tja2fumen/converters.py` & `tja2fumen-0.5.2/src/tja2fumen/converters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,12 @@
-from copy import deepcopy
 import re
 
 from tja2fumen.utils import computeSoulGaugeBytes
-from tja2fumen.constants import DIFFICULTY_BYTES, sampleHeaderMetadata, simpleHeaders
-
-# Filler metadata that the `writeFumen` function expects
-# TODO: Determine how to properly set the item byte (https://github.com/vivaria/tja2fumen/issues/17)
-default_note = {'type': '', 'pos': 0.0, 'item': 0, 'padding': 0.0,
-                'scoreInit': 0, 'scoreDiff': 0, 'duration': 0.0}
-default_branch = {'length': 0, 'padding': 0, 'speed': 1.0}
-default_measure = {
-    'bpm': 0.0,
-    'fumenOffsetStart': 0.0,
-    'fumenOffsetEnd': 0.0,
-    'duration': 0.0,
-    'gogo': False,
-    'barline': True,
-    'padding1': 0,
-    'branchStart': None,
-    'branchInfo': [-1, -1, -1, -1, -1, -1],
-    'padding2': 0,
-    'normal': deepcopy(default_branch),
-    'advanced': deepcopy(default_branch),
-    'master': deepcopy(default_branch)
-}
+from tja2fumen.constants import DIFFICULTY_BYTES
+from tja2fumen.types import TJAMeasureProcessed, FumenCourse, FumenNote
 
 
 def processTJACommands(tja):
     """
     Merge TJA 'data' and 'event' fields into a single measure property, and split
     measures into sub-measures whenever a mid-measure BPM/SCROLL/GOGO change occurs.
 
@@ -40,269 +19,298 @@
 
     A particular danger is BPM changes. TJA allows multiple BPMs within a single measure,
     but the fumen format permits one BPM per measure. So, a TJA measure must be split up
     if it has multiple BPM changes within a measure.
 
     In the future, this logic should probably be moved into the TJA parser itself.
     """
-    branches = tja['branches']
-    branchesCorrected = {branchName: [] for branchName in branches.keys()}
-    for branchName, branch in branches.items():
-        currentBPM = float(tja['metadata']['bpm'])
+    tjaBranchesProcessed = {branchName: [] for branchName in tja.branches.keys()}
+    for branchName, branchMeasuresTJA in tja.branches.items():
+        currentBPM = tja.BPM
         currentScroll = 1.0
         currentGogo = False
         currentBarline = True
         currentDividend = 4
         currentDivisor = 4
-        for measure in branch:
+        for measureTJA in branchMeasuresTJA:
             # Split measure into submeasure
-            measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo, 'barline': currentBarline,
-                           'subdivisions': len(measure['data']), 'pos_start': 0, 'pos_end': 0, 'delay': 0,
-                           'branchStart': None, 'time_sig': [currentDividend, currentDivisor], 'data': []}
-            for data in measure['combined']:
+            measureTJAProcessed = TJAMeasureProcessed(
+                bpm=currentBPM,
+                scroll=currentScroll, 
+                gogo=currentGogo, 
+                barline=currentBarline, 
+                time_sig=[currentDividend, currentDivisor], 
+                subdivisions=len(measureTJA.notes),
+            )
+            for data in measureTJA.combined:
                 # Handle note data
-                if data['type'] == 'note':
-                    measure_cur['data'].append(data)
+                if data.name == 'note':
+                    measureTJAProcessed.data.append(data)
 
                 # Handle commands that can only be placed between measures (i.e. no mid-measure variations)
-                elif data['type'] == 'delay':
-                    measure_cur['delay'] = data['value'] * 1000  # ms -> s
-                elif data['type'] == 'branchStart':
-                    measure_cur['branchStart'] = data['value']
-                elif data['type'] == 'barline':
-                    currentBarline = bool(int(data['value']))
-                    measure_cur['barline'] = currentBarline
-                elif data['type'] == 'measure':
-                    matchMeasure = re.match(r"(\d+)/(\d+)", data['value'])
+                elif data.name == 'delay':
+                    measureTJAProcessed.delay = data.value * 1000  # ms -> s
+                elif data.name == 'branchStart':
+                    measureTJAProcessed.branchStart = data.value
+                    # If the measure immediately preceding a #BRANCHSTART has a #SECTION command, then remove it.
+                    # From TJA spec: "Placing [a #SECTION command] near #BRANCHSTART or a measure before does not reset
+                    #                 the accuracy for that branch. The value is calculated before it and a measure
+                    #                 has not started yet at that point."
+                    if tjaBranchesProcessed[branchName][-1].branchStart == ["#SECTION", -1, -1]:
+                        tjaBranchesProcessed[branchName][-1].branchStart = None
+                elif data.name == 'barline':
+                    currentBarline = bool(int(data.value))
+                    measureTJAProcessed.barline = currentBarline
+                elif data.name == 'measure':
+                    matchMeasure = re.match(r"(\d+)/(\d+)", data.value)
                     if not matchMeasure:
                         continue
                     currentDividend = int(matchMeasure.group(1))
                     currentDivisor = int(matchMeasure.group(2))
-                    measure_cur['time_sig'] = [currentDividend, currentDivisor]
+                    measureTJAProcessed.time_sig = [currentDividend, currentDivisor]
 
                 # Handle commands that can be placed in the middle of a measure.
                 #    NB: For fumen files, if there is a mid-measure change to BPM/SCROLL/GOGO, then the measure will
                 #    actually be split into two small submeasures. So, we need to start a new measure in those cases.
-                elif data['type'] in ['bpm', 'scroll', 'gogo']:
+                elif data.name in ['bpm', 'scroll', 'gogo']:
                     # Parse the values
-                    if data['type'] == 'bpm':
-                        new_val = currentBPM = float(data['value'])
-                    elif data['type'] == 'scroll':
-                        new_val = currentScroll = data['value']
-                    elif data['type'] == 'gogo':
-                        new_val = currentGogo = bool(int(data['value']))
+                    if data.name == 'bpm':
+                        new_val = currentBPM = float(data.value)
+                    elif data.name == 'scroll':
+                        new_val = currentScroll = data.value
+                    elif data.name == 'gogo':
+                        new_val = currentGogo = bool(int(data.value))
                     # Check for mid-measure commands
                     # - Case 1: Command happens at the start of a measure; just change the value directly
-                    if data['pos'] == 0:
-                        measure_cur[data['type']] = new_val
+                    if data.pos == 0:
+                        measureTJAProcessed.__setattr__(data.name, new_val)
                     # - Case 2: Command occurs mid-measure, so start a new sub-measure
                     else:
-                        measure_cur['pos_end'] = data['pos']
-                        branchesCorrected[branchName].append(measure_cur)
-                        measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo,
-                                       'barline': currentBarline, 'subdivisions': len(measure['data']),
-                                       'pos_start': data['pos'], 'pos_end': 0, 'delay': 0,
-                                       'branchStart': None, 'time_sig': [currentDividend, currentDivisor], 'data': []}
+                        measureTJAProcessed.pos_end = data.pos
+                        tjaBranchesProcessed[branchName].append(measureTJAProcessed)
+                        measureTJAProcessed = TJAMeasureProcessed(
+                            bpm=currentBPM,
+                            scroll=currentScroll,
+                            gogo=currentGogo,
+                            barline=currentBarline,
+                            time_sig=[currentDividend, currentDivisor],
+                            subdivisions=len(measureTJA.notes),
+                            pos_start=data.pos
+                        )
 
                 else:
-                    print(f"Unexpected event type: {data['type']}")
+                    print(f"Unexpected event type: {data.name}")
 
-            measure_cur['pos_end'] = len(measure['data'])
-            branchesCorrected[branchName].append(measure_cur)
+            measureTJAProcessed.pos_end = len(measureTJA.notes)
+            tjaBranchesProcessed[branchName].append(measureTJAProcessed)
 
-    hasBranches = all(len(b) for b in branchesCorrected.values())
+    hasBranches = all(len(b) for b in tjaBranchesProcessed.values())
     if hasBranches:
-        branch_lens = [len(b) for b in branches.values()]
+        branch_lens = [len(b) for b in tja.branches.values()]
         if not branch_lens.count(branch_lens[0]) == len(branch_lens):
             raise ValueError("Branches do not have the same number of measures.")
         else:
-            branchCorrected_lens = [len(b) for b in branchesCorrected.values()]
+            branchCorrected_lens = [len(b) for b in tjaBranchesProcessed.values()]
             if not branchCorrected_lens.count(branchCorrected_lens[0]) == len(branchCorrected_lens):
                 raise ValueError("Branches do not have matching GOGO/SCROLL/BPM commands.")
 
-    return branchesCorrected
+    return tjaBranchesProcessed
 
 
 def convertTJAToFumen(tja):
     # Preprocess commands
-    tja['branches'] = processTJACommands(tja)
+    processedTJABranches = processTJACommands(tja)
 
     # Pre-allocate the measures for the converted TJA
-    tjaConverted = {'measures': [deepcopy(default_measure) for _ in range(len(tja['branches']['normal']))]}
+    fumen = FumenCourse(
+        measures=len(processedTJABranches['normal']),
+        hasBranches=all([len(b) for b in processedTJABranches.values()]),
+        scoreInit=tja.scoreInit,
+        scoreDiff=tja.scoreDiff,
+    )
 
     # Iterate through the different branches in the TJA
-    for currentBranch, branch in tja['branches'].items():
-        if not len(branch):
+    for currentBranch, branchMeasuresTJAProcessed in processedTJABranches.items():
+        if not len(branchMeasuresTJAProcessed):
             continue
         total_notes = 0
         total_notes_branch = 0
         note_counter_branch = 0
         currentDrumroll = None
-        courseBalloons = tja['metadata']['balloon'].copy()
+        courseBalloons = tja.balloon.copy()
 
         # Iterate through the measures within the branch
-        for idx_m, measureTJA in enumerate(branch):
+        for idx_m, measureTJAProcessed in enumerate(branchMeasuresTJAProcessed):
             # Fetch a pair of measures
-            measureFumenPrev = tjaConverted['measures'][idx_m-1] if idx_m != 0 else None
-            measureFumen = tjaConverted['measures'][idx_m]
+            measureFumenPrev = fumen.measures[idx_m-1] if idx_m != 0 else None
+            measureFumen = fumen.measures[idx_m]
 
             # Copy over basic measure properties from the TJA (that don't depend on notes or commands)
-            measureFumen[currentBranch]['speed'] = measureTJA['scroll']
-            measureFumen['gogo'] = measureTJA['gogo']
-            measureFumen['bpm'] = measureTJA['bpm']
+            measureFumen.branches[currentBranch].speed = measureTJAProcessed.scroll
+            measureFumen.gogo = measureTJAProcessed.gogo
+            measureFumen.bpm = measureTJAProcessed.bpm
 
             # Compute the duration of the measure
             # First, we compute the duration for a full 4/4 measure
-            measureDurationFullMeasure = 4 * 60_000 / measureTJA['bpm']
+            measureDurationFullMeasure = 4 * 60_000 / measureTJAProcessed.bpm
             # Next, we adjust this duration based on both:
             #   1. The *actual* measure size (e.g. #MEASURE 1/8, #MEASURE 5/4, etc.)
-            measureSize = measureTJA['time_sig'][0] / measureTJA['time_sig'][1]
+            measureSize = measureTJAProcessed.time_sig[0] / measureTJAProcessed.time_sig[1]
             #   2. Whether this is a "submeasure" (i.e. it contains mid-measure commands, which split up the measure)
             #      - If this is a submeasure, then `measureLength` will be less than the total number of subdivisions.
-            measureLength = measureTJA['pos_end'] - measureTJA['pos_start']
+            measureLength = measureTJAProcessed.pos_end - measureTJAProcessed.pos_start
             #      - In other words, `measureRatio` will be less than 1.0:
-            measureRatio = (1.0 if measureTJA['subdivisions'] == 0.0  # Avoid division by 0 for empty measures
-                            else (measureLength / measureTJA['subdivisions']))
+            measureRatio = (1.0 if measureTJAProcessed.subdivisions == 0.0  # Avoid division by 0 for empty measures
+                            else (measureLength / measureTJAProcessed.subdivisions))
             # Apply the 2 adjustments to the measure duration
-            measureFumen['duration'] = measureDuration = measureDurationFullMeasure * measureSize * measureRatio
+            measureFumen.duration = measureDuration = measureDurationFullMeasure * measureSize * measureRatio
 
             # Compute the millisecond offsets for the start and end of each measure
             #  - Start: When the notes first appear on screen (to the right)
             #  - End:   When the notes arrive at the judgment line, and the note gets hit.
             if idx_m == 0:
-                tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
-                measureFumen['fumenOffsetStart'] = tjaOffset - measureDurationFullMeasure
+                measureFumen.fumenOffsetStart = (tja.offset * 1000 * -1) - measureDurationFullMeasure
             else:
                 # First, start the measure using the end timing of the previous measure (plus any #DELAY commands)
-                measureFumen['fumenOffsetStart'] = measureFumenPrev['fumenOffsetEnd'] + measureTJA['delay']
+                measureFumen.fumenOffsetStart = measureFumenPrev.fumenOffsetEnd + measureTJAProcessed.delay
                 # Next, adjust the start timing to account for #BPMCHANGE commands (!!! Discovered by tana :3 !!!)
                 # To understand what's going on here, imagine the following simple example:
                 #   * You have a very slow-moving note (i.e. low BPM), like the big DON in Donkama 2000.
                 #   * All the other notes move fast (i.e. high BPM), moving past the big slow note.
                 #   * To get this overlapping to work, you need the big slow note to START EARLY, but also END LATE:
                 #      - An early start means you need to subtract a LOT of time from the starting fumenOffset.
                 #      - Thankfully, the low BPM of the slow note will create a HUGE `measureOffsetAdjustment`,
                 #        since we are dividing by the BPMs, and dividing by a small number will result in a big number.
-                measureOffsetAdjustment = (4 * 60_000 / measureTJA['bpm']) - (4 * 60_000 / measureFumenPrev['bpm'])
+                measureOffsetAdjustment = (4 * 60_000 / measureFumen.bpm) - (4 * 60_000 / measureFumenPrev.bpm)
                 #      - When we subtract this adjustment from the fumenOffsetStart, we get the "START EARLY" part:
-                measureFumen['fumenOffsetStart'] -= measureOffsetAdjustment
+                measureFumen.fumenOffsetStart -= measureOffsetAdjustment
                 #      - The low BPM of the slow note will also create a HUGE measure duration.
                 #      - When we add this long duration to the EARLY START, we end up with the "END LATE" part:
-            measureFumen['fumenOffsetEnd'] = measureFumen['fumenOffsetStart'] + measureFumen['duration']
+            measureFumen.fumenOffsetEnd = measureFumen.fumenOffsetStart + measureFumen.duration
 
             # Best guess at what 'barline' status means for each measure:
             # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
             # - 'False' means that the measure doesn't land on a barline, and thus barline should be hidden.
             #   For example:
             #     1. Measures where #BARLINEOFF has been set
             #     2. Sub-measures that don't fall on the barline
-            if measureTJA['barline'] is False or (measureRatio != 1.0 and measureTJA['pos_start'] != 0):
-                measureFumen['barline'] = False
+            if measureTJAProcessed.barline is False or (measureRatio != 1.0 and measureTJAProcessed.pos_start != 0):
+                measureFumen.barline = False
 
             # Check to see if the measure contains a branching condition
-            if measureTJA['branchStart']:
+            if measureTJAProcessed.branchStart:
                 # Determine which values to assign based on the type of branching condition
-                if measureTJA['branchStart'][0] == 'p':
-                    vals = [int(total_notes_branch * v * 20) if 0 <= v <= 1  # Ensure value is actually a percentage
-                            else int(v * 100)                                # If it's not, pass the value as-is
-                            for v in measureTJA['branchStart'][1:]]
-                elif measureTJA['branchStart'][0] == 'r':
-                    vals = measureTJA['branchStart'][1:]
+                if measureTJAProcessed.branchStart[0] == 'p':
+                    vals = []
+                    for percent in measureTJAProcessed.branchStart[1:]:
+                        # Ensure percentage is actually a percentage value
+                        if 0 <= percent <= 1:
+                            val = total_notes_branch * percent * 20
+                            # If the result is very close, then round to account for lack of precision in percentage
+                            if abs(val - round(val)) < 0.1:
+                                val = round(val)
+                            vals.append(int(val))
+                        # If it isn't a percentage value, then pass it back as-is
+                        else:
+                            vals.append(int(percent * 100))
+                # If it's a drumroll then use the branch condition values as-is
+                elif measureTJAProcessed.branchStart[0] == 'r':
+                    vals = measureTJAProcessed.branchStart[1:]
+                # If it's a #SECTION command, use the branch condition values as-is AND reset the accuracy
+                elif measureTJAProcessed.branchStart[0] == '#SECTION':
+                    vals = measureTJAProcessed.branchStart[1:]
+                    note_counter_branch = 0
                 # Determine which bytes to assign the values to
                 if currentBranch == 'normal':
                     idx_b1, idx_b2 = 0, 1
                 elif currentBranch == 'advanced':
                     idx_b1, idx_b2 = 2, 3
                 elif currentBranch == 'master':
                     idx_b1, idx_b2 = 4, 5
                 # Assign the values to their intended bytes
-                measureFumen['branchInfo'][idx_b1] = vals[0]
-                measureFumen['branchInfo'][idx_b2] = vals[1]
-                # Reset the note counter corresponding to this branch
+                measureFumen.branchInfo[idx_b1] = vals[0]
+                measureFumen.branchInfo[idx_b2] = vals[1]
+                # Reset the note counter corresponding to this branch (i.e. reset the accuracy)
                 total_notes_branch = 0
+
+            # NB: We update the branch condition note counter *after* we check the current measure's branch condition.
+            # This is because the TJA spec says:
+            #    "The requirement is calculated one measure before #BRANCHSTART, changing the branch visually when it
+            #     is calculated and changing the notes after #BRANCHSTART."
+            # So, by delaying the summation by one measure, we perform the calculation with notes "one measure before".
             total_notes_branch += note_counter_branch
 
-            # Create note dictionaries based on TJA measure data (containing 0's plus 1/2/3/4/etc. for notes)
+            # Create notes based on TJA measure data
             note_counter_branch = 0
             note_counter = 0
-            for idx_d, data in enumerate(measureTJA['data']):
-                if data['type'] == 'note':
+            for idx_d, data in enumerate(measureTJAProcessed.data):
+                if data.name == 'note':
+                    note = FumenNote()
                     # Note positions must be calculated using the base measure duration (that uses a single BPM value)
                     # (In other words, note positions do not take into account any mid-measure BPM change adjustments.)
-                    note_pos = measureDuration * (data['pos'] - measureTJA['pos_start']) / measureLength
+                    note.pos = measureDuration * (data.pos - measureTJAProcessed.pos_start) / measureLength
                     # Handle the note that represents the end of a drumroll/balloon
-                    if data['value'] == "EndDRB":
+                    if data.value == "EndDRB":
                         # If a drumroll spans a single measure, then add the difference between start/end position
-                        if 'multimeasure' not in currentDrumroll.keys():
-                            currentDrumroll['duration'] += (note_pos - currentDrumroll['pos'])
+                        if not currentDrumroll.multimeasure:
+                            currentDrumroll.duration += (note.pos - currentDrumroll.pos)
                         # Otherwise, if a drumroll spans multiple measures, then we want to add the duration between
                         # the start of the measure (i.e. pos=0.0) and the drumroll's end position.
                         else:
-                            currentDrumroll['duration'] += (note_pos - 0.0)
+                            currentDrumroll.duration += (note.pos - 0.0)
                         # 1182, 1385, 1588, 2469, 1568, 752, 1568
-                        currentDrumroll['duration'] = float(int(currentDrumroll['duration']))
+                        currentDrumroll.duration = float(int(currentDrumroll.duration))
                         currentDrumroll = None
                         continue
                     # The TJA spec technically allows you to place double-Kusudama notes:
                     #    "Use another 9 to specify when to lower the points for clearing."
                     # But this is unsupported in fumens, so just skip the second Kusudama note.
-                    if data['value'] == "Kusudama" and currentDrumroll:
+                    if data.value == "Kusudama" and currentDrumroll:
                         continue
                     # Handle the remaining non-EndDRB, non-double Kusudama notes
-                    note = deepcopy(default_note)
-                    note['pos'] = note_pos
-                    note['type'] = data['value']
-                    note['scoreInit'] = tja['metadata']['scoreInit']  # Probably not fully accurate
-                    note['scoreDiff'] = tja['metadata']['scoreDiff']  # Probably not fully accurate
+                    note.type = data.value
+                    note.scoreInit = tja.scoreInit
+                    note.scoreDiff = tja.scoreDiff
                     # Handle drumroll/balloon-specific metadata
-                    if note['type'] in ["Balloon", "Kusudama"]:
-                        note['hits'] = courseBalloons.pop(0)
-                        note['hitsPadding'] = 0
+                    if note.type in ["Balloon", "Kusudama"]:
+                        note.hits = courseBalloons.pop(0)
                         currentDrumroll = note
                         total_notes -= 1
-                    if note['type'] in ["Drumroll", "DRUMROLL"]:
-                        note['drumrollBytes'] = b'\x00\x00\x00\x00\x00\x00\x00\x00'
+                    if note.type in ["Drumroll", "DRUMROLL"]:
                         currentDrumroll = note
                         total_notes -= 1
                     # Count dons, kas, and balloons for the purpose of tracking branching accuracy
-                    if note['type'].lower() in ['don', 'ka']:
+                    if note.type.lower() in ['don', 'ka']:
                         note_counter_branch += 1
-                    elif note['type'].lower() in ['balloon', 'kusudama']:
+                    elif note.type.lower() in ['balloon', 'kusudama']:
                         note_counter_branch += 1.5
-                    measureFumen[currentBranch][note_counter] = note
+                    measureFumen.branches[currentBranch].notes.append(note)
                     note_counter += 1
 
             # If drumroll hasn't ended by the end of this measure, increase duration by measure timing
             if currentDrumroll:
-                if currentDrumroll['duration'] == 0.0:
-                    currentDrumroll['duration'] += (measureDuration - currentDrumroll['pos'])
-                    currentDrumroll['multimeasure'] = True
+                if currentDrumroll.duration == 0.0:
+                    currentDrumroll.duration += (measureDuration - currentDrumroll.pos)
+                    currentDrumroll.multimeasure = True
                 else:
-                    currentDrumroll['duration'] += measureDuration
+                    currentDrumroll.duration += measureDuration
 
-            measureFumen[currentBranch]['length'] = note_counter
+            measureFumen.branches[currentBranch].length = note_counter
             total_notes += note_counter
 
     # Take a stock header metadata sample and add song-specific metadata
-    headerMetadata = sampleHeaderMetadata.copy()
-    headerMetadata[8] = DIFFICULTY_BYTES[tja['metadata']['course']][0]
-    headerMetadata[9] = DIFFICULTY_BYTES[tja['metadata']['course']][1]
+    fumen.headerMetadata[8] = DIFFICULTY_BYTES[tja.course][0]
+    fumen.headerMetadata[9] = DIFFICULTY_BYTES[tja.course][1]
     soulGaugeBytes = computeSoulGaugeBytes(
         n_notes=total_notes,
-        difficulty=tja['metadata']['course'],
-        stars=tja['metadata']['level']
+        difficulty=tja.course,
+        stars=tja.level
     )
-    headerMetadata[12] = soulGaugeBytes[0]
-    headerMetadata[13] = soulGaugeBytes[1]
-    headerMetadata[16] = soulGaugeBytes[2]
-    headerMetadata[17] = soulGaugeBytes[3]
-    headerMetadata[20] = soulGaugeBytes[4]
-    headerMetadata[21] = soulGaugeBytes[5]
-    tjaConverted['headerMetadata'] = b"".join(i.to_bytes(1, 'little') for i in headerMetadata)
-    tjaConverted['headerPadding'] = simpleHeaders[0]  # Use a basic, known set of header bytes
-    tjaConverted['order'] = '<'
-    tjaConverted['unknownMetadata'] = 0
-    tjaConverted['branches'] = all([len(b) for b in tja['branches'].values()])
-    tjaConverted['scoreInit'] = tja['metadata']['scoreInit']
-    tjaConverted['scoreDiff'] = tja['metadata']['scoreDiff']
+    fumen.headerMetadata[12] = soulGaugeBytes[0]
+    fumen.headerMetadata[13] = soulGaugeBytes[1]
+    fumen.headerMetadata[16] = soulGaugeBytes[2]
+    fumen.headerMetadata[17] = soulGaugeBytes[3]
+    fumen.headerMetadata[20] = soulGaugeBytes[4]
+    fumen.headerMetadata[21] = soulGaugeBytes[5]
+    fumen.headerMetadata = b"".join(i.to_bytes(1, 'little') for i in fumen.headerMetadata)
 
-    return tjaConverted
+    return fumen
```

### Comparing `tja2fumen-0.5.1/src/tja2fumen/parsers.py` & `tja2fumen-0.5.2/src/tja2fumen/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 import os
 import re
 from copy import deepcopy
 
 from tja2fumen.utils import readStruct, getBool, shortHex
 from tja2fumen.constants import NORMALIZE_COURSE, TJA_NOTE_TYPES, branchNames, noteTypes
-
+from tja2fumen.types import TJASong, TJAMeasure, TJAData, FumenCourse, FumenMeasure, FumenBranch, FumenNote
 
 ########################################################################################################################
 # TJA-parsing functions ( Original source: https://github.com/WHMHammer/tja-tools/blob/master/src/js/parseTJA.js)
 ########################################################################################################################
 
 
 def parseTJA(fnameTJA):
     try:
         tja_text = open(fnameTJA, "r", encoding="utf-8-sig").read()
     except UnicodeDecodeError:
         tja_text = open(fnameTJA, "r", encoding="shift-jis").read()
 
     lines = [line for line in tja_text.splitlines() if line.strip() != '']
-    courses = getCourseData(lines)
-    for courseData in courses.values():
-        courseData['branches'] = parseCourseMeasures(courseData['data'])
+    parsedTJA = getCourseData(lines)
+    for course in parsedTJA.courses.values():
+        parseCourseMeasures(course)
 
-    return courses
+    return parsedTJA
 
 
 def getCourseData(lines):
-    courses = {}
+    parsedTJA = None
     currentCourse = ''
     currentCourseCached = ''
     songBPM = 0
     songOffset = 0
 
     for line in lines:
         # Case 1: Header metadata
         match_header = re.match(r"^([A-Z]+):(.*)", line)
         if match_header:
             nameUpper = match_header.group(1).upper()
             value = match_header.group(2).strip()
 
             # Global header fields
-            if nameUpper == 'BPM':
-                songBPM = value
-            elif nameUpper == 'OFFSET':
-                songOffset = value
+            if nameUpper in ['BPM', 'OFFSET']:
+                if nameUpper == 'BPM':
+                    songBPM = value
+                elif nameUpper == 'OFFSET':
+                    songOffset = value
+                if songBPM and songOffset:
+                    parsedTJA = TJASong(songBPM, songOffset)
 
             # Course-specific header fields
             elif nameUpper == 'COURSE':
                 currentCourse = NORMALIZE_COURSE[value]
                 currentCourseCached = currentCourse
-                if currentCourse not in courses.keys():
-                    courses[currentCourse] = {
-                        'metadata': {'course': currentCourse, 'bpm': songBPM, 'offset': songOffset, 'level': 0,
-                                     'balloon': [], 'scoreInit': 0, 'scoreDiff': 0},
-                        'data': [],
-                    }
+                if currentCourse not in parsedTJA.courses.keys():
+                    raise ValueError()
             elif nameUpper == 'LEVEL':
-                courses[currentCourse]['metadata']['level'] = int(value) if value else 0
+                parsedTJA.courses[currentCourse].level = int(value) if value else 0
+            # NB: If there are multiple SCOREINIT/SCOREDIFF values, use the last one (shinuti)
             elif nameUpper == 'SCOREINIT':
-                courses[currentCourse]['metadata']['scoreInit'] = int(value) if value else 0
+                parsedTJA.courses[currentCourse].scoreInit = int(value.split(",")[-1]) if value else 0
             elif nameUpper == 'SCOREDIFF':
-                courses[currentCourse]['metadata']['scoreDiff'] = int(value) if value else 0
+                parsedTJA.courses[currentCourse].scoreDiff = int(value.split(",")[-1]) if value else 0
             elif nameUpper == 'BALLOON':
                 if value:
                     balloons = [int(v) for v in value.split(",") if v]
-                    courses[currentCourse]['metadata']['balloon'] = balloons
+                    parsedTJA.courses[currentCourse].balloon = balloons
             elif nameUpper == 'STYLE':
                 # Reset the course name to remove "P1/P2" that may have been added by a previous STYLE:DOUBLE chart
                 if value == 'Single':
                     currentCourse = currentCourseCached
             else:
                 pass  # Ignore other header fields such as 'TITLE', 'SUBTITLE', 'WAVE', etc.
 
@@ -80,168 +80,170 @@
                 nameUpper = match_command.group(1).upper()
                 value = match_command.group(2).strip() if match_command.group(2) else ''
                 # For STYLE:Double, #START P1/P2 indicates the start of a new chart
                 # But, we want multiplayer charts to inherit the metadata from the course as a whole, so we deepcopy
                 if nameUpper == "START":
                     if value in ["P1", "P2"]:
                         currentCourse = currentCourseCached + value
-                        courses[currentCourse] = deepcopy(courses[currentCourseCached])
-                        courses[currentCourse]['data'] = list()  # Keep the metadata, but reset the note data
+                        parsedTJA.courses[currentCourse] = deepcopy(parsedTJA.courses[currentCourseCached])
+                        parsedTJA.courses[currentCourse].data = list()  # Keep the metadata, but reset the note data
                         value = ''  # Once we've made the new course, we can reset this to a normal #START command
                     elif value:
                         raise ValueError(f"Invalid value '{value}' for #START command.")
             elif match_notes:
                 nameUpper = 'NOTES'
                 value = match_notes.group(1)
-            courses[currentCourse]['data'].append({"name": nameUpper, "value": value})
+            parsedTJA.courses[currentCourse].data.append(TJAData(nameUpper, value))
             
     # If a course has no song data, then this is likely because the course has "STYLE: Double" but no "STYLE: Single".
     # To fix this, we copy over the P1 chart from "STYLE: Double" to fill the "STYLE: Single" role.
-    for courseName, course in courses.items():
-        if not course['data']:
-            if courseName+"P1" in courses.keys():
-                courses[courseName] = deepcopy(courses[courseName+"P1"])
+    for courseName, course in parsedTJA.courses.items():
+        if not course.data:
+            if courseName+"P1" in parsedTJA.courses.keys():
+                parsedTJA.courses[courseName] = deepcopy(parsedTJA.courses[courseName+"P1"])
+
+    # Remove any charts (e.g. P1/P2) not present in the TJA file
+    for course_name in [k for k, v in parsedTJA.courses.items() if not v.data]:
+        del parsedTJA.courses[course_name]
 
-    return courses
+    return parsedTJA
 
 
-def parseCourseMeasures(lines):
+def parseCourseMeasures(course):
     # Check if the course has branches or not
-    hasBranches = True if [l for l in lines if l['name'] == 'BRANCHSTART'] else False
+    hasBranches = True if [l for l in course.data if l.name == 'BRANCHSTART'] else False
     currentBranch = 'all' if hasBranches else 'normal'
+    branch_condition = None
     flagLevelhold = False
 
     # Process course lines
     idx_m = 0
     idx_m_branchstart = 0
-    emptyMeasure = {'data': '', 'events': []}
-    branches = {'normal': [deepcopy(emptyMeasure)], 'advanced': [deepcopy(emptyMeasure)], 'master': [deepcopy(emptyMeasure)]}
-    for line in lines:
+    for line in course.data:
         # 1. Parse measure notes
-        if line['name'] == 'NOTES':
-            notes = line['value']
+        if line.name == 'NOTES':
+            notes = line.value
             # If measure has ended, then add notes to the current measure, then start a new one by incrementing idx_m
             if notes.endswith(','):
-                for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
-                    branches[branch][idx_m]['data'] += notes[0:-1]
-                    branches[branch].append(deepcopy(emptyMeasure))
+                for branch in course.branches.keys() if currentBranch == 'all' else [currentBranch]:
+                    course.branches[branch][idx_m].notes += notes[0:-1]
+                    course.branches[branch].append(TJAMeasure())
                 idx_m += 1
             # Otherwise, keep adding notes to the current measure ('idx_m')
             else:
-                for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
-                    branches[branch][idx_m]['data'] += notes
+                for branch in course.branches.keys() if currentBranch == 'all' else [currentBranch]:
+                    course.branches[branch][idx_m].notes += notes
 
         # 2. Parse measure commands that produce an "event"
-        elif line['name'] in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF', 'DELAY',
-                              'SCROLL', 'BPMCHANGE', 'MEASURE', 'BRANCHSTART']:
+        elif line.name in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF', 'DELAY',
+                           'SCROLL', 'BPMCHANGE', 'MEASURE', 'SECTION', 'BRANCHSTART']:
             # Get position of the event
-            for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
-                pos = len(branches[branch][idx_m]['data'])
+            for branch in course.branches.keys() if currentBranch == 'all' else [currentBranch]:
+                pos = len(course.branches[branch][idx_m].notes)
 
             # Parse event type
-            if line['name'] == 'GOGOSTART':
-                currentEvent = {"name": 'gogo', "position": pos, "value": '1'}
-            elif line['name'] == 'GOGOEND':
-                currentEvent = {"name": 'gogo', "position": pos, "value": '0'}
-            elif line['name'] == 'BARLINEON':
-                currentEvent = {"name": 'barline', "position": pos, "value": '1'}
-            elif line['name'] == 'BARLINEOFF':
-                currentEvent = {"name": 'barline', "position": pos, "value": '0'}
-            elif line['name'] == 'DELAY':
-                currentEvent = {"name": 'delay', "position": pos, "value": float(line['value'])}
-            elif line['name'] == 'SCROLL':
-                currentEvent = {"name": 'scroll', "position": pos, "value": float(line['value'])}
-            elif line['name'] == 'BPMCHANGE':
-                currentEvent = {"name": 'bpm', "position": pos, "value": float(line['value'])}
-            elif line['name'] == 'MEASURE':
-                currentEvent = {"name": 'measure', "position": pos, "value": line['value']}
-            elif line["name"] == 'BRANCHSTART':
+            if line.name == 'GOGOSTART':
+                currentEvent = TJAData('gogo', '1', pos)
+            elif line.name == 'GOGOEND':
+                currentEvent = TJAData('gogo', '0', pos)
+            elif line.name == 'BARLINEON':
+                currentEvent = TJAData('barline', '1', pos)
+            elif line.name == 'BARLINEOFF':
+                currentEvent = TJAData('barline', '0', pos)
+            elif line.name == 'DELAY':
+                currentEvent = TJAData('delay', float(line.value), pos)
+            elif line.name == 'SCROLL':
+                currentEvent = TJAData('scroll', float(line.value), pos)
+            elif line.name == 'BPMCHANGE':
+                currentEvent = TJAData('bpm', float(line.value), pos)
+            elif line.name == 'MEASURE':
+                currentEvent = TJAData('measure', line.value, pos)
+            elif line.name == 'SECTION':
+                # If #SECTION occurs before the first #BRANCHSTART condition, then we have no percentage/drumroll values
+                # to use for the branchInfo bytes when writing to the fumen. So, we just use default values (-1, -1).
+                if branch_condition is None:
+                    branch_condition = ['#SECTION', -1, -1]
+                # Otherwise, if #SECTION occurs after a #BRANCHSTART condition, then we just repeat the previous
+                # condition (to set the correct branchInfo bytes for this measure.)
+                currentEvent = TJAData('branchStart', branch_condition, pos)
+            elif line.name == 'BRANCHSTART':
                 if flagLevelhold:
                     continue
                 currentBranch = 'all'  # Ensure that the #BRANCHSTART command is present for all branches
-                values = line['value'].split(',')
-                if values[0] == 'r':  # r = drumRoll
-                    values[1] = int(values[1])  # # of drumrolls
-                    values[2] = int(values[2])  # # of drumrolls
-                elif values[0] == 'p':  # p = Percentage
-                    values[1] = float(values[1]) / 100  # %
-                    values[2] = float(values[2]) / 100  # %
-                currentEvent = {"name": 'branchStart', "position": pos, "value": values}
+                branch_condition = line.value.split(',')
+                if branch_condition[0] == 'r':  # r = drumRoll
+                    branch_condition[1] = int(branch_condition[1])  # # of drumrolls
+                    branch_condition[2] = int(branch_condition[2])  # # of drumrolls
+                elif branch_condition[0] == 'p':  # p = Percentage
+                    branch_condition[1] = float(branch_condition[1]) / 100  # %
+                    branch_condition[2] = float(branch_condition[2]) / 100  # %
+                currentEvent = TJAData('branchStart', branch_condition, pos)
                 idx_m_branchstart = idx_m  # Preserve the index of the BRANCHSTART command to re-use for each branch
 
             # Append event to the current measure's events
-            for branch in branches.keys() if currentBranch == 'all' else [currentBranch]:
-                branches[branch][idx_m]['events'].append(currentEvent)
-        elif line['name'] == 'SECTION':
-            # Simply repeat the same #BRANCHSTART condition that happened previously
-            # The purpose of #SECTION is to "Reset accuracy values for notes and drumrolls on the next measure."
-            branches[branch][idx_m]['events'].append({"name": 'branchStart', "position": pos, "value": values})
+            for branch in course.branches.keys() if currentBranch == 'all' else [currentBranch]:
+                course.branches[branch][idx_m].events.append(currentEvent)
 
         # 3. Parse commands that don't create an event (e.g. simply changing the current branch)
         else:
-            if line["name"] == 'START' or line['name'] == 'END':
+            if line.name == 'START' or line.name == 'END':
                 currentBranch = 'all' if hasBranches else 'normal'
                 flagLevelhold = False
-            elif line['name'] == 'LEVELHOLD':
+            elif line.name == 'LEVELHOLD':
                 flagLevelhold = True
-            elif line["name"] == 'N':
+            elif line.name == 'N':
                 currentBranch = 'normal'
                 idx_m = idx_m_branchstart
-            elif line["name"] == 'E':
+            elif line.name == 'E':
                 currentBranch = 'advanced'
                 idx_m = idx_m_branchstart
-            elif line["name"] == 'M':
+            elif line.name == 'M':
                 currentBranch = 'master'
                 idx_m = idx_m_branchstart
-            elif line["name"] == 'BRANCHEND':
+            elif line.name == 'BRANCHEND':
                 currentBranch = 'all'
 
             # Ignored commands
-            elif line['name'] == 'LYRIC':
+            elif line.name == 'LYRIC':
                 pass
-            elif line['name'] == 'NEXTSONG':
+            elif line.name == 'NEXTSONG':
                 pass
 
             # Not implemented commands
             else:
                 raise NotImplementedError
 
     # Delete the last measure in the branch if no notes or events were added to it (due to preallocating empty measures)
-    for branch in branches.values():
-        if not branch[-1]['data'] and not branch[-1]['events']:
+    for branch in course.branches.values():
+        if not branch[-1].notes and not branch[-1].events:
             del branch[-1]
 
     # Merge measure data and measure events in chronological order
-    for branchName, branch in branches.items():
+    for branchName, branch in course.branches.items():
         for measure in branch:
-            notes = [{'pos': i, 'type': 'note', 'value': TJA_NOTE_TYPES[note]}
-                     for i, note in enumerate(measure['data']) if note != '0']
-            events = [{'pos': e['position'], 'type': e['name'], 'value': e['value']}
-                      for e in measure['events']]
-            combined = []
+            notes = [TJAData('note', TJA_NOTE_TYPES[note], i)
+                     for i, note in enumerate(measure.notes) if note != '0']
+            events = measure.events
             while notes or events:
                 if events and notes:
-                    if notes[0]['pos'] >= events[0]['pos']:
-                        combined.append(events.pop(0))
+                    if notes[0].pos >= events[0].pos:
+                        measure.combined.append(events.pop(0))
                     else:
-                        combined.append(notes.pop(0))
+                        measure.combined.append(notes.pop(0))
                 elif events:
-                    combined.append(events.pop(0))
+                    measure.combined.append(events.pop(0))
                 elif notes:
-                    combined.append(notes.pop(0))
-            measure['combined'] = combined
+                    measure.combined.append(notes.pop(0))
 
     # Ensure all branches have the same number of measures
     if hasBranches:
-        branch_lens = [len(b) for b in branches.values()]
+        branch_lens = [len(b) for b in course.branches.values()]
         if not branch_lens.count(branch_lens[0]) == len(branch_lens):
             raise ValueError("Branches do not have the same number of measures.")
 
-    return branches
-
 
 ########################################################################################################################
 # Fumen-parsing functions
 ########################################################################################################################
 
 # Fumen format reverse engineering TODOs
 # TODO: Figure out what drumroll bytes are (8 bytes after every drumroll)
@@ -271,26 +273,21 @@
         order = ">"
         totalMeasures = measuresBig
     else:
         order = "<"
         totalMeasures = measuresLittle
 
     # Initialize the dict that will contain the chart information
-    song = {'measures': []}
-    song['headerPadding'] = fumenHeader[:432]
-    song['headerMetadata'] = fumenHeader[-80:]
-    song['order'] = order
-
-    # I am unsure what byte this represents
-    unknownMetadata = readStruct(file, order, format_string="I", seek=0x204)[0]
-    song["unknownMetadata"] = unknownMetadata
-
-    # Determine whether the song has branches from byte 0x1b0 (decimal 432)
-    hasBranches = getBool(readStruct(file, order, format_string="B", seek=0x1b0)[0])
-    song["branches"] = hasBranches
+    song = FumenCourse(
+        headerPadding=fumenHeader[:432],
+        headerMetadata=fumenHeader[-80:],
+        order=order,
+        unknownMetadata=readStruct(file, order, format_string="I", seek=0x204)[0],
+        hasBranches=getBool(readStruct(file, order, format_string="B", seek=0x1b0)[0])
+    )
 
     # Start reading measure data from position 0x208 (decimal 520)
     file.seek(0x208)
     for measureNumber in range(totalMeasures):
         # Parse the measure data using the following `format_string`:
         #   "ffBBHiiiiiii" (12 format characters, 40 bytes per measure)
         #     - 'f': BPM              (represented by one float (4 bytes))
@@ -299,38 +296,40 @@
         #     - 'B': barline           (represented by one unsigned char (1 byte))
         #     - 'H': <padding>        (represented by one unsigned short (2 bytes))
         #     - 'iiiiii': branchInfo  (represented by six integers (24 bytes))
         #     - 'i': <padding>        (represented by one integer (4 bytes)
         measureStruct = readStruct(file, order, format_string="ffBBHiiiiiii")
 
         # Create the measure dictionary using the newly-parsed measure data
-        measure = {}
-        measure["bpm"] = measureStruct[0]
-        measure["fumenOffsetStart"] = measureStruct[1]
-        measure["gogo"] = getBool(measureStruct[2])
-        measure["barline"] = getBool(measureStruct[3])
-        measure["padding1"] = measureStruct[4]
-        measure["branchInfo"] = list(measureStruct[5:11])
-        measure["padding2"] = measureStruct[11]
+        measure = FumenMeasure(
+            bpm=measureStruct[0],
+            fumenOffsetStart=measureStruct[1],
+            gogo=getBool(measureStruct[2]),
+            barline=getBool(measureStruct[3]),
+            padding1=measureStruct[4],
+            branchInfo=list(measureStruct[5:11]),
+            padding2=measureStruct[11]
+        )
 
         # Iterate through the three branch types
-        for branchNumber in range(len(branchNames)):
+        for branchName in branchNames:
             # Parse the measure data using the following `format_string`:
             #   "HHf" (3 format characters, 8 bytes per branch)
             #     - 'H': totalNotes (represented by one unsigned short (2 bytes))
             #     - 'H': <padding>  (represented by one unsigned short (2 bytes))
             #     - 'f': speed      (represented by one float (4 bytes)
             branchStruct = readStruct(file, order, format_string="HHf")
 
             # Create the branch dictionary using the newly-parsed branch data
-            branch = {}
             totalNotes = branchStruct[0]
-            branch["length"] = totalNotes
-            branch["padding"] = branchStruct[1]
-            branch["speed"] = branchStruct[2]
+            branch = FumenBranch(
+                length=totalNotes,
+                padding=branchStruct[1],
+                speed=branchStruct[2],
+            )
 
             # Iterate through each note in the measure (per branch)
             for noteNumber in range(totalNotes):
                 # Parse the note data using the following `format_string`:
                 #   "ififHHf" (7 format characters, 24 bytes per note cluster)
                 #     - 'i': note type
                 #     - 'f': note position
@@ -347,54 +346,56 @@
                 if noteType not in noteTypes:
                     raise ValueError("Error: Unknown note type '{0}' at offset {1}".format(
                         shortHex(noteType).upper(),
                         hex(file.tell() - 0x18))
                     )
 
                 # Create the note dictionary using the newly-parsed note data
-                note = {}
-                note["type"] = noteTypes[noteType]
-                note["pos"] = noteStruct[1]
-                note["item"] = noteStruct[2]
-                note["padding"] = noteStruct[3]
+                note = FumenNote(
+                    note_type=noteTypes[noteType],
+                    pos=noteStruct[1],
+                    item=noteStruct[2],
+                    padding=noteStruct[3],
+                )
+
                 if noteType == 0xa or noteType == 0xc:
                     # Balloon hits
-                    note["hits"] = noteStruct[4]
-                    note["hitsPadding"] = noteStruct[5]
+                    note.hits = noteStruct[4]
+                    note.hitsPadding = noteStruct[5]
                 else:
-                    note['scoreInit'] = noteStruct[4]
-                    note['scoreDiff'] = noteStruct[5] // 4
-                    if "scoreInit" not in song:
-                        song["scoreInit"] = note['scoreInit']
-                        song["scoreDiff"] = note['scoreDiff']
+                    note.scoreInit = noteStruct[4]
+                    note.scoreDiff = noteStruct[5] // 4
+                    if not song.scoreInit:
+                        song.scoreInit = note.scoreInit
+                        song.scoreDiff = note.scoreDiff
                 if noteType == 0x6 or noteType == 0x9 or noteType == 0xa or noteType == 0xc:
                     # Drumroll and balloon duration in ms
-                    note["duration"] = noteStruct[6]
+                    note.duration = noteStruct[6]
                 else:
-                    note['duration'] = noteStruct[6]
+                    note.duration = noteStruct[6]
 
                 # Seek forward 8 bytes to account for padding bytes at the end of drumrolls
                 if noteType == 0x6 or noteType == 0x9 or noteType == 0x62:
-                    note["drumrollBytes"] = file.read(8)
+                    note.drumrollBytes = file.read(8)
 
                 # Assign the note to the branch
-                branch[noteNumber] = note
+                branch.notes.append(note)
 
             # Assign the branch to the measure
-            measure[branchNames[branchNumber]] = branch
+            measure.branches[branchName] = branch
 
         # Assign the measure to the song
-        song['measures'].append(measure)
+        song.measures.append(measure)
         if file.tell() >= size:
             break
 
     file.close()
 
     # NB: Official fumens often include empty measures as a way of inserting barlines for visual effect.
     #     But, TJA authors tend not to add these empty measures, because even without them, the song plays correctly.
     #     So, in tests, if we want to only compare the timing of the non-empty measures between an official fumen and
     #     a converted non-official TJA, then it's useful to  exclude the empty measures.
     if exclude_empty_measures:
-        song['measures'] = [m for m in song['measures']
-                            if m['normal']['length'] or m['advanced']['length'] or m['master']['length']]
+        song.measures = [m for m in song.measures
+                         if m.branches['normal'].length or m.branches['advanced'].length or m.branches['master'].length]
 
     return song
```

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-1.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-2-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-4-5.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-1-2.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-4.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-5-8.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-1-2.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-4.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-5-7.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-1-7.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-8.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-9-10.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-1.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-2-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-4-5.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-1-2.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-4.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-5-8.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-1-2.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-4.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-5-7.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-1-7.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-8.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-9-10.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-1.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-2-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-4-5.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-1-2.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-4.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-5-8.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-1-2.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-3.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-4.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-5-7.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-1-7.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-8.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-9-10.csv` & `tja2fumen-0.5.2/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/utils.py` & `tja2fumen-0.5.2/src/tja2fumen/utils.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.1/src/tja2fumen/writers.py` & `tja2fumen-0.5.2/src/tja2fumen/writers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 from tja2fumen.utils import writeStruct, putBool
 from tja2fumen.constants import branchNames, typeNotes
 
 
 def writeFumen(path_out, song):
     # Fetch the byte order (little/big endian)
-    order = song['order']
+    order = song.order
 
     # Write the header
     file = open(path_out, "wb")
-    file.write(song['headerPadding'])   # Write header padding bytes
-    file.write(song['headerMetadata'])  # Write header metadata bytes
+    file.write(song.headerPadding)   # Write header padding bytes
+    file.write(song.headerMetadata)  # Write header metadata bytes
 
     # Preallocate space in the file
     len_metadata = 8
     len_measures = 0
-    for measureNumber in range(len(song['measures'])):
+    for measureNumber in range(len(song.measures)):
         len_measures += 40
-        measure = song['measures'][measureNumber]
+        measure = song.measures[measureNumber]
         for branchNumber in range(len(branchNames)):
             len_measures += 8
-            branch = measure[branchNames[branchNumber]]
-            for noteNumber in range(branch['length']):
+            branch = measure.branches[branchNames[branchNumber]]
+            for noteNumber in range(branch.length):
                 len_measures += 24
-                note = branch[noteNumber]
-                if note['type'].lower() == "drumroll":
+                note = branch.notes[noteNumber]
+                if note.type.lower() == "drumroll":
                     len_measures += 8
     file.write(b'\x00' * (len_metadata + len_measures))
 
     # Write metadata
-    writeStruct(file, order, format_string="B", value_list=[putBool(song['branches'])], seek=0x1b0)
-    writeStruct(file, order, format_string="I", value_list=[len(song['measures'])], seek=0x200)
-    writeStruct(file, order, format_string="I", value_list=[song['unknownMetadata']], seek=0x204)
+    writeStruct(file, order, format_string="B", value_list=[putBool(song.hasBranches)], seek=0x1b0)
+    writeStruct(file, order, format_string="I", value_list=[len(song.measures)], seek=0x200)
+    writeStruct(file, order, format_string="I", value_list=[song.unknownMetadata], seek=0x204)
 
     # Write measure data
     file.seek(0x208)
-    for measureNumber in range(len(song['measures'])):
-        measure = song['measures'][measureNumber]
-        measureStruct = [measure['bpm'], measure['fumenOffsetStart'], int(measure['gogo']), int(measure['barline'])]
-        measureStruct.extend([measure['padding1']] + measure['branchInfo'] + [measure['padding2']])
+    for measureNumber in range(len(song.measures)):
+        measure = song.measures[measureNumber]
+        measureStruct = [measure.bpm, measure.fumenOffsetStart, int(measure.gogo), int(measure.barline)]
+        measureStruct.extend([measure.padding1] + measure.branchInfo + [measure.padding2])
         writeStruct(file, order, format_string="ffBBHiiiiiii", value_list=measureStruct)
 
         for branchNumber in range(len(branchNames)):
-            branch = measure[branchNames[branchNumber]]
-            branchStruct = [branch['length'], branch['padding'], branch['speed']]
+            branch = measure.branches[branchNames[branchNumber]]
+            branchStruct = [branch.length, branch.padding, branch.speed]
             writeStruct(file, order, format_string="HHf", value_list=branchStruct)
 
-            for noteNumber in range(branch['length']):
-                note = branch[noteNumber]
-                noteStruct = [typeNotes[note['type']], note['pos'], note['item'], note['padding']]
+            for noteNumber in range(branch.length):
+                note = branch.notes[noteNumber]
+                noteStruct = [typeNotes[note.type], note.pos, note.item, note.padding]
                 # Balloon hits
-                if 'hits' in note.keys():
-                    noteStruct.extend([note["hits"], note['hitsPadding']])
+                if note.hits:
+                    noteStruct.extend([note.hits, note.hitsPadding])
                 else:
-                    noteStruct.extend([note['scoreInit'], note['scoreDiff'] * 4])
+                    noteStruct.extend([note.scoreInit, note.scoreDiff * 4])
                 # Drumroll or balloon duration
-                noteStruct.append(note['duration'])
+                noteStruct.append(note.duration)
                 writeStruct(file, order, format_string="ififHHf", value_list=noteStruct)
-                if note['type'].lower() == "drumroll":
-                    file.write(note['drumrollBytes'])
+                if note.type.lower() == "drumroll":
+                    file.write(note.drumrollBytes)
     file.close()
```

### Comparing `tja2fumen-0.5.1/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.5.2/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.5.1
+Version: 0.5.2
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -38,14 +38,15 @@
 
 This project attempts to replace/complement the existing closed-source [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter packaged alongside TakoTako. 
 
 ## Goals
 
 - Act as a drop-in replacement for `tja2bin.exe` in TakoTako.
 - Fix https://github.com/Fluto/TakoTako/issues/16. (The original `tjabin.exe` doesn't properly handle `#BPMCHANGE` commands.)
+- Better handle commands that `tjabin.exe` fails for (`#SECTION`, `#NEXTSONG`, `#LYRIC`, etc.)
 - Provide open source code to act as a reference for parsing and writing both the TJA and Fumen file formats.
 - Stick to the Python stdlib, i.e. no external dependencies if possible.
 
 ## Usage
 
 ### Option 1: Standalone Python installation
```

### Comparing `tja2fumen-0.5.1/src/tja2fumen.egg-info/SOURCES.txt` & `tja2fumen-0.5.2/src/tja2fumen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 src/tja2fumen/__init__.py
 src/tja2fumen/constants.py
 src/tja2fumen/converters.py
 src/tja2fumen/parsers.py
+src/tja2fumen/types.py
 src/tja2fumen/utils.py
 src/tja2fumen/writers.py
 src/tja2fumen.egg-info/PKG-INFO
 src/tja2fumen.egg-info/SOURCES.txt
 src/tja2fumen.egg-info/dependency_links.txt
 src/tja2fumen.egg-info/entry_points.txt
 src/tja2fumen.egg-info/requires.txt
```

