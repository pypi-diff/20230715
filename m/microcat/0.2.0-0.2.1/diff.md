# Comparing `tmp/microcat-0.2.0.tar.gz` & `tmp/microcat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.2.0.tar", last modified: Sat Jul  8 04:57:08 2023, max compression
+gzip compressed data, was "microcat-0.2.1.tar", last modified: Sat Jul 15 11:52:20 2023, max compression
```

## Comparing `microcat-0.2.0.tar` & `microcat-0.2.1.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.845013 microcat-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-07-08 04:52:18.000000 microcat-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-08 04:57:08.845013 microcat-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.837013 microcat-0.2.0/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-08 04:35:29.000000 microcat-0.2.0/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.2.0/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.841013 microcat-0.2.0/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-19 01:50:35.000000 microcat-0.2.0/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     9364 2023-07-08 04:57:07.000000 microcat-0.2.0/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    34429 2023-07-06 07:45:55.000000 microcat-0.2.0/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.841013 microcat-0.2.0/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-17 10:22:04.000000 microcat-0.2.0/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.2.0/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.2.0/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.2.0/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.2.0/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.2.0/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.2.0/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.2.0/microcat/envs/trimming.yaml
--rwxr-xr-x   0 root         (0) root         (0)     5065 2023-07-08 04:34:53.000000 microcat-0.2.0/microcat/prepare.py
--rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.2.0/microcat/rich_agrpase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.841013 microcat-0.2.0/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.2.0/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.2.0/microcat/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.2.0/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.2.0/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    74506 2023-07-06 06:41:05.000000 microcat-0.2.0/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.2.0/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.841013 microcat-0.2.0/microcat/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.0/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.0/microcat/scripts/add_tags_to_PathSeq_bam.py
--rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.0/microcat/scripts/create_hdf5.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.0/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.2.0/microcat/scripts/extract_microbiome_output.R
--rw-r--r--   0 root         (0) root         (0)     1214 2023-06-23 14:00:52.000000 microcat-0.2.0/microcat/scripts/generate_PE_manifest_file.py
--rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.0/microcat/scripts/get_ncbi_domains.py
--rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.2.0/microcat/scripts/krak2_output_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.0/microcat/scripts/kraken2mpa.py
--rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.0/microcat/scripts/kraken2sc.py
--rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.0/microcat/scripts/microcat_bam_handle.Rmd
--rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.2.0/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.2.0/microcat/scripts/sckmer_unpaired.R
--rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.0/microcat/scripts/spilt_bam_by_tag.py
--rwxrwxrwx   0 root         (0) root         (0)     1973 2023-06-24 01:45:21.000000 microcat-0.2.0/microcat/scripts/split_Starsolo_BAM_by_RG.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.845013 microcat-0.2.0/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.0/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1928 2023-06-24 02:40:05.000000 microcat-0.2.0/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)     8723 2023-07-02 16:16:54.000000 microcat-0.2.0/microcat/snakefiles/scRNA_wf_test.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.0/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 04:57:08.841013 microcat-0.2.0/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-08 04:57:08.000000 microcat-0.2.0/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1484 2023-07-08 04:57:08.000000 microcat-0.2.0/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 04:57:08.000000 microcat-0.2.0/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-08 04:57:08.000000 microcat-0.2.0/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-08 04:57:08.000000 microcat-0.2.0/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-08 04:57:08.000000 microcat-0.2.0/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 04:57:08.845013 microcat-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-08 04:52:22.000000 microcat-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-07-08 04:52:18.000000 microcat-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:52:20.377187 microcat-0.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.373187 microcat-0.2.1/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-15 11:52:18.000000 microcat-0.2.1/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      913 2023-06-17 14:38:27.000000 microcat-0.2.1/microcat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.1/microcat/chemistry_defs.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.373187 microcat-0.2.1/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-07-13 12:54:29.000000 microcat-0.2.1/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     9364 2023-07-09 15:21:44.000000 microcat-0.2.1/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    35789 2023-07-15 11:49:55.000000 microcat-0.2.1/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-13 08:58:40.000000 microcat-0.2.1/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-13 08:58:14.000000 microcat-0.2.1/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.2.1/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.2.1/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.2.1/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.2.1/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.2.1/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.2.1/microcat/envs/trimming.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     5065 2023-07-08 04:34:53.000000 microcat-0.2.1/microcat/prepare.py
+-rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.2.1/microcat/rich_agrpase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.2.1/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.2.1/microcat/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.2.1/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.2.1/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    38249 2023-07-15 11:51:50.000000 microcat-0.2.1/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    11923 2023-07-13 09:56:14.000000 microcat-0.2.1/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.1/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.1/microcat/scripts/add_tags_to_PathSeq_bam.py
+-rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.1/microcat/scripts/create_hdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.1/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.2.1/microcat/scripts/extract_microbiome_output.R
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.1/microcat/scripts/generate_PE_manifest_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.1/microcat/scripts/get_ncbi_domains.py
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.2.1/microcat/scripts/krak2_output_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.1/microcat/scripts/kraken2mpa.py
+-rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.1/microcat/scripts/kraken2sc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.1/microcat/scripts/microcat_bam_handle.Rmd
+-rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.2.1/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.2.1/microcat/scripts/sckmer_unpaired.R
+-rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.1/microcat/scripts/spilt_bam_by_tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.1/microcat/scripts/split_Starsolo_BAM_by_RG.py
+-rw-r--r--   0 root         (0) root         (0)    13555 2023-07-15 04:01:31.000000 microcat-0.2.1/microcat/scripts/starsolo_tenX_auto.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.377187 microcat-0.2.1/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.1/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-13 07:09:46.000000 microcat-0.2.1/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)    21138 2023-07-13 07:08:00.000000 microcat-0.2.1/microcat/snakefiles/scRNA_wf_test.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.1/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:52:20.373187 microcat-0.2.1/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 11:52:20.000000 microcat-0.2.1/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 11:52:20.377187 microcat-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-08 04:52:22.000000 microcat-0.2.1/setup.py
```

### Comparing `microcat-0.2.0/LICENSE` & `microcat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/PKG-INFO` & `microcat-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.0
+Version: 0.2.1
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.0/microcat/__init__.py` & `microcat-0.2.1/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/config/config.yaml` & `microcat-0.2.1/microcat/config/config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,34 @@
       do: false
       reference: "/data/database/refdata-gex-GRCh38-2020-A"
       variousParams: ""
       threads: 40
     starsolo:
       do: True
       reference: "/data/database/STAR_refdata-gex-GRCh38-2020-A"
