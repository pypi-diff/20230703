# Comparing `tmp/ExpoSeq-1.1.12.tar.gz` & `tmp/ExpoSeq-1.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.12.tar", last modified: Mon Jul  3 08:34:58 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.13.tar", last modified: Mon Jul  3 08:58:54 2023, max compression
```

## Comparing `ExpoSeq-1.1.12.tar` & `ExpoSeq-1.1.13.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:58.209170 ExpoSeq-1.1.12/
--rw-rw-rw-   0        0        0    11558 2023-06-30 13:21:19.000000 ExpoSeq-1.1.12/LICENSE
--rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.12/MANIFEST.in
--rw-rw-rw-   0        0        0     4107 2023-07-03 08:34:58.209170 ExpoSeq-1.1.12/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.12/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 08:34:58.209170 ExpoSeq-1.1.12/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-07-03 08:33:19.000000 ExpoSeq-1.1.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:57.837161 ExpoSeq-1.1.12/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:57.877242 ExpoSeq-1.1.12/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:57.942520 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7915 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10619 2023-06-29 12:41:04.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6814 2023-07-02 11:44:34.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    17434 2023-06-29 12:43:18.000000 ExpoSeq-1.1.12/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-06-12 12:16:56.000000 ExpoSeq-1.1.12/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    39758 2023-07-02 13:01:57.000000 ExpoSeq-1.1.12/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:58.041027 ExpoSeq-1.1.12/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-02 09:18:51.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3348 2023-07-02 13:14:31.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4284 2023-07-02 13:14:50.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-02 12:03:32.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1634 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1136 2023-07-02 13:24:34.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2542 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:58.065027 ExpoSeq-1.1.12/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-06-12 12:10:03.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 12:10:03.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-06-12 12:10:03.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      179 2023-07-02 13:29:17.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-06-12 12:10:03.000000 ExpoSeq-1.1.12/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:58.073064 ExpoSeq-1.1.12/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:58.113063 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-06-16 09:43:27.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-06-16 09:43:29.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-06-16 09:43:29.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    87391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   210829 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    94420 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-06-12 12:05:40.000000 ExpoSeq-1.1.12/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:58.172889 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:58.202662 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-06-12 12:03:02.000000 ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:34:57.885163 ExpoSeq-1.1.12/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4107 2023-07-03 08:34:57.000000 ExpoSeq-1.1.12/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2971 2023-07-03 08:34:57.000000 ExpoSeq-1.1.12/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 08:34:57.000000 ExpoSeq-1.1.12/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-03 08:34:57.000000 ExpoSeq-1.1.12/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 08:34:57.000000 ExpoSeq-1.1.12/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/
+-rw-rw-rw-   0        0        0    11558 2023-06-30 13:21:19.000000 ExpoSeq-1.1.13/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     4107 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.13/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-07-03 08:58:26.000000 ExpoSeq-1.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.799871 ExpoSeq-1.1.13/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.840129 ExpoSeq-1.1.13/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.904496 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1007 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0     7915 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_cl.py
+-rw-rw-rw-   0        0        0    10619 2023-06-29 12:41:04.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6814 2023-07-02 11:44:34.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    17434 2023-06-29 12:43:18.000000 ExpoSeq-1.1.13/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-06-12 12:16:56.000000 ExpoSeq-1.1.13/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    39758 2023-07-02 13:01:57.000000 ExpoSeq-1.1.13/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.960495 ExpoSeq-1.1.13/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-02 09:18:51.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3348 2023-07-02 13:14:31.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4284 2023-07-02 13:14:50.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-02 12:03:32.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1634 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1136 2023-07-02 13:24:34.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2542 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.984511 ExpoSeq-1.1.13/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      179 2023-07-02 13:29:17.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:10:03.000000 ExpoSeq-1.1.13/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.992483 ExpoSeq-1.1.13/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.064646 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-06-16 09:43:27.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-06-16 09:43:29.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-06-16 09:43:29.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    87391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   210829 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    94420 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-06-12 12:05:40.000000 ExpoSeq-1.1.13/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.121623 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:54.152709 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-06-12 12:03:02.000000 ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:58:53.848402 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4107 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2971 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 08:58:53.000000 ExpoSeq-1.1.13/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.12/LICENSE` & `ExpoSeq-1.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/PKG-INFO` & `ExpoSeq-1.1.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.12
+Version: 1.1.13
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.1.12/README.md` & `ExpoSeq-1.1.13/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/setup.py` & `ExpoSeq-1.1.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.12",
+    version = "1.1.13",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
```

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_cl.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.13/src/ExpoSeq/augment_data/uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/full_pipe.py` & `ExpoSeq-1.1.13/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.13/src/ExpoSeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.13/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.13/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.13/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.13/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.13/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-1.1.13/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/test_uploader.py` & `ExpoSeq-1.1.13/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.13/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.13/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.12
+Version: 1.1.13
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.1.12/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.13/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

