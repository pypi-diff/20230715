# Comparing `tmp/microcat-0.2.1.tar.gz` & `tmp/microcat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.2.1.tar", last modified: Sat Jul 15 11:52:20 2023, max compression
+gzip compressed data, was "microcat-0.2.2.tar", last modified: Sat Jul 15 11:59:05 2023, max compression
```

## Comparing `microcat-0.2.1.tar` & `microcat-0.2.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-07-08 04:52:18.000000 microcat-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:52:20.377187 microcat-0.2.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.373187 microcat-0.2.1/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-15 11:52:18.000000 microcat-0.2.1/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.2.1/microcat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.1/microcat/chemistry_defs.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.373187 microcat-0.2.1/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     3300 2023-07-13 12:54:29.000000 microcat-0.2.1/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     9364 2023-07-09 15:21:44.000000 microcat-0.2.1/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    35789 2023-07-15 11:49:55.000000 microcat-0.2.1/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-13 08:58:40.000000 microcat-0.2.1/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-13 08:58:14.000000 microcat-0.2.1/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.2.1/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.2.1/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.2.1/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.2.1/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.2.1/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.2.1/microcat/envs/trimming.yaml
--rwxr-xr-x   0 root         (0) root         (0)     5065 2023-07-08 04:34:53.000000 microcat-0.2.1/microcat/prepare.py
--rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.2.1/microcat/rich_agrpase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.2.1/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.2.1/microcat/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.2.1/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.2.1/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    38249 2023-07-15 11:51:50.000000 microcat-0.2.1/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    11923 2023-07-13 09:56:14.000000 microcat-0.2.1/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.1/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.1/microcat/scripts/add_tags_to_PathSeq_bam.py
--rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.1/microcat/scripts/create_hdf5.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.1/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.2.1/microcat/scripts/extract_microbiome_output.R
--rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.1/microcat/scripts/generate_PE_manifest_file.py
--rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.1/microcat/scripts/get_ncbi_domains.py
--rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.2.1/microcat/scripts/krak2_output_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.1/microcat/scripts/kraken2mpa.py
--rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.1/microcat/scripts/kraken2sc.py
--rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.1/microcat/scripts/microcat_bam_handle.Rmd
--rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.2.1/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.2.1/microcat/scripts/sckmer_unpaired.R
--rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.1/microcat/scripts/spilt_bam_by_tag.py
--rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.1/microcat/scripts/split_Starsolo_BAM_by_RG.py
--rw-r--r--   0 root         (0) root         (0)    13555 2023-07-15 04:01:31.000000 microcat-0.2.1/microcat/scripts/starsolo_tenX_auto.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.1/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-13 07:09:46.000000 microcat-0.2.1/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)    21138 2023-07-13 07:08:00.000000 microcat-0.2.1/microcat/snakefiles/scRNA_wf_test.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.1/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.373187 microcat-0.2.1/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1552 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 11:52:20.377187 microcat-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-08 04:52:22.000000 microcat-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.344248 microcat-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-07-08 04:52:18.000000 microcat-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:59:05.344248 microcat-0.2.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-15 11:59:01.000000 microcat-0.2.2/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      968 2023-07-15 11:56:59.000000 microcat-0.2.2/microcat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.2/microcat/chemistry_defs.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-07-13 12:54:29.000000 microcat-0.2.2/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     9364 2023-07-09 15:21:44.000000 microcat-0.2.2/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    35789 2023-07-15 11:49:55.000000 microcat-0.2.2/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-13 08:58:40.000000 microcat-0.2.2/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-13 08:58:14.000000 microcat-0.2.2/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.2.2/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.2.2/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.2.2/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.2.2/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.2.2/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.2.2/microcat/envs/trimming.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     5065 2023-07-08 04:34:53.000000 microcat-0.2.2/microcat/prepare.py
+-rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.2.2/microcat/rich_agrpase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.2.2/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.2.2/microcat/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.2.2/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.2.2/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    38249 2023-07-15 11:51:50.000000 microcat-0.2.2/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    11923 2023-07-13 09:56:14.000000 microcat-0.2.2/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.344248 microcat-0.2.2/microcat/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.2/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.2/microcat/scripts/add_tags_to_PathSeq_bam.py
+-rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.2/microcat/scripts/create_hdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.2/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.2.2/microcat/scripts/extract_microbiome_output.R
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.2/microcat/scripts/generate_PE_manifest_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.2/microcat/scripts/get_ncbi_domains.py
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.2.2/microcat/scripts/krak2_output_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.2/microcat/scripts/kraken2mpa.py
+-rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.2/microcat/scripts/kraken2sc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.2/microcat/scripts/microcat_bam_handle.Rmd
+-rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.2.2/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.2.2/microcat/scripts/sckmer_unpaired.R
+-rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.2/microcat/scripts/spilt_bam_by_tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.2/microcat/scripts/split_Starsolo_BAM_by_RG.py
+-rw-r--r--   0 root         (0) root         (0)    13555 2023-07-15 04:01:31.000000 microcat-0.2.2/microcat/scripts/starsolo_tenX_auto.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.344248 microcat-0.2.2/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.2/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-13 07:09:46.000000 microcat-0.2.2/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)    21138 2023-07-13 07:08:00.000000 microcat-0.2.2/microcat/snakefiles/scRNA_wf_test.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.2/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 11:59:05.344248 microcat-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-08 04:52:22.000000 microcat-0.2.2/setup.py
```

### Comparing `microcat-0.2.1/LICENSE` & `microcat-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/PKG-INFO` & `microcat-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.1
+Version: 0.2.2
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.1/microcat/__init__.py` & `microcat-0.2.2/microcat/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 from microcat.sample import get_samples_bax
 
 from microcat.sample import get_samples_id_by_tissue
 from microcat.sample import get_samples_id_by_patient
 from microcat.sample import get_samples_id_by_lane
 from microcat.sample import get_samples_id_by_library
 from microcat.sample import get_tissue_by_patient