+      barcode:
+        soloCBwhitelist:
+        soloCBstart:
+        soloCBlen:
+        soloUMIstart:
+        soloUMIlen:
+        soloCBposition:
+        soloUMIposition:
+      algorithm:
+        soloUMIdedup:
+        soloCBmatchWLtype:
+        soloUMIfiltering:
+        soloCellFilter:
+        clipAdapterType:
+        outFilterScoreMin:
+        soloMultiMappers:
+      soloType: 
+      soloAdapterSequence: ""
+      soloStrand:
       variousParams: ""
-      assay: tenX_v3
       threads: 40
 
   classifier:
     kraken2uniq:
       do: true
       kraken2_database: "/data/database/kraken2_RefSeqV217_Complete_Chrom_nont"
       threads: 40
@@ -100,8 +118,9 @@
   kraken2mpa: scripts/kraken2mpa.py
   kraken2sc: scripts/kraken2sc.py
   extract_kraken_reads: scripts/extract_kraken_reads.py
   krak2_output_denosing: scripts/krak2_output_denosing.R
   sckmer_unpaired: scripts/sckmer_unpaired.R
   spilt_bam_by_tag: scripts/spilt_bam_by_tag.py
   sample_denosing: scripts/sample_denosing.R
-  INVADEseq: scripts/INVADEseq.py
+  INVADEseq: scripts/INVADEseq.py
+  starsolo_10X_auto: scripts/starsolo_tenX_auto.sh
```

### Comparing `microcat-0.2.0/microcat/configer.py` & `microcat-0.2.1/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/corer.py` & `microcat-0.2.1/microcat/corer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 import os
 import subprocess
 import sys
 import textwrap
 from io import StringIO
 import pandas as pd
