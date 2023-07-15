# Comparing `tmp/ExpoSeq-1.1.14.tar.gz` & `tmp/ExpoSeq-1.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.14.tar", last modified: Sat Jul 15 09:48:25 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.16.tar", last modified: Sat Jul 15 11:29:00 2023, max compression
```

## Comparing `ExpoSeq-1.1.14.tar` & `ExpoSeq-1.1.16.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:25.462905 ExpoSeq-1.1.14/
--rw-rw-rw-   0        0        0    11543 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/LICENSE
--rw-rw-rw-   0        0        0       59 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/MANIFEST.in
--rw-rw-rw-   0        0        0     4134 2023-07-15 09:48:25.462905 ExpoSeq-1.1.14/PKG-INFO
--rw-rw-rw-   0        0        0     3751 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 09:48:25.462905 ExpoSeq-1.1.14/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-07-15 09:43:45.000000 ExpoSeq-1.1.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:22.742137 ExpoSeq-1.1.14/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:22.976516 ExpoSeq-1.1.14/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:23.612617 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7915 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10625 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6814 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    17750 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10311 2023-07-15 09:42:35.000000 ExpoSeq-1.1.14/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    40079 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.347021 ExpoSeq-1.1.14/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3292 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4284 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1724 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1136 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2542 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.518896 ExpoSeq-1.1.14/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1890 2023-07-15 09:42:35.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      179 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.550151 ExpoSeq-1.1.14/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:24.612645 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    88335 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   213105 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    95440 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2634 2023-07-15 09:42:35.000000 ExpoSeq-1.1.14/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:25.150394 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:25.416024 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-07-15 09:40:09.000000 ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:48:23.023384 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4134 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2971 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-15 09:48:22.000000 ExpoSeq-1.1.14/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.759494 ExpoSeq-1.1.16/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/MANIFEST.in
+-rw-rw-rw-   0        0        0     4133 2023-07-15 11:29:00.759494 ExpoSeq-1.1.16/PKG-INFO
+-rw-rw-rw-   0        0        0     3751 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 11:29:00.759494 ExpoSeq-1.1.16/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-07-15 11:28:40.000000 ExpoSeq-1.1.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.495241 ExpoSeq-1.1.16/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.526493 ExpoSeq-1.1.16/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.573915 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0     7915 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/mixcr_cl.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6814 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    19691 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10311 2023-07-15 11:21:27.000000 ExpoSeq-1.1.16/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    40754 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.620793 ExpoSeq-1.1.16/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3292 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4284 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1136 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2542 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.652117 ExpoSeq-1.1.16/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1890 2023-07-15 11:21:27.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      173 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.652117 ExpoSeq-1.1.16/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.683397 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2634 2023-07-15 11:21:27.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.728151 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.743782 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.526493 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4133 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2971 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.14/LICENSE` & `ExpoSeq-1.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/PKG-INFO` & `ExpoSeq-1.1.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.14
-Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns.
+Version: 1.1.16
+Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ExpoSeq-1.1.14/README.md` & `ExpoSeq-1.1.16/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/setup.py` & `ExpoSeq-1.1.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.14",
-    description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns.",
+    version = "1.1.16",
+    description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
     package_data={
```

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/binding_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,12 +21,16 @@
         except:
             while True:
                 binding_file = input("copy and paste the path to your binding report")
                 if os.path.isfile(os.path.abspath(binding_file)):
                     break
                 else:
                     print("Please enter a valid filepath. ")
-        binding_data = pd.concat([binding_data, binding_file])
+        if binding_file.endswith(".xlsx"):
+            binding_new = pd.read_excel(binding_file)
+        elif binding_file.endswith(".csv"):
+            binding_new = pd.read_csv(binding_file)
+        binding_data = pd.concat([binding_data, binding_new])
         response = input("Do you want to continue adding files? (Y/n) ")
         if response.lower() == "n":
             break
     return binding_data
```

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/mixcr_cl.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,26 @@
     seq_report_dir = os.path.join(module_dir,
                                   "my_experiments",
                                   experiment,
                                   "sequencing_report.csv")
     sequencing_report.to_csv(seq_report_dir)
     return sequencing_report,all_alignment_reports, experiment
 
+
+def write_last_exp(pkg_path, experiment):
+    glob_vars = os.path.join(pkg_path,
+                             "settings",
+                             "global_vars.txt")
+    with open(glob_vars, "r") as f:
+        data = f.read()
+    data = literal_eval(data)
+    data["last_experiment"] = experiment
+    with open(glob_vars, "w") as f:
+        f.write(str(data))
+
 def check_last_exp(pkg_path, module_dir, testing):
     if not testing:
         glob_vars = os.path.join(pkg_path,
                                 "settings",
                                 "global_vars.txt")
         with open(glob_vars, "r") as f:
             data = f.read()
@@ -364,24 +376,44 @@
 def upload(testing=False, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1'):
    # module_dir = os.path.abspath("")
     module_dir = os.getcwd()
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     repo_path, last_experiment = check_last_exp(pkg_path, module_dir, testing)
 
     if os.path.isfile(repo_path):
-        continue_analysis = get_continue_analysis_input(last_experiment, testing,continue_analysis)
+        continue_analysis = get_continue_analysis_input(last_experiment,
+                                                        testing,
+                                                        continue_analysis)
         if continue_analysis.lower() in ["n", "no"]:
             next_step = get_next_step_input(testing, choose_exp)
             if next_step == "1":
-                sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,repo_path, testing, upload_type, paired_end_test, experiment_column)
+                sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,
+                                                                                             repo_path,
+                                                                                             testing,
+                                                                                             upload_type,
+                                                                                             paired_end_test,
+                                                                                             experiment_column)
             elif next_step == "2":