-
+from microcat.sample import get_SAMattrRGline_by_sample
 from microcat.sample import get_SAMattrRGline_from_manifest
 
 from microcat.__about__ import __version__, __author__
 
 
 name = "microcat"
```

### Comparing `microcat-0.2.1/microcat/chemistry_defs.json` & `microcat-0.2.2/microcat/chemistry_defs.json`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/config/config.yaml` & `microcat-0.2.2/microcat/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/configer.py` & `microcat-0.2.2/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/corer.py` & `microcat-0.2.2/microcat/corer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/prepare.py` & `microcat-0.2.2/microcat/prepare.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/rich_agrpase.py` & `microcat-0.2.2/microcat/rich_agrpase.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/rules/ERCC.smk` & `microcat-0.2.2/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/rules/build.smk` & `microcat-0.2.2/microcat/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/rules/classfier.smk` & `microcat-0.2.2/microcat/rules/classfier.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/rules/database.smk` & `microcat-0.2.2/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/rules/host.smk` & `microcat-0.2.2/microcat/rules/host.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/sample.py` & `microcat-0.2.2/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/INVADEseq.py` & `microcat-0.2.2/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/add_tags_to_PathSeq_bam.py` & `microcat-0.2.2/microcat/scripts/add_tags_to_PathSeq_bam.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/create_hdf5.py` & `microcat-0.2.2/microcat/scripts/create_hdf5.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/extract_kraken_reads.py` & `microcat-0.2.2/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/extract_microbiome_output.R` & `microcat-0.2.2/microcat/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/generate_PE_manifest_file.py` & `microcat-0.2.2/microcat/scripts/generate_PE_manifest_file.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/get_ncbi_domains.py` & `microcat-0.2.2/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/krak2_output_denosing.R` & `microcat-0.2.2/microcat/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/kraken2mpa.py` & `microcat-0.2.2/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/kraken2sc.py` & `microcat-0.2.2/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/microcat_bam_handle.Rmd` & `microcat-0.2.2/microcat/scripts/microcat_bam_handle.Rmd`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/sample_denosing.R` & `microcat-0.2.2/microcat/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/sckmer_unpaired.R` & `microcat-0.2.2/microcat/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.2.2/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/split_Starsolo_BAM_by_RG.py` & `microcat-0.2.2/microcat/scripts/split_Starsolo_BAM_by_RG.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/scripts/starsolo_tenX_auto.sh` & `microcat-0.2.2/microcat/scripts/starsolo_tenX_auto.sh`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.2.2/microcat/snakefiles/scRNA_wf.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat/snakefiles/scRNA_wf_test.smk` & `microcat-0.2.2/microcat/snakefiles/scRNA_wf_test.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/microcat.egg-info/PKG-INFO` & `microcat-0.2.2/microcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.1
+Version: 0.2.2
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.1/microcat.egg-info/SOURCES.txt` & `microcat-0.2.2/microcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcat-0.2.1/setup.py` & `microcat-0.2.2/setup.py`

 * *Files identical despite different names*