-
+import json
 import microcat
 import re
 import sys
 from typing import TYPE_CHECKING, Callable, ClassVar, Iterable, Iterator
 
 # rich is only used to display help. It is imported inside the functions in order
 # not to add delays to command line tools that use this formatter.
@@ -402,39 +402,58 @@
 
 def add_parser(*args, **kwds):
     kwds.setdefault("formatter_class", parser.formatter_class)
     return subparsers.add_parser(*args, **kwds)
 
 WORKFLOWS_MAG = [
     "host_all",
-    "check_all",]
+    "classifier_all",]
 
 WORKFLOWS_SCRNA = [
     "host_all",
     "kraken2uniq_classified_all",
     "krakenuniq_classified_all",
     "pathseq_classified_all",
     "metaphlan_classified_all",
     "classifier_all",]
 
-def update_config_tools(conf, host, classifier,assay=None):
+def update_config_tools(conf, host, classifier,chemistry=None,chemistry_defs=None):
     conf["params"]["simulate"]["do"] = False
     # conf["params"]["begin"] = begin
 
     # for trimmer_ in ["sickle", "fastp"]:
     #     if trimmer_ == trimmer:
     #         conf["params"]["trimming"][trimmer_]["do"] = True
     #     else:
     #         conf["params"]["trimming"][trimmer_]["do"] = False
 
     for hoster_ in ["starsolo","cellranger"]:
         if hoster_ == host:
             conf["params"]["host"][hoster_]["do"] = True
             if hoster_ == "starsolo":
-                conf["params"]["host"][hoster_]["assay"] = assay
+                if chemistry in chemistry_defs:
+                    chem_params = chemistry_defs[chemistry]
+
+                    # 更新host.starsolo.barcode下的参数
+                    barcode_params = chem_params.get("barcode")
+
+                    if barcode_params:
+                        for key, value in barcode_params[0].items():
+                            conf["params"]["host"]["starsolo"]["barcode"][key] = value
+
+                    # 更新host.starsolo.algorithm下的参数
+                    algorithm_params = chem_params.get("algorithm")
+                    if algorithm_params:
+                        for key, value in algorithm_params[0].items():
+                            conf["params"]["host"]["starsolo"]["algorithm"][key] = value
+
+                    # 更新host.starsolo下的其他参数
+                    for key, value in chem_params.items():
+                        if key not in ["barcode", "algorithm"]:
+                            conf["params"]["host"]["starsolo"][key] = value
         else:
             conf["params"]["host"][hoster_]["do"] = False
 
     for classifier_ in ["kraken2uniq","krakenuniq","pathseq","metaphlan"]:
         if classifier_ in classifier:
             conf["params"]["classifier"][classifier_]["do"] = True
         else:
@@ -473,41 +492,44 @@
         # Print the project structure and create the necessary subdirectories
         print(project.__str__())
         project.create_dirs()
 
         # Get the default configuration
         conf = project.get_config()
 
+        with open(os.path.join(os.path.join(os.path.dirname(__file__),"chemistry_defs.json"))) as file:
+            CHEMISTRY_DEFS = json.load(file)
 
         # Update environment configuration file paths
         for env_name in conf["envs"]:
             conf["envs"][env_name] = os.path.join(os.path.realpath(args.workdir), f"envs/{env_name}.yaml")
 
 
         for script_path in conf["scripts"]:
             origin_path = conf["scripts"][script_path]
             conf["scripts"][script_path] = os.path.join(os.path.dirname(__file__),f"{origin_path}")
 
         # Update the configuration with the selected tools
         conf = update_config_tools(
-            conf,args.host,args.classifier,args.assay
+            conf,args.host,args.classifier,args.chemistry,chemistry_defs=CHEMISTRY_DEFS
         )
 
         # Add the user-supplied samples table to the configuration
         if args.samples:
