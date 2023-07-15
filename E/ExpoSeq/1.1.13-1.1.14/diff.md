# Comparing `tmp/ExpoSeq-1.1.13.tar.gz` & `tmp/ExpoSeq-1.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.13.tar", last modified: Mon Jul  3 08:58:54 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.14.tar", last modified: Sat Jul 15 09:48:25 2023, max compression
```

## Comparing `ExpoSeq-1.1.13.tar` & `ExpoSeq-1.1.14.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/
--rw-rw-rw-   0        0        0    11558 2023-06-30 13:21:19.000000 ExpoSeq-1.1.13/LICENSE
--rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.13/MANIFEST.in
--rw-rw-rw-   0        0        0     4107 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.13/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-07-03 08:58:26.000000 ExpoSeq-1.1.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.799871 ExpoSeq-1.1.13/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.840129 ExpoSeq-1.1.13/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.904496 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7915 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10619 2023-06-29 12:41:04.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6814 2023-07-02 11:44:34.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    17434 2023-06-29 12:43:18.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-06-12 12:16:56.000000 ExpoSeq-1.1.13/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    39758 2023-07-02 13:01:57.000000 ExpoSeq-1.1.13/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.960495 ExpoSeq-1.1.13/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-02 09:18:51.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3348 2023-07-02 13:14:31.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4284 2023-07-02 13:14:50.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-02 12:03:32.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1634 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1136 2023-07-02 13:24:34.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2542 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.984511 ExpoSeq-1.1.13/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      179 2023-07-02 13:29:17.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.992483 ExpoSeq-1.1.13/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.064646 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-06-16 09:43:27.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-06-16 09:43:29.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-06-16 09:43:29.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    87391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   210829 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    94420 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-06-12 12:05:40.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.121623 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.848402 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4107 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2971 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:25.462905 ExpoSeq-1.1.14/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     4134 2023-07-15 09:48:25.462905 ExpoSeq-1.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     3751 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 09:48:25.462905 ExpoSeq-1.1.14/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-07-15 09:43:45.000000 ExpoSeq-1.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:22.742137 ExpoSeq-1.1.14/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:22.976516 ExpoSeq-1.1.14/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:23.612617 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1007 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0     7915 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_cl.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6814 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    17750 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10311 2023-07-15 09:42:35.000000 ExpoSeq-1.1.14/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    40079 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.347021 ExpoSeq-1.1.14/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3292 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4284 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1136 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2542 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.518896 ExpoSeq-1.1.14/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1890 2023-07-15 09:42:35.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      179 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.550151 ExpoSeq-1.1.14/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.612645 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2634 2023-07-15 09:42:35.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:25.150394 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:25.416024 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:48:23.023384 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4134 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2971 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.13/LICENSE` & `ExpoSeq-1.1.14/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Nils Hofmann
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ExpoSeq-1.1.13/PKG-INFO` & `ExpoSeq-1.1.14/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.13
-Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
+Version: 1.1.14
+Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns.
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to ExpoSeq
 
-ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](expoSeq_overview.png)
+ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
 
 To get started, please download and follow the instructions for MiXCR under the following link: https://docs.milaboratories.com/mixcr/getting-started/installation/ 
 You can also only use the test version without installing it.
@@ -29,15 +29,15 @@
 If you want to use the fast and easy version you can ignore the rest of the instructions and just import in your Console:
 ```import ExpoSeq.run```
 ## Using the PlotManager
 
 The PlotManager is the main interface for creating various plots using your FASTQ data. You can create an instance of the PlotManager by running the following command:
 ```plot = PlotManager()```
 To use the PlotManager to create plots, you will need to upload your FASTQ data to the pipeline. This will automatically happen as soon as you have called the PlotManager. In the following you can obtain an insight in the worklow of the pipeline after the initial call. There, the blue boxes indicate your input, gray are optional inputs while black and red are processing steps and output, respectively.
-![relative_path_to_image](workflow_ExpoSeq.png)
+![relative_path_to_image](pictures_gen/workflow_ExpoSeq.png)
 If you just want to test the pipeline and see its functions you can call: ```plot = PlotManager(test_version = True)```
 
 Once you have called the test version or have finished the data processing, you can use the PlotManager to create a variety of plots, such as an identity plot based on the jaccard similarity. Here is an example of how to create this type of plot:
 ```plot.jaccard()```
 If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
 ```import matplotlib.pyplot as plt```
```

### Comparing `ExpoSeq-1.1.13/README.md` & `ExpoSeq-1.1.14/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Welcome to ExpoSeq
 
-ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](expoSeq_overview.png)
+ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
 
 To get started, please download and follow the instructions for MiXCR under the following link: https://docs.milaboratories.com/mixcr/getting-started/installation/ 
 You can also only use the test version without installing it.
@@ -17,15 +17,15 @@
 If you want to use the fast and easy version you can ignore the rest of the instructions and just import in your Console:
 ```import ExpoSeq.run```
 ## Using the PlotManager
 
 The PlotManager is the main interface for creating various plots using your FASTQ data. You can create an instance of the PlotManager by running the following command:
 ```plot = PlotManager()```
 To use the PlotManager to create plots, you will need to upload your FASTQ data to the pipeline. This will automatically happen as soon as you have called the PlotManager. In the following you can obtain an insight in the worklow of the pipeline after the initial call. There, the blue boxes indicate your input, gray are optional inputs while black and red are processing steps and output, respectively.
-![relative_path_to_image](workflow_ExpoSeq.png)
+![relative_path_to_image](pictures_gen/workflow_ExpoSeq.png)
 If you just want to test the pipeline and see its functions you can call: ```plot = PlotManager(test_version = True)```
 
 Once you have called the test version or have finished the data processing, you can use the PlotManager to create a variety of plots, such as an identity plot based on the jaccard similarity. Here is an example of how to create this type of plot:
 ```plot.jaccard()```
 If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
 ```import matplotlib.pyplot as plt```
```

### Comparing `ExpoSeq-1.1.13/setup.py` & `ExpoSeq-1.1.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.13",
-    description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
+    version = "1.1.14",
+    description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns.",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
     package_data={
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_cl.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             os.mkdir(os.path.join(module_dir, "my_experiments", experiment, "alignment_reports"))
 
     else:
 
         filenames = glob(os.path.join(pkg_path,"test_data","test_files", "*.fastq"))
         print(filenames)
         experiment = "test_directory"
+    
     settings_dir = os.path.join(pkg_path,
                                 "settings",
                                 "global_vars.txt")
     with open(settings_dir) as f:
         data = f.read()
     data = literal_eval(data)
     path_to_mixcr = data["mixcr_path"]
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from ExpoSeq.augment_data.mixcr_nils import process_mixcr
 from ast import literal_eval
 import os
 from ExpoSeq.augment_data.loop_collect_reports import load_mixed_files, load_alignment_reports
 import pandas as pd
 from glob import glob
 from ExpoSeq.augment_data.check_reports import check_completeness
-import sys
 import pickle
 import pkg_resources
 from ExpoSeq.augment_data.trimming import trimming
 try:
     import tkinter as tk
     from tkinter import filedialog
 except:
@@ -60,27 +59,25 @@
 def check_experiment(module_dir, testing):
     if not testing:
         while True:
             experiment = input("How do you want to call your new experiment?")
             if os.path.isdir(os.path.join(module_dir, "my_experiments", experiment)) == True:
                 replace = input("The given directory already exists. Do you want to replace it? (Y/n)")
                 if replace in ["Y", "y", "n", "N"]:
+                    if replace in ["Y", "y"]:
+                        shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
                     break
                 else:
                     print("Please enter another name.")
-                if replace in ["Y", "y"]:
-                    shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
-                    os.mkdir(os.path.join(module_dir, "my_experiments", experiment))
             else:
                 break
 
 
     else:
         experiment = get_random_string(10)
-   
     os.mkdir(os.path.join(module_dir,
                     "my_experiments",
                     experiment))
     return experiment
 
 def method_one(experiment, repo_path, module_dir, testing, paired_end_test = "n"):
     if repo_path == "":
@@ -234,15 +231,19 @@
                     pickle.dump(experiment_dic, f)
                 break
             else:
                 print("Sorry, but we could not find the column Experiment in your sequencing report. Please check if you have this")
         else:
             print("Sorry, but the filepath you entered is invalid.")
     all_alignment_reports = None
-
+    seq_report_dir = os.path.join(module_dir,
+                                  "my_experiments",
+                                  experiment,
+                                  "sequencing_report.csv")
+    sequencing_report.to_csv(seq_report_dir)
     return sequencing_report,all_alignment_reports, experiment
 
 def check_last_exp(pkg_path, module_dir, testing):
     if not testing:
         glob_vars = os.path.join(pkg_path,
                                 "settings",
                                 "global_vars.txt")
@@ -293,24 +294,29 @@
     else:
         experiment_name = get_random_string(10)
     return experiment_name 
 
 def upload_new_experiment(module_dir, repo_path, testing, testing_value, paired_end_test, experiment_column):
     experiment = check_experiment(module_dir, testing)
     choose_method = get_choose_method_input(testing, testing_value)
-   
-    if choose_method == "1":
-       
-        sequencing_report, all_alignment_reports = method_one(experiment, repo_path,module_dir,testing, paired_end_test )
-    elif choose_method == "2":
-        sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
-    elif choose_method == "3":
-        sequencing_report, all_alignment_reports, experiment = method_three(module_dir, experiment, testing)
-    else:
-        raise ValueError("Invalid option")
+    
+    while True:
+        if choose_method in ["1", "2", "3"]:
+            if choose_method == "1":
+            
+                sequencing_report, all_alignment_reports = method_one(experiment, repo_path,module_dir,testing, paired_end_test )
+            elif choose_method == "2":
+                sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
+            elif choose_method == "3":
+                sequencing_report, all_alignment_reports, experiment = method_three(module_dir, experiment, testing)
+            break
+        else:
+            print("Please enter a correct value.")
+
+        
 
     return sequencing_report, all_alignment_reports, experiment
 
 def choose_existing_experiment(module_dir, testing):
     if not testing:
         while True:
             user_input = get_experiment_name_input()
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/full_pipe.py` & `ExpoSeq-1.1.14/src/ExpoSeq/full_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 import pkg_resources
 from ast import literal_eval
 
 def run_pipeline(antigens = None, usq_multiple = "n", pass_interrupt = True, test = False):
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     save_settings_path = os.path.join(pkg_path,
-                 "settings",
+                                      "settings",
                  "save_settings.txt")
     with open(save_settings_path, "r") as f:
         save_settings = f.read()
     save_settings = literal_eval(save_settings)
     original_path = save_settings["fname"]
     if antigens == True or antigens == False or antigens == None:
         pass
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.14/src/ExpoSeq/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,24 @@
     def __init__(self, test_version = False, test_exp_num = 3, test_panrou_num = 1):
         self.is_test = test_version
         self.module_dir = os.path.abspath("")
         self.pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
         common_vars_path = os.path.join(self.pkg_path,
                                         "settings",
                                         "global_vars.txt")
+        if not os.path.isdir(os.path.join(self.module_dir, "my_experiments")):
+            print("create my_experiments directory")
+            os.mkdir(os.path.join(self.module_dir, "my_experiments"))
+        if not os.path.isdir(os.path.join(self.module_dir, "temp")):
+            print("create temp directory")
+            os.mkdir(os.path.join(self.module_dir, "temp"))
+            
         with open(common_vars_path, "r") as f:
             self.global_params = f.read()
         self.global_params = literal_eval(self.global_params)
-        print(self.global_params)
         if test_version == True:
             if os.path.isdir(os.path.join(self.module_dir, "my_experiments")):
                 pass
             else:
                 os.mkdir(os.path.join(self.module_dir, "my_experiments"))
             if os.path.isdir(os.path.join(self.module_dir, "temp")):
                 pass
@@ -141,15 +147,15 @@
         saveFig(name)
     def close(self):
         plt.close()
 
     def change_experiment_names(self, specific = None, change_whole_dic = False):
         """
         :param specific: optional parameter. You can use this function to change the names of a specific sample.
-        :param change_whole_dic: optional Parameter. In general the renaming is done be using a dictionary and map it to the labels. You can change the whole dictionary for ExpoSeq your original labels by adding the new dictionary for this parameter.
+        :param change_whole_dic: optional Parameter. The renaming can be done by using a dictionary and map it to the labels. You can change multiple or all labels by adding the new dictionary for this parameter.
         :return:You can use this function to change the name of your samples. Thus, you can change the labels of your plots.
         """
 
         if specific != None:
             assert type(specific) == str, "You have to give a string (inside: "") as input for the specific sample you want to change"
         if change_whole_dic != False:
             assert type(change_whole_dic) == dict, "You have to give a dictionary as input for the specific sample you want to change"
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/length_distribution.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import matplotlib.pyplot as plt
 
 def length_distribution_single(fig,ax, sequencing_report, sample, font_settings):
     batch = sequencing_report[sequencing_report["Experiment"] == sample]
     length = batch["aaSeqCDR3"].str.len()
     unique_length, counts_length = np.unique(np.array(length)
                                                 , return_counts = True)
-    max_length = np.max(unique_length)
-
     ax.bar(unique_length, counts_length)  # Or whatever you want in the subplot
     #ax.set_xticks(range(0, max_length + 1, 1), range(0, max_length + 1, 1))
     ax.title.set_text(sample)
     ax.title.set_size(10)
     ax.set_ylabel("Read Count",
                     **font_settings)  # Y label
     ax.set_xlabel('Read Length',
                 **font_settings)  # X label
 
     original_fontsize = font_settings["fontsize"]
     font_settings["fontsize"] = 22
-    plt.title("Length Distribution of " + sample, pad=12, **font_settings)
+    plt.title("Length Distribution of " + sample,
+              pad=12,
+              **font_settings)
     font_settings["fontsize"] = original_fontsize
 
 
 
 def length_distribution_multi(fig, sequencing_report, samples,num_cols, font_settings, test_version = False):
     if samples == "all":
         unique_experiments = sequencing_report["Experiment"].unique()
@@ -48,15 +48,14 @@
     n = 0
    # fig = plt.figure(1, constrained_layout=True)
     for experiment in unique_experiments:
         batch = sequencing_report[sequencing_report["Experiment"] == experiment]
         length = batch["aaSeqCDR3"].str.len()
         unique_length, counts_length = np.unique(np.array(length)
                                                  , return_counts = True)
-        max_length = np.max(unique_length)
             # add every single subplot to the figure with a for loop
         ax = fig.add_subplot(Rows, Cols, Position[n])
         ax.bar(unique_length, counts_length)  # Or whatever you want in the subplot
        # ax.set_xticks(range(0, max_length + 1, 1), range(0, max_length + 1, 1))
         ax.title.set_text(experiment)
         ax.title.set_size(10)
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/saveFig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os.path
 from matplotlib.pyplot import savefig
-
 from ast import literal_eval
-
 import pkg_resources
 try:
     import tkinter as tk
     from tkinter import filedialog
 except:
     pass
 
@@ -21,15 +19,15 @@
     if name == False:
         filename = input("how do you want to call the plot?")
     else:
         filename = name
     if save_settings["fname"] == "":
     #    print("Please choose a directory where you want to store your files")
         try:
-
+            print("Choose the directory where you want to save the file with the filechooser")
             save_dir = filedialog.askdirectory()
         except:
             while True:
                 save_dir = input("copy and paste the path to the directory where you want to save the files here.")
                 if os.path.isdir(os.path.abspath(save_dir)):
                     break
                 else:
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.14/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.14/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.14/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.14/src/ExpoSeq/settings/change_save_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     pass
 class Change_save_settings():
     def __init__(self):
         self.pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
 
         self.save_settings_path = os.path.join(self.pkg_path,
                                           "settings",
-                                        "save_settings.txt")
+                                               "save_settings.txt")
         with open(self.save_settings_path, "r") as f:
             save_settings = f.read()
         self.save_settings = literal_eval(save_settings)
     def change_dpi(self, dpi):
         self.save_settings["dpi"] = dpi
         with open(self.save_settings_path, "w") as f:
             f.write(str(self.save_settings))
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.14/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files 15% similar despite different names*

```diff
@@ -1,944 +1,1020 @@
-@A00604:387:HLC22DSX2:3:1101:5837:1297 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCGATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,:F,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:30373:1360 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTCATACACAGCCGTGTCCTCGGGAGGCACAGAGTTCAGCTGCAGGGCGAACTGGTTCTTGGAGGT
-+
-F:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFF:FFF,FFF:FFFFFFFFFF,:FFFFFFF,FFFFFF:FF:FFF,FF,:FF:F,,,FFF:,F,FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31376:1407 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCTTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FF:FFFFF:F:FFFFFFF:,F:FFF:FFFFFFFF:FFFF:FFFFF,FFFFFFFF,FF:F,FFFFFFFFFFF,FF,,,FFFFFFFFFFF,FF:FFFFFFFFF:FFF::::F:FF:FFFFF:FF,F,FFFFFFFF::F:FF::FF,FFFF,FF
-@A00604:387:HLC22DSX2:3:1101:4146:1438 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTTGCCCCAGTAGTCAAATAGTCCCCTAGCTCCCCACGATGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTGGGCTGTGTCTGTAGA
-+
-FF,:FFF:FFF,FFF:F:,FFFFF,FFF,FFFFFF:,,F::,,F,::FF,F,,F:FFFFF,FFFF:,F,FFF:F:F,FF,:,:,FFFF:FFF,::F,,,F::,FFFF,F,:F,F,FF,,F:F::FF,FFFF,FF,FFF:FF,:FF,,F::F
-@A00604:387:HLC22DSX2:3:1101:30798:1438 2:N:0:AGAGGAGG+GGACGACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATAGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-F,:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF,:F,FFFFFFFFFF::FFF,FFFFF,FFFF:,F:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFF:F,:FFFF
-@A00604:387:HLC22DSX2:3:1101:21368:1454 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCGGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFF:F,FF:,F,:F::FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31349:1454 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGATCAG
-+
-FFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:F:FFFFFFFFFF:FFFFF:FFFFFF,FFF:FF:FFF:FFFFFF,FFF:FFFFFFFF:FF:FFFFFFFFFFFFFFF,,FFF
-@A00604:387:HLC22DSX2:3:1101:32768:1532 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11442:1642 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:17300:1767 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFF:FFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:32371:1846 2:N:0:AGAGGAGG+GGACTACT
-TAAAGGTGTAACCAGAAGCCTTGCAGGAGACCTTCACTGAGGCCCCAGGCTTCTTCACCTCAGCCCCAGACTGCACCAGCTGAACCTGGGCCATGGCCGGCTGGGCCGCATAGAAAGGAACAACCAAAGGAATTGCGAATAATAATTTCTC
-+
-FFF,FFFFF,F:FFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:4246:1986 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFF:FF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:17345:2002 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:3830:2018 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF::FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FF,FFFFF
-@A00604:387:HLC22DSX2:3:1101:4408:2018 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:F,FFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:2139:2065 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF::FFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFF::FFFFFFF:FFFFFF,FFFFFFFFFFFFFFFF,FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:1615:2096 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCAGGCCCCAGTTGTGATAACCAGACAAAATCTCCCAAGTCGCGAAGGAGGCAGCGTAATACACCGCCGTGTCCTCAGATCACCGGCTGCACAGCTCCATGTAGGCTGTGTC
-+
-FF:FF:FFFFFFFFFFFF:FFFFFFFFFF:FFFFF:F,FFF,FFFFFF:F,:,FFF,FF,F,F,FFFF::,:F,,:,,,,,:F,,:F,,:F:,,F:,,:,FFF,:,FFF:,:F:FF,F,F,F,,:FFF,,FF,F,,:F::,,:F:F:F:,,
-@A00604:387:HLC22DSX2:3:1101:4444:2112 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACGCGAGAAGGTGACAAGGGATCCAAGGCCCCAGAAGTCAAAGTAGTATTTCTCGTAGCATCTACCACCACTACAATAACCCCCTCTAGCACAGTAATACACATCAGTGACCTCGGGAGTCACAGAGATCAGCTG
-+
-:F,F,:FF:,FFF,F,,,,,FF,F,:,FFFF,F:,:,FFF,,,FFF::,:,F,:F,FF,:,:,FF,:,FFF,F:FF,F,FF:FFFFF:F,:FFFFF,:F:,,F:,FFFF,F,FFF:FFF,F,,F:,FF::F,FF:F,FF,,FF,,:FFFFF
-@A00604:387:HLC22DSX2:3:1101:1967:2174 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:F::FFFFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFF:F::FFF:FFF:FF:FF
-@A00604:387:HLC22DSX2:3:1101:21368:2174 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFF:FFFFFFFFFFFFF:FF,:FFFFFFFFFFF,FF
-@A00604:387:HLC22DSX2:3:1101:19036:2206 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGATCCCCGATCCCCTGACGGGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTG
-+
-FFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFF,
-@A00604:387:HLC22DSX2:3:1101:32235:2237 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCGTACCGCCCTCATAGCAGCTGGTACTACTACAATATCCAACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:
-@A00604:387:HLC22DSX2:3:1101:31566:2456 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3712:2597 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:1985:2644 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFF,:FFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:29559:2644 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGGTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FF,FFFFFFFFFFFFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5791:2660 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACAGCAAAAGCACCGATGTCGTACCAGCCACTGCGATACCCGGCCTTGGGCTCCCTCGCACAGTCATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,F:FF:F,FFFFFFFFF,FF,FFFFFFFFFFFF,FFFF,FFF:FFFFF::F,F,FF:FFFFF,,FFF,FF:FFFFF,:F:F::FFFFF:FFFFFFFFFFF,F,:FFF,FFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1101:26060:2660 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:10782:2722 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGTCAAGCCACTGCCGAATCTGTTGCACAGTAATACACAGACGTGTCCTCGGGAGTCACAGAGTTCAGCTGAAGGGAGAACTGGTTCTTGGAGGT
-+
-F:FFFFF::,F,:FF,F,,FFF,F:,FFFFFFFFFF,FF,FF,,,F,FF,FFFFFFF:,F,FF,,FFF:,:,FFFF:,FF,FFF:FFFF:FFFFFF,,:F:FFFFFFF,FF:FFF:,F:FFF::F,F,:FFFF:FFFFF:FFF:::F:,FF
-@A00604:387:HLC22DSX2:3:1101:19759:2895 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTATAACTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:19388:2942 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTATAACTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28574:2973 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFF:FFFF:FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20564:3067 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGGCAGAGTTACCACCGTCCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGACTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32796:3145 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFFF:,FFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:19244:3255 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTATAACTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:19614:3270 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22128:3270 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:5231:3286 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGATG
-+
-FFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFF:FF,FFFF,FFF:FFFFFFFFFFFF:FFFFFFF:FF:FFFF,FFFFFFFF,FFFFFF:F:FFFFFFFFF,FFF,FFFFF:FFF,,FFFFFFFFFFFF:,:,FF
-@A00604:387:HLC22DSX2:3:1101:16875:3474 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:F:FFFFFFFFFFFFFFFFFF:FF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:25455:3521 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5050:3537 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:23402:3568 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF::FFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26946:3568 2:N:0:AGAGGAGG+GGACTACT
-CTGGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1101:15058:3615 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:17779:3693 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:29731:3693 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:8187:3740 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
-+
-FFFF:FFFFFFFF,FFFFFFFFFFFFF,FFFF:,FFFF:FFF,:::FFF:F,:FFF,FFFFFFFFFFF:FFF,F,F:F,,F:F:FFF,FF::FFFFFFFFFFFF,FFFFFF:FFFFFFFFFFF:FFFFFF:FFFF::FFF,,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:17680:4178 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F:FFFF:FFFFFFFFFF,FFFFFFFFFF,FFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFF:F:FFFFFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11803:4366 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFF:F:FFFFF:FFFF:FFFFFFFFFFFF,FF:FFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFF,:FFFFFFF:FFFFF,FFFFFFF:FFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20618:4413 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-F:F:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFFF::FFFFF:F:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:25292:4711 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-:FFF,F:FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF::FFF,:::FFFF:FFFFFFFFFFFFFFFF,FFFFFFF:FFFF,FF:FFFFFF:FFF:FFF:FFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9453:4930 2:N:0:AGAGGATG+GGACTACT
-CTGAAACGCATCCACCACTCGAGACGGTCACCAGGGATCCTTGGCCCCAGATATCAAAAGCATCAGTTGTTTTTAACCGAGAACAGTAATAAGAGGCAGAGTCCACACGGTCCATGTTGGACATTGTAAGGACCACCTGGCTTTTGGAGGT
-+
-FF,FF,F:F,F:FFF:F,FFF,FFF:,,,F,,F:,,,FFF,FF,F,FF:,F,FF,:FFFFFF,:,,,FFFFFFFF,FFF,:,,F:,,::,F,:,,F:,:,FFF:FF:,FF:FFFFFFF,,,F:,,F,F,:,FFFF,FF:FF:F,FF,FFF,
-@A00604:387:HLC22DSX2:3:1101:30906:5196 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26313:5228 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:27633:5228 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFF:FFFFFFFFFFFFF,:FFFF,F,FFFFFF::FFFFFFFFFFFFF:F,FFF:F,FFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:28537:5321 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGGGAGTTGGTAGCAGCTACCACCACTACAATAGCGCCAATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:11541:5384 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATCACCGACGTAGTCACCGTAGTCATCAGGATCTGATGGCGGGGCCAGTCTCGCACAGTAATACATAGCGGTGTCCGAGGCCTTCAGGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:25626:5447 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATAGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:F,FFFFFF:FFFFFFFFFFFFF,FFFFFFFFF:FFFF,FFFFF,F:FF:FFF:FFFFFFFFFFFFFFF,::FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5593:5478 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFF:FFFFFFFFFF,FFFFFFFFF,F:F:FFFF:FFFFF:FFF:FF:FFF:FFFFFF:FFFFFFFFFFFFFF,F::FFFFFFFFFFFFFFFF:FF:F,FFFFFFF:FFFF:FFFFFFFFFFF:FFFF::F:FFFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1101:19452:5494 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATACCCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFF:FFFFFFFFFFFFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1101:21495:5556 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-:FFFFFFFFF,FFFFF:FFFF:FFFFFF:FFFFFFFFFFFFF:FF::F,FFFFFFFFF:FFF:FFFFFF:F:F,F:FFFF,FFF,FFFFFF:FFF,FF:FFF:FF,,FFFFFFF:FFFFFFFFFFF,FFFFFFFFFF:F::FFFFF:FF:F
-@A00604:387:HLC22DSX2:3:1101:3287:5619 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF:,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16062:5666 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTCTAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFF:FFFFF:FF:FFFF:FFFF,FFFFFFFFFFFFFFF::FFFFFFFFFFFF,FFFFFF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18864:5666 2:N:0:AGAGGATG+GGACTACT
-ATGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGAAAAAGTACCAGCCACAGCTATATGCCCTGTCACCGGTAGAACAGTAATAAACCTCCGTGACCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-,FF:FFF,FF,:FFFF,FFF,:,F,F,FFF,:FF:,F,,FFF,,F,F,FFFF:,,FF,FF,F,F,F,FF,F,:F,F,FFFF,,F,,F,FF:,F,,F,,:F,,,,:F,,FF:F,,:FFFF,FFFFFF:FFFFF:FFFF::FFFFFFFF,F,:
-@A00604:387:HLC22DSX2:3:1101:31593:5697 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:2067:5791 2:N:0:AGAGGATG+GGACGACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTACTACACGGCCGTGTCCTCAGATCTCCGGCTGCTCAG
-+
-F:FFFFFF,,F:F:F,F:FF,FF,FFFFF:F,::,::FFF,:FF:FFF,F,F:FF,F:,:,,:FFF,,,F::,F:FFF,F,,,F:,F:FFF,FF,,FFF:F:F:F,FFFFFFFF,,F,FFF,FFFF:F,FFF:F,F,:::,FFF,::F,,,
-@A00604:387:HLC22DSX2:3:1101:15320:6042 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATCTCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTT
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF:FFFF:FFFF,FF:FFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFF::F,FFFFFFFFFFFFF:F,
-@A00604:387:HLC22DSX2:3:1101:8296:6277 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFF:FFF:FFF,F,FFFFFF:F,F,,FF:F:::F:FFFF:,F:,,FF,F:,FFF:FFF,FFF:,FF:FFFFFF:F:FFFFFFFFFF,F:FFF,:FF,FF::FFFF:F,FFFF:FF::FFF,:F,FFFF:FF,F,FF:FFFFFFF,:F:
-@A00604:387:HLC22DSX2:3:1101:30454:6324 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFF:FFFFF:FFFF,FFFFFFFFFFFFFFFFFFF:,FFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FF,FFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FF:F::FFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:10474:6511 2:N:0:AGAGGATG+GGACTACT
-CTGGACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFF,:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1101:2428:6543 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFF::F:FFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:::FFFFFFFFFFFFF:FFFFFFFF:FFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21034:6574 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTACACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGCTGTATGTTCCAAAGTAATACACGGCCGAGTCATCAGATCTCAGGCTGCTCAGCTCCAAGTAGGCTGTGTCTGTATA
-+
-FFFF:FF::,:,:F,,FFFF,FFFFF::FF,,FF,F,FFF:F:,FFFFF,FF,F:F,F,F,,,:,F:,,,FF:FFF,FFFFFF,,F,FF,F:FFFF,F:,FF,,:,,F:F:F:,F::F,:F:,FFF,F,,,F,,,F,,FFFFFFF:F,F:F
-@A00604:387:HLC22DSX2:3:1101:31638:6652 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCACCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFF:F,F,FFFFFFFFF:FFFFF,FF::FF:F:,FFFF,F,F,F:FFF:F,FFFFF:,FFF,FFFFF:FFF:,FFFFFFFFF:F:FFF:FF:F::FFFFFFF:F:,:,,FF,:F:FFFFFFFF,FF:FFFF:F:F,F:F:F,FFF:,
-@A00604:387:HLC22DSX2:3:1101:18629:6731 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGCCCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF,FFF,FF:F:,:,:F:F,FFFF::,FF,FFF,:::F:F:,,FFF,FFF:,,,:FFF::,,F,::F::FFFF,:F,F:FFFFF,FFFF,,,:::FF,:FFF,FFFFF,F,FFFFFFFFF,F,F:FFFF:,FFF:FFFF,FFFFF:FFF,F
-@A00604:387:HLC22DSX2:3:1101:10203:6762 2:N:0:AGAGGAGG+GGACTACT
-CGATGGGGACTGCCTGATCCAGATCCAAGCAGCACTGTTGCTAGAGACACTGTCCCCGGAGATGTCACAGGTGAGTGAGAGGGTCTGCGAGGGCTTCACCAGTCCTGGACCTGACTGCTGCAGCTGTACCTGGGCCATGGCCGGCTGGGCC
-+
-FFFF:FF,FF,:FFF:F,FFFF,,F:FFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFF,FF:,F,FFFF:,F:F::,F,,FFFF:FFFFFFF:FFF:FFFF,FFFFF:FF,F:FFFFFFF:FFFF,:FF:F:F:,FFFF:F:,,F,FFF,F
-@A00604:387:HLC22DSX2:3:1101:13250:6840 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22761:6840 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGGGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCACGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFF,FFFFF:FFFFFFFFFF:FFFFF,FFFF::FFF:,F,:FF:F::FFF:F:F::FF:FFF,FFF::F:FF:FF,FFFFFFF,:F,F,:,F:,F:FFFFFFFF:,FFFF:FF,FFFFFFFFFFFFF:F:F,F:,F:F,:FF:FFF,,FF
-@A00604:387:HLC22DSX2:3:1101:12554:7263 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:29071:7279 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:15266:7357 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATCCAG
-+
-FFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFF,FFFFFFFFFF,FFFFFFF,FFFFF:FFF,FFFF:FFFF:F:FFFFFFF,,F,FFFF:F,FFF:FFFFFFFFFF,::FF,F:::FF:F:,FF:FFFFFF:FFFFF,F,:,F
-@A00604:387:HLC22DSX2:3:1101:14452:7420 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF:FF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1101:1136:7498 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-F:FFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:F,FF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1101:15320:7513 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5394:7639 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:2953:7733 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAACTCCTCCTCTCGGCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTTATGGAGGTGTT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFF:F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,F:FFFFFF:FFFFFF,FF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22498:7764 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCTCAGTATTACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCCG
-+
-F:FFFFF:F:FFFFFFFFFFFF::FFFFFFFFFFF:FFF,FFFF:FFF:F,FFFF,FFFFFFFFFF::F:FFF:FFFFFF:FFF::FFFFFFFFFFFF:FFFF,:FFFF,FFFFFFFF:FFFFFF:FFFFFFFFF:,FFFFFFF:FFFF,:
-@A00604:387:HLC22DSX2:3:1101:23041:7764 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FF:F:,FFF::FFFFFF:FF
-@A00604:387:HLC22DSX2:3:1101:18096:7905 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATCTTGGGCCTCTCTTGCACAATAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGACAACTGGTTCTTGGATGTGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FF::FFFFFFFFFFFFF,:FFFF:FFFFFF:FFFF:F
-@A00604:387:HLC22DSX2:3:1101:22788:8234 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5430:8484 2:N:0:AGAGGATC+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATGTCTCGCACAGTAATACACGGCCGTGTCGTCCGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFF,FFFFFF,FFF::F,FF,:,:F,:FF:FFF:FFF:,F:FF:::FFFFFFF,FFFF:FFFFFF:::FF:FFFFF::,:F:FFFFFFFF,,F:,FFFFFF,FFFFFFF:,FFFF:FF,F:F,FF,FFFF:F::F,F,FF,FFFFF
-@A00604:387:HLC22DSX2:3:1101:22236:8719 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-F:FF:FF,F,F,FFFFF,,FFFF:FFFFFFFFFFFF::F,F:F:FF,FFF:FFF:F:,FFF:F:FFFFFFFFFFFFF:FFFFFFFFFFFFF,:FF,F:FFFF::FF:F:,F,FFFFFFF,F,F,:FFF:,,FFFF:,FFF,F:FF,,FFF,
-@A00604:387:HLC22DSX2:3:1101:20564:8797 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFF:,FFFF::FFF:FFFF:FFF:FFFFFFF:FFFFFFFFFF:FFFFFF,FFFF:FFF:FFFFFFFFFFFFF:FFF:FFFFFFFFFF,FFFF:,F,FFFFFFFFFFFF:FFFFFFFFFF:FF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:2239:9157 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTACTAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFF:,FFFFF:FFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:10682:9189 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FF,FF,FFFFFFFFFFFFFFFF:::FF:FFFFFFFFFFFFFFFFFF:FFFF:FFFF:FFFFFFFFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32027:9549 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:2555:9831 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFF::F:FFFFFFFF:FFFFFFFF,FFFF,FFFFFFF:::FF
-@A00604:387:HLC22DSX2:3:1101:25437:9846 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF:FFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:14073:10081 2:N:0:AGAGGATG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28682:10113 2:N:0:AGAGGATG+GGACTACA
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCATTGGCCCAAGTAGTCAAAGTAGTATTTCTAGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCGTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF:F,FFFFF,FFFFF:,FF:FFFF:FFFFF:F:,F:FFFF::FFF,:F::F:F,,FFF:FFF,FFF:,::FFFF,F,::FFFFFFFFFFF:FFFFFFFFF,,FF,F,F:FFFF,:FF:F,F,FFF,FF:,FFF:F,FFFFFF,F:FF,:
-@A00604:387:HLC22DSX2:3:1101:8865:10144 2:N:0:AGAGGATG+GGACTACT
-CTGAACCCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCCAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
-+
-FFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,:FFF:F:FF:FFFFFFFFFFFFFFFFFFFFF,:FFFFFF::FFF,FFF
-@A00604:387:HLC22DSX2:3:1101:19614:10222 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:10700:10379 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGGGAGTTGGTAGCAGCTACCACCACTACAATAGCGCCAATCTCTCGCACAGTAATACACAGCCGTGTCCTCGGGAGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31910:10629 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:25717:10770 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:7826:10817 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFF,F:FFFF:FFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:7157:10880 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFF,FF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:8467:10895 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF,FFFFFFFFF:FFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1101:20916:11005 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9200:11068 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF,F,FFFFFFFFFFF:FFF:FFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:13295:11083 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFFFFFFF:F:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:25120:11271 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9118:11365 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGAGGTAGCAGCTACCACCACTACACCTCAACTCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTTAGGCTGTTCAT
-+
-FFF:F:FFF:FFFF:,F::FFFF:FFFFFFF,FFFFFFFFFF:FFFFFFFFF:F:FFFF::FFFFF,FFFFF,FFFF:,FFFFFF,FFFFF,FFFFFFF,,FF:FFFFFF,FFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:27642:11443 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:1994:11772 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFF:FFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1101:17137:11788 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFF,F:FFF::F,FFFFFF,
-@A00604:387:HLC22DSX2:3:1101:21251:11898 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32886:11945 2:N:0:AGAGGATG+NGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATAACCGGCCTTGGGCTCCCTCGCACAGTACTACACGGCCGAGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFF:F,FFFFFFFFFFF,FFFF:FFFFFFF::FFFFFF:FFFFFFFFFFFFFFF,FF::FF:FF,,FFFFFF,FFFFFFF:FF,:FF,F,:FF:FFFFFFFFFFFF:FFF,F:F:F:FFFF,FFFFFFFF:F:FFFFFF:FFFFF:
-@A00604:387:HLC22DSX2:3:1101:23619:11960 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:23827:11976 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTAGAGACGGTGACCGTGTTCCCTTGCCCACAGTAGTCAAATTCCAAGTAATAACCACTACTATAAATGGCGCTTTTAGCACAGTAATATACGGCCGTGTCATCTGCTCTCATGATGTTAATATGCAGATACAG
-+
-FFFF:FF:F,,FFF:,FF,,FFF:FF:FFFF,FFF,F,,,,,,F:F,FFFFF:FFFFF,F:FFFFFFF,FFFFF:,:F,FFF,F,:,F:,FFF,,F,FF,,FFFFFFF,,,FF,FFFF,F:,FFFF,FF,,,F:,,,FF,F:,F::,FF:,
-@A00604:387:HLC22DSX2:3:1101:17020:12023 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGTTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGAGCTCTCGCACAGTAATACACGGCCGAGTCGTCAGATCTCAGGCTCCTCAGATC
-+
-FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFF,FFF,F,:F:FFFFFF,:,F:FFFFFFFFF,,FFFFFF:FFFF:FF,FFFFFF:,FFF,FFFF:F,FF,,F,:,FFFFFFF,,FF:F::F:,FFFF,FF
-@A00604:387:HLC22DSX2:3:1101:21847:12023 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:16523:12038 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGATTCCCAGCCACTGCTGTGTCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAACTGCAGGGAGAACTGGTTCTT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32687:12070 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTTGCCAGTCATGGGTGACACAGCCCCCTCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTAGGC
-+
-FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFF::FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:21685:12085 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:23167:12085 2:N:0:ACAGGATG+GGACTACA
-CTGAACCGCCACCACCACTCGAGACGGAGAACGTGCACCATAGCCACCATATAACAAAAGCATCACAGACGTAGTCACCCTAGTAATCAGCATCAGATGGCGTGACAAGACACGCACAGAAAAACATAGCTGTGTCAGATGCCAACAGGCT
-+
-FFFFFFF,FF:FFF,FF,FF,:,FF:F,F,,FFFF,,FF,F,,FF::FF,,FF,,FFF:FFF,FFF,F:F,FFFF,F,F,FFFF,F:,F::FFF,,::,:F,,F,F,,FFF:,FF:,F,,FF:,,FFF,F,FFFFF,FF,,FF,,FF:F:,
-@A00604:387:HLC22DSX2:3:1101:6922:12226 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:7383:12242 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF,FFFFFFFFFFFFFFFFFFF:,FFF,FFFFFFFFFFFFFF:,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18069:12242 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:19506:12383 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGCCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:1958:12399 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFF,:FFF,F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:14724:12461 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:F:FFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9046:12524 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:19931:12555 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFF:FF::FFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFF
-@A00604:387:HLC22DSX2:3:1101:8856:12602 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:9218:12602 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22182:12665 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22996:12665 2:N:0:AGAGGAGG+GGACTGCT
-TAAACAGCCTACACCAATCTAGACGGTTACCACGGTACCCTGGCCACAGTAGTCAACAAACCAGCCACTGCAATAGGCCCTGTAACCGCATGAACAGTAATAAACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAACTAGGATTTG
-+
-F,,FF,,,,F:,FF:,,FF,F,:,F,F,FF,F,,F:,FF::,,,,,FF,,:,F:,FF,,F,FF,,,F:F,F,FF:::F,F,,F,FFF,,F,,::F,:,FFFF,,:FF:FFFF,,FF:F,FFFF:FF,F,F,FFFFF:FFF:,FF:F:F,FF
-@A00604:387:HLC22DSX2:3:1101:29550:12743 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATAACCCGAAACATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFF:FFFFFFFFFFFFF,FFFFFFFF::FF,FFFF:,FFFFFFF::::FFFF,FFFF:::::,,FFF:F::F,FFFF:FFFF:FF,F:FFF,F:F:F,,FF,,F,,F,FFFFFF,,:F:::,FF,FFFFFFF,:FFF,FFF:F,F:
-@A00604:387:HLC22DSX2:3:1101:5810:12774 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:F:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:23475:12774 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACCCCATCAGATCTCTCGCACAGTAATACCCGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCCTGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF,FFFF:FFFFFFFFFFFFF:FFFFFF:,FF:FF:,FF,FFFF,F:FF:,,FFF:,F:F,,F,F:,FFFFFF,FF,::F:F:,FF:FFFFF,FFF:F:FFF,,FF,FF,:F:
-@A00604:387:HLC22DSX2:3:1101:20374:12853 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24740:12868 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATCCACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:6099:12900 2:N:0:AGAGGATG+GGACTACT
-CTGAAACGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACAAACAGAACTCTCGCACAGTAATACACGGCCGTGACGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFF,,:FFFFFFF,F,FF:FFFF,FFFFFFFFF,FF:F,FFFF:F:FFFFFFF::F:FF:FFFFFFFFFFFFFFFFF,F,FF,F,F:FFFF,FF,FFFF:FFFFFF:FF:F,FFFFFF::,FF::FFFFFFFF::F,,F:F,:F,FFFF
-@A00604:387:HLC22DSX2:3:1101:25563:12915 2:N:0:AGAGGATG+GGACTACT
-AACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FF
-@A00604:387:HLC22DSX2:3:1101:12635:12947 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATAAATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCATCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFF:FFFFFFFF,F:FFF,::,FFFFF,FFFFFFFFF:FFF,FF,F,:FFF::FF:FFFFFF:FFFF::FFFFF:F,FF:,F:F::FFF:FFFFFFFF,FFFF:F,FF:FFF,F,F,:F:F,F:F,FFFF:FF,F:,FFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:14787:13009 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26196:13009 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:,:F,FFFF,FFFFFFFFFF::FFF:F,FFFF:::FF:FFFFF::FFFF:F,FFFF,FF:FFF:F,FFFFF,FF,FFFFFFFFF,FFFFFFFF,,FFFF:,FFF
-@A00604:387:HLC22DSX2:3:1101:28438:13009 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF,FF,,F,FF:,FFFFF:FFF,FFFFFFFFFFF::FFFF:F:FFF:,FFFF,FFFFFF::F,FFFF,FFF:FFFFFF:::FFF,FFF:F:F,F,:,,:::F,FFFFFFF:FFFFFFFF,::FF:,FFFFFFFFFFF:FFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:17861:13166 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:8232:13307 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:F:FFFF
-@A00604:387:HLC22DSX2:3:1101:27570:13322 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFF,FFFFFFFFFFFFFFFF::FFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF,FFFFF:FFFF,F:FF,FFFFF:F:F:FFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28845:13463 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21423:13542 2:N:0:AGAGGATG+GGCCTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTCGCAGCTACCACCACTCCAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFF,FF,FFFF:,F:FFFFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFF:FFF:
-@A00604:387:HLC22DSX2:3:1101:32235:13542 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCTATATTACAATAATACCCCCACTCTCTCTCACAGTAATAAACGGCCGTGTACTCAGA
-+
-F:FFFFFFFF,FFFFFFFF,FFFFF:FF,FFFFFFFFFFF,F,FFFFFF:F,:FFFF,FF:F:F,,FFFF,FF:,:,,F,FFFFF:FF,FFF::,,,F,,FF:FFFF,F,,,,F,,,FFFFF,FF,,F,,F:F:FF,,F,,,,,,F,:::F
-@A00604:387:HLC22DSX2:3:1101:31512:13573 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24659:13604 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCATGTCCCGCCCCACCACTCCAAAAATCCCCTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3784:13683 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:27245:13730 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FFFFFFFFFFFFFF:FFFF:FFFFFFFFFFF:FFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3676:14278 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:1561:14591 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:
-@A00604:387:HLC22DSX2:3:1101:20365:14591 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTCTCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF,FFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FF:FF,FF,FFFFFFFFFFFF:FFFFF,,FFFFF::FFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1101:7808:14732 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:6379:14763 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:F:FFFFFF:F,F,FFF:F:FFF:FFFF,FFFFFFFFFFFFFFFFF,F::FFFFF:FFF:FFF
-@A00604:387:HLC22DSX2:3:1101:9381:14763 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1101:8169:14794 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCATCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCATCCCCTGCTATACCAGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCGCAGATCTCAGGCTGCTCAG
-+
-::::FFF,F,FF,F:F,F,,:FFFF,,F:FF,FF:,FFF::F::,FFFF:FF:FFF,FFFFFFF,,FFFF:FFFFF,,,,,FFFFF:FFF,FF:F:F:,F:FFF,F,:FFFF,FFFFFF:FFFFFFF,,F,,F,:FFFFFFF:FFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:1823:14888 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FF:FFFFFFFFFFFFF:F:FFFFFFFFFFFFF:,FF:FFFFFFFFFFFFFF::FFF:FF,FFFFFF:FFF::FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,F,F:F:FFF,FFFFFFFFFFFFFFFF,FFF:FFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:5330:14888 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCGATACCCGGCCTTGGGCTCCCTCGCACAGTCATACACGGCCGTGTCCTCAGCTCTCAGGCTGCTCAG
-+
-FF:FFFF,FF:,F,FFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFF,FFF,FFFFFFFFF:F:FFF,FF::F:FF,FF:,:F:,FFFFFFFF,,,:FFFFFF:FFF:FFFFFF,FFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:19886:15013 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F:
-@A00604:387:HLC22DSX2:3:1101:32271:15076 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFF::,:FF,FFFFFF
-@A00604:387:HLC22DSX2:3:1101:27543:15092 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF,FFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF:,FFFFFFFFF,,F:FFFFFF:FF:FFF:FF,FFFFF:FFFF:F:FFFF:FFFFFF::FFFFFFF:FFF::FFFFFFFFFFF::FFF:FFF,FFFFFF,FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5746:15139 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFF,FFFFFFFFFFF:,FF
-@A00604:387:HLC22DSX2:3:1101:12210:15217 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFF::FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32868:15233 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF:FFFFF,FFFFF:F:F:FFFFFFF,FFF:F:FFF:FF:FFFFFFF,F::FFFF:,FF:,F,F:FFF,FFFFF:FF:,FFF,FF:F:F,FF
-@A00604:387:HLC22DSX2:3:1101:7771:15264 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFF:,FFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFF,FFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11243:15421 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF:FFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFF:,FFFFFFFFFFF,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3992:15702 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF,FFFFFFFFFFFFFFFFFF:FF:FFFFFFF:F:FFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFF,FF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFF,F,,FFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3920:15734 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCCCAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF:FFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFF:FFFFF:FF:FFF:FFFFFFFFF:,FF,FFFFFFFFFFFFFF,FFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:10809:15734 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFF:FFFFFFFF,FFFFFFFFFFFF::::FFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:32045:15843 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FF:FFF,FFFFFFFF:F:FFF,FFF
-@A00604:387:HLC22DSX2:3:1101:28221:16047 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:28890:16172 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFF:FFF:F::FFF
-@A00604:387:HLC22DSX2:3:1101:6171:16188 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCCCTCGAGACGGTGACCATTGTCCCTTGGCACCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-F,:F:FF:F,:F,,,F,,F:F,F,FF,FFFFFF,F:FFFFFFFFF,F:F,F:FFFFF::FFF,FFFFF:FFFF:FFFFFFF,:F,F::F:F:FF::FFFFF:FFF:FFF,FFFFF,F:,FFF:FF,F::FF,FFFFFFFF,FF:FF,FF:F
-@A00604:387:HLC22DSX2:3:1101:18204:16329 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATGTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18358:16438 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFF::FFFFF,FFF:F:FFFFF:FFFFF:FFFFFFFFFFF:F:FFFFFFFFFFFFFF:::FF,FFFFFFFFFF:FFFFFFFF:F:FFFFFFFF:FFFF:FFFFFFFFFFFFFFFF:F,:FFFFF:FFFFFFFFFFFFF::FFFF:
-@A00604:387:HLC22DSX2:3:1101:15230:16564 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-F:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28393:16752 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGACTCCACCACTCGAGACGGTCACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCAATCTCCGCATCCCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGT
-+
-F,,FF,F:,F,:FFFFFF,F,FFF,,:F,FFF,,FF:F,::F:FFF,:FFF:FFFFFFF,FFFF:F,F:,F,FF:FFF:F:F,FFF,F::::::FFFFFF,FFFFF,,:FFFFFFFF:FFFFFFFF,:FFFFFF,FF::,,FFFF,,,FFF
-@A00604:387:HLC22DSX2:3:1101:3540:16830 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1101:6596:16892 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:4878:16955 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFF:F:FFFF:FFFFFFFFFF:FFFFF:FFFFFF:F,FFFFFFFFFFFFF:FFFFFFFFFFFF,FF,,F,FFFFFFFFFFF:FFF,F,FFFFFFFFFFFF:FF::FFF:FFFFFFFF::FFFFFFF:FFF:FFF:FFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:21884:17002 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11840:17018 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF,FF:FFFFF:FFF,FFFFFFFFFFFFFF,,F:FFF,,:FFFFFFFF:FFFFFFFFF:FFF:F,FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18837:17049 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,:FFFFFFFFF,FFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1101:27959:17190 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1101:4345:17253 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFF:F,FFFF:F:
-@A00604:387:HLC22DSX2:3:1101:20998:17284 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26567:17315 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:27724:17409 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:28429:17440 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20302:17550 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFF:F:FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFF:FF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FF,FFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFF,:FFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:14651:17785 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:8449:17816 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTACCACCCCCGGGATCCATCTCGTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFF::FFFFFFFFFFF:FFFFFF,,FFFF:FF:FFFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:23909:17816 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTTGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGAGTCCTCAGAACTCAGGCAGCTCAG
-+
-F,,FFFF:FFFFFFFFFF,FFF,FFF:,:FFFF,:F,F::,,,FFF,FF:FF,:,F,,F,FFFF,,,:,F,F:FFFFF::F,FFFF,:F,FFFFF,::,FF:FF::F,FF:::F,FFFF,,F,FF,,F:,FFF::F,F,FFF,,,,:FFFF
-@A00604:387:HLC22DSX2:3:1101:11885:17848 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22887:17926 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11478:17957 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACCGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,F,FF,FFFF,FFFFFFFFFFFFFFFFFFFF,FFFFF::FFFFFF
-@A00604:387:HLC22DSX2:3:1101:29514:18004 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFF:FFF::FFFF,:FFFFFFFFFFFF:FFFF,F:FFFFFFFF:FFFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1101:28375:18129 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGAACGGACGAATCCCGTGTCTGGTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCTGAT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:30933:18176 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:8793:18255 2:N:0:AGAGGATT+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:25491:18302 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACCAAAATCGTTGACAGATCTCTCGCACAGTACTACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FFFFFFF:FFF:F,FFFFFF,F:FF,F:F:F:F:FFFF,:F,FFF,:F,,,FFF:,FFFFFFFFFFFF,F:FFFFF,FFFF:FF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26142:18458 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFF,FFFFFFFFFF:FFF::FFFFFFFF:FFFFFFFFFFF:F:FFFFFFFFFFFFFFF:FFFFFF:FF,FFFFFFFFFFFF:FFFFF:FFFFF:FFFFF,FF,FF
-@A00604:387:HLC22DSX2:3:1101:12355:18474 2:N:0:AGAGGATG+GGACTACT
-CAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTCTGCCCTGGAACTTCTGTGCATAGTTTGTGCCACCACTGTTAGGGTTGATCCATCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGCACC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28501:18568 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFF:FFFFFF:FFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24532:18677 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFF:FFFFFFFFFFFFF,FFFF,FFFFF::FFFFFFFF:FFFFF:FF:FFFFFFF:FF:F:F,FFF,:FFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFF,FFFFFFFF:FFF:FFF:FFFF:FFFFFFF:FF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:10411:19022 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FF,F:FFFFFFFFFFFFF:FFFFFF,FFF,FFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:11731:19147 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1101:27163:19225 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:30355:19304 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:13286:19429 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF:FFFFFFFFFFFFF,FFFFFF:FFFFFFF,F,FFFFFFFFFFFF:FFFFFF,FFFF,FFFFFFFFFF::FFFFFF:FFFFF:F,FFFFFFF,FFF:FFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFF:FFF,F:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:4553:19836 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF::FFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:F:FFFFFFFFFFFF:FFF:FFFFFFF,,FFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:8133:19867 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF:FFFF
-@A00604:387:HLC22DSX2:3:1101:16993:19993 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGACGTCCATACCGTAGTAGTAGTCTAAGGTAGAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:12825:20071 2:N:0:AGAGGATG+GGAATACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFF,FFFFFFFFFFFFF,:FFFFFFFFF,F:FFFF:,:FFFFFF:FFFFFFFFFFFFF::FFFFFFF,FFFFFFFFF:FFFFFFF:FFFF:FFFFFFFFFF::FFF:FFFFFF,FFFFFFF,:FFFFFFFFFFFFFFF:FF::FF,
-@A00604:387:HLC22DSX2:3:1101:23556:20212 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:15320:20290 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCA
-+
-FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:21404:20337 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGACTCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-:F:FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFF::FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF,F:FFFFFFFFFF,FFFFFFFFF:F,FFFFFF,F,FFFFF,FFF,FFFFFFFFF:FFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:8712:20494 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18005:20494 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGATATCAAAAGCATCGGTGTCATCCCCTTTATAATAACCACTCCAAATATCGTAATACGTTCGAAGCGGGCCACTCGCACAGTAATACACGGCCGTGTCGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,::FFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFF:F,FFF:FFFFFFFFFFFFFF:FF:FFFFFF,F:FFF:FFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5077:20525 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFF,FFFFFF:FFF,F:FFF:FFFFF:F,FFFFFF:FF:FFFFFFF:FF:F,F,FFFF:FF::FFFFF:F:F:F,FFF,FF,F:FF
-@A00604:387:HLC22DSX2:3:1101:12563:20525 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
-+
-:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,:FFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF::FFFFFFFFFFFFF,FF:FF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26133:20603 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22724:20838 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGAGGTAGCAGCTACCACCACTACACCTCAACTCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTTAGGCTGTTCAT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20139:20901 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF:::FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9362:20964 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCCCAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGAGGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF:FFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FF,FF,F:,FFF,F:,:FFF,FF:FFFF,FF
-@A00604:387:HLC22DSX2:3:1101:28103:20979 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FFFFFF:F:FFFF:F:FFFF:FFF,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32262:21010 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:5059:31391 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFF::FF:F:,FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13006:31532 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FF::FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:22923:31641 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGATATCAAAAGCATGGGGCCCGGAGTAGCAGCTACCACCACTGCAATATGCGGCTCGCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCCCCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:20528:31688 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFF::F:FFFFFFFF:FFFFFFFFFFFFFFFFF:FFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFF:FF,F,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7383:31751 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:19045:31876 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6922:31892 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATCCGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
++
+FFFFFFFF:FFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFF:FFFFFFFFFFFFFFFFF:F:FFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFF:F,FF:FFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13422:31939 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF:FFFF:FFF,FF:FFFFFFFFF:FFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:20211:32236 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF::FFFFFFFFFFFFFFFFFFFFFF:FF::FFFF,FFFFFFFFFF:FFF:FFFFFFFFFFFFFFF,FFFFFFFF,FFFFFF,FFFF::FFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:20229:32236 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFF:FFF:FFFFFFFFFF:FFFF:FF:FFFFF,FFFFFF:FFFF,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10221:32409 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:14136:32424 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11053:32440 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:,FFFFF::FFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:21124:32565 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTCATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFF,FFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FF:FFFFFFFFFFFFFFF,FFFF:F,FFFF,FFF,FFFF:FFFF:F:FFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:29017:32737 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCACCTAACGGTATCATAGTAGACCCTCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11062:32831 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF,F:FFFF:FFFFF,FFFFFFF:FFFFF:F,FFFFFFFFFF:FFFFFFFFF:FF:FFFFFF:F,F:,FFFFF,FFFFFFFF,FFF:FFFFF:F:F,,:FFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:29686:32831 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACCGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:31006:33051 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:F:FF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:5385:33113 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFF:FFFF:FF:FF:,,:FFF:F,FFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:18828:33160 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF:FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:10601:33223 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+F:FFFFFFFFFFFFFF,FFFFF:FFFFFFFFFF::FFFFFFFFFFFFFFFF:,FF,,FFFFFFFFFF:FF:FFFFFFFFFFFFF,FFF:FFFFFFFFFF:FFFFFFFFFFFFF:FFFFFF::FFFFFF:FFFFFF:FFFFFFF:,FF:FF:
+@A00604:387:HLC22DSX2:3:1102:15058:33270 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:4435:33317 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCCGACGTCCATGTAGTAGTAGTAGTTCCTCTGATAGTCTGTCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFF:FF,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13295:33348 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFF,FFFFFFFFFFFF,FFF:F,:F:FFFFF:FFFF,FF
+@A00604:387:HLC22DSX2:3:1102:4490:33473 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATGTAGTAGTAGTAGTTCCTCTGATAGTCTGTCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTAAGGCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFF:FFFF:FFFFFFFF:F,FFF:,FFFFFF:FFFFFFFFF:FFFFFFF,FF,F:F,:FF:FFFFFFFFFFF,F,,FFF:FFFFFF,FFFFF:FFFFFF:FFFFFFFFF,:FFFFFFF,,F:,FF:FFFF,:FFFFFFF,::,
+@A00604:387:HLC22DSX2:3:1102:29215:33583 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:3848:33646 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATGTAGTAGTAGTAGTTCCTCTGATAGTCTGTCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:15447:33661 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGAACGGACGAATCCCGTGTCTGGTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCTGAT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1102:3956:33739 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGAAATACCAGCCACTGCTATAGACGTTAACATTCGACGTAAGATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFF:F,FFF:FF,FFFFFFFFFFFFFFFFFF:FFFFFFF:FFFF:FFFFFFFFFFF:FFF:FFFFF,FF
+@A00604:387:HLC22DSX2:3:1102:13141:33833 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGACGTCCATACCGTAGTAGTTGGGTTCCCGCCATGCTAAATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:23511:34194 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FF:FFFF
+@A00604:387:HLC22DSX2:3:1102:9995:34240 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCCGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+,FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFF,FFFFFFFFFF,FFFFFFFFF:FFFFFFFF:,FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFF,FF,FFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:29812:34303 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:F:FFFFF:FFFF:F::FFFFFFFF:,FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFF,FFFFFF:,FF
+@A00604:387:HLC22DSX2:3:1102:14163:34350 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,:FFFFFFFFFF,FFFFFF:FFFFFFFF,FFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF,FF
+@A00604:387:HLC22DSX2:3:1102:14190:34397 2:N:0:AGAGGATG+GGAATACT
+CTCAACCGACTCAACCACTAGAGACGGTGACCAGGCTGCCCTGGACCCAGTAGTCCAAGTAGTATTTCTAGTAGCAGCTACCACCACTACAATAAACCCCTCTTGCACAGTCATACACAGCCGAGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FF,:F:FF,:,:,:,,FF,,,,,FF,FF,F::,:,,FFFFF:,,,F,FFFFFFF:::,FFFFF,,FFFF,FFFFFF,:,:FFFF,,FFFFFFFF:,:,,F,:,F,FFFFFF,FFFFFFF,FFF,,:FFF::,FFFFFFFFF:FFFFFFF::
+@A00604:387:HLC22DSX2:3:1102:21016:34413 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFF:FF:FFF:FFFFFFF:,F:FFF,FFF
+@A00604:387:HLC22DSX2:3:1102:8495:34460 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF:FFFFFFFF,FFFFFFFFF:FFF:F:FFFFFFFFFFFFFFFFFFFF::F,F,FFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:25238:34554 2:N:0:GGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCATCGTACCAGCCACTGCTATACGCCCGGCCCGCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTAGGCTGT
++
+FFFF:FFFFFFF:FFFFF:FFFFFFFFFFFFF:FFFFF:FFFFFFFFF,F,FFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFF:F:::F,F:FFFF:FFFFFFFF::FFFF:F,FFFFFFFFFFF,F:FFFF,FFFFFFFFFFFFFFF,F:
+@A00604:387:HLC22DSX2:3:1102:20139:34616 2:N:0:AGAGGATG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCA
++
+F:,FFFFFF:FFFF,FFFFFFFFFF::FFFF:FF::FFFFF:FFFFFFFF:,FFFFFFF::FFFFFF,FFFFFFFFFFFF,FFFF:FF,FFFFFFFFF,FFFF:,FFFFFFFF:FF:::FFFFFFF:FFFFFF,F,,FFFFFFF,::FFF:
+@A00604:387:HLC22DSX2:3:1102:27552:34648 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFF,FFFFFFFFFFFF,F,FF:FFFFFFFFFFFFFFFF,F:FFFFFFFFFFF:FFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:14380:34788 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCTCCATCTCTCGCACAGTAATCCACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFF,FFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF:FFFF:FFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12581:34804 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:2184:35086 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFF,F::FFFFF:F:FFFFFF,F,FF,:FF,FF:FF:F:FF::FFF:FFFFFFFFFFFF,F::FF:FFFF,F,F,FFFFF,FF,,FF,FFFF:FFFFF:FFF:F,F::FFFFFF:FFFF,FFFF:FF:FFFFF:F:FFFFFFF:
+@A00604:387:HLC22DSX2:3:1102:12735:35133 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,F,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10728:35227 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFF:FF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF,FFFFF,FFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:6686:35274 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FF:FFFFFFFFF:FFFFFFFF:FFFFFFF:FFF,FF:FF,FFF:F,F:FFFFFFFFFFF:FFFFFF,F:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:32145:35493 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACAGATGTCGTACCAGCCACAGCTATACCCGGCCTAGGGCTCCCTCGCACAGTAATACACGGCCCTGTCATCAGATCTCAGGCTGCTCAG
++
+,FFFF::::::,FF::F:,:,FFF:,:F,FF:F:F,,FF,F::,F::FF:F,F,:FFFF,FF,,,F,,FFF,F:,,,,,F,,,,:F,FF,::::F,,:F::,F,F:F:F:FFF:FFFFFFF,,FF,:,,F,,FF:FFFF::F,:,F,:,F:
+@A00604:387:HLC22DSX2:3:1102:12255:35524 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAGAGTGGTCCCCACTACTATCATAGTAGAGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFF:FFFFFFFF:FFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27091:35571 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF::FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:2600:35587 2:N:0:AGAGGATG+GGACAACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,F:::FFFFFF:FFF,FFFFFFFFFFFF:F:FF,:FFFFFFFF,FFFFFF:FFFFFFF:F,FFFF:FFFFFF,F:FFFFFFF:FFFFFFFFFFFFF,FFFF:
+@A00604:387:HLC22DSX2:3:1102:11966:35650 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFF:,FFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FF:,FFFF,FFFFFFFFFFFFFFFF:FFFFFF:F:FF,FFFFFFFF::FFFFF::FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9164:35681 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FF:FFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27453:35759 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:25220:35837 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTACTTCCCCGTAGTGTACCAGCTGCTGCTCCATTCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFF:FFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF,F:F:FFFFFFFFFFFFFFFFFFF:FFFFF:F,FFFFF:FFFFFFFF,FFFF:FFFFFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11822:35869 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTACCTTGGCCCCAGAAGTCAAACCCCCCAATTGTATATAATACAACACCAGAACAATAAATCACTGTTGCACAGACATACACGTCCGACTCAGCATCGCTCAGGATCCTCAGCTC
++
+F:FFFFF:FFFFFFFF:F:FFF:FF:F,:FFFF,,,,,FFFFF:FFFFFF,F,FF,F,F,F:,,,F,,,,:,,,,,FFF:,FFFF,,,FF,F::,,F:,:,,F:::F,F,::,F:F,,F,FF:,,F,,,:,,,,FFFF:,,,,,,FF,:,:
+@A00604:387:HLC22DSX2:3:1102:27670:35978 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGCGACTCACTGCACCCCCGTAGTTCCAGTTATCGGGTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:28492:35994 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:32551:36010 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7527:36041 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATAAACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FF:FFFF,FFFFFFFFFF:FFF,FFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF:FF,FF,:FFFFF,FFFFF,FFFFFFFFFF,F:FFFF,FFFFFF,F:FF:FFFF,FFFF:,FFFFFFFFFFFF:FFFFF:,FFFF
+@A00604:387:HLC22DSX2:3:1102:17327:36041 2:N:0:AGAGGATG+GGACTACT
+TCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTCCGCGGTAATCGTGACTCTGCCCTGGAACTTCTGTGCGTAGTTTGCTGTACCAAAGATAGGGATGATCCCTCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9100:36072 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFF:FF,FFF:FF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:32624:36198 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FF:FF:FFFFFFFF,FFF:FFFFF:FFFFFFF:FF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1814:36292 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFF:FF:FFFFFFFFF:FF,:FFF:,F:FFFF,FF
+@A00604:387:HLC22DSX2:3:1102:3902:36558 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFF::FF:FFFFFFFFF,FFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:11379:36573 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:F:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFF,FFFFFFFFFF:FFFFF:FFFF,FFFFFFFF,FFFFF:,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FF,FFFFFFFFF:FFFFFFF:FF:FFFFFF,FFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:14271:36573 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFF:FF:FFFF:FFFF:FF:FFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:3188:36605 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:8585:36620 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:9073:36652 2:N:0:AGAGGAAG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACAAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FF:FF:FFFFFFF,FF,FFFFFFF:F:FFFF,FF,FFFFFFFF,FFFF,FF,:FFFF:FFFFFF:F,F,FF:FF,::FFFFF,:FF,FFFF,FFF,FF,:FFFF,F:,FFFFF:F,::F:FFF,FFFFFFFFFFF,,,:FFFFFF,FFFF:
+@A00604:387:HLC22DSX2:3:1102:5710:36839 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGACAAACGCGTAGTCACCGTAGTCACTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGT
++
+FFFFFF:FFF:FF:FFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFF:FFFFFFF:FF,FFFFFFFFFFFFFFFFFF::FFFF,F:FFF,:FFFFFFFF:FFF:F:FFFFFFF,FF:FFFFF:FFF,FFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6479:36855 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:12319:37012 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1103:12138:1031 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFF,FFFF,F,F,FFFF,FFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:12780:1141 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:19325:1172 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:17698:1204 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCACCTGCTATAGGCCCTGTACCCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCATCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:F:,F:F,FF,F:FFFFFFFFFFFFF,,FF:FFF,F,,F,:,,,F,FFFF,FFFF:,FFFFFFFFF,:,FF,:FF,:FFFF:F:FFF,FF:,F,,,FFFF:FFFFFF:,F,
+@A00604:387:HLC22DSX2:3:1103:32533:1501 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+F:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF::F:FFFF:FFF:F::FFFFFFFFFF:::FFF,F:FFFFFF:F,F:FF,,FFFF,FFF::,FFFFFFFFFFF:FFFFFFFFFFF:FF:FFFFFFFFF,FFFFFFFFFF:F:,FFFF
+@A00604:387:HLC22DSX2:3:1103:26802:1595 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCAACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCCTGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF,F,FFFFFF,FFFFFFFFFF:FFF,F:FFFFF:FFFFFF:F:FFFF:FFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:27968:1830 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCACTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCATGCTGCTCAG
++
+FF::F,:F,,FFFFF:FF,F,F:FFF::F,F,FFFF:F,FF,:F,FF:FFFFFF:FFF:FFF,FFF,,FF,::FFF,:FF,F:FFFFFFFF:FFFFFF::FF:FFFFFFF,:FFFFFF,,FF,:FFFFFFFFFFFFFFFFF,FFF,FF,FF
+@A00604:387:HLC22DSX2:3:1103:18656:1861 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCAACACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1103:15266:1877 2:N:0:AGAGGATG+GGACTCCT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFF:FFFFFFF:FFFFF:F:FFFFFFF,FFFFF:FF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFF:FFFFFFF:F:FFFFFF:FF:FFF
+@A00604:387:HLC22DSX2:3:1103:1344:1939 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCCCCCACGTGGATGTCTCCATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTT
++
+F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFF,F:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF:F:FF,FFFFFFFFFFFFF:FFFFFFFFF:FFFF:FFF,,,
+@A00604:387:HLC22DSX2:3:1103:9082:1939 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTGCTGGAAGTATTCACCAGATTCGTACCAGCCACCACTGTGTGCACAGTAATATGTGGCTGTGTCTACAGGGTCCATGTTGGTCATTGTAAGGACCACCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:F:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F,FFFFF:FFFFFFFFFFFFFFFFFFF:,FFF,:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:26205:1971 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTACGGGGGCGTAGTTACTGTCAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,F,FFF:FFFFFFFF,F,FFFFF:F:F:FFFF:FFF:FFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:11541:2002 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTACCTGGCCCCAGTAGACAACGTAACAGACACATCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCACAGATCTCAGGCTGCTCACCTCCATTTAGTCTGT
++
+FF,FFFF,::,FFFFF,F,,,FFFFF,:F:FFF,,FF,,FFF,,FF,,:,FF,,:FF,F,F,:F,,FF:,,FFFFF,F,F,,,FFFF:,:F,,:F::F:::FF:F,,,F,FF,,F,,FF,F,FFFF,,,F,FFFF,FFFFFF,:F,,FF,:
+@A00604:387:HLC22DSX2:3:1103:15772:2096 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FF:FFFF:F
+@A00604:387:HLC22DSX2:3:1103:24126:2096 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:9118:2159 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:10908:2253 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGGCAGCACCCCCTTTCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGAGTTCTTGGCGTTGTCTCT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:23140:2300 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:23466:2362 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF::FFFFFFF
+@A00604:387:HLC22DSX2:3:1103:27850:2409 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGGCAGCACCCCCTTTCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGAGTTCTTGGCGTTGTCTCT
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:::FFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1103:30183:2660 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFF:FFFFF,FF:F,,F,F,FF:FFFFFFF::,FF::FFFFFFF,FF,F,,::FFF,,FFF::FF:FF,,FFFFF::F:F,:FF
+@A00604:387:HLC22DSX2:3:1103:21712:2769 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:22670:2769 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATCAGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFFFFFF,FF,FF,FFFFFFF:FFFF,FFFF,FFF:FFFFFFFFF:FFFFFFFFF,FFFF::,FFF,:F,,FFF,FFFF,FFFFF,FFF,F::FFF,FFFFF:F,:FFFF:FF:FFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:14714:2832 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTGGCACAGTAATACACAGCCGTGTCCTCGGGCGTCACAGAGTTCAGCTG
++
+FFFFFF:FFFFFFFFFF:FF,FFFFF:::F:FFFFF,,FFFFFFFFFF,F:FFFFFFFF,FF,F,,F,,FF,:F:,:FF,,F,FF:FFFF,FFFFFFF,F:FF,,,:FFF:FFF,FF,F,FF,,FFFFFFF::,:FFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:19976:2832 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1103:19687:3020 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGAAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGAAATACACAGACGTGTCCTCGGGAGTCCCAGAGTTCAGCTG
++
+FFFFFFFFF,,FFFFF,F:FF,FFF::FF:FFF,:F:,FF,,,F:F:F:,,FF:FF,FF,F:F,,:,FFFF,F:F:FFFF:FF,F,F,FF,FFFFF,F:FFF:FFFF:FF,FFFFF:,F,,FF,FFFF,FFF:F,F:,,FFF,,,:F:FFF
+@A00604:387:HLC22DSX2:3:1103:12735:3098 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFF,:,F:FF,FFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FF,F:FF::FFF:FFFFFFFF::FFFFF:F:
+@A00604:387:HLC22DSX2:3:1103:28872:3114 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:1687:3129 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,:F,FFFFFF,FF:FF:
+@A00604:387:HLC22DSX2:3:1103:7066:3145 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:21866:3192 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCCCTGCTCTACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:9860:3255 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1103:18530:3270 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFF:FF:F:
+@A00604:387:HLC22DSX2:3:1103:8477:3364 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:12744:3364 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFF:FFFFFFF,FFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:22571:3380 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFF:FFFFF:FFFFFFFFFFF:FFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFF:FFFFF,FFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1103:24912:3427 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFF::FFFFFFFFFFF:FF,FF:FFFF,FFFFFFFFFFFF,FF,F:FF::FFFFFF,FFFF::FFF,FFFFFFFFFFFFF,F:FFFFF,F:FF,:F:F:FFFFF,FFF,FFFFFFFFFFFF:F:FFFF,:F:,FFFFFFFF,:FFF:FF
+@A00604:387:HLC22DSX2:3:1103:8106:3443 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCACATATCAAAAGCATTGTAGTAGCTCCCACTCTCTCTCGCACAGTAATACGCAGCCGTGTCTTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGC
++
+FFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:13630:3615 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAGAAGCATCATCCGGAGGATGGGCCCCATTGTCTTTCGCACAGTAATATATGGCCGTGTCCTCGGCTCTCAGGCTGCTCATTTGCAGATACAGCGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:9290:3646 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:27796:3693 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFF,FF:FFFFFFF:FFFF:FF
+@A00604:387:HLC22DSX2:3:1103:13874:3850 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF:FFF:FFFFFFFFF,FF::FFFF,:FFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:28284:4131 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFF,FF,FFFFF:,FFF,FFFFFFFFFFFF,:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:,FF::F,FFFF:FFFFFFFFFFFFFFF:F:F:FFFF:FF
+@A00604:387:HLC22DSX2:3:1103:24225:4178 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:1145:4288 2:N:0:AGAGGAGG+GGACTACT
+CTCAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCTCCTCCGTAGTTCCAGTCATCCCTCGCACAGTAATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGTGAT
++
+FF:F:FF:FFFF::FFFF:FFF::FFFFFFFFF,FFFFFFFFFFFFFFFFF,FFFFF::FFFF:,:FFFFF,,FF,FFFFFFF,FFFFF,FFFFFFF,:FFFFFFFFF,FFFFFFFFFFFFFF,:FF:FFFF:,FFFFF::FF,:,:FF,,
+@A00604:387:HLC22DSX2:3:1103:6524:4366 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1103:10113:4413 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFF::,FFFFFFFFFFFFFFFFFFF:F,FFFFFFF,FFF:FF,FFF:FFFFF:,F,FFFFFF:FFFFFFFF:FFF:FFFFFF,FFFFF:,FFFF,FF,FFFF,FF:FFFF,F:F,FF:FFF:F,FFFF:FFFF:FFFFF,FF,FFFFF
+@A00604:387:HLC22DSX2:3:1103:25988:4445 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGTCGATCGTATAGCAGCTGGTTGCCATTCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCAT
++
+:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:F:FFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFF:FFFF:FFFFFF:FFFFFFFFF:FFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:4209:4523 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:25870:4554 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFF:F:FFFFFFFF:FFFFFFFFFFFFFFF:FFFF,FFFFFF,FFFF,FFF,FFFFFFFFF:FFFFFFFFFFFFFF:FFF::FFFFFFFF:FFFFFFFFFFFFFFF,FF,FF::FFF:FFFF:FFF,FFFFFFFFFFFFF,FFFFF
+@A00604:387:HLC22DSX2:3:1103:10456:4570 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFF,:FFFFFFFF::FFF:F::FFFFFFF:FF:FFF,F,F,F,FF:FF:FF:FFFFFF:FFF::,FFFFFF:F,FFFFFF:FFFFFFFF:::,F,,FFFFFFF,:F:::::F:F::FFFFFF:FFFFFF:FF,,FFF,FFFF:F:,F
+@A00604:387:HLC22DSX2:3:1103:27407:4617 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFF:FFFF:FFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:7256:4633 2:N:0:AGAGGCTG+GGACTAAT
+CGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFF:F:FFFFFFFFF:FFFFFFFFFFFFF:FF,FFF,:FF:FFFFFFFF,F::FFF,FFFFFFFFFF:FFFFFFFFFF,FFFFF:FF:FFF,,FFF
+@A00604:387:HLC22DSX2:3:1103:27344:4726 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGCGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFF:FFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFF,:FFF,FFFFFFF,FFFFFFFFFFFFFF:FFFFF:FFFF,FFFFFFFFFF:FFFF,FFFFF,FFFFFFFFF:FFFFFFFFFFFFFFF,FFFF,FFFFFFF,FF
+@A00604:387:HLC22DSX2:3:1103:1687:4758 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:12608:4852 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACCTCAAAAGCACCGATGTCGTACCAGCCACTGCTATCCCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF:FFF,FFFFFFFF,FFFFFFFFFFF,FFFFFF:F:F:FFFFFF,FFFFF:FF,FF,F:FFFFFFFFFFF:FFFFFF:FFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:8983:4867 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:24605:4867 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCATGCCCCCAGACGTCCATACCGTAGTAGTAGTAGACGGAGTAGCAGCTACCACCACTACAATATACTAAGGGCTCCCCTCTCGCACAGTAATACACGGCCCTGTACTCAGA
++
+FFFF,,F,F:,F::FFFFFF,F,FFFFF,,F:,FF,F,F,,F,::,,:F,,,,FFFFFFF,FFF,:F::FF:F,,F,,FF:FF::F,FFFF::FFFFFFFFFFF,,::,FFFFF:F,FFFF:,:,F:FFFFFFF,FF,FF,FFF,,FFFF,
+@A00604:387:HLC22DSX2:3:1103:11125:5008 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGCCGTTACCACCGTAGTCATAGTAAGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCATTTGCAGATACAGCGTGTTCTTGGA
++
+FFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFF,F,FFF:FF:FFF:FFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:25129:5181 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTGTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFF,F:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:,FFFFFF:FFF:,FFF:FFFFFFFFF,FF:FFF::FFFFFFFFFFFFFFF:FFFFFF:FF:FF:FF,F:FFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1103:16107:5212 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF,F:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:17978:5228 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:7961:5259 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,:FFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:25084:5259 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATCCAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFF:,FFF,FF:FFFF,FFF
+@A00604:387:HLC22DSX2:3:1103:26313:5384 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFF,FFF,FF:FFF:FFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:::FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:5367:5588 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATCACCTATATCATAGCTCCCATCACCCCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFF:FF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:8395:5603 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFF,FFFF:FFFFFFFFFFFFFFFF:FFF:F:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFF:FFFFFFFF,F:
+@A00604:387:HLC22DSX2:3:1103:23665:5619 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:18195:5635 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,:FFFFF:
+@A00604:387:HLC22DSX2:3:1103:30960:5666 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:16577:5713 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:8359:5791 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:32208:5791 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:19090:6026 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:F:F:F:FFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1103:30165:6042 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:26829:6339 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACCGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATCCAG
++
+FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,F,FFFFFF:FF:F,F:FF,F,FF:FFFFF::F:,,F:,F:,FFFFF:FF,FF,,,FFFF,F,F,FF:,F,FF:,FFFFFF,,,:,F
+@A00604:387:HLC22DSX2:3:1103:22028:6449 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:27977:6605 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATAGGCCGGGGATCCTCCCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFF,FFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:12961:6684 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCATAAACCACACGAGAATGTGACCAGGGAACCTTCGCCCCAGGGGTCGAACCACCCACTCAATCCGTCATACACAAAAAACGATGACATATCTCTCGCACAGTAAAACACGGCCGAGTCGTCAGATCTCAGTCTCCTCAGCTC
++
+FFFFF,F,F,F,,F,:FF,:,:,F,,F,FFFF:,,:,,FF:,,,F,,FF,,,,:F,FFF::F:FFF,FF,FF,,,FFF,,:FF:FF:,,F,,,FFF,F:FFF,F:FF,,,F,F:FFFFF,,F,,,:,F:FF:F:F:FF:,:,F,:F,,F:,
+@A00604:387:HLC22DSX2:3:1103:10764:6762 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF,F:FF:FFF,FF,FF:
+@A00604:387:HLC22DSX2:3:1103:22426:6825 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCATGTCCCGCCCCACCACTCCAAAAATCCCCTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCT
++
+F:FF,:F::F:FFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFF:FF,FFF:FFFF,FFFFF,FFF
+@A00604:387:HLC22DSX2:3:1103:4164:6856 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FF:FFF
+@A00604:387:HLC22DSX2:3:1103:13160:6903 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFF:FFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFF,F:FFFFFF,F::FF:FFFFFFFFFFFF:F:FFFFFF:FFFFFFFF:FFFFFFFFF,FFF,FF:F:FFFFFFFFF,:FFFF::FF:FFF:FF:F,:FFFFF
+@A00604:387:HLC22DSX2:3:1103:17264:7028 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:2492:7247 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGCCCCCAGTAGTCAAAGGAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGAACTACACAGCCGAGTCCTCGGGCGTCCCAGAGTTCTGCTG
++
+FF:FFF:,FF,F:FFFFFFF,F,F:FF,:FFF:FF:FFF::FF,F,FFFFFFFFF,,F:,,:,FF:FFFFF:FFFFFF::FFFFFFF:FFF:,FFFFFFF,F,FFFF,,F,F:F:FFF,FFFF,F,F,FFFFF,F,F,FFFFF:,F,,F,,
+@A00604:387:HLC22DSX2:3:1103:28745:7247 2:N:0:AGAGGATG+GGACTACT
+CTGAACAGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACAGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTAGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGATGT
++
+F:F,F,,F:F,F:F,FF:FF:FFF:F,FFFFFF::F,FF:FF,:FF:FF,FFFF,FF:F,FFFFFFF:F,F:,F::FFF,,FFFF:,FFFFFFFF,FFF,:FF,,,F::F,:FF:F,:F:FF,:,F,:FFF:FFF:FF:F,FFF,:,:::F
+@A00604:387:HLC22DSX2:3:1103:27606:7310 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCATGGGCTACCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFFFFFFFFF,FF,F:FFFFF,:,FF:FFFFFF,FFFFF,,FFFF,:FF:FF,FFFFFF:FFF:,:,FF,FF,F,F,FFFFF,FFFF:FF:,:,FFF,,FFF:FFF,FFFFFFFF,,FFF,F:FFFF::FFF:FFFFFFF:F,F,FF
+@A00604:387:HLC22DSX2:3:1103:23963:7576 2:N:0:AGAGGAGG+GGACTACT
+CTGAACAGCCTACACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGGTCTTGGATGT
++
+,,,FFF,FF,F,FFFFF,F,,F:,FFF::F,,F,,,,FFFFF,::F,,:F,FFFFFFFFF:F,FFF,,,FFFFFF,F,FF,FFFF,:FF,F:FFFF,:FF:FF,F,FFFF:F:FF,:FF:FF:F:F,,F,FF,FF:,:,:,FFF,FFF,F,
+@A00604:387:HLC22DSX2:3:1103:26449:7592 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFF:FFFFFFF,FF:FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:1398:7639 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACGGGTTCTTGGATGT
++
+FFFF:FFFF:,FFFFFFFFFFFF:,FFFFFFFFFF:FFFFF:FFFFFFFFFF::FFFFFFFF:FFF,FFFFFFFFFF:FFFFFF:F,FFFFFF::FF:F::FF:,:,FFFFFFFF:FF:F::FFFFFF,F::FFF,F,:FFFFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1103:26702:7686 2:N:0:AGAGGATG+GGACTACT
+ATGAAACGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGTCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+,:F:F,F:F,::FF:F:,FFFFFF:FFFFFFFFFF,,FFFFFF,FF,FFFFFFFFFFFFF:F:FFFFF,:FFFFF,FFFF:F:FFFFF,FF,FF,FF:F:FFFF:F:,FFFFF,FFFF:FF,,,F,F,F,,F,F,FF,FFF,FF,F,FFFF
+@A00604:387:HLC22DSX2:3:1103:27434:7733 2:N:0:AGAGGATG+GGACTACT
+CTGGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFF,FF,FF,
+@A00604:387:HLC22DSX2:3:1103:17598:7764 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFF:FF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FF:F:FFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFF:FF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:7247:7999 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCGGGGTTGCGTGAGTTACTGTCCTTCCTTTGCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,:::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:F:::FFFFFFFFFFFF::FFFFFF:FF,FFFF,,FFFFF:FF:FFFFFFFFFFFFFFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1103:21097:8093 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGTGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFF:FF:,F:FFF:F:F::FF:FFFFFFFFF,FF:,F:F,FFFFFFFFF,F:,,FFFFFFFF,:FFF:FF:,:F:F:FFFFF,FF::FF,F:FFFFF,,FFFFF:FFFFFF::F:F,:F,FFFFF,F,:FF,:FFFF:,FFFFFF:,,
+@A00604:387:HLC22DSX2:3:1103:22507:8093 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+:FFFFF:FFFFFFFFF:FFFFF:F,F:FFF:FFFFFFFFFF:FF,FFFF:FF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFF::FFFFF:FFFFFFFFF,FFFF::FFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:1271:8265 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTACCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGGTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF:::F:F,:,F,FF:FFFFFFF:::FFFFFFFFF,FFF:FF:F:F,FF,F:F:FFF,F,,FF:FFFFF::F,FFF::::,F:FF,,F,:FFF,FF,FFF,F:FF:FFF:F:FFFFF,FFFFF:,FFF::FFF,FFFF,,:F:F:,,FF
+@A00604:387:HLC22DSX2:3:1103:4951:8281 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,F:FFFFFFF,FFFFFF::FFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:17770:8312 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1103:31512:8343 2:N:0:AGAGGATG+GGACTAAT
+CTTAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFF:FFF:F:FFF,FFF::FF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:F:FFFFFFF,F,F,FFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:F,FFFFFF,F,FFFFFF
+@A00604:387:HLC22DSX2:3:1103:31521:8359 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:2311:8406 2:N:0:AGAGGAGG+GGACTACT
+GTGCCACCACTGTTAGGGTTGATCCATCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGCACCCAGTGCATATAGTAGCCGGTGAAGGTGTATCCAGAAGCCTTGCAGGAGACCTTCACTGAGGCCCCAGGCTTCTTCACCTCAGCCC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:26187:8547 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FF:FF:FFFFFFFFFFFFFFFFFFFFFF::FF:FFFFFFFF,F:FF,FF:FFF:FFFF,FFFFFFFFFFFF,FFFFFFFFFFFFF,:FFFFFFFFF:FF:FFF,,FFFF::FFF,:FFFFFFFF,FFFFFFFF,,FFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:5466:8609 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF,FFFFFFF,F:FFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:12445:8609 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1103:22073:8625 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAAACGTCCATACCGTAGTAGTAGTAGTACGTGCCAGCCACTGCTACCCCCCCTTGCCTAGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:25518:8672 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:20338:8719 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF:FFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1103:29704:8719 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:19027:8829 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:13666:9095 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTATGAGGCGTAATCAACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:22110:9220 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:31132:9283 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FF:FFFFFFFFFFFFFFFF:FFFFF,FF::FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:13612:9408 2:N:0:AGAGGAGG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGAAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
++
+FFFFFFF:FFF:FFFFFFF::FF,FF,FFFFF,FFF:FF::F,:FFFFFF,,FF,FFFFFFFFFFFFFFFF,FFF:FFFFFFF:,F:F::FF,FFF:FFF:::FFFFFFFFFFFFFF:FFFFF:F:,FFFF:FFFFF:,F:,FFFFFFF,F
+@A00604:387:HLC22DSX2:3:1103:22507:9596 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1103:23366:9612 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCCCAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFF:FFFFFFFFFFFFF:FFFFFFF:F:F,,F:FFF:,F:F:FFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FF,FFFFF:FFF,FFF,F,FF,,FF::FFFFFF,FFF:FF:FF,FFFFFFFFFF::FF
+@A00604:387:HLC22DSX2:3:1103:23448:9659 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1103:26829:9659 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGACTCCACCACTCTAGACGGTGACCATTGTACCTTGGCCCCAGACATCAAAAGCACCTATGTCTTACCATACAATTCTATACCCGTCCTAGGTCTACCAAGCACAGTAATACAAGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF,F:,FF,F,,FF:FFFF:,F,FF,FF:F,:F,,,F:FFF:FF,,:F:FFFF:,FFFF:FF,F,FF,FF,FF,,F,,:F,F,FFFFF,,FF,::F,,,,FF,::,,,:FFF,FFFFF:F,,:,,:F,F,F,FFFFFFF:F:,FF,,FFF,
+@A00604:387:HLC22DSX2:3:1103:26639:9674 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+FFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFF,FFFFFF,FFFFFFFFF,FF,F,F:FF:,F:FFF:FFFFFFFFFFFF,F,,FFFFFFFFFFFFF,:FFF,FFFFFFFFFFF::,FF
+@A00604:387:HLC22DSX2:3:1103:16477:10081 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCAGTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:F:,FFF,FFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFF,F,F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFF
+@A00604:387:HLC22DSX2:3:1103:29378:10160 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFF:FF:FFFFFFFFF:FFFFFF:FFFF,FFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:::,FF,FF:FFF
+@A00604:387:HLC22DSX2:3:1103:2275:10191 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFF:FFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFF:F:FFFFF:FFFFFFFFFFFFFFFFF,FF:FFFFF:FFFFFFF:FFFFFFFFFFFF,FFF:FFFFF:FFFFFFFFFFFF,FF:F:FF::FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:18421:10473 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:31665:10488 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1103:28583:10848 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFF,FFF:FFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,F:FFFFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1103:3902:10911 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFF,FFFFF:FFF,FFFFF:FF
+@A00604:387:HLC22DSX2:3:1103:19000:10911 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:29270:10911 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFF:FFFFFFFFF,FFFFFFFFFF,F,FF:F:F:,FFF:F:FFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:31467:10927 2:N:0:AGATGATG+CGACTACT
+CTGAACCGCATCCAACACTAGAGACTGAGAACGTGGTCACATGCCCCCAGAAGTCAAAGTCCAAGTAATAACCACTAAAATACATGGCGCATTACTCACATTAATATACGGACGTGACATCGGATAACAGTCTGTTAATTTGCAGATACAT
++
+FFFFFF,,F:FFFF,,F,,,FFFF,,:,,,,F:F,,FF,F,FFFF,FFF,,F,F::FFFF:FFF:,FF,,:FFF:FF,:FFF,FF,,:,:,,F,FF,FFF,,FF,FFFF,,,,,,,::,,,,,,F:,:,:,F,,FFFFF,:,,FFFFFF,,
+@A00604:387:HLC22DSX2:3:1103:28646:10958 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTCTGCCGCGCCGACTCTCGCACAGTAATACACGGCCGTGTCGTCAGACCTCAGCCTGCTCAGCTCCATGTAGGCTGTGCTGATGGACGTGTCCCTGGTCAT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1103:32371:10989 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAAAAGGCCTGTTCTAACTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:31403:11036 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:,FFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1103:22598:11162 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFF,:,FF:FF:F,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,:F,F,F:FFFFFF:F,F,F,FF,F::,::FFFFF,F:::F:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:32497:11209 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTAGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCAATGTAGGCTGT
++
+,F,,F:FF,FF,FFF,F:F,FFFFF:FF:FFFFFF,,F,FFFF,F:FF:FFFFFF:FFFF,:FFFFFF,FFFFFFF,FF:,::F:FF,FFFFFF,::FF,:F,F:FF,FFFFF,FFFFFF,F,FFF:FF:FFF,FF,FF,FFFF:F,FFFF
+@A00604:387:HLC22DSX2:3:1103:16550:11397 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAGGTTTCCCTGATCCTTATCTCTCGCACAGTAATACATGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTTATGGAGGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:25220:11506 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFF,F:
+@A00604:387:HLC22DSX2:3:1103:21531:11694 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:1208:11725 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTCATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFF,FFFFFFF::FFFFFFFFFFFFFFFF,FFFFFFF,:FFFF,FFF:,FF,FFFFFFFFFF:FFFFFFFF,:FFFFF:FFFF,,:FFF,F:,FF,F
+@A00604:387:HLC22DSX2:3:1103:21377:11741 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FF:F:FF,,FF:FFFFFFFFFFFFFFFFFFF:F,FFFFF:FFFFFFF:FFF::FF::FFF:FFFFFFF,FF
+@A00604:387:HLC22DSX2:3:1103:21856:11757 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFF:,FFFFF:FFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:12915:12524 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFF:FF
+@A00604:387:HLC22DSX2:3:1103:13503:12665 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATCTTGGGCCTCTCTTGCACAATAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGACAACTGGTTCTTGGATGTGTC
++
+FF,FFFFFFF:FFF:FFF::FFFFFFFFFFFFF,,FFFFFF,:FFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF,FF:FFFF::FFFFFF,F,::F,FFF::,FFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,F:F:FFFF:
+@A00604:387:HLC22DSX2:3:1103:7202:12712 2:N:0:AGAGGATG+GGACTACA
+CTGAACCGCCTCCACCACTCGAGACGGTTACAATTGTCCCTTGGCCCCAGAAAACAAAAGCACAGATGTATTACAAGCCACTGCTATACACGGCCTAGGGCTCCCTCGCACAGTAATAAACGGACGTGACCTCAGATCTCAGGCAGCTCAG
++
+FF:FFF,FFFFFFFF,,FF,,F,FF,,F,FF,:F::F,FFF:F:FF:,F,F,F,,FFF:FFFF,::F,F,,FFF,F:,FFFF,F:,F,,,F,FFFF,:,F:FF,:::,FFFFF:FF,F,FF,F:F,:F,::FFF:FFFFFFFF:,:FFF,F
+@A00604:387:HLC22DSX2:3:1103:18349:12727 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCTCCTCCGTAGTTCCCGTCATCCCTCGCACAGTAATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGTGTT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFF:FFFFFFFFF:FFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF,FFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:31033:12868 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFF:FFFFFF:FFFFF,FFF
+@A00604:387:HLC22DSX2:3:1103:32434:12884 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCAACACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTCCCAAGCCTCGGTATAGCAGCTGGTACTACTACAATATCGAGGGACGTCTCTAGAACAGTAATACACGGCTGTGTCCTCGGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:F:FF,:F:FFFFF:FFFFFFF::FFFFFFFF,FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:7292:12962 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FF:F
+@A00604:387:HLC22DSX2:3:1103:32154:12962 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCTGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFF:FF:FF:FF
+@A00604:387:HLC22DSX2:3:1103:26964:13025 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:25925:13166 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTAAAATAGTCCCCTAGCTCCCCACGATGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTGGGCTGTGTCTGTAGA
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFF:FFFFFFF:FFFF:F:FFFFF:FFFF:FFFFFFFF:FFFF,FFFFFFFFFFFFFFFF:FFF:FFFFFFFFF::FFFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1103:32768:13182 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCAACACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTCCCAAGCCTCGGTATAGCAGCTGGTACTACTACAATATCGAGGGACGTCTCTAGAACAGTAATACACGGCTGTGTCCTCGGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFF:F,FFF:FFFFF,FFF:FFFFFFFFFFF,FFFFF
+@A00604:387:HLC22DSX2:3:1103:16242:13338 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFF:FFFFF:FF,::FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:11225:13354 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:FFFF:FF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1103:31602:13354 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFF:FFFFFFFFFFFFF,FF:FFFFF
+@A00604:387:HLC22DSX2:3:1103:6081:13526 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FF:FFFF:FFF:,F,FF,:,FFFFF,::,F:,FF::FFFFFF:::F,F::F,FF,FFFF,FFF:::F::,:FF:,F:F,:FFFFFFFFF,,FF:FFF:FFFFF,,FF:FFF,FFFFFFF,,,FF:FFFFF,FFFFFF,FFFFFFFF:F,,F
+@A00604:387:HLC22DSX2:3:1103:3956:13542 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTCATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACCG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,FFFFFFFFFFF:FFFFF,FFFF,FFFF::FFFFFF,FFF:FFFFFF,FFF:FFFFFFFFF,FFFFFFFFFFF:FFF,F:FFF,FFFF,FF:FF,F
+@A00604:387:HLC22DSX2:3:1103:18087:13557 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1103:29767:13683 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:9426:13714 2:N:0:AGAGGATG+GTACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFF,F:FF:FFFFF:FFFFF:FFFFFF:FF:FF::FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1103:31439:13855 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFF:FF::FF:FFFFF,:FF:FFFF:FFFFFF:FFFFFFFFFF:FF:,FFFFFFFFFF:F,FFFFFFF:FFFFF:FFFFFFF:FFFFFFFFFFFFFFFF:FFFF:FF:FFFFFF:FFFFFFFFF:FF,FFF:,FFFF
+@A00604:387:HLC22DSX2:3:1103:8413:13870 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFF:F:,FFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1103:10267:13886 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1103:25861:14246 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:28501:14434 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,:F:FFF,FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF,
+@A00604:387:HLC22DSX2:3:1103:30291:14434 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:7600:14465 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGCGTCGAACCACCCACTCATTAGTTCATACACAAAAATCGTTGCCAGTTCTCGCGCACAGAAATACACGGACGTGGCGTCAGAACTCAGGCTCCTCAGATC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FF:F::FF,F,,F,FF,,,,F,FF,,:,F:,FFF,,FFF,,F,F,:F,F,,F:,F,F,F:,,FFFFF,,:,:,F,:,,FF,,F:FF:,F,,FFFF,FF
+@A00604:387:HLC22DSX2:3:1103:6813:14544 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTCGTCACCGGCAGCACCCCCTTTCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGAGTTCTTGGCGTTGTCTCT
++
+FF:F:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFF:F:FFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1103:11442:14544 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFF:FFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:5846:14841 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF::FF
+@A00604:387:HLC22DSX2:3:1103:21287:14998 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1103:27887:14998 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:1334:15013 2:N:0:AGAGGATG+GGACTACT
+ACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATG
++
+FFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:5403:15045 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
++
+:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFF,FFFFFFFFFFFFFFFF:FF::FFFFFF,FFFFFFF:FFFF:FFF,FFFFFFFF:FFFFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1103:12075:15076 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1103:11939:15092 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGCTGTATCCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTGCTCAGCTCCATGTAGGTTGTGCTGATGGACGTGTCCCTGGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:28022:15170 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1103:17056:15217 2:N:0:AGAGGATG+GGACTACT
+AGGGAGAACTGGTTCTTGGATGTGTCTGGGTTGATGGTTATTCGACTTTTCACAGATACTGCATAATCATTATACCACTTGGACCTGTAGTATGTCCTTCCCAGCCACTCAAGGCCTCTCGATGGGGACTGCCTGATCCAGTTCCAAGCAG
++
+FFFFFFF,F:FF:FFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:28501:15217 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTGCTCGTAGCAGCTACCACCACTACAATATCCAGAGCCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCT
++
+FF,FFF,FFFFF,,:FFFFFFFFFFFFF,,FFFFFFFF::F:FF,F::FFF:FFFF:F:,F:FF:F:FFFF:F,F,F,FF,,:FF:F:F,:FFFFFF:,FFF,FF:F:FFFF,F,F:FFFFFFFFFF,F:F:FFF:,FFFFFF,:FFF,:F
+@A00604:387:HLC22DSX2:3:1103:19054:15233 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FF:FFF:FFFFFFFFFFFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1103:31539:15248 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAGCATACCACTACTATCATAGTAACCTTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:4227:15295 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGGTCATACACACAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFF:FFF::F,FFF,FFFF:FF:::FF:FF:FFFFF:FFFFFFFF:FFFFFFFFFFFFFFF,FFFF,F:FF:F::FFF:FFFFFFFFFFFFFFF:FF:FFFFF:,FFFFFFFFFFFFFFF:FFFF,FF::FFFF,FFFF
+@A00604:387:HLC22DSX2:3:1103:23014:15389 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1103:3812:15483 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFF::FFFFFFFFFFFF:FFFFFF:FF:FFFFFFFFF:FFFFFF:FFFFFFFFFF:F:FFF,:FFFFF:FFF:FFFFF:FFF,FFF:FFFFF,:FF
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,2276 +1,2276 @@
-@A00604:387:HLC22DSX2:3:1101:31810:21198 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACAAGGGTGCCCTGGCCCCAAAAGTCAAGGTACTGGCCTTTAGCCATCCGTGCACAGTAATATGTGGCTGTGTCCATAGGGTCAGTGTTGGTCAGTGTAAGGATCACTTGGTTTCTGGAGGT
-+
-FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:17942:21324 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:,:FFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF:F:FFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28293:21339 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFF:FF:FFFFFFFFF,FFF:FFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFF:FFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1101:24135:21371 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCACCACCACTCGAGACGGTGACCAGGGTTCCCAGGCCCCAGTAGTCAAGGCCCGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-:FF:FFFFFF,F:F,::F::,FFFF,,F:,FFFFFFFF:::,FF:F,,FF:FF,FFFFFFF,FF,FFFF:FF:FFF,::FFF:FFF,,FFFFFFFFFFF::FFFFF:F,FFFFFF:::F,FFFF::FF:,,FFFFF:,FF::,F:,::FFF
-@A00604:387:HLC22DSX2:3:1101:18575:21386 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:7563:21418 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:12852:21433 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACAACTACTATACATTGCGCTTTTCGCACAGTAATATACGGCCGATTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFF:F:FF,FF:FF:F,FFF:F:F,::,::F:FFFFF:,,:F,,,F:F,FFFF:F,FF:FFFFF,F,FF,F,FFF:F,F:F:,FFFFF,F,::,FFF::F:FFFFF,,F,:,,:FF,F,,FFFFF:FF:FF,FFFF:F,,F,:F:,FF
-@A00604:387:HLC22DSX2:3:1101:15076:21527 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGGAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTCGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFF:F:FFF:FFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFF:FFFFF:FFFF,FF,,FFFF,F,FFF:FFFFFFFFFFFFFFFFFFF:F,FFFFFFFF,FFF:F:FFFF
-@A00604:387:HLC22DSX2:3:1101:8386:21559 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFF:FFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24270:21637 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFF:FFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFF,FFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24921:21637 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF:FF,FFFF,,FF:FFF:F,FFFF:FF,::,::F:F:FF:,:,:FFFFFF:FFFF:FF:F,,FFFFF:FFFF,FFF:FFFF::FFF:,FFF:,:FFF:FFF:,:,::FFFFFFFF,F,F,,F,:FF,:F:F,,FF,,FFF:FFF:,FFF:
-@A00604:387:HLC22DSX2:3:1101:16062:21668 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTCATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFF:,:FFFFFFFFFFFFFF,FFFF,:FF:FFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:13422:21699 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:23981:21699 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:6795:21715 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1101:10447:21778 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5882:21793 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFF:FFFFFFFFFFF,:FF
-@A00604:387:HLC22DSX2:3:1101:17779:21825 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:,,FFFFFFFFFF,FFF,FFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24514:21840 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFF,,FFF:F:FFFFFFFF:FFFFFFFF::FFFF,FFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:15564:21872 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFF::FFFF:FFF:FF:FFFFFFFF:FFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF,F:
-@A00604:387:HLC22DSX2:3:1101:24641:21872 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22489:21903 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF::FFFF:FFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:2465:21919 2:N:0:AGAGGATG+GGACTACT
-TTCTGTGCATAGCCTGTGTCACCACTATTAGGGTTCATCCATCCCACCCACTCAAGCCCTTGTCCAGTGGCCTGTCGCACCCAATTGATATCATAACTGCTGAAAGTGTCTCCAGAAGCCTTGCAGGAGACCTTCACTGAGGCCCCAGGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,,FFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22670:22310 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21269:22420 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF:FFFF
-@A00604:387:HLC22DSX2:3:1101:18566:22435 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTCATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFF:FFFFFF:F:FFFFFFFFFF:F,:FF,F:F:,,FF,FFFFFFFFFFFF,FFFF:FFF:FFF:FF:FFFFF,FFF:FFFFFF:FFFFFFF:FFF:FFF,FFFFF,F:FF,FF,,F:F
-@A00604:387:HLC22DSX2:3:1101:28375:22451 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFF,:F:FFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,,FFF,FFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1101:1533:22498 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATCATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,F::FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:F:,FF:FFFFFFFFFFFFFFF:F,FF,FF,FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31259:22561 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFF:F:FFFFFFFFFFFFFFFFF:FFFF:FFF::FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF,F,FFFFFF,:F:F,FFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21766:22686 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9525:22780 2:N:0:AGAGGATG+GAACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:2862:22921 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFF:FFF:,FFF:FFF:FFFFFF::FFFFFFFFF,,FF,FFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFF,FF:FFFFF:FFFF,F:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24840:22999 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACCCAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF:F:FFFFFF,FF:,:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1101:27317:23093 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-FFFFFFFFFFFFFFFFFFFFFF:FFFFFF::FFFFFF:FFFFFF:F,F,FFFFFFFFFFFF:FF:,FFFFF,F:FFFFFFF:,FFF,,F:FFFFFFFFFFF:F::FF:FFF:FFFFFFFFFFF:FFF,FFFFFFFFFFFFF::FFFF:F:F
-@A00604:387:HLC22DSX2:3:1101:31901:23202 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFF:FFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21920:23265 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTCACCAGGGTTCCCTGGCCCCAGTAGTCACGGCCAGCCACTGCCGAATCTCTTGCACAGAAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FF,FF:F:F:,:FF:F:F:F:FFFF:F:,FFFF,:F:FFF,FF::F,FF,,FF,F,,F::F::FF:FF,F:FFF,FFFFFFFFF,F,FF,,FFFF,F:F,F:FF,F,,FFFFFFFF:FFFFFFFFF:F,:FFFF::FFFFF::FF:FFFF,
-@A00604:387:HLC22DSX2:3:1101:1687:23328 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCCCTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:
-@A00604:387:HLC22DSX2:3:1101:31828:23390 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCAATGCCGAATCTCTTGAACAGTAATACACAGCCGTGTCCTCGGGAGTCAAAGAGTTCAGCTGCAGGGAGAAGTGGTTCTATGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF,FF,FF:FFFFFF,FFFF,F,:FF,:,,F,FF,FFF,F,F,FFF,F::,,F:FF,F:F,FFF,FF,,FF,,,FFF:,,:,:F,F,F,FFFF,F,,FF,F,F,F:F:F,,F,FF:
-@A00604:387:HLC22DSX2:3:1101:19669:23563 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:F,:FFFFFF:FFFFF:FFFFFF:FFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:30906:23578 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFF::FFFFFFFFF:FFFFFFFFFFFFFFFF,:F:FFFFFFFFFFFF:FFFFFFFFF:F,FFF:FFFFFFFFFFFFFFFFFFFFF,FFFF:FF
-@A00604:387:HLC22DSX2:3:1101:3522:23719 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGGATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
-+
-F:FFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFF,FFFF,FFFF::FFFFF,FFF,,FFFFFFFFF:FFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26648:23719 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21730:23844 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFF,FFFFF:FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:F
-@A00604:387:HLC22DSX2:3:1101:13901:23876 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3351:24173 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCCAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFF,FFFFF,F:F,,FFF:FFFFFFFFF:FFFFFFFFFFF:FFF:FFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26449:24189 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:30427:24189 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCGCCAGGTACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTCCGCGGTTAT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFF,F:F
-@A00604:387:HLC22DSX2:3:1101:16694:24298 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF:FFFF:FFFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFF,FFFFF:FF:FF:FFFF,F,:FFFFFF,FFFFF:FFFFF,FFFFF:,:FFFFFFFF,FFFF:F:FF:FFFFF:FFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32560:24345 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGTCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTTCGTAGCAGCTACCACCACTACAATATCCCGCGGGGTGGCTCGCACAGAAATACACGGCCGTGTCCTCAGATCT
-+
-F:FF,,FFFF:F:FFFFFFFF,:FF:FFF,F:F,:FF,,F:FF,:F:FF,,:::FFFFFFF:F,FFFF,FF:FF,,:F:FFFF,FFFFFFFFFFF:FFFF,F:,,FFF:,,FF,F:FFFFF,:F,,FFFF:F:F::FF,FFFFFFF,:FFF
-@A00604:387:HLC22DSX2:3:1101:25201:24408 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:F,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22742:24627 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFF:FF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:1081:24659 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-F::FFFF:FF,F:FFFFFFFFF:FF:FFFF:FFFFFFFF:FFFF:FFFFFF:FFFFFFFFFF,:FFFF:FFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFF:F,:F:FFFFFFFF:FFFFF,::FFFFFF:FF,F:FF:F:F,F,FFFF
-@A00604:387:HLC22DSX2:3:1101:6569:24674 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24135:25003 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFF,FF:FFFF:FFFF::FFF:FFF:FF,FFF::FFF:F:FF:FF::FFF::FF:FFFFFF::FF
-@A00604:387:HLC22DSX2:3:1101:26449:25034 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:6849:25066 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF::FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16550:25113 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:6578:25128 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFF:,FFFFFFFFFFFFFFFF:FFFFFFFFFFFF::FFFFFFF:FFFFFFF:FFF:FFFF:::FFFFFFFFFFF,FFFFF,FF,FF:F
-@A00604:387:HLC22DSX2:3:1101:27444:25285 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:30228:25347 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31421:25379 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCGAGGCCCGCCACTGCCGAATCTCTTGCCCAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
-+
-FFFF:::FFFFFFFFF,FF:FFF:,F:FFFFF:FFFFFFF:FFFFFF,:F,FFF,,FFFFF,FFF,F:FFFF,F:FFFF,FF,,FF:,::F,,F,FFFFFFF,F:::FFFFF,,F,F,F:F:FF,,F:::FF:F,,,:FF,F,F:FF,FF,
-@A00604:387:HLC22DSX2:3:1101:7012:25441 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFF:FFFFFF,FFFF,F:,FFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF:FFFFFFFFFFF:,FFFF:FFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1101:28131:25504 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAACAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF,:F::FF,F:FFFFFFFF:FFF:FFFFFFFFFFFFF:FFF,F:FFFFFFFFFF,:FF:FFFFFFFFF,FFFFF,F,F,FFF,F:FFF:FFF:,F:FFFFF:FFFFF::F:FFFFFFFFFFF,F:F:FFFFFFFF:FFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:15112:25567 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:4553:25661 2:N:0:CGAGGATG+GGACTACT
-CTGGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGATGCTCA
-+
-FFF,,FF:FFF,F,F:,FFF:FF,FFFFF:FFFFFF,:F,FFFF:F:FFF:FFFF:FFFFFFFFF:FFFF:FF:F:FFFF:FFF:FFFFFFF:FF,FFF,FF:FFFFF,FFFF::FFFFF:,F:F,FF:F,FFF:,F:FFFFFF,FFFFF:
-@A00604:387:HLC22DSX2:3:1101:10303:25661 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF,FFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5141:25708 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1101:8892:25755 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16676:25770 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFF::FF:FF:F::FFFFFFFFFF,FFF,FF:FFFF:F:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28664:25770 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTACTACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFF:FFFFF,FFFFF,FFFFFFFFFFFFFFFF::FFFFFFFF:FFFFFFFFFFF,FF:,FFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31105:25801 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18123:25833 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:20889:25989 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:4996:26083 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31729:26162 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:15040:26256 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,F:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:19723:26287 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:14009:26318 2:N:0:AGAGGATG+GGACTACT
-CTGGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCA
-+
-FFFFF:FFFF,FF:,FFFFFFFFFFFFFFFFFF,F:FFFFF,FFF:FFFF:,:,,FFFFFFFFFFFFFFFFFFFF,FF:FFFF:FFFFFFFF,F:FF:FFFFFFFFFF,FF:,FFFFFFFFFF,FFFFFFFFFFF:F:FFFF:FFF:F::F
-@A00604:387:HLC22DSX2:3:1101:15275:26381 2:N:0:AGAGGATG+GGACTACT
-CTGACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCAGTGTCGTCAGATCTCAGGCTCCTCAGCTCC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF,FFFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9064:26522 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
-+
-FF,FFFFF,,:FFFFF,FFFFFFFFFFF,FFFF:FFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFF,FFFFFFF,F:FF:FFFFFFFFF:F:FFFF:FF,:::FFFFFFFFFFFFFF:F:FFFFFFFF,FFFF,F:FFFFFFF::FFF
-@A00604:387:HLC22DSX2:3:1101:16658:26522 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGGGAGTTGGTAGCAGCTACCACCACTACAATAGCGCCAATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:14859:26569 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18069:26678 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCT
-+
-:F:FFFF:FFFFFFFFFFFFF:F:FFFFF:FF:F:FF:,F:F:FFFF:FFFFF,,FFFFFFFFFFFFFFFFF:FFFF,FFFFFFFF::,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,F,,FFFFFFFFFFFFFFFF:FFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:24578:26835 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCCTACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFF:FFFFF::F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFF:,FFFFF:FFFFFFFFFFFFFFFFF:FFFFF::,FFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFF::FFFFFF
-@A00604:387:HLC22DSX2:3:1101:17409:26850 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCCCAGCCACTGCTAAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
-+
-FFFFFFFFFF,FFFFFFFFFFFFFF:FF:FFF:FF:FFF:FFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFF,FFF,FFFFF,FFFF,FFFFF::FF,,F:F,FFFFF,FFFFFFFF,F:FFFFFFFF:FFF:,,:,,
-@A00604:387:HLC22DSX2:3:1101:28384:26976 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTCCCAGCCACGGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFF:::FFFFFFFF,FFFFFFFF,FF:,FFFFFFF,FFF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFF,FFFFFFFFFFFFFF:F:FFFFFF:FF:FFF
-@A00604:387:HLC22DSX2:3:1101:1217:27054 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1101:1841:27164 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGACAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACCGGAATACACAGCCGTGTCCTCGGGAGTCACAGAGGTCGGCTG
-+
-FF:,FF,,,:FFFFFF:FFFFFF:F,,::FF,:F,,:FFF,FF,FFF:F::,F,:F:,F,FFFFFFFFFFF,:FFFFF:FFF:FFFFFFFFF,F:,F,FF:FFFF:FF:FFFFF:FFFFF:,FFFF:F:F:FFFF,FF:FFFF,:F,F,,F
-@A00604:387:HLC22DSX2:3:1101:22996:27164 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCTCCTCCGTAGTTCCAGTCATCCCTCGCACAGTAATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGTGTT
-+
-FF:FFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFF::FFF:F
-@A00604:387:HLC22DSX2:3:1101:13512:27211 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1101:28809:27211 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF,FFFFFFF,FF
-@A00604:387:HLC22DSX2:3:1101:6280:27242 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFF,FFFFFF:FFFFF:FFFF:FFFF,FFFFF:FFFFFFFF:FFF::F:FFF:FFF:FFFFFFF:F:FF,:FF:FFF,FFFF::,F,FFFF:F,FFFF,FFFFFFF,F,FF,FFFFFFFFFFFFFFF:F:FFF:F:F:FFFF:,,FFFF::
-@A00604:387:HLC22DSX2:3:1101:13675:27242 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:F:F,FFFFFFFF,F,:F,FF,FFFFFF:F,F:F:FFFFFFFFFFFFFF,,:FFFFFFF:FFF::FFFFF:,:F:FFFF:FFF:FFFFF:F:
-@A00604:387:HLC22DSX2:3:1101:27950:27320 2:N:0:AGAGGAGG+GGACTACT
-CTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTCTGCCCTGGAGCTTCTGTGCATAGTTTGTGTTACCATTGTAAGCGCTGATCCATCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGCA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:23149:27336 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFF:FF:FFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16269:27445 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:7889:27461 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:30291:27492 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32515:27524 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACATAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFF,FFFFFFFFFF,FFFFF,F,F:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFF,FF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:F:FFFFFFFFF,F:FF:FFFF,FFF:F:F,:FFFFFF:FFFFF:FF
-@A00604:387:HLC22DSX2:3:1101:9995:27571 2:N:0:AGAGGAGG+GGACTACT
-CTGAACAGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAACATCGTTTTTCGTAGCATACACCCAACGGGACTCTCGCACAGTAATACACGGCCGTATCGTCAGATCTCAGCCT
-+
-FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFF:FFFFFF::FFF,F,F:FFFFFFF:F,F:FFFFFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18900:27649 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:30617:27649 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20229:27790 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22905:27915 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:F:FFFFFFFFFFFFF:F:FFFFF:,FFFFFFF:FFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21278:28009 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF:FFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF,FFFFFFF:FFFFFFFFFFFFF:F:FFFFFFFF:FFFFF:F::FF:F:F:FFF:FFF:FFFFFFFFFFFF:FFF:FF:F
-@A00604:387:HLC22DSX2:3:1101:8766:28228 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF:FFFFFFFFF:FFFFFFFFF:FFFF,:F:FFFF:FF
-@A00604:387:HLC22DSX2:3:1101:26639:28307 2:N:0:AGAGTATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACCGAGTTCAGCTGCAG
-+
-,F,:FFFFFFFFFFFFFFFF,F:FFFF:FFFF:,FFFFFFF:F:FFFF:F,FF,FFFFFF:FF:FFFFFFFF:FFFFFFFFFFF::,::FFF::FFFFFF,,FFFFF:,,FFF:F,FFFFFFFFFFFFFF,F,F:F,FFF:,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:5692:28354 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:22218:28479 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTGCGGCCAGCCACTGCCATAAACTCCTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGCGAGTTCTTGGCATT
-+
-FFF:FFFFFFFF:FFFFFFFFFFFFF:FF:FFFFFF:F:,F,F:FFFF:FFFFFFFFFFFF:::FF,FFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFF,FFFFFFFFFFFFFFFFFFF,FFF,,FF:FFFFF,FF:FF::F,FFFF,FF:
-@A00604:387:HLC22DSX2:3:1101:17544:28526 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF,F:FFFF:F,,F:FFFF:F,FFFF,:FFFFF:FFFFFFFFFFFFF:FFF:,:FFF,FF:::F:F,FFFF:,FFFFFFFFFF::FF::FFF:FF,,FFF:FF::F:FFFFFF,FF:FF,:FF:FFF:,:FFFFFFFFFFFFFF,:F:FF
-@A00604:387:HLC22DSX2:3:1101:22634:28729 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACATCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCATGCTGCTCAG
-+
-FFFFFF,FFF:,,:FF,FFFFFFFFFFFFFF:F,F,:FFF:,FFFFFFFF,FFF,FFF:F,::F,FFF,F,:FFFF:FFFFFFFFFF,FFF,:,FFFF:F,F,FFFFFFF:F,FFFFFFFF:FFFF::FFFF,:,:,FF,F,FFFFFF:,,
-@A00604:387:HLC22DSX2:3:1101:27932:28761 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:13304:28823 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1101:19397:28823 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTCCAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,F:FFFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFF:
-@A00604:387:HLC22DSX2:3:1101:4806:29105 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFF,FFFF,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFF:F::FFF:FFFFFF:FF
-@A00604:387:HLC22DSX2:3:1101:10104:29199 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:17481:29199 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:31955:29215 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFF:FFFF:FFFF:FFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:14154:29293 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFF:FFFFFF,FFFF:FFFF,FFFFFFFFFFFF::FFF,F::FF,FFFFF:F:FFFFFF::FFFF::FFFFF:FFFFFFF::FFFFFFFFFFFFFFF,F:FFFFF:FFFFFF:FFFFF,FF
-@A00604:387:HLC22DSX2:3:1101:17752:29293 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF:FFFFFFFFF::FFF:F:F:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:14778:29465 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFF::FFFFFFFFFFF:FF:FFFF
-@A00604:387:HLC22DSX2:3:1101:28754:29465 2:N:0:CGAGGATG+GGACTACT
-ATCCCCACCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTTGGAATTGTCTCTGGAGATGGTGAACCGGCCCTTCACGGAGTCTGCGTAGTATGTGCTACCACCACTACC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16703:29481 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:16749:29622 2:N:0:AGAGGATG+GGACTACT
-CCTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFF,FFFFFF,FFFFFFFFFFF:F:F:F:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:7934:29731 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:24216:29747 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTACACATCAGTATAGCATACACCATTAGTACAGTATCCCTCTAAGACTCTCGCACAGTAATACACGGCCGTGTCGTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFF,::F:FF:FF,F,FFFF,FFFFFF,FFF:FFFFFF:FFF:FFFFFFFFFF::FF,FFFFF:FFFFF:FFFFF,FFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3233:29763 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:18385:29982 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFF:FFFFFFF:FFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFF:FFF:FFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFF,FFFFF:FF,FFFFFFFFFFFFF,FF,FFFFFFF:FF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16459:30060 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21893:30076 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:26422:30123 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:19379:30138 2:N:0:AGAGTATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACACCCCAATTGTATAGCATACACCACCAGTACAATAATAGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGATGATCAGCTC
-+
-FF,FFFFF,FFFFFFFFF:FFF:FF::FFFFFF,::,F,FFF:FFF,FFF,FF:F:FFF,FF,FFF,FFFFFF,::FFFFFF:,FFF,,F:F,,F:,:FFF,F::FFFFFFFF:FFFF,,,FFFFFFFFFF,FFFF:,,F,,F,FFFF,FF
-@A00604:387:HLC22DSX2:3:1101:23348:30342 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:4924:30373 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:,FFFFFF:FF::FFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFFFFFFFFFFFFFFF,FF:FFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:15365:30671 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCCTGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:F,FFFFFFF:FFF,FFF:FFF:F::F:FFFF:F:FFFF:FFFFFF,F,FFFFF,,FFF,FF,FF
-@A00604:387:HLC22DSX2:3:1101:21206:30765 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF::FFFFFFFFF:FFFFFF:FFFFFF:FFFFFFFFFF:FFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:21070:30906 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCAGACACCGGTAGTCCAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFF,FFFFFF,FFFF,FF:FFFFFFFFFFFFFFFFFFFFF:,FF,FFFFFFFFFFF:FF:FFF,F:
-@A00604:387:HLC22DSX2:3:1101:32434:30953 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF:FFFFFFFFFFFFF::FF:FFFFFF,FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16712:31125 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20021:31219 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTCATTCTCTCGCACAGTAATATACGGCCGGGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FFFFFFFFFFFFFFF,FFFF:FFFFFF,FFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:11026:31485 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFF:FFFF:FFFF,F:FFFFFFFFFFFFFFFFFF:FFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1101:14416:31814 2:N:0:AGAGGATG+GGACTACT
-CTGGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFF:FFFFFF,FFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11831:31845 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:2736:32002 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1101:19009:32002 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28565:32080 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCTAAGCTGTTTCTCCCTCTCGCACAGTGATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTTGGAATTGTCTCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,F:FFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21251:32095 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTAGTAGTATGCCCAACCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
-+
-FFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFF,FFFFF,FFFFFF:FFFFFFFFFFFFFF,FFFFFFFFF:F:FFFFFF,FFFFFFFFFF:FFFF,FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:16957:32236 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:,FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:F,FF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:13304:32362 2:N:0:AGAGGATG+GGACTACT
-CTGACCCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCACCCTCGCACCGTAATACACGGCCGTGTCCTCCGAGCTCAGGCTGCTCAG
-+
-FFFF,:F:,FF::FFFFFFFFFFFFF,FFFFF,,FF,F,F,,FFF,FFF,FFF:FF,::FFFF:F:FFF:FFFFFFFF,F,FF:F,FFF:FF:F,,FFF:F,F:,F::F:,,F,F:FFFF:FFF,FFF,FFF:,FF,FFFFF::F,:,FFF
-@A00604:387:HLC22DSX2:3:1101:15799:32424 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:F:FFFFFFFF,F:F,FFFFFFFFFFF:FFFFF:FFFFF:FFF,FF
-@A00604:387:HLC22DSX2:3:1101:12228:32440 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9679:32503 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTTGACGTAGCAGCTACCACCACTACAAGATCCTAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCT
-+
-FF:FF,FF,FFFFFFFFFFFFF:FFFFFFFF:,FFFFFFFF:FFF,FFFFFF,:FFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:,FFFFF:FFF:,FF:FF:FFF,F,FFFFFFFFF:FFFFF:::FFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1101:25373:32784 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FF,F:FFFF,FFFFFFFFFFFFFFFFF:,FFFF,FFFFFFFFFFFFFFFFF,FFFFFF:FFF::,,:FF:FF,FF,F
-@A00604:387:HLC22DSX2:3:1101:30553:32800 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTACACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGAAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTACTACACGGCCGTGTCGTCAGAGCTCAGGCTCCTCAGCTCCATGTAGGCAGT
-+
-FF,FFFF:FF:,,FFFFFF,F,F:FFFF:FFFF,FFFF:FFFFFFFFFF:,,F,FFFFFFFF,FFFFFFFFF:FFFFFFF:,FF:,F:FF,FFFFFFF:,,FF,,F,:FFF,F:FFF::F,,FFFFF:FF:FFFF,FFFF,,F,,FFF,FF
-@A00604:387:HLC22DSX2:3:1101:9444:32847 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:27832:32878 2:N:0:AGAGGATG+GGACTACT
-CAGAACCGCCTCCACCACTCTAGACGTAGACCATTGACCCATGGCCCCAGACATCAAAAGCACCTAAGACGTACAAGCCACTGCTAAACCCGTCCTTGGCCTCCCTCTCACAGTAATACACGGCCTTGTCCTCCGATCTCAGGCAGATCAG
-+
-F,FFFFF,F,FFFF,FFF,F,F,:F:,,,:F,FFF,,:,,,F,:FF,::,FFF,FFFF,,F,,F::::,FF,FF,,,,:FF,,:,F,,F:FF,F::FFF,F,FFFFF,FFF,,F,FF:FF:F,FF,,:FFFFF,F,:F,F:F,,,,,,,FF
-@A00604:387:HLC22DSX2:3:1101:2356:32941 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF:FFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFF:FFFFFFF:FFFFFFFF:FFFFFFFFF:FFFFFF:FFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32398:32957 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFF:FFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:14886:32972 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCGTCATCGTAGGGGCTATACAGCGCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:27263:32988 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FFFFFFFFFF,FFF:F:FFFF,:FFFFFF:FFFFF:FFFF:FFFFFFF,::FF:FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:4734:33144 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:31313:33176 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTACACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGTGAGAACTGGTTCTTGGATGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:29848:33270 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11704:33442 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:28040:33458 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATAACGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-::FFFFFFF,F:FFFFFFF:FFFFFFFFFFF:FFFFFFFFF,FFF,FFFFFFFFF,FF,,F,FF::FFF,:,FFFFFFFFFF::FFFF,F:FFFF::FFFFFFFF,FFFF,FFFFFFFFFF,FFFFF:FFFFFF,:FFFFF:FFF,,FFF:
-@A00604:387:HLC22DSX2:3:1101:30120:33583 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFF:F:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:F:FFFFF
-@A00604:387:HLC22DSX2:3:1101:28772:33630 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:32226:33943 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:29668:34021 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,:FF
-@A00604:387:HLC22DSX2:3:1101:19416:34209 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11858:34334 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FF:FFF:F:,FF,FFFF,FFFFF,FFFFFF,FFFFFFFFFFF:FF:FFFFFFFF,FFFFFFFF::FF:FFFF:FFFFFF,FFFFF
-@A00604:387:HLC22DSX2:3:1101:26196:34334 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20491:34350 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF:FF,FFFF,FF
-@A00604:387:HLC22DSX2:3:1101:22887:34491 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGTAGTCAATCCCCCCATGACCAGCCACTGCGGCGCGTGCACAATAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1101:25617:34648 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:3766:34851 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:14091:34851 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:13422:34914 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACCGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFF:FFFFFFF,,FFFF:F,,FFFF,F,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF::FF:FFFFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1101:30572:34961 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:21395:34976 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACAGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
-+
-,FF:FFFFFFFFFF,:FFFFFFFFFFF:FFFFF,FFFFF:FFFFFFFFFF,FFFF,FF::FFFF,FF,F:F,F:,FF:FFFFFFFFFFFFFF:FF,FFFFF,FFFF,FFFFFFFFFFFF,:FF::FFF:FFFFF,F,FFF,F,F:FFF,FF
-@A00604:387:HLC22DSX2:3:1101:10276:35102 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:23619:35227 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:14534:35274 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCACCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGATTTAAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-F::FFFF,:::FFF,,F:FF:FF:FFFFFF:,F:,:,F,FFF,FF,FFFF,:FFF,:F,FF:F,FFF:,F,FFFFF:FFFFF:FFFFFFF,,FFF:,:F:FFF,:FF:FFF:FFFF:F,,,,FFF,FFF,:FFFFF,:,,FFFFF,F,FFF
-@A00604:387:HLC22DSX2:3:1101:13078:35352 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAATTCCCCCTCGAGAATAGCAGCTACCACCACTACAATATCCTACTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-,FFFFF:FF:FFFFFFFF,FFFFFF:FFFFFFFF:FFFF:FF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,F:FF,F,FFFFFF:FFFFFFF,:FFF:FF:F:FFFFFF:FF:FFFF:FF::FFFFFFFFFFFF:FF,FFF:FFFF:
-@A00604:387:HLC22DSX2:3:1101:19633:35493 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:20428:35493 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9272:35556 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:24948:35587 2:N:0:AGAGGAGG+GGACTACT
-CCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFF:FFFFFFFFF:FF:FFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:2826:35853 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFF,FFFFFFFFFFF:FFFF:,FFFF:FFFFFFFFF,FFFFFFFFFF,:FF:FFFFFFFFFFFFFFFFF,FF:,FF,FFF:FFFFF,F:,FF,FFFFFFFFFFFFFF,F:F:FF:FFFFFF:FF:FF:FFFFFFF:FF,F,:FFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:11595:35916 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:9878:35978 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1101:2519:36010 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFF:FFFFF:FF,FFFFFF:FFFFF,F,FFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:2899:36041 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCCGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-F:FFFFFF:FFFFFF:FF::FF,FFF::FFFFF:FFFFFFF:FFFFFFFF:FF,:FFFFFFFFFFFFFFFFFFFF,:FF:FFF:F,FFFF:F,FFFFF:FF:,F:,F:FFFF:FF:FFFFFFFFFF,FFFF,F:FF,FFFFFFF,FFFFF,
-@A00604:387:HLC22DSX2:3:1101:5547:36213 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:7699:36245 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCACACCGTATTCGTAGCAGCTACCACCACTACAATACCCCTCCCCCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFF:FFFFFFF,FFFFFF:FFFFFFFFF:F:FFF,F:FFFF::FFF,FFFFFFFFFFF,FFF,FFFFFFFFFFF:F,F
-@A00604:387:HLC22DSX2:3:1101:23502:36464 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGACCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTGCATTTGCAGATACAG
-+
-:,FFFFFFFFFF:FFFF,FFFFFF,F:,FFF,F:FFFF,,F,F,F,FFFF,F:,FFF:FFFFFF:FF:FFFFF:,FFFF:,,,F,:F:F,FFF,FFF:,F,FFF,FFFF::FFFFF,FF:FF::FFFF:FFFFFF,FFFF:FFF:,:FF:F
-@A00604:387:HLC22DSX2:3:1101:17508:36479 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFF:FFFF:FFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF,FF:F:FF,FFFFFFF:FFF:FFFFFF:FFFFFFFFFFFFF,F,FFFF:F,FFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1101:10954:36526 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:29333:36605 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGAAGGTGACCAGGGATCCCTGCCCCAAGACGACCAAAGCGCCGAAGTAATAATCACCAGTATCATATTAATAAATGTGTGCTCTCGCACAGTAATACACAGCCGTGACATCATATCTCAGGCTGCTCAG
-+
-F,,FF,,,::,F,FFF,F,F,F,F,:FFFFFF,:,,,F,,FF,,:FF,:,FF:,,FFF,FF,F,:,F:F:FFF,:,:,,F,::,:,,F,FFF,FFFF,FF,,FFF:FFF:FFF::,FFFFF:FF,,,F:,,FFF,FFF,FF,,FFFF:,,,
-@A00604:387:HLC22DSX2:3:1101:25319:36699 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTAGTACCAGCCACTGCTATACCCGGCCTTGGGCTCACTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFF:FFF,,F,FFFFF::FFFFFFFFF:FFF:FFFF:FF:FFFF,FF::FF:FF:FFFFFF,:FFFFFF,FFFF,FFFFF,FF:FF,F:FFF,FF,FFFF,F::F:FFFFFF,F:FF:FFFF,FF,,FFF:FF:FFF:FFFFF
-@A00604:387:HLC22DSX2:3:1101:10158:36714 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCAGCCACTGCTATACGTCAGAGCTGTTGCACAGTAGTACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGT
-+
-FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:12735:36730 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAAGAAGTCAGCTGCTGCTATAAGGGTCCGTGCACAGTAATACGTGGCTGTGTCCACAGGGTCCATGTTGGTCATTGTAAGGACCACCTGGTTTTT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1101:11451:36761 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCAACCACTCGAGACGGAGACCAGGGTTCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGAAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFF,:,:F,FFFFF,F,FFFF,:,FFFFF,F:,,FF,FFFFFFFF,FFF,FF,FF:FFFF,,,,FFF,FFF:FFFFFFF:,FFFF,FF,:FFFF,FFFFFF,F,FFFFF,FF,,FFF,:FF,FFFF,:FF:,,FF:FFFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1101:29234:36777 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:12870:36808 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1101:26223:36855 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1101:28049:36855 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACACAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFF:F:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFF,F::FFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFF:FFFFFFFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1101:4924:36949 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATACGAGATCGTAGCCACGTCACGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFF:FFFFF:FFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFF:,FFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12038:1047 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5430:1063 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFF:F:F:FFFFFFFFFF:FFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:FF,FFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:14317:1360 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFF,FFFFFFF,:F:FFFFFFF,FFFF:F,FFFFFFFFFFFFFFF,FFFFFFF:FFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFF:,FFFFF,FFF::FFFFFFF,FFFFFFF:FFFFFFF:F:FFFF::FFFFFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:4996:1438 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFF:FFFF,FFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:14796:1438 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FF:F,FFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27019:1501 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFF:F,FFFFFF
-@A00604:387:HLC22DSX2:3:1102:11134:1548 2:N:0:AGAGGAGG+GGACTAAT
-CTGAACCGCCTACACCACTCGAGACGGTGACCGTGGTCCCTTGACCCCAGTAGTCAAAGTCAAAGTAATAACAACTACTATACATGGCGATTTTCGCACATTAATATACGGCCGTGTACTCGGCTCTCAGGCTGTTCTTTTTCAGATACAG
-+
-,FFFF,FFF:,,F,FFF,,F,FFF:,FFFF,:,F:,F:,FF:,,,F:,FF,F::,FFF,,F,FF:F:FFFFF,F,FF,FF,F,F:F,:F::F,F:,,FFF,,FF,FFFF:,FF,F,F,:FFF,,F:FFFF::F:FFF,,F:,FFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:22896:1689 2:N:0:ACAGGATG+GGACTACA
-CTGAACCGCGGCCACCACTCGAGACGGTGACCAGGGTTACCTGTCGCCAGAATGCAATGCCAGCAAATGCCTAAGCTCTTGCACAGTAATCAACATCCGAGTACTCGGTAGTGACATATTTAAGATGCAGGGAGAACTGGTTCTTTCATGT
-+
-FFFFFF,,F,,F::F:,FFFF,,:F:,FF:,,F,,,F,,FF,:,F,,F:F,F,,,F,,,FFFFF,F:,,F,:,:,FFFFFF,::F,F,FF,F,,F,F,,,,F:,::F,,F:F,,,F,F,,,,F:,F,FFF,FFFF,,F,F,FF,F,,FF,F
-@A00604:387:HLC22DSX2:3:1102:25726:1705 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:19325:1799 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:8160:1908 2:N:0:AGAGGATG+GGACTACT
-CTGCACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACCTGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGAGACAG
-+
-FFF,FFFFFF:FF:F:FFFFFF:FFFFFFFFFFF:FF:FFF:FFFFFFFF,FF:FFFFFF:FFFF:,,FFFFF,F,F::FFF:,FFFFFF:,,:FFF:F,F::FF:FFFFFF:F:FFFFFFFFFFF,F:FF:,F,F,:,FFFFFFF,:FFF
-@A00604:387:HLC22DSX2:3:1102:18231:1939 2:N:0:AGAGGATG+GGACTACT
-CGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTCTGCCCTGGAGCTTCTGTGCATAGTTTGTGCCACCACTGTTAGGGTTGATCCATCCCATCCACTCAAGCCCTTGTCCA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:25735:2002 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:24578:2065 2:N:0:AGAGGCTG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCATCTCTCAGGCTGTTCATTT
-+
-FFFFFFF:,FF:FFF:FFFFFFFFFFFFFFFFFFF:,,FF:F,,:FF,::F:FFFFF,:F,F,F,:FFF:FF:FF:FF:FFFFFFFF:FFFFFFF,F:FF:::FF,F,FFF:FFF,:F,F:FFF,F:FFFFF,FFFFFFFF:,F:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:17852:2127 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATAATCCCCAGTTGTGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1102:28646:2127 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF,,F:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FF:FFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6280:2190 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:15935:2190 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF,FFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:19208:2253 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTCGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTGGGGCTCTCGCACAGTCATATACGGCCGTGTCCTCGGCTCTCAG
-+
-FF:FFF:FFFFF:::FFFF,FFFFF,::FFFFFFFF,F,FFF,F:F,:FFF::,FFF,F::FF,FFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFF:FF:F,FFFFF:FFF:F,F,,FFFFFFF:FFF,:FF,:FF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:14045:2394 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:27471:2440 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCCAGACGCTGACCGAGGTCCCTAGCCCCCAGTAGTCAAAGTACAATTAATAACCACTACTAAACATGGCGCATATCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTCTTCATATCAACAAACAG
-+
-,FFFF,:FFF,::FF:F:::,F,F,:,F,F,:,,,FFFFF,,,FF,:F,FF:FFFFF,,F,FFF,,F,FFFFFFFF,F:,,FF::F,F:,,F,:FFFFFF:,FF,FFFFF,FFF,F,FF,:FFF,FF:F,FFF,:F:FF,,,,:,F,::F:
-@A00604:387:HLC22DSX2:3:1102:18502:2534 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:28556:2628 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9950:2942 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAATTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-F:FFFFF:FFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFF:FFFF:,F,FFFFFFFFFFFFFFF::FFFFF,FF:FFFFFF:FFFFFFFFF,FFFF:FFFFFFF:FFF:FFFFFFFFF:F,F,FFFF:FFFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1102:9462:2973 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:
-@A00604:387:HLC22DSX2:3:1102:25708:2988 2:N:0:AGAGGATG+GGACTACT
-AAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTTGGAATTGTCTCTGGAGATGGTGAACCGGCCCTTCACGGAGTCTGCGTAGTATG
-+
-F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,:FFFFF
-@A00604:387:HLC22DSX2:3:1102:32805:3129 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:32145:3239 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:17499:3552 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-:FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFF::FFFFFFFFFF,:F,FFFFFF,FFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1353:3583 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6054:3583 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FFFFF:FF,FF,:FF
-@A00604:387:HLC22DSX2:3:1102:2456:3991 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACACGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGGCCCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTC
-+
-FF:FFFFFFFF:FFFFFF,:FF:FF:F:FFFFFFFF:::FFFF:,F:FFFFFFFFFF:FFF,FFF:FFFFF,:FF:FFFFF,:FF,:FFF,FF,FFFFFFFFFFFFFF,FFFFFFF,FFFF:F:FFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11234:4131 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:4842:4178 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGATATCAAAAGCATCGGTGTCATCCCCTTTATAATAACCACTCCAAAAATCGTAATACGTTCGAAGCGGGCCACTCGCACAGTACTACACGGCCGTGTCGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:F:F,FFFFFFFFFFFFFFF:F:FFFFF:FFFFFFFFFFFFFFFFFFF:F:FFFFFFFFF,FFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:15854:4178 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5737:4194 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFF:FF,FF,FFF:F,FFFFFFFFFFFF,F,FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:F,FFF
-@A00604:387:HLC22DSX2:3:1102:16224:4225 2:N:0:AGAGGATG+GGACTACT
-CGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFF:F,FF:FFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:29939:4241 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27968:4366 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1102:25907:4460 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:29812:4523 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9335:4601 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFF:FF:FFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:9263:4695 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FF:FFFFFFFFFFFFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:10031:4711 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCACCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCCCTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF,,FF:,::F:FFFF:F::FFF,:FFFFF,:FF:FFFF:,:F,F:FFF:FF:F,FFFFF:FFFF::FFFFFF:FF,:FFFF,FFFFF:FFF:FFFFFFF:FFFF:,F,:F:FFFFFFFFF,F,FFFFFFFFFF,:FF:FFFFFFFF,
-@A00604:387:HLC22DSX2:3:1102:22236:4930 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30038:5040 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9263:5321 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATCTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:2103:5415 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCGCGCACAGTCATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-:FFF,FF:FFFFFFFF:F,FFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFF:FFF,FF,,FF,FFFF,F:FF::FF,FF,FFFFFFFFFFF,FFFFF,:F,FFFF,FFFFF:FF,FF,F:F:FFFFFFFF,,FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:2691:5556 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFF:FFF:FFF,FFFFFF,FFFFFFF:::,,:,FF:FFFFFFFFF:F:FF:,FFF,FFFFFF,F:FFFFFFFFFFF:FF,FF,,F,F,FFFFFFF,F:F
-@A00604:387:HLC22DSX2:3:1102:9426:5635 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11659:5682 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCGTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FF,FF,FFFF:F,
-@A00604:387:HLC22DSX2:3:1102:30481:5682 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30879:5776 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:9525:5838 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCCGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCCGCTC
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FF:FFF,FFFF,FFFFFFF:FFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF:FF,FFFF
-@A00604:387:HLC22DSX2:3:1102:26151:5854 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGGGGATTAAGTAGCAGCTACCACCACTACAATACCCGAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6912:5885 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACCCACAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FF,,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11785:5901 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
-+
-FFFFFFFFFF::FFFFFF,FFF,FFFFF,FFFFFF:FFFFFFFFFFFFFF:FFFF,F,FFFFFFFFFF:,FFFFFFFFFFF:FFF:,:FF,FFFF:F::FFFFFFFF,,FF:F:F,FFFFFFFFF:FF:FFFF:FFFFFFFFFFF:FF,FF
-@A00604:387:HLC22DSX2:3:1102:8214:5916 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-F:FFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF,FFFFFF:FFFFFFFFFFFF:FFFFFFFFF::FFFFFF:F:F:,FFFFF:FFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:23312:5979 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:18891:5995 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:18891:6026 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:27914:6057 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFF:,FFF:FFFFFFFFFFFFFFFFFFF:FF,FFFFFF:FFFF:FFF:FFFF,FFFFF,,FFF,FFF,F:F::FF
-@A00604:387:HLC22DSX2:3:1102:6108:6151 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF,F:FFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:27968:6151 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1102:32090:6245 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCACTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:29396:6339 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTAAGCTG
-+
-FFFFF,FFFFFFFFF:FFFFFFFFFF,:FFFFFFF:FFFFFF:FF,FFFFFFFFFFFFF:FFF:FFF:F:FFFFFFF:FFF,FFFFF,FFFF:,FFFFFF:FFFFFF:F:FFFF:FFFFFF,:,:FFFF::FFFF:FFFFFFFFF,FFF:F
-@A00604:387:HLC22DSX2:3:1102:25229:6480 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFF,F,:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11442:6558 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:4227:6903 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:F:,,FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:8187:6903 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFF:FFF,:FFFFFFF,FFFFFF,F:FFFFFFFFFFF:FFFFFF:,F,F:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:3893:6918 2:N:0:AGAGGCTG+GGACTACT
-AAGGTGAATCCAGAGGCTGCACAGGAGAGTCTCAGGGACCCCCCAGGCTGTACGAAGCCTCCCCCAGACTCCACCAGCTGCACCTCGGCCATGGCCGGCTGGGCCGCATAGAAAGGAACAACCAAAGGAATTGCGAATAATAATTTCTCAA
-+
-F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30219:7106 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCTAAGCCGCTATCAAAGTTTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCCTGTAGGCTGTGTCTGTAGACGTGTC
-+
-FFFFFFFFF,F:FFFF:FFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFF,FFFFF,FFF:FF:FF,FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF,:FF:FFFFFFFFFFFF:FF:FFFFF
-@A00604:387:HLC22DSX2:3:1102:5837:7216 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-F:,FFFFFFFFFF:FFFFF,FFFFF:F:FFFFF:,:FF:FFF:,F,:,FF:FF:FFFF,FFFFF,,FFF:F,FF:FFFFF,,:,F,:FFFF,FFF:F::FFFF,FF:FFFFFFF::FFFFFFF,,,:,F:,,FFF:,F,FF,FF:F,,,FF
-@A00604:387:HLC22DSX2:3:1102:5737:7232 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGGCCCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTC
-+
-FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7636:7263 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9697:7263 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTGGACAGATCTCTCGCACCGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFF:FFFFFFFFFFFF::F,FFF:FFFF,FFF,FFFF,:FFFFF::FFFF,FFFFFFFFFFFFFF:,,FF,FFF:FFFFFFFFFFFFFF:FF,FFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:24551:7435 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:
-@A00604:387:HLC22DSX2:3:1102:2040:7498 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1226:7529 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFF:FFFFF:FFFFFFFF:FFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,F:FFFFFFFFFFFF:::F,FFF:FF:FFFFFFF,,,FFFFFFF:FFFF:FFF:FF,FF::FFFFF,
-@A00604:387:HLC22DSX2:3:1102:16622:7607 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCAAAACACGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-,F:,:FF:::F:,F,,F:,F,FFFF,,FFFFFFFFFF:F,FFF:,F:FF:F,,FFFFFFFF,FF,,FF::FF:FF,FFFFFFF::FFFF,FFFFFF:FFFFFF,F:FF:F,FF:FF:FFFFF:FFF:FFFFFFFFFFFF,,::FFF,FFFF
-@A00604:387:HLC22DSX2:3:1102:1371:7686 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F::FFFF:FFFFFFF:FFFFFFFF:FF:FFFFFFFF:FF:FFF,F:FFFFF:FFFFFFFFFFFFFFFFFF,FFFF:FFFFFF::FFF
-@A00604:387:HLC22DSX2:3:1102:8368:7780 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:2591:7795 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,F:F,FFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF::FF,FFFFFF
-@A00604:387:HLC22DSX2:3:1102:7871:7795 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF,FFF
-@A00604:387:HLC22DSX2:3:1102:8486:7795 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5068:7889 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCAACCACTAGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTCCCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-,F,FFF::,FF:,F,,FF:,,FFF,::FFF,:F:FFFF,:FF,F,F,FFFFFF,F,F,FFFFFF::FFFFFF,F:FF,:F,FFFFF:FFFFFFFF:F:FFFFFF::FFFFF:F,F,F,FF,FF,,F,,FFFF:FFF:,F,FF,:F::FFF:
-@A00604:387:HLC22DSX2:3:1102:8467:7889 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:F:FFFFFFFFFF:F:FFFF:FFFF:FFFFFFFFFFF:FFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:14461:7905 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5466:8015 2:N:0:AGAGGATG+GGACTACT
-TAGGTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTCCGCGGCAATCGTGACTCTGCCCTGGAACTTCTGTGCGTAGTTTGCTATACCAAGGATAGGGATGATC
-+
-:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFF
-@A00604:387:HLC22DSX2:3:1102:8567:8061 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCGCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:31503:8077 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:3360:8375 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:,FFFF:FFFFFFFFFFFFFFF,:FF:FF,FFFFFFFFFFFFFFF,F,FFFFFFFFFFFF,FFFFFF:FFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:32606:8422 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF::FFFFFF:F,FFF,FFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:29261:8516 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGATATCAAAAGCATGGGGCCCGGAGTAGCAGCTACCACCACTGCAATATGCGGCTCGCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCCCCTCAG
-+
-FF,FFFFF::F:FF:FF,,FFFFFFF,F:FFF::FFFFFFFFFFFF:FFF,:F:FFFF::F,::F:FF:F:FF:F,,F,F:,,FFFF,,FFFFF,FF,FFFFFFFFFFFFF,FFFFFFFFF:,FFFFFFF,FFFFFFFFFF,FFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:30454:8641 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:25825:8703 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFF::FFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:31937:8735 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFF:FF:FFFF
-@A00604:387:HLC22DSX2:3:1102:25165:8750 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCATCCACTGCTATACCCGGCCATGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGAACTCAGGCTCCGCAG
-+
-FFFFFFF,F,,FFFFFFFF,FF,,F,FFFF:FFFFFFFFF::FFFFFFF,FF,F:FF,FF:::F,,:F,FF,,,FF,F:F:,FFFFFFF,F:FF:,,FFFFF,:FFFFFFF:::,FFFFF:FFF,F,F:FFFF,:F,::::::,:F,,FF:
-@A00604:387:HLC22DSX2:3:1102:3794:9032 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:,FFFF:FFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1102:7039:9048 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFF:FF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFF:FFFFFFFFFFFF,FFFFFFFFF:::FFF::FFFFFFFFFF:,FF,FFFFFF:FF:F,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12626:9204 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFF::FFFFFFFFFFFFFFFFFF:F::,FFFFFFFFFFFFFF:FFF,FFFF,
-@A00604:387:HLC22DSX2:3:1102:7220:9236 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFF:FF,FFFF:FFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFF:F:FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:18765:9408 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1102:1533:9721 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6054:9721 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCAGGTACCAGCCACTGCTCCCCAAAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:9824:9831 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF:FFFFFFFFFFF:,FFF
-@A00604:387:HLC22DSX2:3:1102:4001:10019 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:8874:10034 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:18756:10113 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:28474:10128 2:N:0:AGAGGATG+GGACTACT
-CTGAACCCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12093:10191 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFF:FFFFF:FFFFFFFFFFF:FF:F:F:FFF,:FFF:FFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27805:10191 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF::FFF,FF::FFFFFF
-@A00604:387:HLC22DSX2:3:1102:12219:10222 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FF:FFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:19497:10269 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATCATAAGGTACCACCGAGAGGGTGGAAATATCTTTTGCACAGTAATACAAGGCCGTGTCCTCAGCTCTCAGACTGTTCATTTGCAGATA
-+
-FFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11062:10285 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCGCAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFF:F:FF,F,,FFFFFFFFFFF:FF,:,FFFFFFF:FFFF:FFFFFF:F:FF,FFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13747:10394 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:21766:10441 2:N:0:AGAGGATG+GGACTACA
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTAGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-F::FF,FF:F,,:F,FFF::,F,FFFF,:F:FFF,F:FF:F,FF,:FFF,,FFFFFFFF:FFFF,FFFFFFFFFFF:FFFF,FFFFFFFF::FF:,,,FFFFFF:::,F:,,,FFFFFFFFFFFFF:FFFF,FFFF:F:F,F::FFF,,FF
-@A00604:387:HLC22DSX2:3:1102:11903:10457 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFF:F:FFFF:FFFFFFFFFFFFFFF:FFF:FFFFF:FFFFFFFFF,,FFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFF,:F::FFFF:F:FF,FFFFFFFF,FFFFFFFFFFFF,F:FFFFFFFFFFF:FFF:,FF:FF,F
-@A00604:387:HLC22DSX2:3:1102:6325:10473 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF,FFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5412:10488 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6307:10567 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCTCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:32687:10692 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9146:10723 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FFFFFFF,FF
-@A00604:387:HLC22DSX2:3:1102:12590:10927 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCAGCCACTGCTATACGTCAGAGCTGTTGCACAGTAGTACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13792:11005 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:15320:11052 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:6759:11099 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAACGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:24487:11146 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFF,FFFFF,FFFFF:FFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13060:11209 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FF
-@A00604:387:HLC22DSX2:3:1102:18412:11334 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1102:23276:11490 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFF:FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFF:,F:FFFFFFFF:FFFFFFFF,,F:,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5918:11522 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCTCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFF:FFFFF:FF:FFFFFFFFFFFFFFFFFFFFFF,F:FF,F:FFF,F:FFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFFFFFFF::FFFFFF,,F
-@A00604:387:HLC22DSX2:3:1102:23339:11537 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFF::FFF,FFFF:FF:F:FFFFFFFFFFFFFFFFFF,FFFF,:FFFFFFFFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1102:8214:11710 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAATGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF,FFFF,FF:F,,F,:F:FFFF::FFFFFFFFFF,FF:FFF:FFFF::FFF,F:FF:FFFFFF:FFFFFFFFFFFFFFFFFF:F:FFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1102:11722:11835 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCGTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACTGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFF,F,FFFFFFFF:FFFFF:FFFFFFFFFFFFF,FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:16577:11882 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGTCCAGCCACTGCCGAATCTCTTGCACAGTAAAACACAGCCGTGTCCTCGGGAGTCACAGAGTGCAGCTGCAGTGAGAACTGGTTCTTGGATGT
-+
-FFFFF:F,F,:FFFFFFFFF:FFFFFFFFF:FF,,FFF:F,,FFF:F,FFFF:F:FF,,FFF:,,FFFFF::F:FFFFFFF,:FFF,FF,FFFFF:,,:,,FF,:FFF,FFFFFFFFFF:,FF,,:,FF:,FFFFF:,:,:FFFFFF,FF,
-@A00604:387:HLC22DSX2:3:1102:26702:11913 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFF,FF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:
-@A00604:387:HLC22DSX2:3:1102:13006:11992 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFF::FFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:24804:12007 2:N:0:AGAGGAGG+GGACTACT
-CTCTTCAGAGATGTGCTGTAGGATTTTTCGTCATTCGAAAAAATGTGTGCAAGCCACTCCAGGGCCTTCCCTGGGGGCTGACGGATCCAGCTCACACCCATTCTAGCATTGCTGAGTGAGAACCCAGAGACGGTGCAGGTCAGCGTGAGGG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:21504:12117 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGAGCTCAGGCTCCTCAGCTC
-+
-FF:FFFFFF:F:FFF:FFFFFFFFFFF:FF:FFFFFFFFFFFFFF:FF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFF,,FF,FFFFFF:FF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:20961:12273 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTCTAAGGTAGAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:16523:12320 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF,FFFFF:F,,FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFF,FFFFFFF,FF
-@A00604:387:HLC22DSX2:3:1102:20139:12383 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTCTAAGGTAGAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFF:F::FFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30490:12524 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF,:FFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFF:FFFF:FFFF:FF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFF::FFF:FF:FFFFFFFFF:::F:F,FFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFF:
-@A00604:387:HLC22DSX2:3:1102:22155:12587 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAAGTAGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCCCCATGTA
-+
-FFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFF:FFF
-@A00604:387:HLC22DSX2:3:1102:7762:12618 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCGCCTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:10321:12633 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFF,FFF,FFFFFFFFFFFFFFFFFFFFFFFF::F:FFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:14597:12837 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCATGGCCCCAGGGGTCGAACCACCCACTCAGACGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGAAATACACGGCCGTGTCGTCAGATCTAAGGCTCCTCAGCTC
-+
-FF:FFFFF,F,:FFFF::FF:FFFFFFFFF,:FF,FFF::FFFFFFFF:,,FF::,FFFFF,F,FF,FF,,F::,FFFFF:FFFF:FFF:FF,FFF,FFF:FF,FF,FFF,FF,F:FFFFFFF,,,FFFF:,FF:F,,:,:FFFFFF:FF,
-@A00604:387:HLC22DSX2:3:1102:26503:12853 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFF::FFFFFF:F:FF:FFFFF:FFFFFFF,FF,FFF::FFFFFFFFFF,FFFFFFFFFFF:FFF:FFFFF
-@A00604:387:HLC22DSX2:3:1102:12491:12915 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13593:13009 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:18213:13056 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFF,,F,FFF::,FFFF::FFFFFFFF:FF:FFFFFF,FFFFFFFFFFFFF,F::F::FFFF:FF:FFFFF:FFFFFF:,FFFFFFFFFF,FFFFFFFFFF:F:FFFFFFFFFFFFFFFF,F:F,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1054:13088 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF::FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFFFF,FFFF::FF:FFF,FF
-@A00604:387:HLC22DSX2:3:1102:16224:13088 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,F:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF:FFFF:F:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5339:13432 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAACATCGTTTTTCGTAGCATACACCCAACGGGACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:8214:13463 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:3088:13604 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFF:F,F:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFF:FFFFFFFF:FFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:22851:13667 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:3025:13714 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FF:FFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:28429:13808 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF:FFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:1651:14027 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCCTTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFF,F,:F:FFFFFFFF,F,F:F,FF:F,F:FFFFFFFF:FFFFF:F::F:FFFFF:F:,FFF,:FF:FF:,F:FFF,,F,,FFFF:,F:,F:F::F,FFF,F,F::::FFFFFFF:,:FFF:FFF:FFF:FFFFFF::FFFFFF,F
-@A00604:387:HLC22DSX2:3:1102:11460:14074 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFF,F:FF::F:FF:FFFFFFF:FFF,:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11180:14090 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FF:,FF,FF,FFFFFFF:F::FFF,FFFFFFFFF::F:FF:FF:FFF:FF::,:,:FFFF:FFF:FFFF:FFFFFF::,FFFF,FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:31602:14105 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCGATACAACATCAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:F,FFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:17996:14121 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF:FFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFF:FFF:F,F,FFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:17969:14137 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF:FF::FFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFF,:FFFFFF,F:F:F:FFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF:F
-@A00604:387:HLC22DSX2:3:1102:21287:14152 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGAATCACAGACGTAGTCACCGTAGTCATCAGGATCTGATGGCGGGGCCAGTCTCGCACAGTAATACATAGCGGTGTCCGAGGCCTTCAGGCT
-+
-,FFFFF,:FFFFF:F:FFFFFF,F:::F,FF:F,FF:FFFF:F,:,F::,FFF,FFFFFF,F::FF,FFF,F,,::,FF:FF:FF,FFF,:F:F,FFFF:,FFFFF:,FFF,FF,FFFFFF::F,FFFF:F:F,FF::FFF,FFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:14362:14184 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:18069:14215 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCCCTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-,F,FFFFF:FFFFF:F:FF,FFFF:FFFFF:FFFFFFFFF:FFFFF,FF:FFF:,FFFFFF,FF:FF,FF:F,FFFF,FFFFF,FFFF::F,FF:F:FFFFFFFFFF,FFF:FF,,FFFFFF:FFFFFF,F:F,FFFFF:F::FFF,FFFF
-@A00604:387:HLC22DSX2:3:1102:5177:14246 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:14253:14340 2:N:0:AGAGGATG+GGACTACT
-GGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGCGGATGTGTCCCTGGTAATGGT
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:23267:14418 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTAGGCCCAAGACATCAAAAGCACAGATGTCGAACCAGCCACAGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACAAGGCCTTGTCCTCAGATCTCAGGATGCTCAG
-+
-FFFF:,,::FFF,,:F,FFFFFFF,::F,F,FFF,,FF,:,,,FFF,,,FFFFF,FFFF,F,:,,FFFF,,,F,,FF,FFF,FFFF,F:,,F,FF,FF,,FF,,F:::,,FFFF,,F:,,,FFF:,F,F,,,:FF:FF:,FF:,,FFFFF:
-@A00604:387:HLC22DSX2:3:1102:31566:14450 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFF:FFFFF:FFFFFFFF:FFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1102:15528:14512 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10167:14528 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
-+
-:FFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFF:FFF:FFFFFF:FF:FFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFF,FF:FFFFFFFFFFF:FFFF:FFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:25608:14528 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:14931:14575 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,:FFF
-@A00604:387:HLC22DSX2:3:1102:32642:14591 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGTTGT
-+
-FFFF:FFF:F:FFFFFFFFFFF:F:FFFFF:F,FF:FFFF:::F:,,F::FFFF,FFFFF,FFFFFFFF:FF,FF:FFFF:F:,,:FFFF::FF:FFFFFFFF:FFFFFF:FF,F:FFFFF,:FF:F::FF,FFF,,F,F,::,FFF,,FF
-@A00604:387:HLC22DSX2:3:1102:29749:14622 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCATACACAACTCGAGAAGGTGAAATTGTTCCATTGACCCAAGAAGTCAAAGTCCAAGTAATAACCACTACTAAACATGGCTCTTTTCGCACAGTAATATACGGACGTGTCCTAGGCTCTAAGGCTGTTCATTTGCAGATACAG
-+
-F,FFFF,FF,,,,:F,:,,,FFFF,::,,F,,,FF,F:,,,,::,F,,FF:F,F:FFF,,FFFFFFFFFFFF,FFFF,,:,F,FFF:,,:FF,FFFFFFF:,FF:FFFFF,,FF,F,F::,,,F,FF,FF:F::F::F,,,:FF:F,F,FF
-@A00604:387:HLC22DSX2:3:1102:17210:14826 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGTAGTAGTCCCCGGAGTAGCAGCTACCACCACTACAATATCCCTGATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCAC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFF:FFFFF::FFFFFFF:FFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1102:17336:14826 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:12961:15107 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCAGGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF:,FFF:FFFFF
-@A00604:387:HLC22DSX2:3:1102:10438:15186 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9869:15201 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-:FFFFFFFFFFFFFFF:F,FFFFFFFFFFF:FF:FFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFF::FFFFF:FFFFFFFFFFF:FFFFF:FFFF:FFF:F:FFFFFFFF:FFFFFFF::,FF,:FF,FFFF,FF
-@A00604:387:HLC22DSX2:3:1102:31096:15201 2:N:0:AGAGGATG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGTGTGCCATGGCCCCAGTAGTCAAATGCGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGT
-+
-FFFFFFF::FFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFF,FF:F:F,FFFF:FFF:,FF,FFFF,F:FF:F:F:::FFF:F:FF,FFFF,FF,FFFF:FFFFF,FFFFFFFF:FFFFFFF:FFFFF::FFFF,FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:22923:15327 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTACTACACGGCCGTGTACTCAGATCT
-+
-FFFFF:F:FFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFF,F,FFFFFFFFFFF:FF,,FF,FFFFF:FFFFFFFFFFF,FF,F:FF:F,FF:FFF:FFF,F,FFFFFFF:FF,FF,FFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:5068:15342 2:N:0:AGAGGAGG+GGCCTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFF,FF::FFFFFFFF:FFFFFFFFF,:FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFF,FFFFF::FFFFFFFFFFFF:FFFFF::FF:FFFFFFFFF:FFFFFF::,FFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7844:15358 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:,:FF::,,FFFFF:F:FF:FFF:FFFFF:F:FFFFF,FFF,FF:FFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27028:15483 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10384:15530 2:N:0:AGAGGATG+GGACTACT
-TGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6017:15765 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCAGTTGCAGAGACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,:FFFFFFF:F,FF,,,FF::,FFF:FFFFFFFFF:F,FF::F,::FFFFFF:F:FFFFFF:FF:F,FF::F,F:,,,FFF,FF,,F:F
-@A00604:387:HLC22DSX2:3:1102:32117:15781 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:18683:15906 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTCGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F:FFFFF:FFFF,F:F,F:FFFFFF:F,FFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFF,F,FFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1102:15176:16094 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF::FFFFFFFFFFFFF:FFFFFFFFFF,F:FF:FFFFFFFFFFFFFFFFFFFF:FFF:FFF,FFFF::FF
-@A00604:387:HLC22DSX2:3:1102:17517:16141 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:31530:16141 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCCCCGTAATACTCGGCCGTGTCCTCGGGTCTCAGGCTGTTCATTTGCAGATAGAG
-+
-FFFFFFFFFF,:FF:F,FFF::FFFFFFFFF:FFFFFFFF:FFF:FFFF:F,,F:F:FF:FFF:F,:FFFFF:F,,:FF,:,F,,F,F,,:F:FF:F,F,FF:,,F,FF,:,,FFF,::,F:::,,:,FFF,,F,:,::FFFF::,FF,F:
-@A00604:387:HLC22DSX2:3:1102:31557:16219 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
-+
-FFFF::FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFF,F:FFFFFFFFFFFFFFFFFFFFF:F,::FFFFFF:,FF:FF:FF:FFF:F:FFF,,FF:F,,FF:F:FFFFF:FF,:FFFF,,,F:,,::FF,FFFFF:F,FFF,:
-@A00604:387:HLC22DSX2:3:1102:6759:16360 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCCGCTC
-+
-FFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFF,F,,FF:FFFFFFFFFF:F:FFFF,FFFFFFFF,,FFFFFFFFFFFF,FFFFF:FF:FF:FFFFF:FF,FFFF
-@A00604:387:HLC22DSX2:3:1102:25391:16470 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFF::FFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFF:,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:19108:16485 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFF:,FFFF:,FFFFF,,FF
-@A00604:387:HLC22DSX2:3:1102:4318:16517 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF:FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFF,FFFFF:FFFF::FFFFFFFFFF::FFFFF:F:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:22019:16548 2:N:0:AGAGGATG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
-+
-:FF:FF,F::FFFF:F:,:F,FF:F::FF:FFFFF::FF:,:F:::FFFFFFF:F:FF:FFF:F,,F,::,F,F:FFFFFF,,,,FFFFFFFFFF:,FF,,FF:,:::,:F:FFFFF:FF:F:FFFFFFFFFFFFFF:FFFFF:FFFFFF:
-@A00604:387:HLC22DSX2:3:1102:3974:16830 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFF:FFF:FFFFF::FFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFFFFFFFFF:F:FFF,FFFFF,FFFFFFFF:,FFFFFF:FFFF,FFFFF::FFFF:FFFFFFFFFF:FFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1102:25572:16971 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTGGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGATGT
-+
-FFFFF,:FFFFFFFFFFFF:FF:FFF,F,FFFFFFFFFFFFFFFF,:F,F:FF,F,FF,FFFFFF:FFFFFFF:FF:,F,,F:FF:FFFF,:::FFFFF:F:FFFF,FFFF,,:FFF,FF:F,F:,F,,FF::F,FFFFF,:F,,FF:FFF
-@A00604:387:HLC22DSX2:3:1102:21513:17018 2:N:0:AGAGGATG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:F:F:F:FFFFF:FFFF:FFFFFFFFF:FFFFFFFFF,FFFFFFFF:FFFFFFF,FFF::FF:FFF,F
-@A00604:387:HLC22DSX2:3:1102:29704:17049 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCTCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:14724:17159 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-F,:FFFF:F:FF:FF,FFF,FFFFF:FFFF:FF,,,,F,:FFF:FF,:FFFF:FF,:F:FFFFFF,:F,FF:FFFFFF,FFFFFFF::FFFFF:::FFFFF,FFF::FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,F:FFF:::FFFF
-@A00604:387:HLC22DSX2:3:1102:8919:17440 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF,FF:FFF:,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5159:17628 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:20419:17754 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:::FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFF:FF::FF:FFFF:FFF:FFFFFFFFFF:F,
-@A00604:387:HLC22DSX2:3:1102:19171:17816 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27362:18098 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:5936:18129 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFF:FFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:31548:18239 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:28908:18333 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFF:FFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:15863:18349 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:19642:18380 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCGCAGCTCCAGGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF:FFFFFFF:FFFFFFFFFF:FF,FFFFFFFF,FFFFFF:FFFFFFFFFFFFF,FFFFFFF:,FFFFFF,FF
-@A00604:387:HLC22DSX2:3:1102:15393:18411 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:25943:18458 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFF:FFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:2211:18505 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCAGTTGAAGATACAG
-+
-FFFFFFF,FFFF:F,FFF:,FF:F:F:,,FFFF,FFFFFFF:FFFFFFFFF:FFFFF:F:FFF,F:F:::F,FFFFF,,:FF::,FF,FFFFF,,FFF::FF::F:F,F::FFFFF:F:,,FFFFFF::FFF,FF:F:,:FF,F:FFFFF,
-@A00604:387:HLC22DSX2:3:1102:21703:18505 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,:FF::FFFFFFFFF,FFFF:FFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6244:18599 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAGGAGTAGCTCCCACTATCGGTCTTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFF::FFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:17454:18850 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTTCCCCAGCACGTAGTCACCGTAGTCGCCACCTAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30807:18865 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12264:19132 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12246:19194 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGGAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF:F,FF:F,F:F,FF:FF:FFFF,FFFFF,,F:FFF:FFF:F,:F,FF:FF:FFF::FFF:FF:F:F:F:FFF,FFFFFFFFF,FF,F:FF,FF,:FFFF:,FFFF:,F,F:F:FFFFF:FF:FFFFFFFFF,,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:17589:19210 2:N:0:AGAGGATG+GGTCTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGGAATAACCACTACTATACTTGGCGCTTTTCGCACAGTAATATCCGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
-+
-FFFF:FF:FFFFFFFFFFFFFFFFFF,FF,FFFFFFFFFFFFF,FF:FFF:,FFFFFFFFFF:F:,F,,F:FFFF:FFF:FFF,:F:FFF,,FF::FFFFF,F,F:F,FFFFFF:FFFF,F::FFFF:,FFF:F:FF::,FFFF:FF,FFF
-@A00604:387:HLC22DSX2:3:1102:12391:19257 2:N:0:AGAGGAGG+GGACTACT
-CTGAACAGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:3784:19319 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGACCTCAGA
-+
-:F:FF:FFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFF:FF,FFFF:FF:FFFFFFFFFFF:FF:FFF,,FFFFFFFFF,FFF:FFF,F,::FFFFFF:FFF:F,:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:13087:19335 2:N:0:AGAGGATG+GGACTACT
-CTGGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAG
-+
-FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:30734:19398 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:8919:19476 2:N:0:AGAGGAGG+GGACTACT
-CTAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFF:FFFFFFF,FFFFFFFF,FFFF:,FF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FF,F
-@A00604:387:HLC22DSX2:3:1102:25075:19586 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:19027:19633 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FF:FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFF,:,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:20772:19648 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
-+
-FFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:6099:19695 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF,:FFFFF:FFFFFFFFFFF:,FF
-@A00604:387:HLC22DSX2:3:1102:6343:19805 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,FFFF,FFFFFFFFFFFF:FFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30924:19820 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9272:20149 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:29107:20181 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:4200:20228 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFF,FFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFF,F:FFFFFFFFFFFFFFFFF,:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27543:20290 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:25943:20306 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-,F,FF::,FF,FF:,FFF:,FFFFFF,:,F:FF:F,FF,FF,,F,FFFF:F:FFFF::F:F::F,FFFF,,,,F::FFFFF,FF,FF:,,F,:F,::FFFF:,FF,F,F,FFFFF:FFFF::F,F,F,FFFFFF,::FF:F::FF,,F,FF
-@A00604:387:HLC22DSX2:3:1102:31584:20306 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCTTTCATACACAAAAATCGTTGACAGATCTCTAGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCC
-+
-FFFFFF:F::FF:FFFFF,:FF:FFF:FFF,FF,FF:FF:FF:F:FFF::FFFFFFFF,F,F,FFFFF,FF,::FF:F,FF:F:F:FF:F:FF:FFFFFFFF,FFFFFFFFF:FFFFF,:F,FFFF::FFFFFFFFFFF,FFF:F,:FFFF
-@A00604:387:HLC22DSX2:3:1102:1434:20447 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTCATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTC
-+
-FFFFFFFFFFFFFFFFF::FFFFFFFFFFFFF,FFF:FFFFFF:FFF:FFFFF:F,FFFFF:FFF,FFF:F,::F,FF,:FFFFFF:FFFFFFFFFFFFF,F:FF,FFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1102:27877:20556 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1102:30264:20556 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTTCGTAGCAGCTACCACCACTACAATATCCCGCGGGGTGGCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFF:FFFFFFFFFFF:FFF,FFFF:FFFFFFFFFFFFFF:FFFFFFFFFFF:FF::F:FFF,FFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFF
-@A00604:387:HLC22DSX2:3:1102:3929:20603 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATCTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:F,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:21811:20697 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:2392:20854 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACACTAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF::FF:FFFF:FFFFFF:FFF:FFFFFF,:FFFFFF,,F,F:FFFFFFFFFFFFFFF,F::FF,FFFFF:FFFF,F:FFFFFF,
-@A00604:387:HLC22DSX2:3:1102:6244:21073 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGAAGTAGTAGTAGTCTGAGGAGCAGCTACCACCACTACAAGATCCTATACCCGTTGTTGCACCGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFF,F,FFF:FFF,FFF,FFF,FF,FFFFF,,::FFFFF,FFF,F,F,:FFF,FFFFF::,,:,,,FF:,,,FF,F:F:FF::,F:::,F:F,FF,FFF
-@A00604:387:HLC22DSX2:3:1102:17662:21151 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFF:FFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:1226:21183 2:N:0:AGAGGAGG+GGACTACT
-CTGACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
-+
-FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFF,F:FFFFFFFF:FF:::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFF,:FFFFF,F
-@A00604:387:HLC22DSX2:3:1102:22046:21198 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFF,FF,,FFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFF,FF,FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13539:21214 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:8422:21245 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFF,F:FF:FFFFFF::FF
-@A00604:387:HLC22DSX2:3:1102:10411:21245 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACCGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFF:
-@A00604:387:HLC22DSX2:3:1102:24578:21386 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:8766:21590 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATAGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-,FFFFFF:FFF::F::FFFF,FFFFF,:FFFFFF,FF,:,:F:F,F,FF,FF:::FFF,FF,FFFF::::FFFF,FFFF,:FFFFFFF:,F:,:FF:FFFF,F::FFFFFF:FFFFFFF:F,:FF,FF:F,FFFFFFF:FFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30789:21715 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGAACAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTCAACCATAGCTGTATCCACGACTTCTCTCGCACAGTAATAAACGGCCGCGTCCTCAGATCTCATGCTGCTCAGCTCCATGTAGGC
-+
-FF:FF,FFFF:F:FF,FF:,FF::F:FF:F,FFF,,FFFF,,:FF:FFFFFF,FF:FFFFFFFFFFFFF,FFFFF,,:F:FFFFFFF::,FFF:::FFF,,,,,FF,FFFF:F:F:,:,F:FFFFFFFF,FFFFFFFFFF,:,FF:FFF,:
-@A00604:387:HLC22DSX2:3:1102:8793:21856 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF
-@A00604:387:HLC22DSX2:3:1102:2338:22044 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTACTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FF:FFFFFFFFFFFFFFFFFFFFFF:::,FF,FFF:FF,,F:::FFFF:FFF,FFFFFF,FFF:F:F,,F:FF:FFFF:FF:FFFF,FFFF,:FFFFFFF::FFFFFFFFFFFF,FF,FFF:F:FFFFFF,F,FFF,F,FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:18602:22122 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF,FFFF:FFFF:FFFFFF:FFF,FF:FFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:27434:22232 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACAAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGGCCCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30653:22294 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATAAACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:26901:22404 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:14633:22670 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:F,FFFFFFFFFFF,F:FFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:23637:22670 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:23457:22733 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATCTCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFF:FFFFFFFFFFFFFFFFF,FFFFF,F,FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFF,F:FF
-@A00604:387:HLC22DSX2:3:1102:29423:22764 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:19687:22936 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,
-@A00604:387:HLC22DSX2:3:1102:9968:22952 2:N:0:AGAGGATG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCA
-+
-FFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF,FFF:F,:FFFFFFFFFFFF,FFFFF:FFF,,FF:FFFF,FFFFFFFFFFFFFF,FFF::FFFFF,FF::FF,,FFFFFF,FFFFFF,:FFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:1741:23015 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF,F:FFF:FF:FFFF,FFF::FFFFFFF:FFFFFFFFFF,F,FFF:F,F,FFFFFFFF:FF:FFF::FFF:FFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:5023:23062 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFF:FFF,:F:FF:FFF,,,,F:FF:FFFFFFFFFFF,F,FF,:,:FF,F,FFFFFFFF,,F,F,,,,,FF
-@A00604:387:HLC22DSX2:3:1102:4137:23281 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF::FF:FF:FFF
-@A00604:387:HLC22DSX2:3:1102:28574:23296 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:F:
-@A00604:387:HLC22DSX2:3:1102:24731:23312 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCCGTAGTCAAAGTCCAAGAACTAACCACTAAAAAACATGGCGCTGTTCTCACAGTAATATACGGCCGTGTCCTCGGCAATCAGGCTGTACATTTGCATATACAG
-+
-F,,,:::FFFFFFF:,,,F,,:FF:F:F,FFF,FF,FF:FF:,,FFF,,:F:F:FFFFF:F,FFF,::,:FF,,FF,,,F,:,:FF,FF:F,FFF,,,FFF,:F,FFF,FFFF,,F::F,F::,,,::,::F,F,,F,F,:,FF,F,FFF,
-@A00604:387:HLC22DSX2:3:1102:4797:23390 2:N:0:AGAGGATG+GGCCTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCACCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFF:F,F:FFFF,FFFFFFFFFFFF,F,:FFFF::FFFFFFFFFFFFFFF:FF,:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFF,F,FFF::,FF:F,,FFFFFFFF,::,,FFFF,FFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:32841:23390 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF::,FF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1787:23437 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1199:23453 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFF:FFFFFFF::FFFFFFFFFFFFFFFFF:FFFFF,FFF:FFFFFFFFFFFFFFFFFFF::FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:3956:23688 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7853:23735 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGAACAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCCCAGTAATACACAGCCGAGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCGGGGGCTTGGATGG
-+
-FF,FFF,::FFFFFFF,F,F::::,:F,,F,FFFFFF,F::F::FFF:::,FF,FF,FFF,:FFF::F,FF:F,,F,F,FF:,FFFF,FFFFFFFFF:F,:,FFFFF:F,,FF,F:F:,,FFF:F:,,FFF::FF,,,F,,,:,,F:F,F,
-@A00604:387:HLC22DSX2:3:1102:1705:23766 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTCCCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-FFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFF,:F:FF:FFFFFFFF:FFFFFFFF::FFFFF:FFFFFFFFF:F:FFFFFFFFFF,FFFFF,,FF
-@A00604:387:HLC22DSX2:3:1102:15591:24048 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCCTTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTACTACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-,FFF::FFFFF:,FFFFF:FFFFFFFF:FFFFFF:F:FFFFFF:FFFFFFFFFFFFFFFFFFFF,FFF,FFFFF::,FFF::,FFFFFFFFFFFFFFF::,FFF,F:FFFFF,FFF:FFF,FFFFFFFFF,:F,:FFF,FF,F,,:FFFFF
-@A00604:387:HLC22DSX2:3:1102:28393:24486 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTAACAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFF:FFFFFFFFFFF,FFFFFFF:F:FFFFF,FF:FFFFFFFFFFF:,,:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:22245:24518 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF:F:F,:FF:::F,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFF,FF,FFFF,FFF:FFF:FF:FFFFF,F:FFFFF:FF,FFFFFFFF:,F:FFFFFF:F,FFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:9507:24533 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:6641:24580 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27489:24580 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFF,FFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFF:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:21142:24612 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:32651:24659 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:F:FFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7844:24784 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10339:24909 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFF:FFFFFFFFFFFFF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11794:24956 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:30120:25066 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10122:25191 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1723:25269 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGATATACCCGGCCTGGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-,F,FFF:F:FF:F::F,FFFFF:FFFF,:FFFF:FFFF,F,FFFF,F:F:FFF,:FFF,FFFFFFFFF,,F:FFFF:F:FFF,,FFFFF:FFFFF:,FFFFFFFFFFF::FFFF,FF,FFF,:FFFFFFFFF:FFF,FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:20564:25394 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:22254:25535 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:20329:25551 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F:FFFFF,F,FFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:9896:25582 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTTGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGACTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-F:FFF:F:F:FFFFF,FF,FFF:FF:FFFFFFFFF:FFFFFFFFF,,:FFF,F,:F,,FFFFFF:FFFF:,FFF,F:FF:FFFFFF:FF:FFFFF:::FFF,F,FFFFFF,FFFFFF::,FFF,,:F,FFF::,FFFFFFFFFF,,,:FFF
-@A00604:387:HLC22DSX2:3:1102:23909:25614 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCAACACTCGATACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGAACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCGGCAGGGAGAACTGGTTCTTGGATGT
-+
-F,F:FFF:,F,F,F,FFF,,FF,F:FFFFF:,F::F:F,FFF,,FFFF:FFFFFF,FFFFFFFFFFFFF:FFFF::,:FF,,,F:FF:FFFFFFF:F,F::FF,FFF::FFFFFFF:FFF:F,F,,:F,::F,:::FF,F,FF,,F:,,FF
-@A00604:387:HLC22DSX2:3:1102:20916:25629 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF:F:F,FF:FFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFF::FFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1102:30427:25629 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:24451:25895 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:15890:25911 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATCTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFF,F
-@A00604:387:HLC22DSX2:3:1102:15185:25974 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13946:26146 2:N:0:AGAGGAAG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGAAGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGACACTGCTATACCAGGACTTGGGCTCCCTCGCACAGTAATAAACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFF:,FFFF,F,FFFFF,:,,,F,F,F:F,FFF::FFFFF,F,:F:F,FF,FFF,:FF,,F,:FFFF,FF,FFF,:FFFFFFF:F,F,,F,FF:,F:FFF,:,,FF:FF,:FFFF,FF,F:FF,,,F,,FFFF,:F,F,FF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:3577:26287 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F:FF
-@A00604:387:HLC22DSX2:3:1102:31476:26412 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFF::FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:28574:26584 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFFF:F:FF,FF:FF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:28167:26600 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10899:26850 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF,FF:F,
-@A00604:387:HLC22DSX2:3:1102:27064:26882 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCCTCCTCCTCCCAGCCACTGCTATGACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9037:26976 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTCCTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFF:F,FFF:F,F:FFF
-@A00604:387:HLC22DSX2:3:1102:11180:27023 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10221:27054 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:4869:27085 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:F:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13973:27164 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF::F:FFFFFFFF,:FFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFF:F:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12210:27211 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13521:27289 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFF,F::FFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:22869:27320 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFF:FF:F::FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11595:27398 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7211:27414 2:N:0:AGAGGATG+GGACTACT
-GTATAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTCCGCGGTAATCGTGACTCTGCCCTGGAACTTCTGTGCGTAGTTTGCTGTACCAAAGATAGGGATGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10420:27774 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCCGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCCGGGAGAACTGGTTCTTGGATGT
-+
-,::F::FFFFFFFF:FFF:FFF,:FFFFFF:FFFFF::FFFFFF,,F,,F:FFFFFFFFF:FFFFF,,:,F,FF:F:F,:FFF,F:FFF:FF:FFFF,F:FFFFF:,F,F::F:FF:FFFFFFFFFFF,,F,FFF,F,FF,,,FF,:F::F
-@A00604:387:HLC22DSX2:3:1102:14778:27774 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:4119:27790 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCCGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFF::FFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6234:27821 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:21513:27821 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAATTCCCCCTCGAGAATAGCAGCTACCACCACTACAATATCCTACTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12933:27837 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:16495:27899 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:21368:28040 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFF,FFFFFFFFFF:F:FFFF:FFFFFFFFF,FF::F:FFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:23023:28150 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:16568:28369 2:N:0:AGAGGATG+GGTCTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:21414:28401 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGTTTCCCTGGCCCCAGTAGTCAATGCCAGCCACTGCCGAATCTCTTGCTCAGTAATACACAGCCGTGTCATCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-F,,FFFFFFFFFFFFFFFFFFFFFFF:FFFF,F::,:,F:FFFFFFFFFFFFF:FFF,FFFF,FFFF:FFF,FF,FFF:FFF,FFF:F,FFF:FF:FFF,FFF,:FFFFFF:FFF::FFF,F,FFFFF,F::FFFFF::FFFFF,FF:FFF
-@A00604:387:HLC22DSX2:3:1102:12246:28526 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1967:28541 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAAAAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFF:FFF:FFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFF,,FFFFFFFFF:FFFFF:FFFF,FFFFFFFF:FFFFFFF:FFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:25672:28573 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,:F:FFFF,FF
-@A00604:387:HLC22DSX2:3:1102:10257:28588 2:N:0:AGAGGATG+GGACTACT
-CTGGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FF:FF:FFFFFFFFFFF,F:FF:FFFFF:F:FFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:10312:28588 2:N:0:AGAGGATG+GGACTACT
-CTGGAACCGCCTCCACCACTCTAGACGGTGAACAGGGTCCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCT
-+
-F,:FFF:FF::FF,F,:,FF:,F,FF,FFFF,,F:,,,,FFF:FFFFFFFFF,:FFFF,,FFF:FF:FFFFF,FF:F:F:FFF,FFF:F,F::FFFFFF,,F:::F,,FFF,FFFF:FFF,:FF,:F:FFF:::F:F,,:F:::F,F:FFF
-@A00604:387:HLC22DSX2:3:1102:20835:28651 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACACGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAAAATCTATCTCTCGCACAGTAATAAACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-F,,,FFF:F,,::,,:FF,:,F,FF,FFFF,FFF,FFF:FF,F,,FFFFFFFFFF:F,FFFF,,FFF,FF,FF,FFF,,F,FFFFF,FF:FF,FFFFFFFFFF::,,::::FFFF,FFFF,FF,FF,FFFF:FFFFF:F,,F:FF:F:,FF
-@A00604:387:HLC22DSX2:3:1102:6397:28792 2:N:0:CGAGGATG+GGTCTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTGCTCGTAGCAGCTACCACCACTACAATATCCAGAGCCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFF:F,FFFF,:FFFFFFF,FF:FFFFFFFF,FFFFF:FFFFF:FFFFFFF,FFFF:FFFFF,FF:FFFFFFF:FFFF:FFFFFFFFFF:F:FFF:FFFFF:F,FFF:
-@A00604:387:HLC22DSX2:3:1102:19379:28792 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTACAACACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATCGTCATAAATGTGGGCTCTCGCACAGTAATACACAGCAGTGTCGTCAGATCTCAGGCTGCGCAG
-+
-F:F,:,,,FF,,,F,FF,F,,FFFFF,F:FFF:,F:FFFFFF:,:,,,F:FFF:FFF,F,FFFFFFFFFF:FF:FFFF:,::,F:FF,FF,FFFFFF,FFF:,F:FF:FF:,F:FFF:F::FFF,FF::F,FFFF:,:FFFFF:F,,,FFF
-@A00604:387:HLC22DSX2:3:1102:25979:28886 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:,FFFFF:FFFFFFFF:FFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFF,FFF:FFFFFF:FFFFFFFF:FFFFFF:FFFFFFFF:F:FFFF
-@A00604:387:HLC22DSX2:3:1102:3712:28902 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGGTGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAGGTAGGCTGT
-+
-FFFFFFF,FFFFFFFFFFFFF:FFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFF:FFFFFFFFF,FFFFF,FFF,FFFFFFFF:F:FFFFFFFFF,F:FFF,FFF:FFFFFFFFF,:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:15393:28902 2:N:0:AGAGGAGG+GGACTACT
-AAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTCTGGGTTGATGGTTATTCGACTTTTCACAGATACTGCATAATCATTATACCAC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFF:FFFFFFFF:FFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:21187:29042 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACAACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFF,F:FFFFFFFFFFFFFF:FF:FFF:FF,F:FF::FFF,F:FFF,FFF,F,FFFFFF:FFFFFFF:FFFFFF:FF,F:F,:FF:FF:,FFF,:FFF,:FFFF:FFF,F,FF:F,FF:FF::FF:,FFFF,FFF,F,:FFFFFF,F,
-@A00604:387:HLC22DSX2:3:1102:3685:29168 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:12057:29168 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:F,FF:FF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:19126:29293 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FFF:FFFF::FFFFFFFFFF:FFFFFFFFF,,FFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:28827:29528 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFF:FFFFFFFFFF:FFFFFFFFF:FFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:15311:29543 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGAGGTCGTAGCAGCTACCACCACTACAATATCCGCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FF:FFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:26775:29543 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:16224:29559 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGCGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:F:FFFFFFFF:FFFFFF,FFFFFFFFFFFFFFF:FFFFFFFF:F:FFF:F:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:14760:29590 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFF,:FFFFFFFFF:FFFFFF:FFFFFF:FFFFFFFFFF,FF:FFFFFFFFF:FFFFFF:FFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7771:29700 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFF:FFFF:
-@A00604:387:HLC22DSX2:3:1102:15682:29778 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:18982:29794 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-:FFFFFFFFFFFFFF:F,FFFFFF:FF:FFF:FFF:FFFFFFF:F:FFFFFFFFFFF:F:FFFFFFFF,F:,F:F:,FFF,:F,,:FFF:FFF,FF:::FFFF,FF,FFFFFFF::FFF:,F,FFFFFFFFF,FFFF:F,FFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1102:7645:29825 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFF,FFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9127:29982 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFF,:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:31810:21198 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACAAGGGTGCCCTGGCCCCAAAAGTCAAGGTACTGGCCTTTAGCCATCCGTGCACAGTAATATGTGGCTGTGTCCATAGGGTCAGTGTTGGTCAGTGTAAGGATCACTTGGTTTCTGGAGGT
++
+FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:17942:21324 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:,:FFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF:F:FFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28293:21339 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFF:FF:FFFFFFFFF,FFF:FFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFF:FFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1101:24135:21371 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCACCACCACTCGAGACGGTGACCAGGGTTCCCAGGCCCCAGTAGTCAAGGCCCGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+:FF:FFFFFF,F:F,::F::,FFFF,,F:,FFFFFFFF:::,FF:F,,FF:FF,FFFFFFF,FF,FFFF:FF:FFF,::FFF:FFF,,FFFFFFFFFFF::FFFFF:F,FFFFFF:::F,FFFF::FF:,,FFFFF:,FF::,F:,::FFF
+@A00604:387:HLC22DSX2:3:1101:18575:21386 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:7563:21418 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:12852:21433 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACAACTACTATACATTGCGCTTTTCGCACAGTAATATACGGCCGATTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFF:F:FF,FF:FF:F,FFF:F:F,::,::F:FFFFF:,,:F,,,F:F,FFFF:F,FF:FFFFF,F,FF,F,FFF:F,F:F:,FFFFF,F,::,FFF::F:FFFFF,,F,:,,:FF,F,,FFFFF:FF:FF,FFFF:F,,F,:F:,FF
+@A00604:387:HLC22DSX2:3:1101:15076:21527 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGGAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTCGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFF:F:FFF:FFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFF:FFFFF:FFFF,FF,,FFFF,F,FFF:FFFFFFFFFFFFFFFFFFF:F,FFFFFFFF,FFF:F:FFFF
+@A00604:387:HLC22DSX2:3:1101:8386:21559 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFF:FFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24270:21637 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFF:FFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFF,FFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24921:21637 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF:FF,FFFF,,FF:FFF:F,FFFF:FF,::,::F:F:FF:,:,:FFFFFF:FFFF:FF:F,,FFFFF:FFFF,FFF:FFFF::FFF:,FFF:,:FFF:FFF:,:,::FFFFFFFF,F,F,,F,:FF,:F:F,,FF,,FFF:FFF:,FFF:
+@A00604:387:HLC22DSX2:3:1101:16062:21668 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTCATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFF:,:FFFFFFFFFFFFFF,FFFF,:FF:FFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:13422:21699 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:23981:21699 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:6795:21715 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1101:10447:21778 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5882:21793 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFF:FFFFFFFFFFF,:FF
+@A00604:387:HLC22DSX2:3:1101:17779:21825 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:,,FFFFFFFFFF,FFF,FFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24514:21840 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFF,,FFF:F:FFFFFFFF:FFFFFFFF::FFFF,FFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:15564:21872 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFF::FFFF:FFF:FF:FFFFFFFF:FFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF,F:
+@A00604:387:HLC22DSX2:3:1101:24641:21872 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22489:21903 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF::FFFF:FFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:2465:21919 2:N:0:AGAGGATG+GGACTACT
+TTCTGTGCATAGCCTGTGTCACCACTATTAGGGTTCATCCATCCCACCCACTCAAGCCCTTGTCCAGTGGCCTGTCGCACCCAATTGATATCATAACTGCTGAAAGTGTCTCCAGAAGCCTTGCAGGAGACCTTCACTGAGGCCCCAGGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,,FFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22670:22310 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21269:22420 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF:FFFF
+@A00604:387:HLC22DSX2:3:1101:18566:22435 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTCATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFF:FFFFFF:F:FFFFFFFFFF:F,:FF,F:F:,,FF,FFFFFFFFFFFF,FFFF:FFF:FFF:FF:FFFFF,FFF:FFFFFF:FFFFFFF:FFF:FFF,FFFFF,F:FF,FF,,F:F
+@A00604:387:HLC22DSX2:3:1101:28375:22451 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFF,:F:FFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,,FFF,FFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1101:1533:22498 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATCATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,F::FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:F:,FF:FFFFFFFFFFFFFFF:F,FF,FF,FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31259:22561 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFF:F:FFFFFFFFFFFFFFFFF:FFFF:FFF::FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF,F,FFFFFF,:F:F,FFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21766:22686 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9525:22780 2:N:0:AGAGGATG+GAACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:2862:22921 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFF:FFF:,FFF:FFF:FFFFFF::FFFFFFFFF,,FF,FFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFF,FF:FFFFF:FFFF,F:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24840:22999 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACCCAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF:F:FFFFFF,FF:,:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1101:27317:23093 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+FFFFFFFFFFFFFFFFFFFFFF:FFFFFF::FFFFFF:FFFFFF:F,F,FFFFFFFFFFFF:FF:,FFFFF,F:FFFFFFF:,FFF,,F:FFFFFFFFFFF:F::FF:FFF:FFFFFFFFFFF:FFF,FFFFFFFFFFFFF::FFFF:F:F
+@A00604:387:HLC22DSX2:3:1101:31901:23202 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFF:FFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21920:23265 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTCACCAGGGTTCCCTGGCCCCAGTAGTCACGGCCAGCCACTGCCGAATCTCTTGCACAGAAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FF,FF:F:F:,:FF:F:F:F:FFFF:F:,FFFF,:F:FFF,FF::F,FF,,FF,F,,F::F::FF:FF,F:FFF,FFFFFFFFF,F,FF,,FFFF,F:F,F:FF,F,,FFFFFFFF:FFFFFFFFF:F,:FFFF::FFFFF::FF:FFFF,
+@A00604:387:HLC22DSX2:3:1101:1687:23328 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCCCTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:
+@A00604:387:HLC22DSX2:3:1101:31828:23390 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCAATGCCGAATCTCTTGAACAGTAATACACAGCCGTGTCCTCGGGAGTCAAAGAGTTCAGCTGCAGGGAGAAGTGGTTCTATGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF,FF,FF:FFFFFF,FFFF,F,:FF,:,,F,FF,FFF,F,F,FFF,F::,,F:FF,F:F,FFF,FF,,FF,,,FFF:,,:,:F,F,F,FFFF,F,,FF,F,F,F:F:F,,F,FF:
+@A00604:387:HLC22DSX2:3:1101:19669:23563 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:F,:FFFFFF:FFFFF:FFFFFF:FFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:30906:23578 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFF::FFFFFFFFF:FFFFFFFFFFFFFFFF,:F:FFFFFFFFFFFF:FFFFFFFFF:F,FFF:FFFFFFFFFFFFFFFFFFFFF,FFFF:FF
+@A00604:387:HLC22DSX2:3:1101:3522:23719 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGGATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
++
+F:FFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFF,FFFF,FFFF::FFFFF,FFF,,FFFFFFFFF:FFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26648:23719 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21730:23844 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFF,FFFFF:FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:F
+@A00604:387:HLC22DSX2:3:1101:13901:23876 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3351:24173 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCCAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFF,FFFFF,F:F,,FFF:FFFFFFFFF:FFFFFFFFFFF:FFF:FFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26449:24189 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:30427:24189 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCGCCAGGTACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTCCGCGGTTAT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFF,F:F
+@A00604:387:HLC22DSX2:3:1101:16694:24298 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF:FFFF:FFFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFF,FFFFF:FF:FF:FFFF,F,:FFFFFF,FFFFF:FFFFF,FFFFF:,:FFFFFFFF,FFFF:F:FF:FFFFF:FFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32560:24345 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGTCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTTCGTAGCAGCTACCACCACTACAATATCCCGCGGGGTGGCTCGCACAGAAATACACGGCCGTGTCCTCAGATCT
++
+F:FF,,FFFF:F:FFFFFFFF,:FF:FFF,F:F,:FF,,F:FF,:F:FF,,:::FFFFFFF:F,FFFF,FF:FF,,:F:FFFF,FFFFFFFFFFF:FFFF,F:,,FFF:,,FF,F:FFFFF,:F,,FFFF:F:F::FF,FFFFFFF,:FFF
+@A00604:387:HLC22DSX2:3:1101:25201:24408 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:F,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22742:24627 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFF:FF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:1081:24659 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+F::FFFF:FF,F:FFFFFFFFF:FF:FFFF:FFFFFFFF:FFFF:FFFFFF:FFFFFFFFFF,:FFFF:FFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFF:F,:F:FFFFFFFF:FFFFF,::FFFFFF:FF,F:FF:F:F,F,FFFF
+@A00604:387:HLC22DSX2:3:1101:6569:24674 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24135:25003 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFF,FF:FFFF:FFFF::FFF:FFF:FF,FFF::FFF:F:FF:FF::FFF::FF:FFFFFF::FF
+@A00604:387:HLC22DSX2:3:1101:26449:25034 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:6849:25066 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF::FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16550:25113 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:6578:25128 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFF:,FFFFFFFFFFFFFFFF:FFFFFFFFFFFF::FFFFFFF:FFFFFFF:FFF:FFFF:::FFFFFFFFFFF,FFFFF,FF,FF:F
+@A00604:387:HLC22DSX2:3:1101:27444:25285 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:30228:25347 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31421:25379 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCGAGGCCCGCCACTGCCGAATCTCTTGCCCAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
++
+FFFF:::FFFFFFFFF,FF:FFF:,F:FFFFF:FFFFFFF:FFFFFF,:F,FFF,,FFFFF,FFF,F:FFFF,F:FFFF,FF,,FF:,::F,,F,FFFFFFF,F:::FFFFF,,F,F,F:F:FF,,F:::FF:F,,,:FF,F,F:FF,FF,
+@A00604:387:HLC22DSX2:3:1101:7012:25441 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFF:FFFFFF,FFFF,F:,FFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF:FFFFFFFFFFF:,FFFF:FFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1101:28131:25504 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAACAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF,:F::FF,F:FFFFFFFF:FFF:FFFFFFFFFFFFF:FFF,F:FFFFFFFFFF,:FF:FFFFFFFFF,FFFFF,F,F,FFF,F:FFF:FFF:,F:FFFFF:FFFFF::F:FFFFFFFFFFF,F:F:FFFFFFFF:FFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:15112:25567 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:4553:25661 2:N:0:CGAGGATG+GGACTACT
+CTGGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGATGCTCA
++
+FFF,,FF:FFF,F,F:,FFF:FF,FFFFF:FFFFFF,:F,FFFF:F:FFF:FFFF:FFFFFFFFF:FFFF:FF:F:FFFF:FFF:FFFFFFF:FF,FFF,FF:FFFFF,FFFF::FFFFF:,F:F,FF:F,FFF:,F:FFFFFF,FFFFF:
+@A00604:387:HLC22DSX2:3:1101:10303:25661 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF,FFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5141:25708 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1101:8892:25755 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16676:25770 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFF::FF:FF:F::FFFFFFFFFF,FFF,FF:FFFF:F:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28664:25770 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTACTACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFF:FFFFF,FFFFF,FFFFFFFFFFFFFFFF::FFFFFFFF:FFFFFFFFFFF,FF:,FFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31105:25801 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18123:25833 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:20889:25989 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:4996:26083 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31729:26162 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:15040:26256 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,F:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:19723:26287 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:14009:26318 2:N:0:AGAGGATG+GGACTACT
+CTGGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCA
++
+FFFFF:FFFF,FF:,FFFFFFFFFFFFFFFFFF,F:FFFFF,FFF:FFFF:,:,,FFFFFFFFFFFFFFFFFFFF,FF:FFFF:FFFFFFFF,F:FF:FFFFFFFFFF,FF:,FFFFFFFFFF,FFFFFFFFFFF:F:FFFF:FFF:F::F
+@A00604:387:HLC22DSX2:3:1101:15275:26381 2:N:0:AGAGGATG+GGACTACT
+CTGACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCAGTGTCGTCAGATCTCAGGCTCCTCAGCTCC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF,FFFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9064:26522 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
++
+FF,FFFFF,,:FFFFF,FFFFFFFFFFF,FFFF:FFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFF,FFFFFFF,F:FF:FFFFFFFFF:F:FFFF:FF,:::FFFFFFFFFFFFFF:F:FFFFFFFF,FFFF,F:FFFFFFF::FFF
+@A00604:387:HLC22DSX2:3:1101:16658:26522 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGGGAGTTGGTAGCAGCTACCACCACTACAATAGCGCCAATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:14859:26569 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18069:26678 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCT
++
+:F:FFFF:FFFFFFFFFFFFF:F:FFFFF:FF:F:FF:,F:F:FFFF:FFFFF,,FFFFFFFFFFFFFFFFF:FFFF,FFFFFFFF::,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,F,,FFFFFFFFFFFFFFFF:FFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:24578:26835 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCCTACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFF:FFFFF::F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFF:,FFFFF:FFFFFFFFFFFFFFFFF:FFFFF::,FFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFF::FFFFFF
+@A00604:387:HLC22DSX2:3:1101:17409:26850 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCCCAGCCACTGCTAAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
++
+FFFFFFFFFF,FFFFFFFFFFFFFF:FF:FFF:FF:FFF:FFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFF,FFF,FFFFF,FFFF,FFFFF::FF,,F:F,FFFFF,FFFFFFFF,F:FFFFFFFF:FFF:,,:,,
+@A00604:387:HLC22DSX2:3:1101:28384:26976 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTCCCAGCCACGGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFF:::FFFFFFFF,FFFFFFFF,FF:,FFFFFFF,FFF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFF,FFFFFFFFFFFFFF:F:FFFFFF:FF:FFF
+@A00604:387:HLC22DSX2:3:1101:1217:27054 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1101:1841:27164 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGACAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACCGGAATACACAGCCGTGTCCTCGGGAGTCACAGAGGTCGGCTG
++
+FF:,FF,,,:FFFFFF:FFFFFF:F,,::FF,:F,,:FFF,FF,FFF:F::,F,:F:,F,FFFFFFFFFFF,:FFFFF:FFF:FFFFFFFFF,F:,F,FF:FFFF:FF:FFFFF:FFFFF:,FFFF:F:F:FFFF,FF:FFFF,:F,F,,F
+@A00604:387:HLC22DSX2:3:1101:22996:27164 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCTCCTCCGTAGTTCCAGTCATCCCTCGCACAGTAATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGTGTT
++
+FF:FFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFF::FFF:F
+@A00604:387:HLC22DSX2:3:1101:13512:27211 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1101:28809:27211 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF,FFFFFFF,FF
+@A00604:387:HLC22DSX2:3:1101:6280:27242 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFF,FFFFFF:FFFFF:FFFF:FFFF,FFFFF:FFFFFFFF:FFF::F:FFF:FFF:FFFFFFF:F:FF,:FF:FFF,FFFF::,F,FFFF:F,FFFF,FFFFFFF,F,FF,FFFFFFFFFFFFFFF:F:FFF:F:F:FFFF:,,FFFF::
+@A00604:387:HLC22DSX2:3:1101:13675:27242 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:F:F,FFFFFFFF,F,:F,FF,FFFFFF:F,F:F:FFFFFFFFFFFFFF,,:FFFFFFF:FFF::FFFFF:,:F:FFFF:FFF:FFFFF:F:
+@A00604:387:HLC22DSX2:3:1101:27950:27320 2:N:0:AGAGGAGG+GGACTACT
+CTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTCTGCCCTGGAGCTTCTGTGCATAGTTTGTGTTACCATTGTAAGCGCTGATCCATCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGCA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:23149:27336 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFF:FF:FFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16269:27445 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:7889:27461 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:30291:27492 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32515:27524 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACATAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFF,FFFFFFFFFF,FFFFF,F,F:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFF,FF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:F:FFFFFFFFF,F:FF:FFFF,FFF:F:F,:FFFFFF:FFFFF:FF
+@A00604:387:HLC22DSX2:3:1101:9995:27571 2:N:0:AGAGGAGG+GGACTACT
+CTGAACAGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAACATCGTTTTTCGTAGCATACACCCAACGGGACTCTCGCACAGTAATACACGGCCGTATCGTCAGATCTCAGCCT
++
+FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFF:FFFFFF::FFF,F,F:FFFFFFF:F,F:FFFFFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18900:27649 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:30617:27649 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20229:27790 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22905:27915 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:F:FFFFFFFFFFFFF:F:FFFFF:,FFFFFFF:FFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21278:28009 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF:FFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF,FFFFFFF:FFFFFFFFFFFFF:F:FFFFFFFF:FFFFF:F::FF:F:F:FFF:FFF:FFFFFFFFFFFF:FFF:FF:F
+@A00604:387:HLC22DSX2:3:1101:8766:28228 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF:FFFFFFFFF:FFFFFFFFF:FFFF,:F:FFFF:FF
+@A00604:387:HLC22DSX2:3:1101:26639:28307 2:N:0:AGAGTATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACCGAGTTCAGCTGCAG
++
+,F,:FFFFFFFFFFFFFFFF,F:FFFF:FFFF:,FFFFFFF:F:FFFF:F,FF,FFFFFF:FF:FFFFFFFF:FFFFFFFFFFF::,::FFF::FFFFFF,,FFFFF:,,FFF:F,FFFFFFFFFFFFFF,F,F:F,FFF:,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5692:28354 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22218:28479 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTGCGGCCAGCCACTGCCATAAACTCCTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGCGAGTTCTTGGCATT
++
+FFF:FFFFFFFF:FFFFFFFFFFFFF:FF:FFFFFF:F:,F,F:FFFF:FFFFFFFFFFFF:::FF,FFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFF,FFFFFFFFFFFFFFFFFFF,FFF,,FF:FFFFF,FF:FF::F,FFFF,FF:
+@A00604:387:HLC22DSX2:3:1101:17544:28526 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF,F:FFFF:F,,F:FFFF:F,FFFF,:FFFFF:FFFFFFFFFFFFF:FFF:,:FFF,FF:::F:F,FFFF:,FFFFFFFFFF::FF::FFF:FF,,FFF:FF::F:FFFFFF,FF:FF,:FF:FFF:,:FFFFFFFFFFFFFF,:F:FF
+@A00604:387:HLC22DSX2:3:1101:22634:28729 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACATCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCATGCTGCTCAG
++
+FFFFFF,FFF:,,:FF,FFFFFFFFFFFFFF:F,F,:FFF:,FFFFFFFF,FFF,FFF:F,::F,FFF,F,:FFFF:FFFFFFFFFF,FFF,:,FFFF:F,F,FFFFFFF:F,FFFFFFFF:FFFF::FFFF,:,:,FF,F,FFFFFF:,,
+@A00604:387:HLC22DSX2:3:1101:27932:28761 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:13304:28823 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1101:19397:28823 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTCCAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,F:FFFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFF:
+@A00604:387:HLC22DSX2:3:1101:4806:29105 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFF,FFFF,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFF:F::FFF:FFFFFF:FF
+@A00604:387:HLC22DSX2:3:1101:10104:29199 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:17481:29199 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31955:29215 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFF:FFFF:FFFF:FFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:14154:29293 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFF:FFFFFF,FFFF:FFFF,FFFFFFFFFFFF::FFF,F::FF,FFFFF:F:FFFFFF::FFFF::FFFFF:FFFFFFF::FFFFFFFFFFFFFFF,F:FFFFF:FFFFFF:FFFFF,FF
+@A00604:387:HLC22DSX2:3:1101:17752:29293 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF:FFFFFFFFF::FFF:F:F:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:14778:29465 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFF::FFFFFFFFFFF:FF:FFFF
+@A00604:387:HLC22DSX2:3:1101:28754:29465 2:N:0:CGAGGATG+GGACTACT
+ATCCCCACCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTTGGAATTGTCTCTGGAGATGGTGAACCGGCCCTTCACGGAGTCTGCGTAGTATGTGCTACCACCACTACC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16703:29481 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:16749:29622 2:N:0:AGAGGATG+GGACTACT
+CCTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFF,FFFFFF,FFFFFFFFFFF:F:F:F:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:7934:29731 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24216:29747 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTACACATCAGTATAGCATACACCATTAGTACAGTATCCCTCTAAGACTCTCGCACAGTAATACACGGCCGTGTCGTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFF,::F:FF:FF,F,FFFF,FFFFFF,FFF:FFFFFF:FFF:FFFFFFFFFF::FF,FFFFF:FFFFF:FFFFF,FFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3233:29763 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18385:29982 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFF:FFFFFFF:FFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFF:FFF:FFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFF,FFFFF:FF,FFFFFFFFFFFFF,FF,FFFFFFF:FF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16459:30060 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21893:30076 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26422:30123 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:19379:30138 2:N:0:AGAGTATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACACCCCAATTGTATAGCATACACCACCAGTACAATAATAGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGATGATCAGCTC
++
+FF,FFFFF,FFFFFFFFF:FFF:FF::FFFFFF,::,F,FFF:FFF,FFF,FF:F:FFF,FF,FFF,FFFFFF,::FFFFFF:,FFF,,F:F,,F:,:FFF,F::FFFFFFFF:FFFF,,,FFFFFFFFFF,FFFF:,,F,,F,FFFF,FF
+@A00604:387:HLC22DSX2:3:1101:23348:30342 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:4924:30373 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:,FFFFFF:FF::FFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFFFFFFFFFFFFFFF,FF:FFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:15365:30671 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCCTGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:F,FFFFFFF:FFF,FFF:FFF:F::F:FFFF:F:FFFF:FFFFFF,F,FFFFF,,FFF,FF,FF
+@A00604:387:HLC22DSX2:3:1101:21206:30765 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF::FFFFFFFFF:FFFFFF:FFFFFF:FFFFFFFFFF:FFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:21070:30906 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCAGACACCGGTAGTCCAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFF,FFFFFF,FFFF,FF:FFFFFFFFFFFFFFFFFFFFF:,FF,FFFFFFFFFFF:FF:FFF,F:
+@A00604:387:HLC22DSX2:3:1101:32434:30953 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF:FFFFFFFFFFFFF::FF:FFFFFF,FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16712:31125 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20021:31219 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTCATTCTCTCGCACAGTAATATACGGCCGGGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FFFFFFFFFFFFFFF,FFFF:FFFFFF,FFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:11026:31485 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFF:FFFF:FFFF,F:FFFFFFFFFFFFFFFFFF:FFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1101:14416:31814 2:N:0:AGAGGATG+GGACTACT
+CTGGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFF:FFFFFF,FFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11831:31845 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:2736:32002 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:19009:32002 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28565:32080 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCTAAGCTGTTTCTCCCTCTCGCACAGTGATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTTGGAATTGTCTCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,F:FFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21251:32095 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTAGTAGTATGCCCAACCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
++
+FFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFF,FFFFF,FFFFFF:FFFFFFFFFFFFFF,FFFFFFFFF:F:FFFFFF,FFFFFFFFFF:FFFF,FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16957:32236 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:,FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:F,FF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:13304:32362 2:N:0:AGAGGATG+GGACTACT
+CTGACCCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCACCCTCGCACCGTAATACACGGCCGTGTCCTCCGAGCTCAGGCTGCTCAG
++
+FFFF,:F:,FF::FFFFFFFFFFFFF,FFFFF,,FF,F,F,,FFF,FFF,FFF:FF,::FFFF:F:FFF:FFFFFFFF,F,FF:F,FFF:FF:F,,FFF:F,F:,F::F:,,F,F:FFFF:FFF,FFF,FFF:,FF,FFFFF::F,:,FFF
+@A00604:387:HLC22DSX2:3:1101:15799:32424 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:F:FFFFFFFF,F:F,FFFFFFFFFFF:FFFFF:FFFFF:FFF,FF
+@A00604:387:HLC22DSX2:3:1101:12228:32440 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9679:32503 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTTGACGTAGCAGCTACCACCACTACAAGATCCTAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCT
++
+FF:FF,FF,FFFFFFFFFFFFF:FFFFFFFF:,FFFFFFFF:FFF,FFFFFF,:FFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:,FFFFF:FFF:,FF:FF:FFF,F,FFFFFFFFF:FFFFF:::FFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1101:25373:32784 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FF,F:FFFF,FFFFFFFFFFFFFFFFF:,FFFF,FFFFFFFFFFFFFFFFF,FFFFFF:FFF::,,:FF:FF,FF,F
+@A00604:387:HLC22DSX2:3:1101:30553:32800 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTACACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGAAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTACTACACGGCCGTGTCGTCAGAGCTCAGGCTCCTCAGCTCCATGTAGGCAGT
++
+FF,FFFF:FF:,,FFFFFF,F,F:FFFF:FFFF,FFFF:FFFFFFFFFF:,,F,FFFFFFFF,FFFFFFFFF:FFFFFFF:,FF:,F:FF,FFFFFFF:,,FF,,F,:FFF,F:FFF::F,,FFFFF:FF:FFFF,FFFF,,F,,FFF,FF
+@A00604:387:HLC22DSX2:3:1101:9444:32847 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:27832:32878 2:N:0:AGAGGATG+GGACTACT
+CAGAACCGCCTCCACCACTCTAGACGTAGACCATTGACCCATGGCCCCAGACATCAAAAGCACCTAAGACGTACAAGCCACTGCTAAACCCGTCCTTGGCCTCCCTCTCACAGTAATACACGGCCTTGTCCTCCGATCTCAGGCAGATCAG
++
+F,FFFFF,F,FFFF,FFF,F,F,:F:,,,:F,FFF,,:,,,F,:FF,::,FFF,FFFF,,F,,F::::,FF,FF,,,,:FF,,:,F,,F:FF,F::FFF,F,FFFFF,FFF,,F,FF:FF:F,FF,,:FFFFF,F,:F,F:F,,,,,,,FF
+@A00604:387:HLC22DSX2:3:1101:2356:32941 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF:FFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFF:FFFFFFF:FFFFFFFF:FFFFFFFFF:FFFFFF:FFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32398:32957 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFF:FFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:14886:32972 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCGTCATCGTAGGGGCTATACAGCGCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:27263:32988 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FFFFFFFFFF,FFF:F:FFFF,:FFFFFF:FFFFF:FFFF:FFFFFFF,::FF:FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:4734:33144 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:31313:33176 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTACACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGTGAGAACTGGTTCTTGGATGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:29848:33270 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11704:33442 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28040:33458 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATAACGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+::FFFFFFF,F:FFFFFFF:FFFFFFFFFFF:FFFFFFFFF,FFF,FFFFFFFFF,FF,,F,FF::FFF,:,FFFFFFFFFF::FFFF,F:FFFF::FFFFFFFF,FFFF,FFFFFFFFFF,FFFFF:FFFFFF,:FFFFF:FFF,,FFF:
+@A00604:387:HLC22DSX2:3:1101:30120:33583 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFF:F:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:F:FFFFF
+@A00604:387:HLC22DSX2:3:1101:28772:33630 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32226:33943 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:29668:34021 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,:FF
+@A00604:387:HLC22DSX2:3:1101:19416:34209 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11858:34334 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FF:FFF:F:,FF,FFFF,FFFFF,FFFFFF,FFFFFFFFFFF:FF:FFFFFFFF,FFFFFFFF::FF:FFFF:FFFFFF,FFFFF
+@A00604:387:HLC22DSX2:3:1101:26196:34334 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20491:34350 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF:FF,FFFF,FF
+@A00604:387:HLC22DSX2:3:1101:22887:34491 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGTAGTCAATCCCCCCATGACCAGCCACTGCGGCGCGTGCACAATAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1101:25617:34648 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3766:34851 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:14091:34851 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:13422:34914 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACCGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFF:FFFFFFF,,FFFF:F,,FFFF,F,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF::FF:FFFFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1101:30572:34961 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21395:34976 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACAGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
++
+,FF:FFFFFFFFFF,:FFFFFFFFFFF:FFFFF,FFFFF:FFFFFFFFFF,FFFF,FF::FFFF,FF,F:F,F:,FF:FFFFFFFFFFFFFF:FF,FFFFF,FFFF,FFFFFFFFFFFF,:FF::FFF:FFFFF,F,FFF,F,F:FFF,FF
+@A00604:387:HLC22DSX2:3:1101:10276:35102 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:23619:35227 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:14534:35274 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCACCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGATTTAAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+F::FFFF,:::FFF,,F:FF:FF:FFFFFF:,F:,:,F,FFF,FF,FFFF,:FFF,:F,FF:F,FFF:,F,FFFFF:FFFFF:FFFFFFF,,FFF:,:F:FFF,:FF:FFF:FFFF:F,,,,FFF,FFF,:FFFFF,:,,FFFFF,F,FFF
+@A00604:387:HLC22DSX2:3:1101:13078:35352 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAATTCCCCCTCGAGAATAGCAGCTACCACCACTACAATATCCTACTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+,FFFFF:FF:FFFFFFFF,FFFFFF:FFFFFFFF:FFFF:FF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,F:FF,F,FFFFFF:FFFFFFF,:FFF:FF:F:FFFFFF:FF:FFFF:FF::FFFFFFFFFFFF:FF,FFF:FFFF:
+@A00604:387:HLC22DSX2:3:1101:19633:35493 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20428:35493 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9272:35556 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:24948:35587 2:N:0:AGAGGAGG+GGACTACT
+CCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFF:FFFFFFFFF:FF:FFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:2826:35853 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFF,FFFFFFFFFFF:FFFF:,FFFF:FFFFFFFFF,FFFFFFFFFF,:FF:FFFFFFFFFFFFFFFFF,FF:,FF,FFF:FFFFF,F:,FF,FFFFFFFFFFFFFF,F:F:FF:FFFFFF:FF:FF:FFFFFFF:FF,F,:FFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:11595:35916 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9878:35978 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1101:2519:36010 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFF:FFFFF:FF,FFFFFF:FFFFF,F,FFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:2899:36041 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCCGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+F:FFFFFF:FFFFFF:FF::FF,FFF::FFFFF:FFFFFFF:FFFFFFFF:FF,:FFFFFFFFFFFFFFFFFFFF,:FF:FFF:F,FFFF:F,FFFFF:FF:,F:,F:FFFF:FF:FFFFFFFFFF,FFFF,F:FF,FFFFFFF,FFFFF,
+@A00604:387:HLC22DSX2:3:1101:5547:36213 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:7699:36245 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCACACCGTATTCGTAGCAGCTACCACCACTACAATACCCCTCCCCCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFF:FFFFFFF,FFFFFF:FFFFFFFFF:F:FFF,F:FFFF::FFF,FFFFFFFFFFF,FFF,FFFFFFFFFFF:F,F
+@A00604:387:HLC22DSX2:3:1101:23502:36464 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGACCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTGCATTTGCAGATACAG
++
+:,FFFFFFFFFF:FFFF,FFFFFF,F:,FFF,F:FFFF,,F,F,F,FFFF,F:,FFF:FFFFFF:FF:FFFFF:,FFFF:,,,F,:F:F,FFF,FFF:,F,FFF,FFFF::FFFFF,FF:FF::FFFF:FFFFFF,FFFF:FFF:,:FF:F
+@A00604:387:HLC22DSX2:3:1101:17508:36479 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFF:FFFF:FFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFF,FF:F:FF,FFFFFFF:FFF:FFFFFF:FFFFFFFFFFFFF,F,FFFF:F,FFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:10954:36526 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:29333:36605 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGAAGGTGACCAGGGATCCCTGCCCCAAGACGACCAAAGCGCCGAAGTAATAATCACCAGTATCATATTAATAAATGTGTGCTCTCGCACAGTAATACACAGCCGTGACATCATATCTCAGGCTGCTCAG
++
+F,,FF,,,::,F,FFF,F,F,F,F,:FFFFFF,:,,,F,,FF,,:FF,:,FF:,,FFF,FF,F,:,F:F:FFF,:,:,,F,::,:,,F,FFF,FFFF,FF,,FFF:FFF:FFF::,FFFFF:FF,,,F:,,FFF,FFF,FF,,FFFF:,,,
+@A00604:387:HLC22DSX2:3:1101:25319:36699 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTAGTACCAGCCACTGCTATACCCGGCCTTGGGCTCACTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFF:FFF,,F,FFFFF::FFFFFFFFF:FFF:FFFF:FF:FFFF,FF::FF:FF:FFFFFF,:FFFFFF,FFFF,FFFFF,FF:FF,F:FFF,FF,FFFF,F::F:FFFFFF,F:FF:FFFF,FF,,FFF:FF:FFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:10158:36714 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCAGCCACTGCTATACGTCAGAGCTGTTGCACAGTAGTACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGT
++
+FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:12735:36730 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAAGAAGTCAGCTGCTGCTATAAGGGTCCGTGCACAGTAATACGTGGCTGTGTCCACAGGGTCCATGTTGGTCATTGTAAGGACCACCTGGTTTTT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11451:36761 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCAACCACTCGAGACGGAGACCAGGGTTCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGAAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFF,:,:F,FFFFF,F,FFFF,:,FFFFF,F:,,FF,FFFFFFFF,FFF,FF,FF:FFFF,,,,FFF,FFF:FFFFFFF:,FFFF,FF,:FFFF,FFFFFF,F,FFFFF,FF,,FFF,:FF,FFFF,:FF:,,FF:FFFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1101:29234:36777 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:12870:36808 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:26223:36855 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:28049:36855 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACACAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFF:F:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFF,F::FFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFF:FFFFFFFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:4924:36949 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATACGAGATCGTAGCCACGTCACGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFF:FFFFF:FFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFF:,FFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12038:1047 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5430:1063 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFF:F:F:FFFFFFFFFF:FFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:FF,FFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:14317:1360 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFF,FFFFFFF,:F:FFFFFFF,FFFF:F,FFFFFFFFFFFFFFF,FFFFFFF:FFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFF:,FFFFF,FFF::FFFFFFF,FFFFFFF:FFFFFFF:F:FFFF::FFFFFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:4996:1438 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFF:FFFF,FFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:14796:1438 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FF:F,FFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27019:1501 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFF:F,FFFFFF
+@A00604:387:HLC22DSX2:3:1102:11134:1548 2:N:0:AGAGGAGG+GGACTAAT
+CTGAACCGCCTACACCACTCGAGACGGTGACCGTGGTCCCTTGACCCCAGTAGTCAAAGTCAAAGTAATAACAACTACTATACATGGCGATTTTCGCACATTAATATACGGCCGTGTACTCGGCTCTCAGGCTGTTCTTTTTCAGATACAG
++
+,FFFF,FFF:,,F,FFF,,F,FFF:,FFFF,:,F:,F:,FF:,,,F:,FF,F::,FFF,,F,FF:F:FFFFF,F,FF,FF,F,F:F,:F::F,F:,,FFF,,FF,FFFF:,FF,F,F,:FFF,,F:FFFF::F:FFF,,F:,FFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:22896:1689 2:N:0:ACAGGATG+GGACTACA
+CTGAACCGCGGCCACCACTCGAGACGGTGACCAGGGTTACCTGTCGCCAGAATGCAATGCCAGCAAATGCCTAAGCTCTTGCACAGTAATCAACATCCGAGTACTCGGTAGTGACATATTTAAGATGCAGGGAGAACTGGTTCTTTCATGT
++
+FFFFFF,,F,,F::F:,FFFF,,:F:,FF:,,F,,,F,,FF,:,F,,F:F,F,,,F,,,FFFFF,F:,,F,:,:,FFFFFF,::F,F,FF,F,,F,F,,,,F:,::F,,F:F,,,F,F,,,,F:,F,FFF,FFFF,,F,F,FF,F,,FF,F
+@A00604:387:HLC22DSX2:3:1102:25726:1705 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:19325:1799 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:8160:1908 2:N:0:AGAGGATG+GGACTACT
+CTGCACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACCTGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGAGACAG
++
+FFF,FFFFFF:FF:F:FFFFFF:FFFFFFFFFFF:FF:FFF:FFFFFFFF,FF:FFFFFF:FFFF:,,FFFFF,F,F::FFF:,FFFFFF:,,:FFF:F,F::FF:FFFFFF:F:FFFFFFFFFFF,F:FF:,F,F,:,FFFFFFF,:FFF
+@A00604:387:HLC22DSX2:3:1102:18231:1939 2:N:0:AGAGGATG+GGACTACT
+CGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTCTGCCCTGGAGCTTCTGTGCATAGTTTGTGCCACCACTGTTAGGGTTGATCCATCCCATCCACTCAAGCCCTTGTCCA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:25735:2002 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:24578:2065 2:N:0:AGAGGCTG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCATCTCTCAGGCTGTTCATTT
++
+FFFFFFF:,FF:FFF:FFFFFFFFFFFFFFFFFFF:,,FF:F,,:FF,::F:FFFFF,:F,F,F,:FFF:FF:FF:FF:FFFFFFFF:FFFFFFF,F:FF:::FF,F,FFF:FFF,:F,F:FFF,F:FFFFF,FFFFFFFF:,F:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:17852:2127 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATAATCCCCAGTTGTGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1102:28646:2127 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF,,F:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FF:FFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6280:2190 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:15935:2190 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF,FFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:19208:2253 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTCGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTGGGGCTCTCGCACAGTCATATACGGCCGTGTCCTCGGCTCTCAG
++
+FF:FFF:FFFFF:::FFFF,FFFFF,::FFFFFFFF,F,FFF,F:F,:FFF::,FFF,F::FF,FFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFF:FF:F,FFFFF:FFF:F,F,,FFFFFFF:FFF,:FF,:FF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:14045:2394 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:27471:2440 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCCAGACGCTGACCGAGGTCCCTAGCCCCCAGTAGTCAAAGTACAATTAATAACCACTACTAAACATGGCGCATATCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTCTTCATATCAACAAACAG
++
+,FFFF,:FFF,::FF:F:::,F,F,:,F,F,:,,,FFFFF,,,FF,:F,FF:FFFFF,,F,FFF,,F,FFFFFFFF,F:,,FF::F,F:,,F,:FFFFFF:,FF,FFFFF,FFF,F,FF,:FFF,FF:F,FFF,:F:FF,,,,:,F,::F:
+@A00604:387:HLC22DSX2:3:1102:18502:2534 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:28556:2628 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9950:2942 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAATTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+F:FFFFF:FFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFF:FFFF:,F,FFFFFFFFFFFFFFF::FFFFF,FF:FFFFFF:FFFFFFFFF,FFFF:FFFFFFF:FFF:FFFFFFFFF:F,F,FFFF:FFFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1102:9462:2973 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:
+@A00604:387:HLC22DSX2:3:1102:25708:2988 2:N:0:AGAGGATG+GGACTACT
+AAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTTGGAATTGTCTCTGGAGATGGTGAACCGGCCCTTCACGGAGTCTGCGTAGTATG
++
+F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,:FFFFF
+@A00604:387:HLC22DSX2:3:1102:32805:3129 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:32145:3239 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:17499:3552 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+:FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFF::FFFFFFFFFF,:F,FFFFFF,FFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1353:3583 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6054:3583 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FFFFF:FF,FF,:FF
+@A00604:387:HLC22DSX2:3:1102:2456:3991 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACACGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGGCCCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTC
++
+FF:FFFFFFFF:FFFFFF,:FF:FF:F:FFFFFFFF:::FFFF:,F:FFFFFFFFFF:FFF,FFF:FFFFF,:FF:FFFFF,:FF,:FFF,FF,FFFFFFFFFFFFFF,FFFFFFF,FFFF:F:FFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11234:4131 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:4842:4178 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGATATCAAAAGCATCGGTGTCATCCCCTTTATAATAACCACTCCAAAAATCGTAATACGTTCGAAGCGGGCCACTCGCACAGTACTACACGGCCGTGTCGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:F:F,FFFFFFFFFFFFFFF:F:FFFFF:FFFFFFFFFFFFFFFFFFF:F:FFFFFFFFF,FFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:15854:4178 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5737:4194 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFF:FF,FF,FFF:F,FFFFFFFFFFFF,F,FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:F,FFF
+@A00604:387:HLC22DSX2:3:1102:16224:4225 2:N:0:AGAGGATG+GGACTACT
+CGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFF:F,FF:FFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:29939:4241 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27968:4366 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1102:25907:4460 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:29812:4523 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9335:4601 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFF:FF:FFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:9263:4695 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FF:FFFFFFFFFFFFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:10031:4711 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCACCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCCCTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF,,FF:,::F:FFFF:F::FFF,:FFFFF,:FF:FFFF:,:F,F:FFF:FF:F,FFFFF:FFFF::FFFFFF:FF,:FFFF,FFFFF:FFF:FFFFFFF:FFFF:,F,:F:FFFFFFFFF,F,FFFFFFFFFF,:FF:FFFFFFFF,
+@A00604:387:HLC22DSX2:3:1102:22236:4930 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30038:5040 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9263:5321 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATCTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:2103:5415 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCGCGCACAGTCATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+:FFF,FF:FFFFFFFF:F,FFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFF:FFF,FF,,FF,FFFF,F:FF::FF,FF,FFFFFFFFFFF,FFFFF,:F,FFFF,FFFFF:FF,FF,F:F:FFFFFFFF,,FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:2691:5556 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFF:FFF:FFF,FFFFFF,FFFFFFF:::,,:,FF:FFFFFFFFF:F:FF:,FFF,FFFFFF,F:FFFFFFFFFFF:FF,FF,,F,F,FFFFFFF,F:F
+@A00604:387:HLC22DSX2:3:1102:9426:5635 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11659:5682 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCGTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FF,FF,FFFF:F,
+@A00604:387:HLC22DSX2:3:1102:30481:5682 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30879:5776 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:9525:5838 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCCGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCCGCTC
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FF:FFF,FFFF,FFFFFFF:FFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF:FF,FFFF
+@A00604:387:HLC22DSX2:3:1102:26151:5854 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGGGGATTAAGTAGCAGCTACCACCACTACAATACCCGAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6912:5885 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACCCACAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FF,,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11785:5901 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
++
+FFFFFFFFFF::FFFFFF,FFF,FFFFF,FFFFFF:FFFFFFFFFFFFFF:FFFF,F,FFFFFFFFFF:,FFFFFFFFFFF:FFF:,:FF,FFFF:F::FFFFFFFF,,FF:F:F,FFFFFFFFF:FF:FFFF:FFFFFFFFFFF:FF,FF
+@A00604:387:HLC22DSX2:3:1102:8214:5916 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+F:FFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF,FFFFFF:FFFFFFFFFFFF:FFFFFFFFF::FFFFFF:F:F:,FFFFF:FFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:23312:5979 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:18891:5995 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:18891:6026 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:27914:6057 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFF:,FFF:FFFFFFFFFFFFFFFFFFF:FF,FFFFFF:FFFF:FFF:FFFF,FFFFF,,FFF,FFF,F:F::FF
+@A00604:387:HLC22DSX2:3:1102:6108:6151 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF,F:FFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:27968:6151 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1102:32090:6245 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCACTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:29396:6339 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTAAGCTG
++
+FFFFF,FFFFFFFFF:FFFFFFFFFF,:FFFFFFF:FFFFFF:FF,FFFFFFFFFFFFF:FFF:FFF:F:FFFFFFF:FFF,FFFFF,FFFF:,FFFFFF:FFFFFF:F:FFFF:FFFFFF,:,:FFFF::FFFF:FFFFFFFFF,FFF:F
+@A00604:387:HLC22DSX2:3:1102:25229:6480 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFF,F,:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11442:6558 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:4227:6903 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:F:,,FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:8187:6903 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFF:FFF,:FFFFFFF,FFFFFF,F:FFFFFFFFFFF:FFFFFF:,F,F:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:3893:6918 2:N:0:AGAGGCTG+GGACTACT
+AAGGTGAATCCAGAGGCTGCACAGGAGAGTCTCAGGGACCCCCCAGGCTGTACGAAGCCTCCCCCAGACTCCACCAGCTGCACCTCGGCCATGGCCGGCTGGGCCGCATAGAAAGGAACAACCAAAGGAATTGCGAATAATAATTTCTCAA
++
+F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30219:7106 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCTAAGCCGCTATCAAAGTTTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCCTGTAGGCTGTGTCTGTAGACGTGTC
++
+FFFFFFFFF,F:FFFF:FFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFF,FFFFF,FFF:FF:FF,FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF,:FF:FFFFFFFFFFFF:FF:FFFFF
+@A00604:387:HLC22DSX2:3:1102:5837:7216 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+F:,FFFFFFFFFF:FFFFF,FFFFF:F:FFFFF:,:FF:FFF:,F,:,FF:FF:FFFF,FFFFF,,FFF:F,FF:FFFFF,,:,F,:FFFF,FFF:F::FFFF,FF:FFFFFFF::FFFFFFF,,,:,F:,,FFF:,F,FF,FF:F,,,FF
+@A00604:387:HLC22DSX2:3:1102:5737:7232 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGGCCCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTC
++
+FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7636:7263 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9697:7263 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTGGACAGATCTCTCGCACCGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF::FFFFFFF:FFFFFFFFFFFF::F,FFF:FFFF,FFF,FFFF,:FFFFF::FFFF,FFFFFFFFFFFFFF:,,FF,FFF:FFFFFFFFFFFFFF:FF,FFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:24551:7435 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:
+@A00604:387:HLC22DSX2:3:1102:2040:7498 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1226:7529 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFF:FFFFF:FFFFFFFF:FFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,F:FFFFFFFFFFFF:::F,FFF:FF:FFFFFFF,,,FFFFFFF:FFFF:FFF:FF,FF::FFFFF,
+@A00604:387:HLC22DSX2:3:1102:16622:7607 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCAAAACACGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+,F:,:FF:::F:,F,,F:,F,FFFF,,FFFFFFFFFF:F,FFF:,F:FF:F,,FFFFFFFF,FF,,FF::FF:FF,FFFFFFF::FFFF,FFFFFF:FFFFFF,F:FF:F,FF:FF:FFFFF:FFF:FFFFFFFFFFFF,,::FFF,FFFF
+@A00604:387:HLC22DSX2:3:1102:1371:7686 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F::FFFF:FFFFFFF:FFFFFFFF:FF:FFFFFFFF:FF:FFF,F:FFFFF:FFFFFFFFFFFFFFFFFF,FFFF:FFFFFF::FFF
+@A00604:387:HLC22DSX2:3:1102:8368:7780 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:2591:7795 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,F:F,FFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF::FF,FFFFFF
+@A00604:387:HLC22DSX2:3:1102:7871:7795 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF,FFF
+@A00604:387:HLC22DSX2:3:1102:8486:7795 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5068:7889 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCAACCACTAGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTCCCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+,F,FFF::,FF:,F,,FF:,,FFF,::FFF,:F:FFFF,:FF,F,F,FFFFFF,F,F,FFFFFF::FFFFFF,F:FF,:F,FFFFF:FFFFFFFF:F:FFFFFF::FFFFF:F,F,F,FF,FF,,F,,FFFF:FFF:,F,FF,:F::FFF:
+@A00604:387:HLC22DSX2:3:1102:8467:7889 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:F:FFFFFFFFFF:F:FFFF:FFFF:FFFFFFFFFFF:FFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:14461:7905 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5466:8015 2:N:0:AGAGGATG+GGACTACT
+TAGGTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTCCGCGGCAATCGTGACTCTGCCCTGGAACTTCTGTGCGTAGTTTGCTATACCAAGGATAGGGATGATC
++
+:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFF
+@A00604:387:HLC22DSX2:3:1102:8567:8061 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCGCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:31503:8077 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:3360:8375 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:,FFFF:FFFFFFFFFFFFFFF,:FF:FF,FFFFFFFFFFFFFFF,F,FFFFFFFFFFFF,FFFFFF:FFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:32606:8422 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF::FFFFFF:F,FFF,FFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:29261:8516 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGATATCAAAAGCATGGGGCCCGGAGTAGCAGCTACCACCACTGCAATATGCGGCTCGCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCCCCTCAG
++
+FF,FFFFF::F:FF:FF,,FFFFFFF,F:FFF::FFFFFFFFFFFF:FFF,:F:FFFF::F,::F:FF:F:FF:F,,F,F:,,FFFF,,FFFFF,FF,FFFFFFFFFFFFF,FFFFFFFFF:,FFFFFFF,FFFFFFFFFF,FFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:30454:8641 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:25825:8703 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFF::FFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:31937:8735 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFF:FF:FFFF
+@A00604:387:HLC22DSX2:3:1102:25165:8750 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCATCCACTGCTATACCCGGCCATGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGAACTCAGGCTCCGCAG
++
+FFFFFFF,F,,FFFFFFFF,FF,,F,FFFF:FFFFFFFFF::FFFFFFF,FF,F:FF,FF:::F,,:F,FF,,,FF,F:F:,FFFFFFF,F:FF:,,FFFFF,:FFFFFFF:::,FFFFF:FFF,F,F:FFFF,:F,::::::,:F,,FF:
+@A00604:387:HLC22DSX2:3:1102:3794:9032 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:,FFFF:FFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1102:7039:9048 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFF:FF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFF:FFFFFFFFFFFF,FFFFFFFFF:::FFF::FFFFFFFFFF:,FF,FFFFFF:FF:F,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12626:9204 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFF::FFFFFFFFFFFFFFFFFF:F::,FFFFFFFFFFFFFF:FFF,FFFF,
+@A00604:387:HLC22DSX2:3:1102:7220:9236 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFF:FF,FFFF:FFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFF:F:FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:18765:9408 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1102:1533:9721 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6054:9721 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCAGGTACCAGCCACTGCTCCCCAAAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:9824:9831 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF:FFFFFFFFFFF:,FFF
+@A00604:387:HLC22DSX2:3:1102:4001:10019 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:8874:10034 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:18756:10113 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:28474:10128 2:N:0:AGAGGATG+GGACTACT
+CTGAACCCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12093:10191 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFF:FFFFF:FFFFFFFFFFF:FF:F:F:FFF,:FFF:FFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27805:10191 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF::FFF,FF::FFFFFF
+@A00604:387:HLC22DSX2:3:1102:12219:10222 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FF:FFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:19497:10269 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATCATAAGGTACCACCGAGAGGGTGGAAATATCTTTTGCACAGTAATACAAGGCCGTGTCCTCAGCTCTCAGACTGTTCATTTGCAGATA
++
+FFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11062:10285 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCGCAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFF:F:FF,F,,FFFFFFFFFFF:FF,:,FFFFFFF:FFFF:FFFFFF:F:FF,FFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13747:10394 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:21766:10441 2:N:0:AGAGGATG+GGACTACA
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTAGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+F::FF,FF:F,,:F,FFF::,F,FFFF,:F:FFF,F:FF:F,FF,:FFF,,FFFFFFFF:FFFF,FFFFFFFFFFF:FFFF,FFFFFFFF::FF:,,,FFFFFF:::,F:,,,FFFFFFFFFFFFF:FFFF,FFFF:F:F,F::FFF,,FF
+@A00604:387:HLC22DSX2:3:1102:11903:10457 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFF:F:FFFF:FFFFFFFFFFFFFFF:FFF:FFFFF:FFFFFFFFF,,FFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFF,:F::FFFF:F:FF,FFFFFFFF,FFFFFFFFFFFF,F:FFFFFFFFFFF:FFF:,FF:FF,F
+@A00604:387:HLC22DSX2:3:1102:6325:10473 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF,FFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5412:10488 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6307:10567 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCTCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:32687:10692 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9146:10723 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FFFFFFF,FF
+@A00604:387:HLC22DSX2:3:1102:12590:10927 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCAGCCACTGCTATACGTCAGAGCTGTTGCACAGTAGTACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13792:11005 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:15320:11052 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:6759:11099 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAACGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:24487:11146 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFF,FFFFF,FFFFF:FFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13060:11209 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FF
+@A00604:387:HLC22DSX2:3:1102:18412:11334 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1102:23276:11490 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFF:FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFF:,F:FFFFFFFF:FFFFFFFF,,F:,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5918:11522 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCTCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFF:FFFFF:FF:FFFFFFFFFFFFFFFFFFFFFF,F:FF,F:FFF,F:FFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFFFFFFF::FFFFFF,,F
+@A00604:387:HLC22DSX2:3:1102:23339:11537 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFF::FFF,FFFF:FF:F:FFFFFFFFFFFFFFFFFF,FFFF,:FFFFFFFFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1102:8214:11710 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAATGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFF,FFFF,FF:F,,F,:F:FFFF::FFFFFFFFFF,FF:FFF:FFFF::FFF,F:FF:FFFFFF:FFFFFFFFFFFFFFFFFF:F:FFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1102:11722:11835 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCGTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACTGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFF,F,FFFFFFFF:FFFFF:FFFFFFFFFFFFF,FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:16577:11882 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGTCCAGCCACTGCCGAATCTCTTGCACAGTAAAACACAGCCGTGTCCTCGGGAGTCACAGAGTGCAGCTGCAGTGAGAACTGGTTCTTGGATGT
++
+FFFFF:F,F,:FFFFFFFFF:FFFFFFFFF:FF,,FFF:F,,FFF:F,FFFF:F:FF,,FFF:,,FFFFF::F:FFFFFFF,:FFF,FF,FFFFF:,,:,,FF,:FFF,FFFFFFFFFF:,FF,,:,FF:,FFFFF:,:,:FFFFFF,FF,
+@A00604:387:HLC22DSX2:3:1102:26702:11913 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFF,FF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:
+@A00604:387:HLC22DSX2:3:1102:13006:11992 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFF::FFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:24804:12007 2:N:0:AGAGGAGG+GGACTACT
+CTCTTCAGAGATGTGCTGTAGGATTTTTCGTCATTCGAAAAAATGTGTGCAAGCCACTCCAGGGCCTTCCCTGGGGGCTGACGGATCCAGCTCACACCCATTCTAGCATTGCTGAGTGAGAACCCAGAGACGGTGCAGGTCAGCGTGAGGG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:21504:12117 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGAGCTCAGGCTCCTCAGCTC
++
+FF:FFFFFF:F:FFF:FFFFFFFFFFF:FF:FFFFFFFFFFFFFF:FF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFF,,FF,FFFFFF:FF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:20961:12273 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTCTAAGGTAGAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:16523:12320 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF,FFFFF:F,,FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFF,FFFFFFF,FF
+@A00604:387:HLC22DSX2:3:1102:20139:12383 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTCTAAGGTAGAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFF:F::FFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30490:12524 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF,:FFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFF:FFFF:FFFF:FF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFF::FFF:FF:FFFFFFFFF:::F:F,FFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFF:
+@A00604:387:HLC22DSX2:3:1102:22155:12587 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAAGTAGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCCCCATGTA
++
+FFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFF:FFF
+@A00604:387:HLC22DSX2:3:1102:7762:12618 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCGCCTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:10321:12633 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFF,FFF,FFFFFFFFFFFFFFFFFFFFFFFF::F:FFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:14597:12837 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCATGGCCCCAGGGGTCGAACCACCCACTCAGACGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGAAATACACGGCCGTGTCGTCAGATCTAAGGCTCCTCAGCTC
++
+FF:FFFFF,F,:FFFF::FF:FFFFFFFFF,:FF,FFF::FFFFFFFF:,,FF::,FFFFF,F,FF,FF,,F::,FFFFF:FFFF:FFF:FF,FFF,FFF:FF,FF,FFF,FF,F:FFFFFFF,,,FFFF:,FF:F,,:,:FFFFFF:FF,
+@A00604:387:HLC22DSX2:3:1102:26503:12853 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFF::FFFFFF:F:FF:FFFFF:FFFFFFF,FF,FFF::FFFFFFFFFF,FFFFFFFFFFF:FFF:FFFFF
+@A00604:387:HLC22DSX2:3:1102:12491:12915 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13593:13009 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:18213:13056 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFF,,F,FFF::,FFFF::FFFFFFFF:FF:FFFFFF,FFFFFFFFFFFFF,F::F::FFFF:FF:FFFFF:FFFFFF:,FFFFFFFFFF,FFFFFFFFFF:F:FFFFFFFFFFFFFFFF,F:F,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1054:13088 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF::FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFFFF,FFFF::FF:FFF,FF
+@A00604:387:HLC22DSX2:3:1102:16224:13088 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,F:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF:FFFF:F:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5339:13432 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAACATCGTTTTTCGTAGCATACACCCAACGGGACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:8214:13463 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:3088:13604 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFF:F,F:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFF:FFFFFFFF:FFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:22851:13667 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:3025:13714 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FF:FFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:28429:13808 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF:FFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:1651:14027 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCCTTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFF,F,:F:FFFFFFFF,F,F:F,FF:F,F:FFFFFFFF:FFFFF:F::F:FFFFF:F:,FFF,:FF:FF:,F:FFF,,F,,FFFF:,F:,F:F::F,FFF,F,F::::FFFFFFF:,:FFF:FFF:FFF:FFFFFF::FFFFFF,F
+@A00604:387:HLC22DSX2:3:1102:11460:14074 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFF,F:FF::F:FF:FFFFFFF:FFF,:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11180:14090 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FF:,FF,FF,FFFFFFF:F::FFF,FFFFFFFFF::F:FF:FF:FFF:FF::,:,:FFFF:FFF:FFFF:FFFFFF::,FFFF,FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:31602:14105 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCGATACAACATCAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:F,FFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:17996:14121 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF:FFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFF:FFF:F,F,FFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:17969:14137 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF:FF::FFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFF,:FFFFFF,F:F:F:FFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF:F
+@A00604:387:HLC22DSX2:3:1102:21287:14152 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGAATCACAGACGTAGTCACCGTAGTCATCAGGATCTGATGGCGGGGCCAGTCTCGCACAGTAATACATAGCGGTGTCCGAGGCCTTCAGGCT
++
+,FFFFF,:FFFFF:F:FFFFFF,F:::F,FF:F,FF:FFFF:F,:,F::,FFF,FFFFFF,F::FF,FFF,F,,::,FF:FF:FF,FFF,:F:F,FFFF:,FFFFF:,FFF,FF,FFFFFF::F,FFFF:F:F,FF::FFF,FFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:14362:14184 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:18069:14215 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCCCTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+,F,FFFFF:FFFFF:F:FF,FFFF:FFFFF:FFFFFFFFF:FFFFF,FF:FFF:,FFFFFF,FF:FF,FF:F,FFFF,FFFFF,FFFF::F,FF:F:FFFFFFFFFF,FFF:FF,,FFFFFF:FFFFFF,F:F,FFFFF:F::FFF,FFFF
+@A00604:387:HLC22DSX2:3:1102:5177:14246 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:14253:14340 2:N:0:AGAGGATG+GGACTACT
+GGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGCGGATGTGTCCCTGGTAATGGT
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:23267:14418 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTAGGCCCAAGACATCAAAAGCACAGATGTCGAACCAGCCACAGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACAAGGCCTTGTCCTCAGATCTCAGGATGCTCAG
++
+FFFF:,,::FFF,,:F,FFFFFFF,::F,F,FFF,,FF,:,,,FFF,,,FFFFF,FFFF,F,:,,FFFF,,,F,,FF,FFF,FFFF,F:,,F,FF,FF,,FF,,F:::,,FFFF,,F:,,,FFF:,F,F,,,:FF:FF:,FF:,,FFFFF:
+@A00604:387:HLC22DSX2:3:1102:31566:14450 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFF:FFFFF:FFFFFFFF:FFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1102:15528:14512 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10167:14528 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
++
+:FFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFF:FFF:FFFFFF:FF:FFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFF,FF:FFFFFFFFFFF:FFFF:FFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:25608:14528 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:14931:14575 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,:FFF
+@A00604:387:HLC22DSX2:3:1102:32642:14591 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGTTGT
++
+FFFF:FFF:F:FFFFFFFFFFF:F:FFFFF:F,FF:FFFF:::F:,,F::FFFF,FFFFF,FFFFFFFF:FF,FF:FFFF:F:,,:FFFF::FF:FFFFFFFF:FFFFFF:FF,F:FFFFF,:FF:F::FF,FFF,,F,F,::,FFF,,FF
+@A00604:387:HLC22DSX2:3:1102:29749:14622 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCATACACAACTCGAGAAGGTGAAATTGTTCCATTGACCCAAGAAGTCAAAGTCCAAGTAATAACCACTACTAAACATGGCTCTTTTCGCACAGTAATATACGGACGTGTCCTAGGCTCTAAGGCTGTTCATTTGCAGATACAG
++
+F,FFFF,FF,,,,:F,:,,,FFFF,::,,F,,,FF,F:,,,,::,F,,FF:F,F:FFF,,FFFFFFFFFFFF,FFFF,,:,F,FFF:,,:FF,FFFFFFF:,FF:FFFFF,,FF,F,F::,,,F,FF,FF:F::F::F,,,:FF:F,F,FF
+@A00604:387:HLC22DSX2:3:1102:17210:14826 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGTAGTAGTCCCCGGAGTAGCAGCTACCACCACTACAATATCCCTGATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCAC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFF:FFFFF::FFFFFFF:FFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1102:17336:14826 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:12961:15107 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCAGGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF:,FFF:FFFFF
+@A00604:387:HLC22DSX2:3:1102:10438:15186 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9869:15201 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+:FFFFFFFFFFFFFFF:F,FFFFFFFFFFF:FF:FFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFF::FFFFF:FFFFFFFFFFF:FFFFF:FFFF:FFF:F:FFFFFFFF:FFFFFFF::,FF,:FF,FFFF,FF
+@A00604:387:HLC22DSX2:3:1102:31096:15201 2:N:0:AGAGGATG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGTGTGCCATGGCCCCAGTAGTCAAATGCGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGT
++
+FFFFFFF::FFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFF,FF:F:F,FFFF:FFF:,FF,FFFF,F:FF:F:F:::FFF:F:FF,FFFF,FF,FFFF:FFFFF,FFFFFFFF:FFFFFFF:FFFFF::FFFF,FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:22923:15327 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTACTACACGGCCGTGTACTCAGATCT
++
+FFFFF:F:FFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFF,F,FFFFFFFFFFF:FF,,FF,FFFFF:FFFFFFFFFFF,FF,F:FF:F,FF:FFF:FFF,F,FFFFFFF:FF,FF,FFFFFFF:F
+@A00604:387:HLC22DSX2:3:1102:5068:15342 2:N:0:AGAGGAGG+GGCCTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFF,FF::FFFFFFFF:FFFFFFFFF,:FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFF,FFFFF::FFFFFFFFFFFF:FFFFF::FF:FFFFFFFFF:FFFFFF::,FFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7844:15358 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTAATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:,:FF::,,FFFFF:F:FF:FFF:FFFFF:F:FFFFF,FFF,FF:FFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27028:15483 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10384:15530 2:N:0:AGAGGATG+GGACTACT
+TGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6017:15765 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCAGTTGCAGAGACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,:FFFFFFF:F,FF,,,FF::,FFF:FFFFFFFFF:F,FF::F,::FFFFFF:F:FFFFFF:FF:F,FF::F,F:,,,FFF,FF,,F:F
+@A00604:387:HLC22DSX2:3:1102:32117:15781 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:18683:15906 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTCGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F:FFFFF:FFFF,F:F,F:FFFFFF:F,FFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFF,F,FFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1102:15176:16094 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF::FFFFFFFFFFFFF:FFFFFFFFFF,F:FF:FFFFFFFFFFFFFFFFFFFF:FFF:FFF,FFFF::FF
+@A00604:387:HLC22DSX2:3:1102:17517:16141 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:31530:16141 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCCCCGTAATACTCGGCCGTGTCCTCGGGTCTCAGGCTGTTCATTTGCAGATAGAG
++
+FFFFFFFFFF,:FF:F,FFF::FFFFFFFFF:FFFFFFFF:FFF:FFFF:F,,F:F:FF:FFF:F,:FFFFF:F,,:FF,:,F,,F,F,,:F:FF:F,F,FF:,,F,FF,:,,FFF,::,F:::,,:,FFF,,F,:,::FFFF::,FF,F:
+@A00604:387:HLC22DSX2:3:1102:31557:16219 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
++
+FFFF::FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFF,F:FFFFFFFFFFFFFFFFFFFFF:F,::FFFFFF:,FF:FF:FF:FFF:F:FFF,,FF:F,,FF:F:FFFFF:FF,:FFFF,,,F:,,::FF,FFFFF:F,FFF,:
+@A00604:387:HLC22DSX2:3:1102:6759:16360 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCCGCTC
++
+FFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFF,F,,FF:FFFFFFFFFF:F:FFFF,FFFFFFFF,,FFFFFFFFFFFF,FFFFF:FF:FF:FFFFF:FF,FFFF
+@A00604:387:HLC22DSX2:3:1102:25391:16470 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFF::FFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFF:,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:19108:16485 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFF:,FFFF:,FFFFF,,FF
+@A00604:387:HLC22DSX2:3:1102:4318:16517 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF:FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFF,FFFFF:FFFF::FFFFFFFFFF::FFFFF:F:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:22019:16548 2:N:0:AGAGGATG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
++
+:FF:FF,F::FFFF:F:,:F,FF:F::FF:FFFFF::FF:,:F:::FFFFFFF:F:FF:FFF:F,,F,::,F,F:FFFFFF,,,,FFFFFFFFFF:,FF,,FF:,:::,:F:FFFFF:FF:F:FFFFFFFFFFFFFF:FFFFF:FFFFFF:
+@A00604:387:HLC22DSX2:3:1102:3974:16830 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFF:FFF:FFFFF::FFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFFFFFFFFF:F:FFF,FFFFF,FFFFFFFF:,FFFFFF:FFFF,FFFFF::FFFF:FFFFFFFFFF:FFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1102:25572:16971 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTGGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGATGT
++
+FFFFF,:FFFFFFFFFFFF:FF:FFF,F,FFFFFFFFFFFFFFFF,:F,F:FF,F,FF,FFFFFF:FFFFFFF:FF:,F,,F:FF:FFFF,:::FFFFF:F:FFFF,FFFF,,:FFF,FF:F,F:,F,,FF::F,FFFFF,:F,,FF:FFF
+@A00604:387:HLC22DSX2:3:1102:21513:17018 2:N:0:AGAGGATG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:F:F:F:FFFFF:FFFF:FFFFFFFFF:FFFFFFFFF,FFFFFFFF:FFFFFFF,FFF::FF:FFF,F
+@A00604:387:HLC22DSX2:3:1102:29704:17049 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCTCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:14724:17159 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+F,:FFFF:F:FF:FF,FFF,FFFFF:FFFF:FF,,,,F,:FFF:FF,:FFFF:FF,:F:FFFFFF,:F,FF:FFFFFF,FFFFFFF::FFFFF:::FFFFF,FFF::FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,F:FFF:::FFFF
+@A00604:387:HLC22DSX2:3:1102:8919:17440 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF,FF:FFF:,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5159:17628 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:20419:17754 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:::FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFF:FF::FF:FFFF:FFF:FFFFFFFFFF:F,
+@A00604:387:HLC22DSX2:3:1102:19171:17816 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27362:18098 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:5936:18129 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFF:FFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:31548:18239 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:28908:18333 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFF:FFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:15863:18349 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:19642:18380 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCGCAGCTCCAGGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF:FFFFFFF:FFFFFFFFFF:FF,FFFFFFFF,FFFFFF:FFFFFFFFFFFFF,FFFFFFF:,FFFFFF,FF
+@A00604:387:HLC22DSX2:3:1102:15393:18411 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:25943:18458 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFF:FFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:2211:18505 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCAGTTGAAGATACAG
++
+FFFFFFF,FFFF:F,FFF:,FF:F:F:,,FFFF,FFFFFFF:FFFFFFFFF:FFFFF:F:FFF,F:F:::F,FFFFF,,:FF::,FF,FFFFF,,FFF::FF::F:F,F::FFFFF:F:,,FFFFFF::FFF,FF:F:,:FF,F:FFFFF,
+@A00604:387:HLC22DSX2:3:1102:21703:18505 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,:FF::FFFFFFFFF,FFFF:FFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6244:18599 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAGGAGTAGCTCCCACTATCGGTCTTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFF::FFFFFFFFFFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:17454:18850 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTTCCCCAGCACGTAGTCACCGTAGTCGCCACCTAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30807:18865 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12264:19132 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12246:19194 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGGAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF:F,FF:F,F:F,FF:FF:FFFF,FFFFF,,F:FFF:FFF:F,:F,FF:FF:FFF::FFF:FF:F:F:F:FFF,FFFFFFFFF,FF,F:FF,FF,:FFFF:,FFFF:,F,F:F:FFFFF:FF:FFFFFFFFF,,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:17589:19210 2:N:0:AGAGGATG+GGTCTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGGAATAACCACTACTATACTTGGCGCTTTTCGCACAGTAATATCCGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
++
+FFFF:FF:FFFFFFFFFFFFFFFFFF,FF,FFFFFFFFFFFFF,FF:FFF:,FFFFFFFFFF:F:,F,,F:FFFF:FFF:FFF,:F:FFF,,FF::FFFFF,F,F:F,FFFFFF:FFFF,F::FFFF:,FFF:F:FF::,FFFF:FF,FFF
+@A00604:387:HLC22DSX2:3:1102:12391:19257 2:N:0:AGAGGAGG+GGACTACT
+CTGAACAGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:3784:19319 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGACCTCAGA
++
+:F:FF:FFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFF:FF,FFFF:FF:FFFFFFFFFFF:FF:FFF,,FFFFFFFFF,FFF:FFF,F,::FFFFFF:FFF:F,:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:13087:19335 2:N:0:AGAGGATG+GGACTACT
+CTGGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAG
++
+FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:30734:19398 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:8919:19476 2:N:0:AGAGGAGG+GGACTACT
+CTAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFF:FFFFFFF,FFFFFFFF,FFFF:,FF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FF,F
+@A00604:387:HLC22DSX2:3:1102:25075:19586 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:19027:19633 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FF:FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFF,:,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:20772:19648 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
++
+FFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:6099:19695 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF,:FFFFF:FFFFFFFFFFF:,FF
+@A00604:387:HLC22DSX2:3:1102:6343:19805 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,FFFF,FFFFFFFFFFFF:FFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30924:19820 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9272:20149 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:29107:20181 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:4200:20228 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFF,FFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFF,F:FFFFFFFFFFFFFFFFF,:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27543:20290 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:25943:20306 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+,F,FF::,FF,FF:,FFF:,FFFFFF,:,F:FF:F,FF,FF,,F,FFFF:F:FFFF::F:F::F,FFFF,,,,F::FFFFF,FF,FF:,,F,:F,::FFFF:,FF,F,F,FFFFF:FFFF::F,F,F,FFFFFF,::FF:F::FF,,F,FF
+@A00604:387:HLC22DSX2:3:1102:31584:20306 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCTTTCATACACAAAAATCGTTGACAGATCTCTAGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCC
++
+FFFFFF:F::FF:FFFFF,:FF:FFF:FFF,FF,FF:FF:FF:F:FFF::FFFFFFFF,F,F,FFFFF,FF,::FF:F,FF:F:F:FF:F:FF:FFFFFFFF,FFFFFFFFF:FFFFF,:F,FFFF::FFFFFFFFFFF,FFF:F,:FFFF
+@A00604:387:HLC22DSX2:3:1102:1434:20447 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCATCATCGCTATCATAGTCATACTTTTTTCGGCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTC
++
+FFFFFFFFFFFFFFFFF::FFFFFFFFFFFFF,FFF:FFFFFF:FFF:FFFFF:F,FFFFF:FFF,FFF:F,::F,FF,:FFFFFF:FFFFFFFFFFFFF,F:FF,FFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1102:27877:20556 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1102:30264:20556 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTTCGTAGCAGCTACCACCACTACAATATCCCGCGGGGTGGCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFF:FFFFFFFFFFF:FFF,FFFF:FFFFFFFFFFFFFF:FFFFFFFFFFF:FF::F:FFF,FFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFF
+@A00604:387:HLC22DSX2:3:1102:3929:20603 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATCTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:F,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:21811:20697 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:2392:20854 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACACTAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF::FF:FFFF:FFFFFF:FFF:FFFFFF,:FFFFFF,,F,F:FFFFFFFFFFFFFFF,F::FF,FFFFF:FFFF,F:FFFFFF,
+@A00604:387:HLC22DSX2:3:1102:6244:21073 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGAAGTAGTAGTAGTCTGAGGAGCAGCTACCACCACTACAAGATCCTATACCCGTTGTTGCACCGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFF,F,FFF:FFF,FFF,FFF,FF,FFFFF,,::FFFFF,FFF,F,F,:FFF,FFFFF::,,:,,,FF:,,,FF,F:F:FF::,F:::,F:F,FF,FFF
+@A00604:387:HLC22DSX2:3:1102:17662:21151 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFF:FFFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:1226:21183 2:N:0:AGAGGAGG+GGACTACT
+CTGACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
++
+FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFF,F:FFFFFFFF:FF:::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFF,:FFFFF,F
+@A00604:387:HLC22DSX2:3:1102:22046:21198 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFF,FF,,FFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFF,FF,FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13539:21214 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:8422:21245 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFF,F:FF:FFFFFF::FF
+@A00604:387:HLC22DSX2:3:1102:10411:21245 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACCGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFF:
+@A00604:387:HLC22DSX2:3:1102:24578:21386 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:8766:21590 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATAGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+,FFFFFF:FFF::F::FFFF,FFFFF,:FFFFFF,FF,:,:F:F,F,FF,FF:::FFF,FF,FFFF::::FFFF,FFFF,:FFFFFFF:,F:,:FF:FFFF,F::FFFFFF:FFFFFFF:F,:FF,FF:F,FFFFFFF:FFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30789:21715 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGAACAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTCAACCATAGCTGTATCCACGACTTCTCTCGCACAGTAATAAACGGCCGCGTCCTCAGATCTCATGCTGCTCAGCTCCATGTAGGC
++
+FF:FF,FFFF:F:FF,FF:,FF::F:FF:F,FFF,,FFFF,,:FF:FFFFFF,FF:FFFFFFFFFFFFF,FFFFF,,:F:FFFFFFF::,FFF:::FFF,,,,,FF,FFFF:F:F:,:,F:FFFFFFFF,FFFFFFFFFF,:,FF:FFF,:
+@A00604:387:HLC22DSX2:3:1102:8793:21856 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF
+@A00604:387:HLC22DSX2:3:1102:2338:22044 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTACTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FF:FFFFFFFFFFFFFFFFFFFFFF:::,FF,FFF:FF,,F:::FFFF:FFF,FFFFFF,FFF:F:F,,F:FF:FFFF:FF:FFFF,FFFF,:FFFFFFF::FFFFFFFFFFFF,FF,FFF:F:FFFFFF,F,FFF,F,FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:18602:22122 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF,FFFF:FFFF:FFFFFF:FFF,FF:FFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:27434:22232 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACAAGGGTGCCCTGGCCCCAGACGCCCATACCGTAGGCCCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30653:22294 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATAAACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:26901:22404 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,FFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:14633:22670 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:F,FFFFFFFFFFF,F:FFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:23637:22670 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:23457:22733 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATCTCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFF:FFFFFFFFFFFFFFFFF,FFFFF,F,FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFF,F:FF
+@A00604:387:HLC22DSX2:3:1102:29423:22764 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:19687:22936 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,
+@A00604:387:HLC22DSX2:3:1102:9968:22952 2:N:0:AGAGGATG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCA
++
+FFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF,FFF:F,:FFFFFFFFFFFF,FFFFF:FFF,,FF:FFFF,FFFFFFFFFFFFFF,FFF::FFFFF,FF::FF,,FFFFFF,FFFFFF,:FFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:1741:23015 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF,F:FFF:FF:FFFF,FFF::FFFFFFF:FFFFFFFFFF,F,FFF:F,F,FFFFFFFF:FF:FFF::FFF:FFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:5023:23062 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFF:FFF,:F:FF:FFF,,,,F:FF:FFFFFFFFFFF,F,FF,:,:FF,F,FFFFFFFF,,F,F,,,,,FF
+@A00604:387:HLC22DSX2:3:1102:4137:23281 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF::FF:FF:FFF
+@A00604:387:HLC22DSX2:3:1102:28574:23296 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:F:
+@A00604:387:HLC22DSX2:3:1102:24731:23312 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCCGTAGTCAAAGTCCAAGAACTAACCACTAAAAAACATGGCGCTGTTCTCACAGTAATATACGGCCGTGTCCTCGGCAATCAGGCTGTACATTTGCATATACAG
++
+F,,,:::FFFFFFF:,,,F,,:FF:F:F,FFF,FF,FF:FF:,,FFF,,:F:F:FFFFF:F,FFF,::,:FF,,FF,,,F,:,:FF,FF:F,FFF,,,FFF,:F,FFF,FFFF,,F::F,F::,,,::,::F,F,,F,F,:,FF,F,FFF,
+@A00604:387:HLC22DSX2:3:1102:4797:23390 2:N:0:AGAGGATG+GGCCTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCACCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFF:F,F:FFFF,FFFFFFFFFFFF,F,:FFFF::FFFFFFFFFFFFFFF:FF,:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFF,F,FFF::,FF:F,,FFFFFFFF,::,,FFFF,FFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:32841:23390 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF::,FF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1787:23437 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1199:23453 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFF:FFFFFFF::FFFFFFFFFFFFFFFFF:FFFFF,FFF:FFFFFFFFFFFFFFFFFFF::FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:3956:23688 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7853:23735 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGAACAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCCCAGTAATACACAGCCGAGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCGGGGGCTTGGATGG
++
+FF,FFF,::FFFFFFF,F,F::::,:F,,F,FFFFFF,F::F::FFF:::,FF,FF,FFF,:FFF::F,FF:F,,F,F,FF:,FFFF,FFFFFFFFF:F,:,FFFFF:F,,FF,F:F:,,FFF:F:,,FFF::FF,,,F,,,:,,F:F,F,
+@A00604:387:HLC22DSX2:3:1102:1705:23766 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTCCCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+FFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFF,:F:FF:FFFFFFFF:FFFFFFFF::FFFFF:FFFFFFFFF:F:FFFFFFFFFF,FFFFF,,FF
+@A00604:387:HLC22DSX2:3:1102:15591:24048 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCCTTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTACTACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+,FFF::FFFFF:,FFFFF:FFFFFFFF:FFFFFF:F:FFFFFF:FFFFFFFFFFFFFFFFFFFF,FFF,FFFFF::,FFF::,FFFFFFFFFFFFFFF::,FFF,F:FFFFF,FFF:FFF,FFFFFFFFF,:F,:FFF,FF,F,,:FFFFF
+@A00604:387:HLC22DSX2:3:1102:28393:24486 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTAACAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFF:FFFFFFFFFFF,FFFFFFF:F:FFFFF,FF:FFFFFFFFFFF:,,:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:22245:24518 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFF:F:F,:FF:::F,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFF,FF,FFFF,FFF:FFF:FF:FFFFF,F:FFFFF:FF,FFFFFFFF:,F:FFFFFF:F,FFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:9507:24533 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:6641:24580 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:27489:24580 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFF,FFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFF:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:21142:24612 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:32651:24659 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:F:FFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7844:24784 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10339:24909 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFF:FFFFFFFFFFFFF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11794:24956 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:30120:25066 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10122:25191 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1723:25269 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGATATACCCGGCCTGGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+,F,FFF:F:FF:F::F,FFFFF:FFFF,:FFFF:FFFF,F,FFFF,F:F:FFF,:FFF,FFFFFFFFF,,F:FFFF:F:FFF,,FFFFF:FFFFF:,FFFFFFFFFFF::FFFF,FF,FFF,:FFFFFFFFF:FFF,FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:20564:25394 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:22254:25535 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:20329:25551 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:F:FFFFF,F,FFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:9896:25582 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTTGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGACTCCTCGGGAGTCACAGAGTTCAGCTG
++
+F:FFF:F:F:FFFFF,FF,FFF:FF:FFFFFFFFF:FFFFFFFFF,,:FFF,F,:F,,FFFFFF:FFFF:,FFF,F:FF:FFFFFF:FF:FFFFF:::FFF,F,FFFFFF,FFFFFF::,FFF,,:F,FFF::,FFFFFFFFFF,,,:FFF
+@A00604:387:HLC22DSX2:3:1102:23909:25614 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCAACACTCGATACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGAACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCGGCAGGGAGAACTGGTTCTTGGATGT
++
+F,F:FFF:,F,F,F,FFF,,FF,F:FFFFF:,F::F:F,FFF,,FFFF:FFFFFF,FFFFFFFFFFFFF:FFFF::,:FF,,,F:FF:FFFFFFF:F,F::FF,FFF::FFFFFFF:FFF:F,F,,:F,::F,:::FF,F,FF,,F:,,FF
+@A00604:387:HLC22DSX2:3:1102:20916:25629 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF:F:F,FF:FFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFF::FFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1102:30427:25629 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:24451:25895 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:15890:25911 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATCTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1102:15185:25974 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13946:26146 2:N:0:AGAGGAAG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGAAGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGACACTGCTATACCAGGACTTGGGCTCCCTCGCACAGTAATAAACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFF:,FFFF,F,FFFFF,:,,,F,F,F:F,FFF::FFFFF,F,:F:F,FF,FFF,:FF,,F,:FFFF,FF,FFF,:FFFFFFF:F,F,,F,FF:,F:FFF,:,,FF:FF,:FFFF,FF,F:FF,,,F,,FFFF,:F,F,FF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:3577:26287 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F:FF
+@A00604:387:HLC22DSX2:3:1102:31476:26412 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFF::FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:28574:26584 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFFF:F:FF,FF:FF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:28167:26600 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10899:26850 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF,FF:F,
+@A00604:387:HLC22DSX2:3:1102:27064:26882 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCCTCCTCCTCCCAGCCACTGCTATGACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGACGTGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9037:26976 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTCCTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFF:F,FFF:F,F:FFF
+@A00604:387:HLC22DSX2:3:1102:11180:27023 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10221:27054 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:4869:27085 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:F:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13973:27164 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF::F:FFFFFFFF,:FFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFF:F:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12210:27211 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:13521:27289 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFF,F::FFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:22869:27320 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFF:FF:F::FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:11595:27398 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7211:27414 2:N:0:AGAGGATG+GGACTACT
+GTATAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTCCGCGGTAATCGTGACTCTGCCCTGGAACTTCTGTGCGTAGTTTGCTGTACCAAAGATAGGGATGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:10420:27774 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCCGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCCGGGAGAACTGGTTCTTGGATGT
++
+,::F::FFFFFFFF:FFF:FFF,:FFFFFF:FFFFF::FFFFFF,,F,,F:FFFFFFFFF:FFFFF,,:,F,FF:F:F,:FFF,F:FFF:FF:FFFF,F:FFFFF:,F,F::F:FF:FFFFFFFFFFF,,F,FFF,F,FF,,,FF,:F::F
+@A00604:387:HLC22DSX2:3:1102:14778:27774 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:4119:27790 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCCGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFF::FFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:6234:27821 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:21513:27821 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAATTCCCCCTCGAGAATAGCAGCTACCACCACTACAATATCCTACTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:12933:27837 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:16495:27899 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFF:FF
+@A00604:387:HLC22DSX2:3:1102:21368:28040 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFF,FFFFFFFFFF:F:FFFF:FFFFFFFFF,FF::F:FFFFFFFFFFFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:23023:28150 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:16568:28369 2:N:0:AGAGGATG+GGTCTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:21414:28401 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGTTTCCCTGGCCCCAGTAGTCAATGCCAGCCACTGCCGAATCTCTTGCTCAGTAATACACAGCCGTGTCATCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+F,,FFFFFFFFFFFFFFFFFFFFFFF:FFFF,F::,:,F:FFFFFFFFFFFFF:FFF,FFFF,FFFF:FFF,FF,FFF:FFF,FFF:F,FFF:FF:FFF,FFF,:FFFFFF:FFF::FFF,F,FFFFF,F::FFFFF::FFFFF,FF:FFF
+@A00604:387:HLC22DSX2:3:1102:12246:28526 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:1967:28541 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAAAAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFF:FFF:FFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFF,,FFFFFFFFF:FFFFF:FFFF,FFFFFFFF:FFFFFFF:FFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:25672:28573 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,:F:FFFF,FF
+@A00604:387:HLC22DSX2:3:1102:10257:28588 2:N:0:AGAGGATG+GGACTACT
+CTGGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FF:FF:FFFFFFFFFFF,F:FF:FFFFF:F:FFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:10312:28588 2:N:0:AGAGGATG+GGACTACT
+CTGGAACCGCCTCCACCACTCTAGACGGTGAACAGGGTCCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCT
++
+F,:FFF:FF::FF,F,:,FF:,F,FF,FFFF,,F:,,,,FFF:FFFFFFFFF,:FFFF,,FFF:FF:FFFFF,FF:F:F:FFF,FFF:F,F::FFFFFF,,F:::F,,FFF,FFFF:FFF,:FF,:F:FFF:::F:F,,:F:::F,F:FFF
+@A00604:387:HLC22DSX2:3:1102:20835:28651 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACACGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAAAATCTATCTCTCGCACAGTAATAAACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+F,,,FFF:F,,::,,:FF,:,F,FF,FFFF,FFF,FFF:FF,F,,FFFFFFFFFF:F,FFFF,,FFF,FF,FF,FFF,,F,FFFFF,FF:FF,FFFFFFFFFF::,,::::FFFF,FFFF,FF,FF,FFFF:FFFFF:F,,F:FF:F:,FF
+@A00604:387:HLC22DSX2:3:1102:6397:28792 2:N:0:CGAGGATG+GGTCTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTGCTCGTAGCAGCTACCACCACTACAATATCCAGAGCCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFF:F,FFFF,:FFFFFFF,FF:FFFFFFFF,FFFFF:FFFFF:FFFFFFF,FFFF:FFFFF,FF:FFFFFFF:FFFF:FFFFFFFFFF:F:FFF:FFFFF:F,FFF:
+@A00604:387:HLC22DSX2:3:1102:19379:28792 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTACAACACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATCGTCATAAATGTGGGCTCTCGCACAGTAATACACAGCAGTGTCGTCAGATCTCAGGCTGCGCAG
++
+F:F,:,,,FF,,,F,FF,F,,FFFFF,F:FFF:,F:FFFFFF:,:,,,F:FFF:FFF,F,FFFFFFFFFF:FF:FFFF:,::,F:FF,FF,FFFFFF,FFF:,F:FF:FF:,F:FFF:F::FFF,FF::F,FFFF:,:FFFFF:F,,,FFF
+@A00604:387:HLC22DSX2:3:1102:25979:28886 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:,FFFFF:FFFFFFFF:FFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFF,FFF:FFFFFF:FFFFFFFF:FFFFFF:FFFFFFFF:F:FFFF
+@A00604:387:HLC22DSX2:3:1102:3712:28902 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGGTGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAGGTAGGCTGT
++
+FFFFFFF,FFFFFFFFFFFFF:FFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFF:FFFFFFFFF,FFFFF,FFF,FFFFFFFF:F:FFFFFFFFF,F:FFF,FFF:FFFFFFFFF,:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:15393:28902 2:N:0:AGAGGAGG+GGACTACT
+AAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTCTGGGTTGATGGTTATTCGACTTTTCACAGATACTGCATAATCATTATACCAC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFF:FFFFFFFF:FFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1102:21187:29042 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACAACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFF,F:FFFFFFFFFFFFFF:FF:FFF:FF,F:FF::FFF,F:FFF,FFF,F,FFFFFF:FFFFFFF:FFFFFF:FF,F:F,:FF:FF:,FFF,:FFF,:FFFF:FFF,F,FF:F,FF:FF::FF:,FFFF,FFF,F,:FFFFFF,F,
+@A00604:387:HLC22DSX2:3:1102:3685:29168 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:12057:29168 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:F,FF:FF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:19126:29293 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FFF:FFFF::FFFFFFFFFF:FFFFFFFFF,,FFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:28827:29528 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFF:FFFFFFFFFF:FFFFFFFFF:FFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1102:15311:29543 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGAGGTCGTAGCAGCTACCACCACTACAATATCCGCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FF:FFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1102:26775:29543 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1102:16224:29559 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGCGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:F:FFFFFFFF:FFFFFF,FFFFFFFFFFFFFFF:FFFFFFFF:F:FFF:F:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:14760:29590 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFF,:FFFFFFFFF:FFFFFF:FFFFFF:FFFFFFFFFF,FF:FFFFFFFFF:FFFFFF:FFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1102:7771:29700 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFF:FFFF:
+@A00604:387:HLC22DSX2:3:1102:15682:29778 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:18982:29794 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+:FFFFFFFFFFFFFF:F,FFFFFF:FF:FFF:FFF:FFFFFFF:F:FFFFFFFFFFF:F:FFFFFFFF,F:,F:F:,FFF,:F,,:FFF:FFF,FF:::FFFF,FF,FFFFFFF::FFF:,F,FFFFFFFFF,FFFF:F,FFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1102:7645:29825 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFF,FFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1102:9127:29982 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFF,:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files 22% similar despite different names*

```diff
@@ -1,1020 +1,944 @@
-@A00604:387:HLC22DSX2:3:1102:5059:31391 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFF::FF:F:,FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13006:31532 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FF::FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:22923:31641 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGATATCAAAAGCATGGGGCCCGGAGTAGCAGCTACCACCACTGCAATATGCGGCTCGCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCCCCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:20528:31688 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFF::F:FFFFFFFF:FFFFFFFFFFFFFFFFF:FFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFF:FF,F,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7383:31751 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:19045:31876 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6922:31892 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATCCGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACAG
-+
-FFFFFFFF:FFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFF:FFFFFFFFFFFFFFFFF:F:FFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFF:F,FF:FFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13422:31939 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFF:FFFF:FFF,FF:FFFFFFFFF:FFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:20211:32236 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF::FFFFFFFFFFFFFFFFFFFFFF:FF::FFFF,FFFFFFFFFF:FFF:FFFFFFFFFFFFFFF,FFFFFFFF,FFFFFF,FFFF::FFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:20229:32236 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFF:FFF:FFFFFFFFFF:FFFF:FF:FFFFF,FFFFFF:FFFF,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10221:32409 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:14136:32424 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11053:32440 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:,FFFFF::FFF:FFFF
-@A00604:387:HLC22DSX2:3:1102:21124:32565 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTCATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFF,FFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FF:FFFFFFFFFFFFFFF,FFFF:F,FFFF,FFF,FFFF:FFFF:F:FFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:29017:32737 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGATATCAAAAGCACCTAACGGTATCATAGTAGACCCTCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11062:32831 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF,F:FFFF:FFFFF,FFFFFFF:FFFFF:F,FFFFFFFFFF:FFFFFFFFF:FF:FFFFFF:F,F:,FFFFF,FFFFFFFF,FFF:FFFFF:F:F,,:FFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1102:29686:32831 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACCGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:31006:33051 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:F:FF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:5385:33113 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFF:FFFF:FF:FF:,,:FFF:F,FFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1102:18828:33160 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF:FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:10601:33223 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-F:FFFFFFFFFFFFFF,FFFFF:FFFFFFFFFF::FFFFFFFFFFFFFFFF:,FF,,FFFFFFFFFF:FF:FFFFFFFFFFFFF,FFF:FFFFFFFFFF:FFFFFFFFFFFFF:FFFFFF::FFFFFF:FFFFFF:FFFFFFF:,FF:FF:
-@A00604:387:HLC22DSX2:3:1102:15058:33270 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:4435:33317 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCCGACGTCCATGTAGTAGTAGTAGTTCCTCTGATAGTCTGTCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFF:FF,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:13295:33348 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFF,FFFFFFFFFFFF,FFF:F,:F:FFFFF:FFFF,FF
-@A00604:387:HLC22DSX2:3:1102:4490:33473 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATGTAGTAGTAGTAGTTCCTCTGATAGTCTGTCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTAAGGCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFF:FFFF:FFFFFFFF:F,FFF:,FFFFFF:FFFFFFFFF:FFFFFFF,FF,F:F,:FF:FFFFFFFFFFF,F,,FFF:FFFFFF,FFFFF:FFFFFF:FFFFFFFFF,:FFFFFFF,,F:,FF:FFFF,:FFFFFFF,::,
-@A00604:387:HLC22DSX2:3:1102:29215:33583 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:3848:33646 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATGTAGTAGTAGTAGTTCCTCTGATAGTCTGTCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:15447:33661 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGAACGGACGAATCCCGTGTCTGGTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCTGAT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,
-@A00604:387:HLC22DSX2:3:1102:3956:33739 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGAAATACCAGCCACTGCTATAGACGTTAACATTCGACGTAAGATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFF:F,FFF:FF,FFFFFFFFFFFFFFFFFF:FFFFFFF:FFFF:FFFFFFFFFFF:FFF:FFFFF,FF
-@A00604:387:HLC22DSX2:3:1102:13141:33833 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGACGTCCATACCGTAGTAGTTGGGTTCCCGCCATGCTAAATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:23511:34194 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FF:FFFF
-@A00604:387:HLC22DSX2:3:1102:9995:34240 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCCGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-,FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFF,FFFFFFFFFF,FFFFFFFFF:FFFFFFFF:,FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFF,FF,FFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:29812:34303 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:F:FFFFF:FFFF:F::FFFFFFFF:,FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFF,FFFFFF:,FF
-@A00604:387:HLC22DSX2:3:1102:14163:34350 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,:FFFFFFFFFF,FFFFFF:FFFFFFFF,FFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF,FF
-@A00604:387:HLC22DSX2:3:1102:14190:34397 2:N:0:AGAGGATG+GGAATACT
-CTCAACCGACTCAACCACTAGAGACGGTGACCAGGCTGCCCTGGACCCAGTAGTCCAAGTAGTATTTCTAGTAGCAGCTACCACCACTACAATAAACCCCTCTTGCACAGTCATACACAGCCGAGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FF,:F:FF,:,:,:,,FF,,,,,FF,FF,F::,:,,FFFFF:,,,F,FFFFFFF:::,FFFFF,,FFFF,FFFFFF,:,:FFFF,,FFFFFFFF:,:,,F,:,F,FFFFFF,FFFFFFF,FFF,,:FFF::,FFFFFFFFF:FFFFFFF::
-@A00604:387:HLC22DSX2:3:1102:21016:34413 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFF:FF:FFF:FFFFFFF:,F:FFF,FFF
-@A00604:387:HLC22DSX2:3:1102:8495:34460 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF:FFFFFFFF,FFFFFFFFF:FFF:F:FFFFFFFFFFFFFFFFFFFF::F,F,FFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:25238:34554 2:N:0:GGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCATCGTACCAGCCACTGCTATACGCCCGGCCCGCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFF:FFFFFFF:FFFFF:FFFFFFFFFFFFF:FFFFF:FFFFFFFFF,F,FFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFF:F:::F,F:FFFF:FFFFFFFF::FFFF:F,FFFFFFFFFFF,F:FFFF,FFFFFFFFFFFFFFF,F:
-@A00604:387:HLC22DSX2:3:1102:20139:34616 2:N:0:AGAGGATG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCA
-+
-F:,FFFFFF:FFFF,FFFFFFFFFF::FFFF:FF::FFFFF:FFFFFFFF:,FFFFFFF::FFFFFF,FFFFFFFFFFFF,FFFF:FF,FFFFFFFFF,FFFF:,FFFFFFFF:FF:::FFFFFFF:FFFFFF,F,,FFFFFFF,::FFF:
-@A00604:387:HLC22DSX2:3:1102:27552:34648 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFF,FFFFFFFFFFFF,F,FF:FFFFFFFFFFFFFFFF,F:FFFFFFFFFFF:FFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:14380:34788 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGCCACCACTATAGCAGCTGGTACTACTACAATATGCCCCTCCATCTCTCGCACAGTAATCCACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFF,FFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF:FFFF:FFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:12581:34804 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1102:2184:35086 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFF,F::FFFFF:F:FFFFFF,F,FF,:FF,FF:FF:F:FF::FFF:FFFFFFFFFFFF,F::FF:FFFF,F,F,FFFFF,FF,,FF,FFFF:FFFFF:FFF:F,F::FFFFFF:FFFF,FFFF:FF:FFFFF:F:FFFFFFF:
-@A00604:387:HLC22DSX2:3:1102:12735:35133 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,F,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:10728:35227 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFF:FF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FF,FFFFF,FFFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:6686:35274 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FF:FFFFFFFFF:FFFFFFFF:FFFFFFF:FFF,FF:FF,FFF:F,F:FFFFFFFFFFF:FFFFFF,F:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:32145:35493 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACAGATGTCGTACCAGCCACAGCTATACCCGGCCTAGGGCTCCCTCGCACAGTAATACACGGCCCTGTCATCAGATCTCAGGCTGCTCAG
-+
-,FFFF::::::,FF::F:,:,FFF:,:F,FF:F:F,,FF,F::,F::FF:F,F,:FFFF,FF,,,F,,FFF,F:,,,,,F,,,,:F,FF,::::F,,:F::,F,F:F:F:FFF:FFFFFFF,,FF,:,,F,,FF:FFFF::F,:,F,:,F:
-@A00604:387:HLC22DSX2:3:1102:12255:35524 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAGAGTGGTCCCCACTACTATCATAGTAGAGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFF:FFFFFFFF:FFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27091:35571 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF::FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:2600:35587 2:N:0:AGAGGATG+GGACAACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,F:::FFFFFF:FFF,FFFFFFFFFFFF:F:FF,:FFFFFFFF,FFFFFF:FFFFFFF:F,FFFF:FFFFFF,F:FFFFFFF:FFFFFFFFFFFFF,FFFF:
-@A00604:387:HLC22DSX2:3:1102:11966:35650 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFF:,FFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FF:,FFFF,FFFFFFFFFFFFFFFF:FFFFFF:F:FF,FFFFFFFF::FFFFF::FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9164:35681 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FF:FFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:27453:35759 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:25220:35837 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTACTTCCCCGTAGTGTACCAGCTGCTGCTCCATTCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFF:FFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF,F:F:FFFFFFFFFFFFFFFFFFF:FFFFF:F,FFFFF:FFFFFFFF,FFFF:FFFFFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:11822:35869 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTACCTTGGCCCCAGAAGTCAAACCCCCCAATTGTATATAATACAACACCAGAACAATAAATCACTGTTGCACAGACATACACGTCCGACTCAGCATCGCTCAGGATCCTCAGCTC
-+
-F:FFFFF:FFFFFFFF:F:FFF:FF:F,:FFFF,,,,,FFFFF:FFFFFF,F,FF,F,F,F:,,,F,,,,:,,,,,FFF:,FFFF,,,FF,F::,,F:,:,,F:::F,F,::,F:F,,F,FF:,,F,,,:,,,,FFFF:,,,,,,FF,:,:
-@A00604:387:HLC22DSX2:3:1102:27670:35978 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGCGACTCACTGCACCCCCGTAGTTCCAGTTATCGGGTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:28492:35994 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:32551:36010 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:7527:36041 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATAAACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FF:FFFF,FFFFFFFFFF:FFF,FFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF:FF,FF,:FFFFF,FFFFF,FFFFFFFFFF,F:FFFF,FFFFFF,F:FF:FFFF,FFFF:,FFFFFFFFFFFF:FFFFF:,FFFF
-@A00604:387:HLC22DSX2:3:1102:17327:36041 2:N:0:AGAGGATG+GGACTACT
-TCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTCCGCGGTAATCGTGACTCTGCCCTGGAACTTCTGTGCGTAGTTTGCTGTACCAAAGATAGGGATGATCCCTCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:9100:36072 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATACGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFF:FF,FFF:FF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:32624:36198 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FF:FF:FFFFFFFF,FFF:FFFFF:FFFFFFF:FF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:1814:36292 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFF:FF:FFFFFFFFF:FF,:FFF:,F:FFFF,FF
-@A00604:387:HLC22DSX2:3:1102:3902:36558 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFF::FF:FFFFFFFFF,FFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1102:11379:36573 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:F:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFF,FFFFFFFFFF:FFFFF:FFFF,FFFFFFFF,FFFFF:,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FF,FFFFFFFFF:FFFFFFF:FF:FFFFFF,FFFF,FFF
-@A00604:387:HLC22DSX2:3:1102:14271:36573 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFF:FF:FFFF:FFFF:FF:FFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:3188:36605 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:8585:36620 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:9073:36652 2:N:0:AGAGGAAG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACAAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FF:FF:FFFFFFF,FF,FFFFFFF:F:FFFF,FF,FFFFFFFF,FFFF,FF,:FFFF:FFFFFF:F,F,FF:FF,::FFFFF,:FF,FFFF,FFF,FF,:FFFF,F:,FFFFF:F,::F:FFF,FFFFFFFFFFF,,,:FFFFFF,FFFF:
-@A00604:387:HLC22DSX2:3:1102:5710:36839 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGACAAACGCGTAGTCACCGTAGTCACTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGT
-+
-FFFFFF:FFF:FF:FFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFF:FFFFFFF:FF,FFFFFFFFFFFFFFFFFF::FFFF,F:FFF,:FFFFFFFF:FFF:F:FFFFFFF,FF:FFFFF:FFF,FFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1102:6479:36855 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1102:12319:37012 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1103:12138:1031 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFF,FFFF,F,F,FFFF,FFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:12780:1141 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:19325:1172 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:17698:1204 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCACCTGCTATAGGCCCTGTACCCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCATCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:F:,F:F,FF,F:FFFFFFFFFFFFF,,FF:FFF,F,,F,:,,,F,FFFF,FFFF:,FFFFFFFFF,:,FF,:FF,:FFFF:F:FFF,FF:,F,,,FFFF:FFFFFF:,F,
-@A00604:387:HLC22DSX2:3:1103:32533:1501 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-F:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF::F:FFFF:FFF:F::FFFFFFFFFF:::FFF,F:FFFFFF:F,F:FF,,FFFF,FFF::,FFFFFFFFFFF:FFFFFFFFFFF:FF:FFFFFFFFF,FFFFFFFFFF:F:,FFFF
-@A00604:387:HLC22DSX2:3:1103:26802:1595 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCAACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCCTGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF,F,FFFFFF,FFFFFFFFFF:FFF,F:FFFFF:FFFFFF:F:FFFF:FFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:27968:1830 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCACTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCATGCTGCTCAG
-+
-FF::F,:F,,FFFFF:FF,F,F:FFF::F,F,FFFF:F,FF,:F,FF:FFFFFF:FFF:FFF,FFF,,FF,::FFF,:FF,F:FFFFFFFF:FFFFFF::FF:FFFFFFF,:FFFFFF,,FF,:FFFFFFFFFFFFFFFFF,FFF,FF,FF
-@A00604:387:HLC22DSX2:3:1103:18656:1861 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCAACACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1103:15266:1877 2:N:0:AGAGGATG+GGACTCCT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFF:FFFFFFF:FFFFF:F:FFFFFFF,FFFFF:FF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFF:FFFFFFF:F:FFFFFF:FF:FFF
-@A00604:387:HLC22DSX2:3:1103:1344:1939 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCCCCCACGTGGATGTCTCCATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTGCAGATACAGCGTGTTCTT
-+
-F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFF,F:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFF:F:FF,FFFFFFFFFFFFF:FFFFFFFFF:FFFF:FFF,,,
-@A00604:387:HLC22DSX2:3:1103:9082:1939 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTGCTGGAAGTATTCACCAGATTCGTACCAGCCACCACTGTGTGCACAGTAATATGTGGCTGTGTCTACAGGGTCCATGTTGGTCATTGTAAGGACCACCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:F:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F,FFFFF:FFFFFFFFFFFFFFFFFFF:,FFF,:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:26205:1971 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTACGGGGGCGTAGTTACTGTCAGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,F,FFF:FFFFFFFF,F,FFFFF:F:F:FFFF:FFF:FFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:11541:2002 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTACCTGGCCCCAGTAGACAACGTAACAGACACATCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCACAGATCTCAGGCTGCTCACCTCCATTTAGTCTGT
-+
-FF,FFFF,::,FFFFF,F,,,FFFFF,:F:FFF,,FF,,FFF,,FF,,:,FF,,:FF,F,F,:F,,FF:,,FFFFF,F,F,,,FFFF:,:F,,:F::F:::FF:F,,,F,FF,,F,,FF,F,FFFF,,,F,FFFF,FFFFFF,:F,,FF,:
-@A00604:387:HLC22DSX2:3:1103:15772:2096 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FF:FFFF:F
-@A00604:387:HLC22DSX2:3:1103:24126:2096 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:9118:2159 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:10908:2253 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGGCAGCACCCCCTTTCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGAGTTCTTGGCGTTGTCTCT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:23140:2300 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:23466:2362 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF::FFFFFFF
-@A00604:387:HLC22DSX2:3:1103:27850:2409 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGGCAGCACCCCCTTTCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGAGTTCTTGGCGTTGTCTCT
-+
-FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:::FFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1103:30183:2660 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFF:FFFFF,FF:F,,F,F,FF:FFFFFFF::,FF::FFFFFFF,FF,F,,::FFF,,FFF::FF:FF,,FFFFF::F:F,:FF
-@A00604:387:HLC22DSX2:3:1103:21712:2769 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:22670:2769 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAATGAGGGGCCCAAACTATCATAGTAATCAGGGGGAACTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTA
-+
-FFFFFFFFFFFFFFFFFFFFFF,FF,FF,FFFFFFF:FFFF,FFFF,FFF:FFFFFFFFF:FFFFFFFFF,FFFF::,FFF,:F,,FFF,FFFF,FFFFF,FFF,F::FFF,FFFFF:F,:FFFF:FF:FFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:14714:2832 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTGGCACAGTAATACACAGCCGTGTCCTCGGGCGTCACAGAGTTCAGCTG
-+
-FFFFFF:FFFFFFFFFF:FF,FFFFF:::F:FFFFF,,FFFFFFFFFF,F:FFFFFFFF,FF,F,,F,,FF,:F:,:FF,,F,FF:FFFF,FFFFFFF,F:FF,,,:FFF:FFF,FF,F,FF,,FFFFFFF::,:FFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:19976:2832 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1103:19687:3020 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGAAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGAAATACACAGACGTGTCCTCGGGAGTCCCAGAGTTCAGCTG
-+
-FFFFFFFFF,,FFFFF,F:FF,FFF::FF:FFF,:F:,FF,,,F:F:F:,,FF:FF,FF,F:F,,:,FFFF,F:F:FFFF:FF,F,F,FF,FFFFF,F:FFF:FFFF:FF,FFFFF:,F,,FF,FFFF,FFF:F,F:,,FFF,,,:F:FFF
-@A00604:387:HLC22DSX2:3:1103:12735:3098 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFF,:,F:FF,FFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FF,F:FF::FFF:FFFFFFFF::FFFFF:F:
-@A00604:387:HLC22DSX2:3:1103:28872:3114 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:1687:3129 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,:F,FFFFFF,FF:FF:
-@A00604:387:HLC22DSX2:3:1103:7066:3145 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:21866:3192 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCCCTGCTCTACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:9860:3255 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1103:18530:3270 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFF:FF:F:
-@A00604:387:HLC22DSX2:3:1103:8477:3364 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:12744:3364 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFF:FFFFFFF,FFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:22571:3380 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFF:FFFFF:FFFFFFFFFFF:FFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFF:FFFFF,FFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1103:24912:3427 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFF::FFFFFFFFFFF:FF,FF:FFFF,FFFFFFFFFFFF,FF,F:FF::FFFFFF,FFFF::FFF,FFFFFFFFFFFFF,F:FFFFF,F:FF,:F:F:FFFFF,FFF,FFFFFFFFFFFF:F:FFFF,:F:,FFFFFFFF,:FFF:FF
-@A00604:387:HLC22DSX2:3:1103:8106:3443 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCACATATCAAAAGCATTGTAGTAGCTCCCACTCTCTCTCGCACAGTAATACGCAGCCGTGTCTTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGC
-+
-FFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:13630:3615 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAGAAGCATCATCCGGAGGATGGGCCCCATTGTCTTTCGCACAGTAATATATGGCCGTGTCCTCGGCTCTCAGGCTGCTCATTTGCAGATACAGCGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:9290:3646 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:27796:3693 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFF,FF:FFFFFFF:FFFF:FF
-@A00604:387:HLC22DSX2:3:1103:13874:3850 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF:FFF:FFFFFFFFF,FF::FFFF,:FFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:28284:4131 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFF,FF,FFFFF:,FFF,FFFFFFFFFFFF,:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:,FF::F,FFFF:FFFFFFFFFFFFFFF:F:F:FFFF:FF
-@A00604:387:HLC22DSX2:3:1103:24225:4178 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:1145:4288 2:N:0:AGAGGAGG+GGACTACT
-CTCAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCTCCTCCGTAGTTCCAGTCATCCCTCGCACAGTAATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGTGAT
-+
-FF:F:FF:FFFF::FFFF:FFF::FFFFFFFFF,FFFFFFFFFFFFFFFFF,FFFFF::FFFF:,:FFFFF,,FF,FFFFFFF,FFFFF,FFFFFFF,:FFFFFFFFF,FFFFFFFFFFFFFF,:FF:FFFF:,FFFFF::FF,:,:FF,,
-@A00604:387:HLC22DSX2:3:1103:6524:4366 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1103:10113:4413 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFF::,FFFFFFFFFFFFFFFFFFF:F,FFFFFFF,FFF:FF,FFF:FFFFF:,F,FFFFFF:FFFFFFFF:FFF:FFFFFF,FFFFF:,FFFF,FF,FFFF,FF:FFFF,F:F,FF:FFF:F,FFFF:FFFF:FFFFF,FF,FFFFF
-@A00604:387:HLC22DSX2:3:1103:25988:4445 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGTCGATCGTATAGCAGCTGGTTGCCATTCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCAT
-+
-:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:F:FFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFF:FFFF:FFFFFF:FFFFFFFFF:FFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:4209:4523 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:25870:4554 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFF:F:FFFFFFFF:FFFFFFFFFFFFFFF:FFFF,FFFFFF,FFFF,FFF,FFFFFFFFF:FFFFFFFFFFFFFF:FFF::FFFFFFFF:FFFFFFFFFFFFFFF,FF,FF::FFF:FFFF:FFF,FFFFFFFFFFFFF,FFFFF
-@A00604:387:HLC22DSX2:3:1103:10456:4570 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFF,:FFFFFFFF::FFF:F::FFFFFFF:FF:FFF,F,F,F,FF:FF:FF:FFFFFF:FFF::,FFFFFF:F,FFFFFF:FFFFFFFF:::,F,,FFFFFFF,:F:::::F:F::FFFFFF:FFFFFF:FF,,FFF,FFFF:F:,F
-@A00604:387:HLC22DSX2:3:1103:27407:4617 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFF:FFFF:FFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:7256:4633 2:N:0:AGAGGCTG+GGACTAAT
-CGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFF:F:FFFFFFFFF:FFFFFFFFFFFFF:FF,FFF,:FF:FFFFFFFF,F::FFF,FFFFFFFFFF:FFFFFFFFFF,FFFFF:FF:FFF,,FFF
-@A00604:387:HLC22DSX2:3:1103:27344:4726 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGCGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFF:FFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFF,:FFF,FFFFFFF,FFFFFFFFFFFFFF:FFFFF:FFFF,FFFFFFFFFF:FFFF,FFFFF,FFFFFFFFF:FFFFFFFFFFFFFFF,FFFF,FFFFFFF,FF
-@A00604:387:HLC22DSX2:3:1103:1687:4758 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:12608:4852 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACCTCAAAAGCACCGATGTCGTACCAGCCACTGCTATCCCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFF:FFF,FFFFFFFF,FFFFFFFFFFF,FFFFFF:F:F:FFFFFF,FFFFF:FF,FF,F:FFFFFFFFFFF:FFFFFF:FFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:8983:4867 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:24605:4867 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCATGCCCCCAGACGTCCATACCGTAGTAGTAGTAGACGGAGTAGCAGCTACCACCACTACAATATACTAAGGGCTCCCCTCTCGCACAGTAATACACGGCCCTGTACTCAGA
-+
-FFFF,,F,F:,F::FFFFFF,F,FFFFF,,F:,FF,F,F,,F,::,,:F,,,,FFFFFFF,FFF,:F::FF:F,,F,,FF:FF::F,FFFF::FFFFFFFFFFF,,::,FFFFF:F,FFFF:,:,F:FFFFFFF,FF,FF,FFF,,FFFF,
-@A00604:387:HLC22DSX2:3:1103:11125:5008 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGCCGTTACCACCGTAGTCATAGTAAGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCATTTGCAGATACAGCGTGTTCTTGGA
-+
-FFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFF,F,FFF:FF:FFF:FFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:25129:5181 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTGTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFF,F:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:,FFFFFF:FFF:,FFF:FFFFFFFFF,FF:FFF::FFFFFFFFFFFFFFF:FFFFFF:FF:FF:FF,F:FFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1103:16107:5212 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF,F:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:17978:5228 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:7961:5259 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,:FFFFFFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:25084:5259 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATCCAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFF:FFFFFFF:,FFF,FF:FFFF,FFF
-@A00604:387:HLC22DSX2:3:1103:26313:5384 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFF,FFF,FF:FFF:FFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:::FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:5367:5588 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATCACCTATATCATAGCTCCCATCACCCCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFF:FF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:8395:5603 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFF,FFFF:FFFFFFFFFFFFFFFF:FFF:F:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFF:FFFFFFFF,F:
-@A00604:387:HLC22DSX2:3:1103:23665:5619 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:18195:5635 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,:FFFFF:
-@A00604:387:HLC22DSX2:3:1103:30960:5666 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:16577:5713 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:FFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFF:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:8359:5791 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:32208:5791 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:19090:6026 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:F:F:F:FFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFF
-@A00604:387:HLC22DSX2:3:1103:30165:6042 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:26829:6339 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACCGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATCCAG
-+
-FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,F,FFFFFF:FF:F,F:FF,F,FF:FFFFF::F:,,F:,F:,FFFFF:FF,FF,,,FFFF,F,F,FF:,F,FF:,FFFFFF,,,:,F
-@A00604:387:HLC22DSX2:3:1103:22028:6449 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:27977:6605 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATAGGCCGGGGATCCTCCCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFF,FFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:12961:6684 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCATAAACCACACGAGAATGTGACCAGGGAACCTTCGCCCCAGGGGTCGAACCACCCACTCAATCCGTCATACACAAAAAACGATGACATATCTCTCGCACAGTAAAACACGGCCGAGTCGTCAGATCTCAGTCTCCTCAGCTC
-+
-FFFFF,F,F,F,,F,:FF,:,:,F,,F,FFFF:,,:,,FF:,,,F,,FF,,,,:F,FFF::F:FFF,FF,FF,,,FFF,,:FF:FF:,,F,,,FFF,F:FFF,F:FF,,,F,F:FFFFF,,F,,,:,F:FF:F:F:FF:,:,F,:F,,F:,
-@A00604:387:HLC22DSX2:3:1103:10764:6762 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGTTCTTGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF,F:FF:FFF,FF,FF:
-@A00604:387:HLC22DSX2:3:1103:22426:6825 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCATGTCCCGCCCCACCACTCCAAAAATCCCCTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCT
-+
-F:FF,:F::F:FFFFFFFFFFF:FFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFF:FF,FFF:FFFF,FFFFF,FFF
-@A00604:387:HLC22DSX2:3:1103:4164:6856 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FF:FFF
-@A00604:387:HLC22DSX2:3:1103:13160:6903 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFF:FFFFFFFFFFFF:FFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFF,F:FFFFFF,F::FF:FFFFFFFFFFFF:F:FFFFFF:FFFFFFFF:FFFFFFFFF,FFF,FF:F:FFFFFFFFF,:FFFF::FF:FFF:FF:F,:FFFFF
-@A00604:387:HLC22DSX2:3:1103:17264:7028 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:2492:7247 2:N:0:AGAGGATG+GGACTAAT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGCCCCCAGTAGTCAAAGGAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGAACTACACAGCCGAGTCCTCGGGCGTCCCAGAGTTCTGCTG
-+
-FF:FFF:,FF,F:FFFFFFF,F,F:FF,:FFF:FF:FFF::FF,F,FFFFFFFFF,,F:,,:,FF:FFFFF:FFFFFF::FFFFFFF:FFF:,FFFFFFF,F,FFFF,,F,F:F:FFF,FFFF,F,F,FFFFF,F,F,FFFFF:,F,,F,,
-@A00604:387:HLC22DSX2:3:1103:28745:7247 2:N:0:AGAGGATG+GGACTACT
-CTGAACAGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACAGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTAGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGATGT
-+
-F:F,F,,F:F,F:F,FF:FF:FFF:F,FFFFFF::F,FF:FF,:FF:FF,FFFF,FF:F,FFFFFFF:F,F:,F::FFF,,FFFF:,FFFFFFFF,FFF,:FF,,,F::F,:FF:F,:F:FF,:,F,:FFF:FFF:FF:F,FFF,:,:::F
-@A00604:387:HLC22DSX2:3:1103:27606:7310 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCATGGGCTACCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFFFFFFFFF,FF,F:FFFFF,:,FF:FFFFFF,FFFFF,,FFFF,:FF:FF,FFFFFF:FFF:,:,FF,FF,F,F,FFFFF,FFFF:FF:,:,FFF,,FFF:FFF,FFFFFFFF,,FFF,F:FFFF::FFF:FFFFFFF:F,F,FF
-@A00604:387:HLC22DSX2:3:1103:23963:7576 2:N:0:AGAGGAGG+GGACTACT
-CTGAACAGCCTACACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGACCTGGGTCTTGGATGT
-+
-,,,FFF,FF,F,FFFFF,F,,F:,FFF::F,,F,,,,FFFFF,::F,,:F,FFFFFFFFF:F,FFF,,,FFFFFF,F,FF,FFFF,:FF,F:FFFF,:FF:FF,F,FFFF:F:FF,:FF:FF:F:F,,F,FF,FF:,:,:,FFF,FFF,F,
-@A00604:387:HLC22DSX2:3:1103:26449:7592 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFF:FFFFFFF,FF:FFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:1398:7639 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACGGGTTCTTGGATGT
-+
-FFFF:FFFF:,FFFFFFFFFFFF:,FFFFFFFFFF:FFFFF:FFFFFFFFFF::FFFFFFFF:FFF,FFFFFFFFFF:FFFFFF:F,FFFFFF::FF:F::FF:,:,FFFFFFFF:FF:F::FFFFFF,F::FFF,F,:FFFFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1103:26702:7686 2:N:0:AGAGGATG+GGACTACT
-ATGAAACGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGTCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-,:F:F,F:F,::FF:F:,FFFFFF:FFFFFFFFFF,,FFFFFF,FF,FFFFFFFFFFFFF:F:FFFFF,:FFFFF,FFFF:F:FFFFF,FF,FF,FF:F:FFFF:F:,FFFFF,FFFF:FF,,,F,F,F,,F,F,FF,FFF,FF,F,FFFF
-@A00604:387:HLC22DSX2:3:1103:27434:7733 2:N:0:AGAGGATG+GGACTACT
-CTGGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGGTCATTTGCAGATACA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFF,FF,FF,
-@A00604:387:HLC22DSX2:3:1103:17598:7764 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFF:FF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FF:F:FFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFF:FF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:7247:7999 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCGGGGTTGCGTGAGTTACTGTCCTTCCTTTGCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,:::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:F:::FFFFFFFFFFFF::FFFFFF:FF,FFFF,,FFFFF:FF:FFFFFFFFFFFFFFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1103:21097:8093 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGTGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFF:FF:,F:FFF:F:F::FF:FFFFFFFFF,FF:,F:F,FFFFFFFFF,F:,,FFFFFFFF,:FFF:FF:,:F:F:FFFFF,FF::FF,F:FFFFF,,FFFFF:FFFFFF::F:F,:F,FFFFF,F,:FF,:FFFF:,FFFFFF:,,
-@A00604:387:HLC22DSX2:3:1103:22507:8093 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-:FFFFF:FFFFFFFFF:FFFFF:F,F:FFF:FFFFFFFFFF:FF,FFFF:FF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFF::FFFFF:FFFFFFFFF,FFFF::FFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:1271:8265 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTACCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGGTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF:::F:F,:,F,FF:FFFFFFF:::FFFFFFFFF,FFF:FF:F:F,FF,F:F:FFF,F,,FF:FFFFF::F,FFF::::,F:FF,,F,:FFF,FF,FFF,F:FF:FFF:F:FFFFF,FFFFF:,FFF::FFF,FFFF,,:F:F:,,FF
-@A00604:387:HLC22DSX2:3:1103:4951:8281 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,F:FFFFFFF,FFFFFF::FFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:17770:8312 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF
-@A00604:387:HLC22DSX2:3:1103:31512:8343 2:N:0:AGAGGATG+GGACTAAT
-CTTAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFF:FFF:F:FFF,FFF::FF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:F:FFFFFFF,F,F,FFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFF:F,FFFFFF,F,FFFFFF
-@A00604:387:HLC22DSX2:3:1103:31521:8359 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:2311:8406 2:N:0:AGAGGAGG+GGACTACT
-GTGCCACCACTGTTAGGGTTGATCCATCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGCACCCAGTGCATATAGTAGCCGGTGAAGGTGTATCCAGAAGCCTTGCAGGAGACCTTCACTGAGGCCCCAGGCTTCTTCACCTCAGCCC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:26187:8547 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FF:FF:FFFFFFFFFFFFFFFFFFFFFF::FF:FFFFFFFF,F:FF,FF:FFF:FFFF,FFFFFFFFFFFF,FFFFFFFFFFFFF,:FFFFFFFFF:FF:FFF,,FFFF::FFF,:FFFFFFFF,FFFFFFFF,,FFFFFFF:FFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:5466:8609 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF,FFFFFFF,F:FFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:12445:8609 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1103:22073:8625 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAAACGTCCATACCGTAGTAGTAGTAGTACGTGCCAGCCACTGCTACCCCCCCTTGCCTAGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:25518:8672 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:20338:8719 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFF:FFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1103:29704:8719 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:19027:8829 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:13666:9095 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTATGAGGCGTAATCAACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGTCTGTAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:22110:9220 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:31132:9283 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FF:FFFFFFFFFFFFFFFF:FFFFF,FF::FFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:13612:9408 2:N:0:AGAGGAGG+GGACTACT
-CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGAAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
-+
-FFFFFFF:FFF:FFFFFFF::FF,FF,FFFFF,FFF:FF::F,:FFFFFF,,FF,FFFFFFFFFFFFFFFF,FFF:FFFFFFF:,F:F::FF,FFF:FFF:::FFFFFFFFFFFFFF:FFFFF:F:,FFFF:FFFFF:,F:,FFFFFFF,F
-@A00604:387:HLC22DSX2:3:1103:22507:9596 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1103:23366:9612 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCCCAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFF:FFFFFFFFFFFFF:FFFFFFF:F:F,,F:FFF:,F:F:FFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FF,FFFFF:FFF,FFF,F,FF,,FF::FFFFFF,FFF:FF:FF,FFFFFFFFFF::FF
-@A00604:387:HLC22DSX2:3:1103:23448:9659 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1103:26829:9659 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGACTCCACCACTCTAGACGGTGACCATTGTACCTTGGCCCCAGACATCAAAAGCACCTATGTCTTACCATACAATTCTATACCCGTCCTAGGTCTACCAAGCACAGTAATACAAGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FF,F:,FF,F,,FF:FFFF:,F,FF,FF:F,:F,,,F:FFF:FF,,:F:FFFF:,FFFF:FF,F,FF,FF,FF,,F,,:F,F,FFFFF,,FF,::F,,,,FF,::,,,:FFF,FFFFF:F,,:,,:F,F,F,FFFFFFF:F:,FF,,FFF,
-@A00604:387:HLC22DSX2:3:1103:26639:9674 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
-+
-FFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFF,FFFFFF,FFFFFFFFF,FF,F,F:FF:,F:FFF:FFFFFFFFFFFF,F,,FFFFFFFFFFFFF,:FFF,FFFFFFFFFFF::,FF
-@A00604:387:HLC22DSX2:3:1103:16477:10081 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCAGTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:F:,FFF,FFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFF,F,F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFF
-@A00604:387:HLC22DSX2:3:1103:29378:10160 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFF:FF:FFFFFFFFF:FFFFFF:FFFF,FFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:::,FF,FF:FFF
-@A00604:387:HLC22DSX2:3:1103:2275:10191 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFF:FFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFF:F:FFFFF:FFFFFFFFFFFFFFFFF,FF:FFFFF:FFFFFFF:FFFFFFFFFFFF,FFF:FFFFF:FFFFFFFFFFFF,FF:F:FF::FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:18421:10473 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:31665:10488 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1103:28583:10848 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
-+
-FFFFFFFFFFFFFFF,FFF:FFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,F:FFFFFFFFFFFFFF:FFFFF
-@A00604:387:HLC22DSX2:3:1103:3902:10911 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFF,FFFFF:FFF,FFFFF:FF
-@A00604:387:HLC22DSX2:3:1103:19000:10911 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:29270:10911 2:N:0:CGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFF:FFFFFFFFF,FFFFFFFFFF,F,FF:F:F:,FFF:F:FFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:31467:10927 2:N:0:AGATGATG+CGACTACT
-CTGAACCGCATCCAACACTAGAGACTGAGAACGTGGTCACATGCCCCCAGAAGTCAAAGTCCAAGTAATAACCACTAAAATACATGGCGCATTACTCACATTAATATACGGACGTGACATCGGATAACAGTCTGTTAATTTGCAGATACAT
-+
-FFFFFF,,F:FFFF,,F,,,FFFF,,:,,,,F:F,,FF,F,FFFF,FFF,,F,F::FFFF:FFF:,FF,,:FFF:FF,:FFF,FF,,:,:,,F,FF,FFF,,FF,FFFF,,,,,,,::,,,,,,F:,:,:,F,,FFFFF,:,,FFFFFF,,
-@A00604:387:HLC22DSX2:3:1103:28646:10958 2:N:0:AGAGGCTG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTCTGCCGCGCCGACTCTCGCACAGTAATACACGGCCGTGTCGTCAGACCTCAGCCTGCTCAGCTCCATGTAGGCTGTGCTGATGGACGTGTCCCTGGTCAT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1103:32371:10989 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAAAAGGCCTGTTCTAACTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:31403:11036 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:,FFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1103:22598:11162 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFF,:,FF:FF:F,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,,:F,F,F:FFFFFF:F,F,F,FF,F::,::FFFFF,F:::F:FFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:32497:11209 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTAGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCAATGTAGGCTGT
-+
-,F,,F:FF,FF,FFF,F:F,FFFFF:FF:FFFFFF,,F,FFFF,F:FF:FFFFFF:FFFF,:FFFFFF,FFFFFFF,FF:,::F:FF,FFFFFF,::FF,:F,F:FF,FFFFF,FFFFFF,F,FFF:FF:FFF,FF,FF,FFFF:F,FFFF
-@A00604:387:HLC22DSX2:3:1103:16550:11397 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAGGTTTCCCTGATCCTTATCTCTCGCACAGTAATACATGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTTATGGAGGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:25220:11506 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGAGGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFF,F:
-@A00604:387:HLC22DSX2:3:1103:21531:11694 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:1208:11725 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTCATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFF,FFFFFFF::FFFFFFFFFFFFFFFF,FFFFFFF,:FFFF,FFF:,FF,FFFFFFFFFF:FFFFFFFF,:FFFFF:FFFF,,:FFF,F:,FF,F
-@A00604:387:HLC22DSX2:3:1103:21377:11741 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FF:F:FF,,FF:FFFFFFFFFFFFFFFFFFF:F,FFFFF:FFFFFFF:FFF::FF::FFF:FFFFFFF,FF
-@A00604:387:HLC22DSX2:3:1103:21856:11757 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFF:,FFFFF:FFFFFFFFFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:12915:12524 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFF:FF
-@A00604:387:HLC22DSX2:3:1103:13503:12665 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATCTTGGGCCTCTCTTGCACAATAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGACAACTGGTTCTTGGATGTGTC
-+
-FF,FFFFFFF:FFF:FFF::FFFFFFFFFFFFF,,FFFFFF,:FFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFF,FF:FFFF::FFFFFF,F,::F,FFF::,FFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF,F:F:FFFF:
-@A00604:387:HLC22DSX2:3:1103:7202:12712 2:N:0:AGAGGATG+GGACTACA
-CTGAACCGCCTCCACCACTCGAGACGGTTACAATTGTCCCTTGGCCCCAGAAAACAAAAGCACAGATGTATTACAAGCCACTGCTATACACGGCCTAGGGCTCCCTCGCACAGTAATAAACGGACGTGACCTCAGATCTCAGGCAGCTCAG
-+
-FF:FFF,FFFFFFFF,,FF,,F,FF,,F,FF,:F::F,FFF:F:FF:,F,F,F,,FFF:FFFF,::F,F,,FFF,F:,FFFF,F:,F,,,F,FFFF,:,F:FF,:::,FFFFF:FF,F,FF,F:F,:F,::FFF:FFFFFFFF:,:FFF,F
-@A00604:387:HLC22DSX2:3:1103:18349:12727 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCTCCTCCGTAGTTCCCGTCATCCCTCGCACAGTAATACACAGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGTGTT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFF:FFFFFFFFF:FFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF,FFFF:FFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:31033:12868 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFF:FFFFFF:FFFFF,FFF
-@A00604:387:HLC22DSX2:3:1103:32434:12884 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCAACACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTCCCAAGCCTCGGTATAGCAGCTGGTACTACTACAATATCGAGGGACGTCTCTAGAACAGTAATACACGGCTGTGTCCTCGGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:F:FF,:F:FFFFF:FFFFFFF::FFFFFFFF,FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:7292:12962 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FF:F
-@A00604:387:HLC22DSX2:3:1103:32154:12962 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCTGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFF:FF:FF:FF
-@A00604:387:HLC22DSX2:3:1103:26964:13025 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:25925:13166 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTAAAATAGTCCCCTAGCTCCCCACGATGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTGGGCTGTGTCTGTAGA
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFF:FFFFFFF:FFFF:F:FFFFF:FFFF:FFFFFFFF:FFFF,FFFFFFFFFFFFFFFF:FFF:FFFFFFFFF::FFFFFFFFFFFFFF:FFFF
-@A00604:387:HLC22DSX2:3:1103:32768:13182 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCAACACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATACCGTAGTAGTCCCAAGCCTCGGTATAGCAGCTGGTACTACTACAATATCGAGGGACGTCTCTAGAACAGTAATACACGGCTGTGTCCTCGGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFF:F,FFF:FFFFF,FFF:FFFFFFFFFFF,FFFFF
-@A00604:387:HLC22DSX2:3:1103:16242:13338 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF,FFFFFFFFFFFFFF:FFFFF:FF,::FFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:11225:13354 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFF:FFFFFFFF:FFFFFFFFFFFFFF:FFFF:FF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1103:31602:13354 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFF:FFFFFFFFFFFFF,FF:FFFFF
-@A00604:387:HLC22DSX2:3:1103:6081:13526 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
-+
-FF:FFFF:FFF:,F,FF,:,FFFFF,::,F:,FF::FFFFFF:::F,F::F,FF,FFFF,FFF:::F::,:FF:,F:F,:FFFFFFFFF,,FF:FFF:FFFFF,,FF:FFF,FFFFFFF,,,FF:FFFFF,FFFFFF,FFFFFFFF:F,,F
-@A00604:387:HLC22DSX2:3:1103:3956:13542 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTCATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACCG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,FFFFFFFFFFF:FFFFF,FFFF,FFFF::FFFFFF,FFF:FFFFFF,FFF:FFFFFFFFF,FFFFFFFFFFF:FFF,F:FFF,FFFF,FF:FF,F
-@A00604:387:HLC22DSX2:3:1103:18087:13557 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1103:29767:13683 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:9426:13714 2:N:0:AGAGGATG+GTACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFF,F:FF:FFFFF:FFFFF:FFFFFF:FF:FF::FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1103:31439:13855 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFF:FF::FF:FFFFF,:FF:FFFF:FFFFFF:FFFFFFFFFF:FF:,FFFFFFFFFF:F,FFFFFFF:FFFFF:FFFFFFF:FFFFFFFFFFFFFFFF:FFFF:FF:FFFFFF:FFFFFFFFF:FF,FFF:,FFFF
-@A00604:387:HLC22DSX2:3:1103:8413:13870 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFF:F:,FFFFFFFFFFFFFFFFFFFFFFF:FFF,FFFFFFFFFF,FFFFFFF
-@A00604:387:HLC22DSX2:3:1103:10267:13886 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF
-@A00604:387:HLC22DSX2:3:1103:25861:14246 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:28501:14434 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,:F:FFF,FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF,
-@A00604:387:HLC22DSX2:3:1103:30291:14434 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:7600:14465 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGCGTCGAACCACCCACTCATTAGTTCATACACAAAAATCGTTGCCAGTTCTCGCGCACAGAAATACACGGACGTGGCGTCAGAACTCAGGCTCCTCAGATC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FF:F::FF,F,,F,FF,,,,F,FF,,:,F:,FFF,,FFF,,F,F,:F,F,,F:,F,F,F:,,FFFFF,,:,:,F,:,,FF,,F:FF:,F,,FFFF,FF
-@A00604:387:HLC22DSX2:3:1103:6813:14544 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTCGTCACCGGCAGCACCCCCTTTCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAGTGAGTTCTTGGCGTTGTCTCT
-+
-FF:F:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFF:F:FFFFFFFFFFFF:
-@A00604:387:HLC22DSX2:3:1103:11442:14544 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
-+
-FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFF:FFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:5846:14841 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF::FF
-@A00604:387:HLC22DSX2:3:1103:21287:14998 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
-+
-FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1103:27887:14998 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:1334:15013 2:N:0:AGAGGATG+GGACTACT
-ACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATG
-+
-FFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:5403:15045 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
-+
-:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFF,FFFFFFFFFFFFFFFF:FF::FFFFFF,FFFFFFF:FFFF:FFF,FFFFFFFF:FFFFFFFFFFFF:FFFFFFF
-@A00604:387:HLC22DSX2:3:1103:12075:15076 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
-+
-FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
-@A00604:387:HLC22DSX2:3:1103:11939:15092 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGCTGTATCCCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTGCTCAGCTCCATGTAGGTTGTGCTGATGGACGTGTCCCTGGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:28022:15170 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFF
-@A00604:387:HLC22DSX2:3:1103:17056:15217 2:N:0:AGAGGATG+GGACTACT
-AGGGAGAACTGGTTCTTGGATGTGTCTGGGTTGATGGTTATTCGACTTTTCACAGATACTGCATAATCATTATACCACTTGGACCTGTAGTATGTCCTTCCCAGCCACTCAAGGCCTCTCGATGGGGACTGCCTGATCCAGTTCCAAGCAG
-+
-FFFFFFF,F:FF:FFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:28501:15217 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGACGTCCATGTAGTAGTAGTAGTGCTCGTAGCAGCTACCACCACTACAATATCCAGAGCCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCT
-+
-FF,FFF,FFFFF,,:FFFFFFFFFFFFF,,FFFFFFFF::F:FF,F::FFF:FFFF:F:,F:FF:F:FFFF:F,F,F,FF,,:FF:F:F,:FFFFFF:,FFF,FF:F:FFFF,F,F:FFFFFFFFFF,F:F:FFF:,FFFFFF,:FFF,:F
-@A00604:387:HLC22DSX2:3:1103:19054:15233 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATAGCCCACTTCGTACCAGCCACTGCTACCGAGCCGCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATC
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FF:FFF:FFFFFFFFFFFF,FFFFFF
-@A00604:387:HLC22DSX2:3:1103:31539:15248 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAGCATACCACTACTATCATAGTAACCTTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
-+
-FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:4227:15295 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGGTCATACACACAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
-+
-FFFFFFFFFFFFFFF:FFF::F,FFF,FFFF:FF:::FF:FF:FFFFF:FFFFFFFF:FFFFFFFFFFFFFFF,FFFF,F:FF:F::FFF:FFFFFFFFFFFFFFF:FF:FFFFF:,FFFFFFFFFFFFFFF:FFFF,FF::FFFF,FFFF
-@A00604:387:HLC22DSX2:3:1103:23014:15389 2:N:0:AGAGGATG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
-@A00604:387:HLC22DSX2:3:1103:3812:15483 2:N:0:AGAGGAGG+GGACTACT
-CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
-+
-FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFF::FFFFFFFFFFFF:FFFFFF:FF:FFFFFFFFF:FFFFFF:FFFFFFFFFF:F:FFF,:FFFFF:FFF:FFFFF:FFF,FFF:FFFFF,:FF
+@A00604:387:HLC22DSX2:3:1101:5837:1297 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCGATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F,:F,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:30373:1360 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTCATACACAGCCGTGTCCTCGGGAGGCACAGAGTTCAGCTGCAGGGCGAACTGGTTCTTGGAGGT
++
+F:FFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFF:FFF,FFF:FFFFFFFFFF,:FFFFFFF,FFFFFF:FF:FFF,FF,:FF:F,,,FFF:,F,FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31376:1407 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCTTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FF:FFFFF:F:FFFFFFF:,F:FFF:FFFFFFFF:FFFF:FFFFF,FFFFFFFF,FF:F,FFFFFFFFFFF,FF,,,FFFFFFFFFFF,FF:FFFFFFFFF:FFF::::F:FF:FFFFF:FF,F,FFFFFFFF::F:FF::FF,FFFF,FF
+@A00604:387:HLC22DSX2:3:1101:4146:1438 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTTGCCCCAGTAGTCAAATAGTCCCCTAGCTCCCCACGATGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTGGGCTGTGTCTGTAGA
++
+FF,:FFF:FFF,FFF:F:,FFFFF,FFF,FFFFFF:,,F::,,F,::FF,F,,F:FFFFF,FFFF:,F,FFF:F:F,FF,:,:,FFFF:FFF,::F,,,F::,FFFF,F,:F,F,FF,,F:F::FF,FFFF,FF,FFF:FF,:FF,,F::F
+@A00604:387:HLC22DSX2:3:1101:30798:1438 2:N:0:AGAGGAGG+GGACGACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATAGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+F,:FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF,:F,FFFFFFFFFF::FFF,FFFFF,FFFF:,F:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFF:F,:FFFF
+@A00604:387:HLC22DSX2:3:1101:21368:1454 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCGGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFF:F,FF:,F,:F::FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31349:1454 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGATCAG
++
+FFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:F:FFFFFFFFFF:FFFFF:FFFFFF,FFF:FF:FFF:FFFFFF,FFF:FFFFFFFF:FF:FFFFFFFFFFFFFFF,,FFF
+@A00604:387:HLC22DSX2:3:1101:32768:1532 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FF:FFFFF:,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11442:1642 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:17300:1767 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFF:FFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:32371:1846 2:N:0:AGAGGAGG+GGACTACT
+TAAAGGTGTAACCAGAAGCCTTGCAGGAGACCTTCACTGAGGCCCCAGGCTTCTTCACCTCAGCCCCAGACTGCACCAGCTGAACCTGGGCCATGGCCGGCTGGGCCGCATAGAAAGGAACAACCAAAGGAATTGCGAATAATAATTTCTC
++
+FFF,FFFFF,F:FFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:4246:1986 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFF:FF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:17345:2002 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:3830:2018 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF::FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FF,FFFFF
+@A00604:387:HLC22DSX2:3:1101:4408:2018 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:F,FFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:2139:2065 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFF::FFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFF::FFFFFFF:FFFFFF,FFFFFFFFFFFFFFFF,FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:1615:2096 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCAGGCCCCAGTTGTGATAACCAGACAAAATCTCCCAAGTCGCGAAGGAGGCAGCGTAATACACCGCCGTGTCCTCAGATCACCGGCTGCACAGCTCCATGTAGGCTGTGTC
++
+FF:FF:FFFFFFFFFFFF:FFFFFFFFFF:FFFFF:F,FFF,FFFFFF:F,:,FFF,FF,F,F,FFFF::,:F,,:,,,,,:F,,:F,,:F:,,F:,,:,FFF,:,FFF:,:F:FF,F,F,F,,:FFF,,FF,F,,:F::,,:F:F:F:,,
+@A00604:387:HLC22DSX2:3:1101:4444:2112 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACGCGAGAAGGTGACAAGGGATCCAAGGCCCCAGAAGTCAAAGTAGTATTTCTCGTAGCATCTACCACCACTACAATAACCCCCTCTAGCACAGTAATACACATCAGTGACCTCGGGAGTCACAGAGATCAGCTG
++
+:F,F,:FF:,FFF,F,,,,,FF,F,:,FFFF,F:,:,FFF,,,FFF::,:,F,:F,FF,:,:,FF,:,FFF,F:FF,F,FF:FFFFF:F,:FFFFF,:F:,,F:,FFFF,F,FFF:FFF,F,,F:,FF::F,FF:F,FF,,FF,,:FFFFF
+@A00604:387:HLC22DSX2:3:1101:1967:2174 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:F::FFFFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFF:F::FFF:FFF:FF:FF
+@A00604:387:HLC22DSX2:3:1101:21368:2174 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFF:FFFFFFFFFFFFF:FF,:FFFFFFFFFFF,FF
+@A00604:387:HLC22DSX2:3:1101:19036:2206 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGATCCCCGATCCCCTGACGGGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTGTG
++
+FFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFF,
+@A00604:387:HLC22DSX2:3:1101:32235:2237 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCGTACCGCCCTCATAGCAGCTGGTACTACTACAATATCCAACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:
+@A00604:387:HLC22DSX2:3:1101:31566:2456 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3712:2597 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:1985:2644 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFF,:FFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:29559:2644 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGGTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FF,FFFFFFFFFFFFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5791:2660 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACAGCAAAAGCACCGATGTCGTACCAGCCACTGCGATACCCGGCCTTGGGCTCCCTCGCACAGTCATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,F:FF:F,FFFFFFFFF,FF,FFFFFFFFFFFF,FFFF,FFF:FFFFF::F,F,FF:FFFFF,,FFF,FF:FFFFF,:F:F::FFFFF:FFFFFFFFFFF,F,:FFF,FFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1101:26060:2660 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:10782:2722 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGTCAAGCCACTGCCGAATCTGTTGCACAGTAATACACAGACGTGTCCTCGGGAGTCACAGAGTTCAGCTGAAGGGAGAACTGGTTCTTGGAGGT
++
+F:FFFFF::,F,:FF,F,,FFF,F:,FFFFFFFFFF,FF,FF,,,F,FF,FFFFFFF:,F,FF,,FFF:,:,FFFF:,FF,FFF:FFFF:FFFFFF,,:F:FFFFFFF,FF:FFF:,F:FFF::F,F,:FFFF:FFFFF:FFF:::F:,FF
+@A00604:387:HLC22DSX2:3:1101:19759:2895 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTATAACTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:19388:2942 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTATAACTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28574:2973 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFF:FFF:FFFF:FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20564:3067 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGGCAGAGTTACCACCGTCCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGACTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32796:3145 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACCGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:F:FFFFFF:,FFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:19244:3255 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATGTATAACTCGTGATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTCGTGGATTCGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:19614:3270 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22128:3270 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFF::FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:5231:3286 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGATG
++
+FFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFF:FF,FFFF,FFF:FFFFFFFFFFFF:FFFFFFF:FF:FFFF,FFFFFFFF,FFFFFF:F:FFFFFFFFF,FFF,FFFFF:FFF,,FFFFFFFFFFFF:,:,FF
+@A00604:387:HLC22DSX2:3:1101:16875:3474 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:F:FFFFFFFFFFFFFFFFFF:FF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:25455:3521 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5050:3537 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFFF,FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:23402:3568 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF::FFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26946:3568 2:N:0:AGAGGAGG+GGACTACT
+CTGGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1101:15058:3615 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:17779:3693 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:29731:3693 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATAACCCTGGAACCAGACGTAGCAGCTACCACCACTACAATAGGGGCGATCTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:8187:3740 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
++
+FFFF:FFFFFFFF,FFFFFFFFFFFFF,FFFF:,FFFF:FFF,:::FFF:F,:FFF,FFFFFFFFFFF:FFF,F,F:F,,F:F:FFF,FF::FFFFFFFFFFFF,FFFFFF:FFFFFFFFFFF:FFFFFF:FFFF::FFF,,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:17680:4178 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F:FFFF:FFFFFFFFFF,FFFFFFFFFF,FFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFF:F:FFFFFFFF,FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11803:4366 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFF:F:FFFFF:FFFF:FFFFFFFFFFFF,FF:FFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFFFFFFF,:FFFFFFF:FFFFF,FFFFFFF:FFFFFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20618:4413 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+F:F:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF:FFF:FFFFFFFFFFFFFFFF::FFFFF:F:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:25292:4711 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+:FFF,F:FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF::FFF,:::FFFF:FFFFFFFFFFFFFFFF,FFFFFFF:FFFF,FF:FFFFFF:FFF:FFF:FFFFFFFFFFFFF:FFFF,FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9453:4930 2:N:0:AGAGGATG+GGACTACT
+CTGAAACGCATCCACCACTCGAGACGGTCACCAGGGATCCTTGGCCCCAGATATCAAAAGCATCAGTTGTTTTTAACCGAGAACAGTAATAAGAGGCAGAGTCCACACGGTCCATGTTGGACATTGTAAGGACCACCTGGCTTTTGGAGGT
++
+FF,FF,F:F,F:FFF:F,FFF,FFF:,,,F,,F:,,,FFF,FF,F,FF:,F,FF,:FFFFFF,:,,,FFFFFFFF,FFF,:,,F:,,::,F,:,,F:,:,FFF:FF:,FF:FFFFFFF,,,F:,,F,F,:,FFFF,FF:FF:F,FF,FFF,
+@A00604:387:HLC22DSX2:3:1101:30906:5196 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26313:5228 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:27633:5228 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFF:FFFFFFFFFFFFF,:FFFF,F,FFFFFF::FFFFFFFFFFFFF:F,FFF:F,FFFFFFFFFFFFFFFFFF,FFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:28537:5321 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGGGAGTTGGTAGCAGCTACCACCACTACAATAGCGCCAATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:11541:5384 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGATATCAAAAGCATCACCGACGTAGTCACCGTAGTCATCAGGATCTGATGGCGGGGCCAGTCTCGCACAGTAATACATAGCGGTGTCCGAGGCCTTCAGGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:25626:5447 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATAGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:F,FFFFFF:FFFFFFFFFFFFF,FFFFFFFFF:FFFF,FFFFF,F:FF:FFF:FFFFFFFFFFFFFFF,::FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5593:5478 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFF:FFFFFFFFFF,FFFFFFFFF,F:F:FFFF:FFFFF:FFF:FF:FFF:FFFFFF:FFFFFFFFFFFFFF,F::FFFFFFFFFFFFFFFF:FF:F,FFFFFFF:FFFF:FFFFFFFFFFF:FFFF::F:FFFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1101:19452:5494 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATACCCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFF:FFFFFFFFFFFFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1101:21495:5556 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+:FFFFFFFFF,FFFFF:FFFF:FFFFFF:FFFFFFFFFFFFF:FF::F,FFFFFFFFF:FFF:FFFFFF:F:F,F:FFFF,FFF,FFFFFF:FFF,FF:FFF:FF,,FFFFFFF:FFFFFFFFFFF,FFFFFFFFFF:F::FFFFF:FF:F
+@A00604:387:HLC22DSX2:3:1101:3287:5619 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFF:,F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:16062:5666 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTCTAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFF,FFFFFFFFFFF:FFFFF:FF:FFFF:FFFF,FFFFFFFFFFFFFFF::FFFFFFFFFFFF,FFFFFF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18864:5666 2:N:0:AGAGGATG+GGACTACT
+ATGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGAAAAAGTACCAGCCACAGCTATATGCCCTGTCACCGGTAGAACAGTAATAAACCTCCGTGACCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+,FF:FFF,FF,:FFFF,FFF,:,F,F,FFF,:FF:,F,,FFF,,F,F,FFFF:,,FF,FF,F,F,F,FF,F,:F,F,FFFF,,F,,F,FF:,F,,F,,:F,,,,:F,,FF:F,,:FFFF,FFFFFF:FFFFF:FFFF::FFFFFFFF,F,:
+@A00604:387:HLC22DSX2:3:1101:31593:5697 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:2067:5791 2:N:0:AGAGGATG+GGACGACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTACTACACGGCCGTGTCCTCAGATCTCCGGCTGCTCAG
++
+F:FFFFFF,,F:F:F,F:FF,FF,FFFFF:F,::,::FFF,:FF:FFF,F,F:FF,F:,:,,:FFF,,,F::,F:FFF,F,,,F:,F:FFF,FF,,FFF:F:F:F,FFFFFFFF,,F,FFF,FFFF:F,FFF:F,F,:::,FFF,::F,,,
+@A00604:387:HLC22DSX2:3:1101:15320:6042 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATCTCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTT
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFF:FFFF:FFFF,FF:FFFFFFFFF:FFFFFFFFFFFFFFFF,FFFFFF::F,FFFFFFFFFFFFF:F,
+@A00604:387:HLC22DSX2:3:1101:8296:6277 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFF:FFF:FFF,F,FFFFFF:F,F,,FF:F:::F:FFFF:,F:,,FF,F:,FFF:FFF,FFF:,FF:FFFFFF:F:FFFFFFFFFF,F:FFF,:FF,FF::FFFF:F,FFFF:FF::FFF,:F,FFFF:FF,F,FF:FFFFFFF,:F:
+@A00604:387:HLC22DSX2:3:1101:30454:6324 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFF:FFFFF:FFFF,FFFFFFFFFFFFFFFFFFF:,FFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FF,FFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FF:F::FFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:10474:6511 2:N:0:AGAGGATG+GGACTACT
+CTGGACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFF,FFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFF,:FFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1101:2428:6543 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFF::F:FFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:::FFFFFFFFFFFFF:FFFFFFFF:FFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21034:6574 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTACACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGCTGTATGTTCCAAAGTAATACACGGCCGAGTCATCAGATCTCAGGCTGCTCAGCTCCAAGTAGGCTGTGTCTGTATA
++
+FFFF:FF::,:,:F,,FFFF,FFFFF::FF,,FF,F,FFF:F:,FFFFF,FF,F:F,F,F,,,:,F:,,,FF:FFF,FFFFFF,,F,FF,F:FFFF,F:,FF,,:,,F:F:F:,F::F,:F:,FFF,F,,,F,,,F,,FFFFFFF:F,F:F
+@A00604:387:HLC22DSX2:3:1101:31638:6652 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCACCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFF:F,F,FFFFFFFFF:FFFFF,FF::FF:F:,FFFF,F,F,F:FFF:F,FFFFF:,FFF,FFFFF:FFF:,FFFFFFFFF:F:FFF:FF:F::FFFFFFF:F:,:,,FF,:F:FFFFFFFF,FF:FFFF:F:F,F:F:F,FFF:,
+@A00604:387:HLC22DSX2:3:1101:18629:6731 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGCCCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF,FFF,FF:F:,:,:F:F,FFFF::,FF,FFF,:::F:F:,,FFF,FFF:,,,:FFF::,,F,::F::FFFF,:F,F:FFFFF,FFFF,,,:::FF,:FFF,FFFFF,F,FFFFFFFFF,F,F:FFFF:,FFF:FFFF,FFFFF:FFF,F
+@A00604:387:HLC22DSX2:3:1101:10203:6762 2:N:0:AGAGGAGG+GGACTACT
+CGATGGGGACTGCCTGATCCAGATCCAAGCAGCACTGTTGCTAGAGACACTGTCCCCGGAGATGTCACAGGTGAGTGAGAGGGTCTGCGAGGGCTTCACCAGTCCTGGACCTGACTGCTGCAGCTGTACCTGGGCCATGGCCGGCTGGGCC
++
+FFFF:FF,FF,:FFF:F,FFFF,,F:FFFFFF,FFFFFFFFFFF:FFFFFFFFFFFFF,FF:,F,FFFF:,F:F::,F,,FFFF:FFFFFFF:FFF:FFFF,FFFFF:FF,F:FFFFFFF:FFFF,:FF:F:F:,FFFF:F:,,F,FFF,F
+@A00604:387:HLC22DSX2:3:1101:13250:6840 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22761:6840 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGGGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCACGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFF,FFFFF:FFFFFFFFFF:FFFFF,FFFF::FFF:,F,:FF:F::FFF:F:F::FF:FFF,FFF::F:FF:FF,FFFFFFF,:F,F,:,F:,F:FFFFFFFF:,FFFF:FF,FFFFFFFFFFFFF:F:F,F:,F:F,:FF:FFF,,FF
+@A00604:387:HLC22DSX2:3:1101:12554:7263 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:29071:7279 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:15266:7357 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATCCAG
++
+FFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFF,FFFFFFFFFF,FFFFFFF,FFFFF:FFF,FFFF:FFFF:F:FFFFFFF,,F,FFFF:F,FFF:FFFFFFFFFF,::FF,F:::FF:F:,FF:FFFFFF:FFFFF,F,:,F
+@A00604:387:HLC22DSX2:3:1101:14452:7420 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFF:FF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1101:1136:7498 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+F:FFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:F,FF:FF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1101:15320:7513 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFF:FFFFF,FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5394:7639 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FF,FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:2953:7733 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAACTCCTCCTCTCGGCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCTTATGGAGGTGTT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F,FFF:F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,F:FFFFFF:FFFFFF,FF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22498:7764 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCTCAGTATTACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCCG
++
+F:FFFFF:F:FFFFFFFFFFFF::FFFFFFFFFFF:FFF,FFFF:FFF:F,FFFF,FFFFFFFFFF::F:FFF:FFFFFF:FFF::FFFFFFFFFFFF:FFFF,:FFFF,FFFFFFFF:FFFFFF:FFFFFFFFF:,FFFFFFF:FFFF,:
+@A00604:387:HLC22DSX2:3:1101:23041:7764 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FF:F:,FFF::FFFFFF:FF
+@A00604:387:HLC22DSX2:3:1101:18096:7905 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGCATCTTGGGCCTCTCTTGCACAATAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGACAACTGGTTCTTGGATGTGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FF::FFFFFFFFFFFFF,:FFFF:FFFFFF:FFFF:F
+@A00604:387:HLC22DSX2:3:1101:22788:8234 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5430:8484 2:N:0:AGAGGATC+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATGTCTCGCACAGTAATACACGGCCGTGTCGTCCGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFF,FFFFFF,FFF::F,FF,:,:F,:FF:FFF:FFF:,F:FF:::FFFFFFF,FFFF:FFFFFF:::FF:FFFFF::,:F:FFFFFFFF,,F:,FFFFFF,FFFFFFF:,FFFF:FF,F:F,FF,FFFF:F::F,F,FF,FFFFF
+@A00604:387:HLC22DSX2:3:1101:22236:8719 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAATCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+F:FF:FF,F,F,FFFFF,,FFFF:FFFFFFFFFFFF::F,F:F:FF,FFF:FFF:F:,FFF:F:FFFFFFFFFFFFF:FFFFFFFFFFFFF,:FF,F:FFFF::FF:F:,F,FFFFFFF,F,F,:FFF:,,FFFF:,FFF,F:FF,,FFF,
+@A00604:387:HLC22DSX2:3:1101:20564:8797 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFF:,FFFF::FFF:FFFF:FFF:FFFFFFF:FFFFFFFFFF:FFFFFF,FFFF:FFF:FFFFFFFFFFFFF:FFF:FFFFFFFFFF,FFFF:,F,FFFFFFFFFFFF:FFFFFFFFFF:FF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:2239:9157 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTACTAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFF:,FFFFF:FFFFFFFFFF:FFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:10682:9189 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FF,FF,FFFFFFFFFFFFFFFF:::FF:FFFFFFFFFFFFFFFFFF:FFFF:FFFF:FFFFFFFFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32027:9549 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:2555:9831 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFF::F:FFFFFFFF:FFFFFFFF,FFFF,FFFFFFF:::FF
+@A00604:387:HLC22DSX2:3:1101:25437:9846 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF:FFFF:FFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:14073:10081 2:N:0:AGAGGATG+GGACTACT
+CTTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28682:10113 2:N:0:AGAGGATG+GGACTACA
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCATTGGCCCAAGTAGTCAAAGTAGTATTTCTAGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCGTCGGGAGTCACAGAGTTCAGCTG
++
+FFF:F,FFFFF,FFFFF:,FF:FFFF:FFFFF:F:,F:FFFF::FFF,:F::F:F,,FFF:FFF,FFF:,::FFFF,F,::FFFFFFFFFFF:FFFFFFFFF,,FF,F,F:FFFF,:FF:F,F,FFF,FF:,FFF:F,FFFFFF,F:FF,:
+@A00604:387:HLC22DSX2:3:1101:8865:10144 2:N:0:AGAGGATG+GGACTACT
+CTGAACCCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCCAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGTG
++
+FFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF,FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,:FFF:F:FF:FFFFFFFFFFFFFFFFFFFFF,:FFFFFF::FFF,FFF
+@A00604:387:HLC22DSX2:3:1101:19614:10222 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:10700:10379 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGGGGAGTTGGTAGCAGCTACCACCACTACAATAGCGCCAATCTCTCGCACAGTAATACACAGCCGTGTCCTCGGGAGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:31910:10629 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:25717:10770 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:7826:10817 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFF:FFFF,FFFFFFFFFFFFFFFF:FFFFFFFFFFFF,F:FFFF:FFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:7157:10880 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFF:F,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFF,FF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:8467:10895 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFF,FFFFFFFFF:FFFFFFFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF,F
+@A00604:387:HLC22DSX2:3:1101:20916:11005 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:F:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9200:11068 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFF,F,FFFFFFFFFFF:FFF:FFFFF:F:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:13295:11083 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FF:FFFFFFFFFF:F:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:25120:11271 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9118:11365 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGAGGTAGCAGCTACCACCACTACACCTCAACTCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTTAGGCTGTTCAT
++
+FFF:F:FFF:FFFF:,F::FFFF:FFFFFFF,FFFFFFFFFF:FFFFFFFFF:F:FFFF::FFFFF,FFFFF,FFFF:,FFFFFF,FFFFF,FFFFFFF,,FF:FFFFFF,FFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:27642:11443 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:1994:11772 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFF:FFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1101:17137:11788 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FFFFF,F:FFF::F,FFFFFF,
+@A00604:387:HLC22DSX2:3:1101:21251:11898 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32886:11945 2:N:0:AGAGGATG+NGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATAACCGGCCTTGGGCTCCCTCGCACAGTACTACACGGCCGAGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFF:F,FFFFFFFFFFF,FFFF:FFFFFFF::FFFFFF:FFFFFFFFFFFFFFF,FF::FF:FF,,FFFFFF,FFFFFFF:FF,:FF,F,:FF:FFFFFFFFFFFF:FFF,F:F:F:FFFF,FFFFFFFF:F:FFFFFF:FFFFF:
+@A00604:387:HLC22DSX2:3:1101:23619:11960 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:23827:11976 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTAGAGACGGTGACCGTGTTCCCTTGCCCACAGTAGTCAAATTCCAAGTAATAACCACTACTATAAATGGCGCTTTTAGCACAGTAATATACGGCCGTGTCATCTGCTCTCATGATGTTAATATGCAGATACAG
++
+FFFF:FF:F,,FFF:,FF,,FFF:FF:FFFF,FFF,F,,,,,,F:F,FFFFF:FFFFF,F:FFFFFFF,FFFFF:,:F,FFF,F,:,F:,FFF,,F,FF,,FFFFFFF,,,FF,FFFF,F:,FFFF,FF,,,F:,,,FF,F:,F::,FF:,
+@A00604:387:HLC22DSX2:3:1101:17020:12023 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGGGTTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGAGCTCTCGCACAGTAATACACGGCCGAGTCGTCAGATCTCAGGCTCCTCAGATC
++
+FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFF:FFFFFFFF,FFF,F,:F:FFFFFF,:,F:FFFFFFFFF,,FFFFFF:FFFF:FF,FFFFFF:,FFF,FFFF:F,FF,,F,:,FFFFFFF,,FF:F::F:,FFFF,FF
+@A00604:387:HLC22DSX2:3:1101:21847:12023 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:16523:12038 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGATTCCCAGCCACTGCTGTGTCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAACTGCAGGGAGAACTGGTTCTT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32687:12070 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGACGTCCATACCGTTGCCAGTCATGGGTGACACAGCCCCCTCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGCCTGCTCAGCTCCATGTAGGC
++
+FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFF::FF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:21685:12085 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:23167:12085 2:N:0:ACAGGATG+GGACTACA
+CTGAACCGCCACCACCACTCGAGACGGAGAACGTGCACCATAGCCACCATATAACAAAAGCATCACAGACGTAGTCACCCTAGTAATCAGCATCAGATGGCGTGACAAGACACGCACAGAAAAACATAGCTGTGTCAGATGCCAACAGGCT
++
+FFFFFFF,FF:FFF,FF,FF,:,FF:F,F,,FFFF,,FF,F,,FF::FF,,FF,,FFF:FFF,FFF,F:F,FFFF,F,F,FFFF,F:,F::FFF,,::,:F,,F,F,,FFF:,FF:,F,,FF:,,FFF,F,FFFFF,FF,,FF,,FF:F:,
+@A00604:387:HLC22DSX2:3:1101:6922:12226 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATGTAGTAGTAGTAGTAGTTTGAGTAGCAGCTACCACCACTACAATACTCGCTGATCTCTCTCGTACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:7383:12242 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF,FFFFFFFFFFFFFFFFFFF:,FFF,FFFFFFFFFFFFFF:,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18069:12242 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,FFFFFFFFF:FFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:19506:12383 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGTAGCCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:1958:12399 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFF,:FFF,F:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:14724:12461 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:F:FFFF:FF:FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9046:12524 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:19931:12555 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFF:FFFFFFF:FF::FFFFFFFFFFFFFFFFFFFFFFFFFF:FF,FFFF
+@A00604:387:HLC22DSX2:3:1101:8856:12602 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:9218:12602 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22182:12665 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22996:12665 2:N:0:AGAGGAGG+GGACTGCT
+TAAACAGCCTACACCAATCTAGACGGTTACCACGGTACCCTGGCCACAGTAGTCAACAAACCAGCCACTGCAATAGGCCCTGTAACCGCATGAACAGTAATAAACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCAACTAGGATTTG
++
+F,,FF,,,,F:,FF:,,FF,F,:,F,F,FF,F,,F:,FF::,,,,,FF,,:,F:,FF,,F,FF,,,F:F,F,FF:::F,F,,F,FFF,,F,,::F,:,FFFF,,:FF:FFFF,,FF:F,FFFF:FF,F,F,FFFFF:FFF:,FF:F:F,FF
+@A00604:387:HLC22DSX2:3:1101:29550:12743 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTAGCAGCTACCACCACTACAATAACCCGAAACATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFF:FFFFFFFFFFFFF,FFFFFFFF::FF,FFFF:,FFFFFFF::::FFFF,FFFF:::::,,FFF:F::F,FFFF:FFFF:FF,F:FFF,F:F:F,,FF,,F,,F,FFFFFF,,:F:::,FF,FFFFFFF,:FFF,FFF:F,F:
+@A00604:387:HLC22DSX2:3:1101:5810:12774 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF:F:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:23475:12774 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACCCCATCAGATCTCTCGCACAGTAATACCCGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCCTGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFF,FFFF:FFFFFFFFFFFFF:FFFFFF:,FF:FF:,FF,FFFF,F:FF:,,FFF:,F:F,,F,F:,FFFFFF,FF,::F:F:,FF:FFFFF,FFF:F:FFF,,FF,FF,:F:
+@A00604:387:HLC22DSX2:3:1101:20374:12853 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF,FFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24740:12868 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATCCACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:6099:12900 2:N:0:AGAGGATG+GGACTACT
+CTGAAACGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACAAACAGAACTCTCGCACAGTAATACACGGCCGTGACGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFF,,:FFFFFFF,F,FF:FFFF,FFFFFFFFF,FF:F,FFFF:F:FFFFFFF::F:FF:FFFFFFFFFFFFFFFFF,F,FF,F,F:FFFF,FF,FFFF:FFFFFF:FF:F,FFFFFF::,FF::FFFFFFFF::F,,F:F,:F,FFFF
+@A00604:387:HLC22DSX2:3:1101:25563:12915 2:N:0:AGAGGATG+GGACTACT
+AACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FF
+@A00604:387:HLC22DSX2:3:1101:12635:12947 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATAAATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCATCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFF:FFFFFFFF,F:FFF,::,FFFFF,FFFFFFFFF:FFF,FF,F,:FFF::FF:FFFFFF:FFFF::FFFFF:F,FF:,F:F::FFF:FFFFFFFF,FFFF:F,FF:FFF,F,F,:F:F,F:F,FFFF:FF,F:,FFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:14787:13009 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26196:13009 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:,:F,FFFF,FFFFFFFFFF::FFF:F,FFFF:::FF:FFFFF::FFFF:F,FFFF,FF:FFF:F,FFFFF,FF,FFFFFFFFF,FFFFFFFF,,FFFF:,FFF
+@A00604:387:HLC22DSX2:3:1101:28438:13009 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF,FF,,F,FF:,FFFFF:FFF,FFFFFFFFFFF::FFFF:F:FFF:,FFFF,FFFFFF::F,FFFF,FFF:FFFFFF:::FFF,FFF:F:F,F,:,,:::F,FFFFFFF:FFFFFFFF,::FF:,FFFFFFFFFFF:FFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:17861:13166 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:8232:13307 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF,FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFF:F:FFFF
+@A00604:387:HLC22DSX2:3:1101:27570:13322 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFF,FFFFFFFFFFFFFFFF::FFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFF,FFFFF:FFFF,F:FF,FFFFF:F:F:FFFF:FFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28845:13463 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:21423:13542 2:N:0:AGAGGATG+GGCCTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGCCGGAGTCGCAGCTACCACCACTCCAATATCCCGAAACTTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFF,FF,FFFF:,F:FFFFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFF:FFF:
+@A00604:387:HLC22DSX2:3:1101:32235:13542 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCTATATTACAATAATACCCCCACTCTCTCTCACAGTAATAAACGGCCGTGTACTCAGA
++
+F:FFFFFFFF,FFFFFFFF,FFFFF:FF,FFFFFFFFFFF,F,FFFFFF:F,:FFFF,FF:F:F,,FFFF,FF:,:,,F,FFFFF:FF,FFF::,,,F,,FF:FFFF,F,,,,F,,,FFFFF,FF,,F,,F:F:FF,,F,,,,,,F,:::F
+@A00604:387:HLC22DSX2:3:1101:31512:13573 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24659:13604 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCATGTCCCGCCCCACCACTCCAAAAATCCCCTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3784:13683 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:27245:13730 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFF:FFFFFFFFFFFFFF:FFFF:FFFFFFFFFFF:FFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3676:14278 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTAATACGAGTAGCAGCTACCACCACTACAATATCCCGTTAATTCTCTCGCACAGTAATATACGGCCGTGTCTTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF,FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:1561:14591 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:
+@A00604:387:HLC22DSX2:3:1101:20365:14591 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTCTCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFF:FFFFFFFFFFFF,FFFFFFFFFFFFFF,FFF,FFFF,FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FF:FF,FF,FFFFFFFFFFFF:FFFFF,,FFFFF::FFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1101:7808:14732 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:6379:14763 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCGTTGTGGTAGCAGCTACCACCACTACAATATATCCCCCCCGCACAGTAATACACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:F:FFFFFF:F,F,FFF:F:FFF:FFFF,FFFFFFFFFFFFFFFFF,F::FFFFF:FFF:FFF
+@A00604:387:HLC22DSX2:3:1101:9381:14763 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1101:8169:14794 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCATCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCATCCCCTGCTATACCAGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCGCAGATCTCAGGCTGCTCAG
++
+::::FFF,F,FF,F:F,F,,:FFFF,,F:FF,FF:,FFF::F::,FFFF:FF:FFF,FFFFFFF,,FFFF:FFFFF,,,,,FFFFF:FFF,FF:F:F:,F:FFF,F,:FFFF,FFFFFF:FFFFFFF,,F,,F,:FFFFFFF:FFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:1823:14888 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FF:FFFFFFFFFFFFF:F:FFFFFFFFFFFFF:,FF:FFFFFFFFFFFFFF::FFF:FF,FFFFFF:FFF::FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,F,F:F:FFF,FFFFFFFFFFFFFFFF,FFF:FFFFFF:FFFFFF
+@A00604:387:HLC22DSX2:3:1101:5330:14888 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCGATACCCGGCCTTGGGCTCCCTCGCACAGTCATACACGGCCGTGTCCTCAGCTCTCAGGCTGCTCAG
++
+FF:FFFF,FF:,F,FFFFFFFF:FFFFFFFFFFFFF,FFFFFFFFFF,FFF,FFFFFFFFF:F:FFF,FF::F:FF,FF:,:F:,FFFFFFFF,,,:FFFFFF:FFF:FFFFFF,FFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:19886:15013 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:F:
+@A00604:387:HLC22DSX2:3:1101:32271:15076 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF:FFFFFFFF,F,FFFFFFFFFFFFFFFFFFFFF:FFFF:FF:FFFFFFFFF::,:FF,FFFFFF
+@A00604:387:HLC22DSX2:3:1101:27543:15092 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF,FFFFF,FFFFFFFFFFFFF:FFFFFFFFFFFFFF:FF:,FFFFFFFFF,,F:FFFFFF:FF:FFF:FF,FFFFF:FFFF:F:FFFF:FFFFFF::FFFFFFF:FFF::FFFFFFFFFFF::FFF:FFF,FFFFFF,FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5746:15139 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCT
++
+FFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FF:FFFFFFFF,FFFFFFFFFFF:,FF
+@A00604:387:HLC22DSX2:3:1101:12210:15217 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,:FFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFF,FFFFFFF::FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32868:15233 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFF:FFFFF,FFFFF:F:F:FFFFFFF,FFF:F:FFF:FF:FFFFFFF,F::FFFF:,FF:,F,F:FFF,FFFFF:FF:,FFF,FF:F:F,FF
+@A00604:387:HLC22DSX2:3:1101:7771:15264 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCCCAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF,FFF:,FFFFFFFFFFFFFF:F,FFFFFFFFFFFFFFFFFFF,FFFF,FFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11243:15421 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFF:FFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFF:FFFF:,FFFFFFFFFFF,FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3992:15702 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF,FFFFFFFFFFFFFFFFFF:FF:FFFFFFF:F:FFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFF,FF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF,FFFFF,F,,FFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:3920:15734 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCCCAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FF:FFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,,FFFFFFFFFFFFFFFF:FFFFF:FF:FFF:FFFFFFFFF:,FF,FFFFFFFFFFFFFF,FFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF
+@A00604:387:HLC22DSX2:3:1101:10809:15734 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFF:FFFFFFFF,FFFFFFFFFFFF::::FFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:32045:15843 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FF:FFF,FFFFFFFF:F:FFF,FFF
+@A00604:387:HLC22DSX2:3:1101:28221:16047 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:28890:16172 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFF:FFF:F::FFF
+@A00604:387:HLC22DSX2:3:1101:6171:16188 2:N:0:AGAGGATG+GGACTAAT
+CTGAACCGCCTCCACCCCTCGAGACGGTGACCATTGTCCCTTGGCACCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+F,:F:FF:F,:F,,,F,,F:F,F,FF,FFFFFF,F:FFFFFFFFF,F:F,F:FFFFF::FFF,FFFFF:FFFF:FFFFFFF,:F,F::F:F:FF::FFFFF:FFF:FFF,FFFFF,F:,FFF:FF,F::FF,FFFFFFFF,FF:FF,FF:F
+@A00604:387:HLC22DSX2:3:1101:18204:16329 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATGTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18358:16438 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFF::FFFFF,FFF:F:FFFFF:FFFFF:FFFFFFFFFFF:F:FFFFFFFFFFFFFF:::FF,FFFFFFFFFF:FFFFFFFF:F:FFFFFFFF:FFFF:FFFFFFFFFFFFFFFF:F,:FFFFF:FFFFFFFFFFFFF::FFFF:
+@A00604:387:HLC22DSX2:3:1101:15230:16564 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+F:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28393:16752 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGACTCCACCACTCGAGACGGTCACCGTGGTCCCTTGCCCCCAGATATCAAAAGCACCAATCTCCGCATCCCCATCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGT
++
+F,,FF,F:,F,:FFFFFF,F,FFF,,:F,FFF,,FF:F,::F:FFF,:FFF:FFFFFFF,FFFF:F,F:,F,FF:FFF:F:F,FFF,F::::::FFFFFF,FFFFF,,:FFFFFFFF:FFFFFFFF,:FFFFFF,FF::,,FFFF,,,FFF
+@A00604:387:HLC22DSX2:3:1101:3540:16830 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF
+@A00604:387:HLC22DSX2:3:1101:6596:16892 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:4878:16955 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFF:F:FFFF:FFFFFFFFFF:FFFFF:FFFFFF:F,FFFFFFFFFFFFF:FFFFFFFFFFFF,FF,,F,FFFFFFFFFFF:FFF,F,FFFFFFFFFFFF:FF::FFF:FFFFFFFF::FFFFFFF:FFF:FFF:FFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:21884:17002 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFF:FF,FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11840:17018 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTCCTCCGAGTAGCATACACCGTTAGTACAATAATACCCCCTCTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFF,FF:FFFFF:FFF,FFFFFFFFFFFFFF,,F:FFF,,:FFFFFFFF:FFFFFFFFF:FFF:F,FFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18837:17049 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF:FFFFF:FFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF,:FFFFFFFFF,FFFFFFFFFFFFFFFF,FF:FFFFFFFFFFFF:F
+@A00604:387:HLC22DSX2:3:1101:27959:17190 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,
+@A00604:387:HLC22DSX2:3:1101:4345:17253 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFF:FFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFF:F,FFFF:F:
+@A00604:387:HLC22DSX2:3:1101:20998:17284 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26567:17315 2:N:0:AGAGGCTG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:27724:17409 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFF:FFFFFF:FFF:FFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:28429:17440 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGTAGTCGGAGTAGCAGCTACCACCACTACAATATCCTACGGGCTCCCCTCTCGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20302:17550 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCATACCGTAGTAGTAGTAGTAGTCTGAGTAGCAGCTACCACCACTACAATATCCTATCCCCGTTGTTGCACAGTAATACACGGCCGTGTCCTCAGA
++
+FFFF:F:FFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFF,FFFF:FFFFFFFFF:FF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFF,FF,FFFFFFFF:FFFFFF,FFFFFFFFFFFFFFFF,:FFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:14651:17785 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:8449:17816 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTACCACCCCCGGGATCCATCTCGTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGA
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF,FFFFFFFF::FFFFFFFFFFF:FFFFFF,,FFFF:FF:FFFFFFFFFFFFF:FFFFF
+@A00604:387:HLC22DSX2:3:1101:23909:17816 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTTGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGAGTCCTCAGAACTCAGGCAGCTCAG
++
+F,,FFFF:FFFFFFFFFF,FFF,FFF:,:FFFF,:F,F::,,,FFF,FF:FF,:,F,,F,FFFF,,,:,F,F:FFFFF::F,FFFF,:F,FFFFF,::,FF:FF::F,FF:::F,FFFF,,F,FF,,F:,FFF::F,F,FFF,,,,:FFFF
+@A00604:387:HLC22DSX2:3:1101:11885:17848 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,F:FFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22887:17926 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:11478:17957 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGTTACCACCACTACAATAACCCCCTCTTGCACCGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,F,FF,FFFF,FFFFFFFFFFFFFFFFFFFF,FFFFF::FFFFFF
+@A00604:387:HLC22DSX2:3:1101:29514:18004 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFF,FFFFFFFFFFFF,FFFFFFF:FFFFFFFFFFFFFFFFFF:FFF::FFFF,:FFFFFFFFFFFF:FFFF,F:FFFFFFFF:FFFFFFFF,FFFF
+@A00604:387:HLC22DSX2:3:1101:28375:18129 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGATATCAAAAGAACGGACGAATCCCGTGTCTGGTCTCGCACAGTAATACATGGCGGTGTCCGAGGCCTTCAGGCTGCTCCACTGCAGGTAGGCGGTGCTGAT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:30933:18176 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGCGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFF,FFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:8793:18255 2:N:0:AGAGGATT+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFF:FFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:25491:18302 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACCAAAATCGTTGACAGATCTCTCGCACAGTACTACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FFFFFFF:FFF:F,FFFFFF,F:FF,F:F:F:F:FFFF,:F,FFF,:F,,,FFF:,FFFFFFFFFFFF,F:FFFFF,FFFF:FF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26142:18458 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFFFF,FFFFFFFFFF:FFF::FFFFFFFF:FFFFFFFFFFF:F:FFFFFFFFFFFFFFF:FFFFFF:FF,FFFFFFFFFFFF:FFFFF:FFFFF:FFFFF,FF,FF
+@A00604:387:HLC22DSX2:3:1101:12355:18474 2:N:0:AGAGGATG+GGACTACT
+CAGGCTCCTCAGCTCCATGTAGGCTGTGCTCGTGGATGTGTCTGTGGTCATGGTGACTCTGCCCTGGAACTTCTGTGCATAGTTTGTGCCACCACTGTTAGGGTTGATCCATCCCATCCACTCAAGCCCTTGTCCAGGGGCCTGTCGCACC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:28501:18568 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFF:FFF:FFFFFF:FFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFF,FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:24532:18677 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFF:FFFFFFFFFFFFF,FFFF,FFFFF::FFFFFFFF:FFFFF:FF:FFFFFFF:FF:F:F,FFF,:FFFFFFF:FFFFFF,FFFFFFFFFFFFFFFFF,FFFFFFFF:FFF:FFF:FFFF:FFFFFFF:FF:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:10411:19022 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGCCTGCCGCGTACCAGCCACTGTCAAACACCTCCACCGGGGTCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF,FF,F:FFFFFFFFFFFFF:FFFFFF,FFF,FFFFFF:FFF
+@A00604:387:HLC22DSX2:3:1101:11731:19147 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAAGTAGGCGTCGGTGTAGCAGCTACCACCACTACAATATCTATCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTCAGGCTGTTCATTTG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFF,FFFFFF
+@A00604:387:HLC22DSX2:3:1101:27163:19225 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAACGTACCAGCCACTGCTATAGGCCCTGTAACCGGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:30355:19304 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF:FFFFFFFFFFFFFFF:FFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:13286:19429 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFF:FFFFFFFFFFFFF,FFFFFF:FFFFFFF,F,FFFFFFFFFFFF:FFFFFF,FFFF,FFFFFFFFFF::FFFFFF:FFFFF:F,FFFFFFF,FFF:FFFFFFFFFFFFFF,FFFFF:FFFFFFFFFFF:FFF,F:FFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:4553:19836 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF::FFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FF:F:FFFFFFFFFFFF:FFF:FFFFFFF,,FFFFF:FFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:8133:19867 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCAAACCCCCCAATTGTATAGCATACACCACCAGTACAATAATTGACTGTTGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFFFFFF:FFFFFFFFFFFFF:FF:FFFF
+@A00604:387:HLC22DSX2:3:1101:16993:19993 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCACGGCCCCAGACGTCCATACCGTAGTAGTAGTCTAAGGTAGAGTCTCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAGCTCCATGTAGGCTGTGCT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:12825:20071 2:N:0:AGAGGATG+GGAATACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGTAGTCGCCGTACCAGCCACTGCTATACACCATCAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTCCATGTAGGCTGT
++
+FFFFFFFF,FFFFFFFFFFFFF,:FFFFFFFFF,F:FFFF:,:FFFFFF:FFFFFFFFFFFFF::FFFFFFF,FFFFFFFFF:FFFFFFF:FFFF:FFFFFFFFFF::FFF:FFFFFF,FFFFFFF,:FFFFFFFFFFFFFFF:FF::FF,
+@A00604:387:HLC22DSX2:3:1101:23556:20212 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:15320:20290 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCA
++
+FFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF:FFFFFFFFFFFFF:FFFFFFFFFFF:FFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:21404:20337 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGACTCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAGGGAGAACTGGTTCTTGGATGT
++
+:F:FFFFFFFFFFFFF:FFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFF:FFF::FFFFFFFFFFFFFFFF,FFFFFFFFFFFFFF,F:FFFFFFFFFF,FFFFFFFFF:F,FFFFFF,F,FFFFF,FFF,FFFFFFFFF:FFFFFFF:
+@A00604:387:HLC22DSX2:3:1101:8712:20494 2:N:0:CGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTCCCCATACCAGCCACTGCTATACCAGGTTCCCCCACTTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTGCAG
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:18005:20494 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCTTGGCCCCAGATATCAAAAGCATCGGTGTCATCCCCTTTATAATAACCACTCCAAATATCGTAATACGTTCGAAGCGGGCCACTCGCACAGTAATACACGGCCGTGTCGTC
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,::FFFFFFFFFFFFFFFFF,FFF:FFFFFFFFFFFF:F,FFF:FFFFFFFFFFFFFF:FF:FFFFFF,F:FFF:FFFF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:5077:20525 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGTAGTCAAAGTAGTATTTCTCGTAGCAGCTACCACCACTACAATAACCCCCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCACAGAGTTCAGCTG
++
+FFFFFFFFFFFFFFFFFFFFFFF:FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFF::FFFFFFFFFFF,FFFFFF:FFF,F:FFF:FFFFF:F,FFFFFF:FF:FFFFFFF:FF:F,F,FFFF:FF::FFFFF:F:F:F,FFF,FF,F:FF
+@A00604:387:HLC22DSX2:3:1101:12563:20525 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGACGTCCAAAGCGCCGTAGTAATAAGCACCAGTATCATAGTAATAAATGTGGGCTCTCGCACAGTAATACACAGCCGTGTCTTCAGATCTCAGGCTGCTCAG
++
+:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF,:FFFFFFFFFFFFF:FFFFFFFFFFFF:FFFFF::FFFFFFFFFFFFF,FF:FF:FFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:26133:20603 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+FFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFF,FFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:22724:20838 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGACGTCCATACCGTAGTAGTAGAGGTAGCAGCTACCACCACTACACCTCAACTCTCTCGCACAGTAATACACAGCCGTGTCCTCAGCTCTTAGGCTGTTCAT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFF,FFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:20139:20901 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCATTGTCCCTTGGCCCCAGACATCAAAAGCACCGATGTCGTACCAGCCACTGCTATACCCGGCCTTGGGCTCCCTCGCACAGTAATACACGGCCGTGTCCTCAGATCTCAGGCTGCTCAG
++
+FFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFF:FFFFF:::FFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:9362:20964 2:N:0:AGAGGAGG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTTCCCTGGCCCCAGTAGTCAAGGCCAGCCACTGCCGAATCTCTTGCACAGTAATACACAGCCGTGTCCTCGGGAGTCCCAGAGTTCAGCTGCAGGGAGAACTGGGTCTTGGAGGT
++
+FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFF:FFFFFFFFFF:FFFFFFF,FF,FFFFFFFFFFFFFFFFFFFFFFFFF,FFFFF,FF,FF,F:,FFF,F:,:FFF,FF:FFFF,FF
+@A00604:387:HLC22DSX2:3:1101:28103:20979 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCGTGGTCCCTTGCCCCCAGTAGTCAAAGTCCAAGTAATAACCACTACTATACATGGCGCTTTTCGCACAGTAATATACGGCCGTGTCCTCGGCTCTCAGGCTGTTCATTTGCAGATACAG
++
+FFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF,FF,FFFFFF:F:FFFF:F:FFFF:FFF,FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFF:FFFFFFFFFFF
+@A00604:387:HLC22DSX2:3:1101:32262:21010 2:N:0:AGAGGATG+GGACTACT
+CTGAACCGCCTCCACCACTCGAGACGGTGACCAGGGTGCCCTGGCCCCAGGGGTCGAACCACCCACTCATTCGTTCATACACAAAAATCGTTGACAGATCTCTCGCACAGTAATACACGGCCGTGTCGTCAGATCTCAGGCTCCTCAGCTC
++
+,FFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFF:FFFFFFFFFFFFFFFFFFFF:FFFFFFFFF:FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF:F
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/test_uploader.py` & `ExpoSeq-1.1.14/src/ExpoSeq/test_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     if not os.path.isdir(os.path.join(module_dir, "my_experiments")):
         os.mkdir(os.path.join(module_dir, "my_experiments"))
     if not os.path.isdir(os.path.join(module_dir, "temp")):
         os.mkdir(os.path.join(module_dir, "temp"))
     if not os.path.isdir(os.path.join(module_dir, "my_experiments", "test_directory")):
         new_dir = os.path.join(module_dir, "my_experiments", "test_directory")
         os.mkdir(new_dir)
-        source_seq_report = os.path.join(pkg_dir, "test_data","test_files", "sequencing_report.csv")
+        source_seq_report = os.path.join(pkg_dir, "test_data", "test_files", "sequencing_report.csv")
      #   source_align_report = os.path.join(pkg_dir, "test_data", "all_alignment_reports.pickle")
-        source_experiments = os.path.join(pkg_dir, "test_data","test_files", "experiment_names.pickle")
+        source_experiments = os.path.join(pkg_dir, "test_data", "test_files", "experiment_names.pickle")
         assert shutil.copy2(source_seq_report, new_dir), "could not copy sequencing report"
      #   shutil.copy2(source_align_report, new_dir)
         shutil.copy2(source_experiments, new_dir)
     else:
         pass
     
     #upload(testing=True, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1')
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.14/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.13
-Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
+Version: 1.1.14
+Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns.
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to ExpoSeq
 
-ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](expoSeq_overview.png)
+ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
 
 To get started, please download and follow the instructions for MiXCR under the following link: https://docs.milaboratories.com/mixcr/getting-started/installation/ 
 You can also only use the test version without installing it.
@@ -29,15 +29,15 @@
 If you want to use the fast and easy version you can ignore the rest of the instructions and just import in your Console:
 ```import ExpoSeq.run```
 ## Using the PlotManager
 
 The PlotManager is the main interface for creating various plots using your FASTQ data. You can create an instance of the PlotManager by running the following command:
 ```plot = PlotManager()```
 To use the PlotManager to create plots, you will need to upload your FASTQ data to the pipeline. This will automatically happen as soon as you have called the PlotManager. In the following you can obtain an insight in the worklow of the pipeline after the initial call. There, the blue boxes indicate your input, gray are optional inputs while black and red are processing steps and output, respectively.
-![relative_path_to_image](workflow_ExpoSeq.png)
+![relative_path_to_image](pictures_gen/workflow_ExpoSeq.png)
 If you just want to test the pipeline and see its functions you can call: ```plot = PlotManager(test_version = True)```
 
 Once you have called the test version or have finished the data processing, you can use the PlotManager to create a variety of plots, such as an identity plot based on the jaccard similarity. Here is an example of how to create this type of plot:
 ```plot.jaccard()```
 If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
 ```import matplotlib.pyplot as plt```
```

### Comparing `ExpoSeq-1.1.13/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.14/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