-                experiment = choose_existing_experiment(module_dir, testing)
-                sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir, experiment, testing)
+                experiment = choose_existing_experiment(module_dir,
+                                                        testing)
+                sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir,
+                                                                                        experiment,
+                                                                                        testing)
             else:
                 raise ValueError("Invalid option")
         else:
-            sequencing_report, all_alignment_reports, experiment = process_data_with_last_experiment(module_dir, last_experiment, testing)
-    else:
-        sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir, repo_path, testing, upload_type, paired_end_test, experiment_column)
+            sequencing_report, all_alignment_reports, experiment = process_data_with_last_experiment(module_dir,
+                                                                                                     last_experiment,
+                                                                                                     testing)
+    else:
+        sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,
+                                                                                     repo_path,
+                                                                                     testing,
+                                                                                     upload_type,
+                                                                                     paired_end_test,
+                                                                                     experiment_column)
     if testing and experiment != "test_directory":
         shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
+    
+    if not testing and experiment != "test_directory":
+        write_last_exp(pkg_path, experiment)
     return sequencing_report, all_alignment_reports, experiment
```

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/full_pipe.py` & `ExpoSeq-1.1.16/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.16/src/ExpoSeq/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,26 @@
             experiment_path = os.path.join(self.module_dir,
                                             "my_experiments",
                                             self.experiment,
                                             "experiment_names.pickle")
             with open(experiment_path, "rb") as f:
                 self.unique_experiments = pickle.load(f)
             self.sequencing_report["Experiment"] = self.sequencing_report["Experiment"].map(self.unique_experiments)
-            self.add_binding = input("Do you have binding Data? Y/n")
-            if self.add_binding.lower() in ["Y", "y"]:
-                self.binding_data = collect_binding_data()
-            else:
-                self.binding_data = None
+            self.binding_data_dir = os.path.join(self.module_dir,
+                    "my_experiments",
+                    self.experiment,
+                    "sequencing_report.csv")
+            if not os.path.isfile(self.binding_data_dir):
+                self.add_binding = input("Do you have binding Data? Y/n")
+                if self.add_binding.lower() in ["Y", "y"]:
+                    self.binding_data = collect_binding_data()
+
+                    self.binding_data.to_csv(self.binding_data_dir)
+                else:
+                    self.binding_data = None
                 
                 
         font_settings_path = os.path.join(self.pkg_path,
                                           "settings",
                                           "font_settings.txt")
         assert os.path.isfile(font_settings_path), "The font settings file does not exist in the given filepath"
         with open(font_settings_path, "r") as f:
@@ -122,15 +129,22 @@
   #  def askMe(self):
    #     """
     #    :return: calls the chatbot which can help you to customize your plots or with other question in life and science.
      #   """
       #  askMe(self.global_params)
 
     def add_binding_data(self):
+        """"
+        :return: adds binding data to your analysis. You can add mutliple files with the filechooser or a given path to the file. For more information about the necessary file structure, check the supplementary information.
+        """
         self.binding_data = collect_binding_data(binding_data = self.binding_data)
+
+        self.binding_data.to_csv(self.binding_data_dir)
+            
+        
     def print_antigens(self):
         """
         :return: prints the antigens (columns) of your binding data
         """
         try:
             print(self.binding_data.columns.to_list()[1:])
         except:
```

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.16/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.16/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.16/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.16/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.16/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/test_uploader.py` & `ExpoSeq-1.1.16/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.16/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.14
-Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns.
+Version: 1.1.16
+Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ExpoSeq-1.1.14/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.16/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