-            conf["params"]["samples"] = args.samples
+            conf["params"]["samples"] = os.path.abspath(args.samples)
         else:
             print("Please supply samples table")
             sys.exit(-1)
 
         # Update the configuration file
         microcat.update_config(
             project.config_file, project.new_config_file, conf, remove=False
         )
 
+        print("\033[32mNOTE: \nCongfig.yaml reset to default values.\033[0m")
     else:
         # If the user didn't provide a working directory, print an error message and exit
         print("Please supply a workdir!")
         sys.exit(-1)
 
 
 def run_snakemake(args, unknown, snakefile, workflow):
@@ -842,26 +864,26 @@
         type=str,
         default="starsolo",
         required=False,
         choices=["starsolo","cellranger"],
         help="Which rmhoster used",
     )
     parser_init.add_argument(
-        "--assay",
+        "--chemistry",
         type=str,
-        default=None,
-        choices=["Smartseq", "Smartseq2", "tenX_v3", "tenX_v2", "tenX_v1","Seq-well","tenX_auto"],
-        help="Sequencing assay option, required when host is starsolo",
+        default="tenx_auto",
+        choices=["smartseq", "smartseq2", "tenx_3pv1", "tenx_3pv2", "tenx_3pv3","seqwell","tenx_auto","dropseq","tenx_multiome","tenx_5ppe","seqwell","celseq2"],
+        help="Sequencing chemistry option, required when host is starsolo",
     )
     
     parser_init.add_argument(
         "--classifier",
         nargs="+",
         required=False,
-        default="kraken2uniq",
+        default="pathseq",
         choices=["kraken2uniq","krakenuniq","pathseq","metaphlan"],
         help="Which classifier used",
     )
 
     parser_init.set_defaults(func=init)
     
 
@@ -917,16 +939,16 @@
         choices=WORKFLOWS_SCRNA,
         help="pipeline end point. Allowed values are " + ", ".join(WORKFLOWS_MAG),
     )
     parser_scrna_wf.set_defaults(func=scRNA_wf)
 
     args, unknown = parser.parse_known_args()
         
-    if hasattr(args, 'host') and args.host == "starsolo" and args.assay is None:
-        parser_init.error("--assay option is required when host is starsolo")
+    if hasattr(args, 'host') and args.host == "starsolo" and args.chemistry is None:
+        parser_init.error("--chemistry option is required when host is starsolo")
 
     try:
         if args.version:
             print("microcat version %s" % microcat.__version__)
             sys.exit(0)
         args.func(args, unknown)
     except AttributeError as e:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `microcat-0.2.0/microcat/prepare.py` & `microcat-0.2.1/microcat/prepare.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/rich_agrpase.py` & `microcat-0.2.1/microcat/rich_agrpase.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/rules/ERCC.smk` & `microcat-0.2.1/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/rules/build.smk` & `microcat-0.2.1/microcat/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/rules/classfier.smk` & `microcat-0.2.1/microcat/rules/classfier.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/rules/database.smk` & `microcat-0.2.1/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/sample.py` & `microcat-0.2.1/microcat/sample.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,29 +42,38 @@
     if not set(['id', 'fq1', 'fq2']).issubset(samples_df.columns):
         raise ValueError("Columns 'id', 'fq1', 'fq2' must exist in the sample.tsv")
     
     # Extract library, lane, and plate from id
     samples_df[['patient_tissue_lane_plate', 'library']] = samples_df['id'].str.rsplit("_", n=1, expand=True)
     
     # Determine the platform and parse accordingly
-    if platform == 'tenX':
+    if platform == 'lane':
         samples_df['is_lane'] = samples_df['patient_tissue_lane_plate'].apply(lambda x: x.split('_')[-1].startswith("L"))
         samples_df.loc[samples_df['is_lane'], 'lane'] = samples_df['patient_tissue_lane_plate'].apply(lambda x: x.split('_')[-1])
-    elif platform == 'smartseq':
+        # Extract patient and tissue, using the fact that tissue is always "S" followed by a number
+        # and is always the last part in patient_tissue
+        samples_df['patient_tissue'] = samples_df['patient_tissue_lane_plate'].apply(lambda x: '_'.join(x.split('_')[:-1]))
+        samples_df['tissue'] = samples_df['patient_tissue'].apply(lambda x: x.split('_')[-1])
+        samples_df['patient'] = samples_df['patient_tissue'].apply(lambda x: '_'.join(x.split('_')[:-1]))
+        samples_df = samples_df.drop(columns=['patient_tissue_lane_plate'])
+    elif platform == 'plate':
         samples_df['is_plate'] = samples_df['patient_tissue_lane_plate'].apply(lambda x: x.split('_')[-1].startswith("P"))
         samples_df.loc[samples_df['is_plate'], 'plate'] = samples_df['patient_tissue_lane_plate'].apply(lambda x: x.split('_')[-1])
+        samples_df['patient_tissue_cell'] = samples_df['patient_tissue_lane_plate'].apply(lambda x: '_'.join(x.split('_')[:-1]))
+        # Extract patient and tissue, using the fact that tissue is always "S" followed by a number
+        # and is always the last part in patient_tissue
+        samples_df['tissue'] = samples_df['patient_tissue_cell'].str.extract(r'(S\d+)_')
+        # 提取patient和cell
+        samples_df[['patient', 'cell']] = samples_df['patient_tissue_cell'].str.extract(r'(.+)_S\d+_(.+)')
+        samples_df = samples_df.drop(columns=['patient_tissue_lane_plate'])
+        samples_df = samples_df.drop(columns=['patient_tissue_cell'])
+        samples_df['patient_tissue'] = samples_df['patient'] + '_' + samples_df['tissue']
     else:
-        raise ValueError("Platform must be either 'tenX' or 'smartseq'")
-    
-    # Extract patient and tissue, using the fact that tissue is always "S" followed by a number
-    # and is always the last part in patient_tissue
-    samples_df['patient_tissue'] = samples_df['patient_tissue_lane_plate'].apply(lambda x: '_'.join(x.split('_')[:-1]))
-    samples_df['tissue'] = samples_df['patient_tissue'].apply(lambda x: x.split('_')[-1])
-    samples_df['patient'] = samples_df['patient_tissue'].apply(lambda x: '_'.join(x.split('_')[:-1]))
-    samples_df = samples_df.drop(columns=['patient_tissue_lane_plate'])
+        raise ValueError("Platform must be either 'lane' or 'plate'")
+
 
     if samples_df[['patient_tissue', 'library']].isnull().values.any():
         raise ValueError(f"id column must follow the format '{{Patient}}_{{tissue}}_{{lane or plate}}_{{library}}' for platform {platform}")
     
     # Create sample identifier
     samples_df['sample_id'] = samples_df['patient_tissue']
     
@@ -76,18 +85,18 @@
     samples_df['seq_type'] = 'single-end'
     samples_df.loc[samples_df['fq2'].notnull(), 'seq_type'] = 'paired-end'
     
     # Create a 'fastqs_dir' column that contains the directory of the fastq files
     samples_df['fastqs_dir'] = samples_df['fq1'].apply(lambda x: '/'.join(x.split('/')[:-1]))
     
     # Set index
-    if platform == 'tenX':
+    if platform == 'lane':
         samples_df = samples_df.set_index(["sample_id","patient", "tissue", "lane", "library"])
-    elif platform == 'smartseq':
-        samples_df = samples_df.set_index(["sample_id","patient", "tissue", "plate", "library"])
+    elif platform == 'plate':
+        samples_df = samples_df.set_index(["sample_id","patient", "cell","tissue", "plate", "library"])
 
     return samples_df
 
 
 def parse_bam_samples(sample_tsv, platform):
     samples_df = pd.read_csv(sample_tsv, sep="\t")
     
@@ -265,7 +274,22 @@
     df = pd.read_csv(manifest_file, sep="\t", header=None)
     # get the third column which contains the cell ids
     cell_ids = df[2]
     # generate the --outSAMattrRGline input format
     rgline = " , ".join([f"ID:{cell_id}" for cell_id in cell_ids])
     return rgline
 
+def get_SAMattrRGline_by_sample(samples_df, wildcards):
+    sample_id = wildcards.sample
+
+    # Filter samples based on sample_id and plate
+    samples_filtered = samples_df.loc[(samples_df.index.get_level_values("sample_id") == sample_id)]
+
+    # samples_filtered = samples_df.loc[(samples_df.index.get_level_values("sample_id") == sample_id) &
+    #                                 (samples_df.index.get_level_values("plate") == plate)]
+
+    # Get the cell IDs for the filtered samples
+    cell_ids = samples_filtered.index.get_level_values("cell").unique()
+
+    # Generate the --outSAMattrRGline input format
+    rgline = " , ".join([f"ID:{cell_id}" for cell_id in cell_ids])
+    return rgline
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `microcat-0.2.0/microcat/scripts/INVADEseq.py` & `microcat-0.2.1/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/add_tags_to_PathSeq_bam.py` & `microcat-0.2.1/microcat/scripts/add_tags_to_PathSeq_bam.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/create_hdf5.py` & `microcat-0.2.1/microcat/scripts/create_hdf5.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/extract_kraken_reads.py` & `microcat-0.2.1/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/extract_microbiome_output.R` & `microcat-0.2.1/microcat/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/get_ncbi_domains.py` & `microcat-0.2.1/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/krak2_output_denosing.R` & `microcat-0.2.1/microcat/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/kraken2mpa.py` & `microcat-0.2.1/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/kraken2sc.py` & `microcat-0.2.1/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/microcat_bam_handle.Rmd` & `microcat-0.2.1/microcat/scripts/microcat_bam_handle.Rmd`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/sample_denosing.R` & `microcat-0.2.1/microcat/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/sckmer_unpaired.R` & `microcat-0.2.1/microcat/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.2.1/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.0/microcat/scripts/split_Starsolo_BAM_by_RG.py` & `microcat-0.2.1/microcat/scripts/split_Starsolo_BAM_by_RG.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 output = []
 UMI_dict = defaultdict(list)
 # seg is an AlignedSegment object
 for seg in starsolo_bam.fetch(until_eof=True):
     # not all records will have the CB tag and the UB tag - they should now
     if seg.has_tag("RG"):
         if (seg.get_tag(tag="RG") == args.tag):
-            UMI_dict[seg.get_tag(tag="UB")].append(seg)
+            UMI_dict.append(seg)
 
 output_subdir = os.path.join(args.output_dir, "{}".format(tag))
 if not os.path.exists(output_subdir):
     os.makedirs(output_subdir,exist_ok=True)
         
 # split_file = pysam.AlignmentFile(os.path.join(output_subdir, "Aligned_sortedByName_unmapped_out.bam".format(args.tag, tag_itr)), "wb", template=samfile)
 
@@ -41,11 +41,45 @@
     # UMI_reads = UMI_dict[UMI]
     # UMI_read = UMI_reads[0]
     # #print(UMI_read)
     # for read in UMI_reads:
     #     #print(read)
     #     if read.mapping_quality > UMI_read.mapping_quality:
     #         UMI_read = read
-    read_group_bam.write(UMI_read)
+    read_group_bam.write(UMI)
 read_group_bam.close()
 
-starsolo_bam.close()
+starsolo_bam.close()
+
+
+# suppress incorrect error warning - https://github.com/pysam-developers/pysam/issues/939
+save = pysam.set_verbosity(0)
+# load and iterate through the PathSeq BAM file
+STAR_BAM = pysam.AlignmentFile(snakemake.input[0], mode="rb")
+# set verbosity back to original setting
+pysam.set_verbosity(save)
+
+output = []
+UMI_dict = defaultdict(list)
+# seg is an AlignedSegment object
+for seg in STAR_BAM.fetch(until_eof=True):
+    # not all records will have the CB tag and the UB tag - they should now
+    if seg.has_tag("CB") and seg.has_tag("UB"):
+        if (seg.get_tag(tag="CB") == snakemake.wildcards["cell"]):
+            UMI_dict[seg.get_tag(tag="UB")].append(seg)
+
+
+CELL_BAM = pysam.AlignmentFile(snakemake.output[0], mode="wb", template=STAR_BAM)
+for UMI in UMI_dict:
+    #print(UMI)
+    # keep one read per UMI - the read with the highest mapping quality
+    UMI_reads = UMI_dict[UMI]
+    UMI_read = UMI_reads[0]
+    #print(UMI_read)
+    for read in UMI_reads:
+        #print(read)
+        if read.mapping_quality > UMI_read.mapping_quality:
+            UMI_read = read
+    CELL_BAM.write(UMI_read)
+CELL_BAM.close()
+
+STAR_BAM.close()
```

### Comparing `microcat-0.2.0/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.2.1/microcat/snakefiles/scRNA_wf.smk`

 * *Files 14% similar despite different names*

```diff
@@ -28,28 +28,26 @@
 def warning(msg):
     print(f"\n{ansitxt.BOLD}{ansitxt.RED}{msg}{ansitxt.ENDC}\n",file=sys.stderr)
 
 
 PLATFORM = None
 
 if config["params"]["host"]["starsolo"]["do"]:
-    if "tenX" in config["params"]["host"]["starsolo"]["assay"]:
-        PLATFORM = "tenX"
-    elif "Smartseq" in config["params"]["host"]["starsolo"]["assay"]:
-        PLATFORM = "smartseq"
-    elif "Seq-well" in config["params"]["host"]["starsolo"]["assay"]:
-        PLATFORM = "tenX"
+    if  config["params"]["host"]["starsolo"]["soloType"]=="CB_UMI_Simple":
+        PLATFORM = "lane"
+    elif config["params"]["host"]["starsolo"]["soloType"]=="SmartSeq":
+        PLATFORM = "plate"
+    elif config["params"]["host"]["starsolo"]["soloType"]=="CB_UMI_Complex":
+        PLATFORM = "lane"
     else:
-        raise ValueError("Platform must be either 'tenX' or 'smartseq'")
+        raise ValueError("Platform must be either 'CB_UMI' or 'smartseq'")
 elif config["params"]["host"]["cellranger"]["do"]:
-    PLATFORM = "tenX"
+    PLATFORM = "lane"
 else:
-    raise ValueError("Platform must be either 'tenX' or 'smartseq'")
-
-
+    raise ValueError("Platform must be either 'lane' or 'plate'")
 
 
 try:
     SAMPLES = microcat.parse_samples(config["params"]["samples"],platform = PLATFORM)
     SAMPLES_ID_LIST = SAMPLES.index.get_level_values("sample_id").unique()
 except FileNotFoundError:
     warning(f"ERROR: the samples file does not exist. Please see the README file for details. Quitting now.")
```

### Comparing `microcat-0.2.0/microcat.egg-info/PKG-INFO` & `microcat-0.2.1/microcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.0
+Version: 0.2.1
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.0/microcat.egg-info/SOURCES.txt` & `microcat-0.2.1/microcat.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 microcat/__about__.py
 microcat/__init__.py
+microcat/chemistry_defs.json
 microcat/configer.py
 microcat/corer.py
 microcat/prepare.py
 microcat/rich_agrpase.py
 microcat/sample.py
 microcat.egg-info/PKG-INFO
 microcat.egg-info/SOURCES.txt
@@ -41,11 +42,12 @@
 microcat/scripts/kraken2mpa.py
 microcat/scripts/kraken2sc.py
 microcat/scripts/microcat_bam_handle.Rmd
 microcat/scripts/sample_denosing.R
 microcat/scripts/sckmer_unpaired.R
 microcat/scripts/spilt_bam_by_tag.py
 microcat/scripts/split_Starsolo_BAM_by_RG.py
+microcat/scripts/starsolo_tenX_auto.sh
 microcat/snakefiles/bulk_wf.smk
 microcat/snakefiles/scRNA_wf.smk
 microcat/snakefiles/scRNA_wf_test.smk
 microcat/snakefiles/spatial_wf.smk
```

### Comparing `microcat-0.2.0/setup.py` & `microcat-0.2.1/setup.py`

 * *Files identical despite different names*

