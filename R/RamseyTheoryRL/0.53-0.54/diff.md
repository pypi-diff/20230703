# Comparing `tmp/RamseyTheoryRL-0.53.tar.gz` & `tmp/RamseyTheoryRL-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RamseyTheoryRL-0.53.tar", last modified: Mon Jul  3 03:35:28 2023, max compression
+gzip compressed data, was "RamseyTheoryRL-0.54.tar", last modified: Mon Jul  3 03:43:15 2023, max compression
```

## Comparing `RamseyTheoryRL-0.53.tar` & `RamseyTheoryRL-0.54.tar`

### file list

```diff
@@ -1,61 +1,71 @@
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.688487 RamseyTheoryRL-0.53/
--rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.53/LICENSE.txt
--rw-r--r--   0 stevevott   (501) staff       (20)     2826 2023-07-03 03:35:28.688358 RamseyTheoryRL-0.53/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)     2161 2023-07-03 03:33:06.000000 RamseyTheoryRL-0.53/README.md
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.681876 RamseyTheoryRL-0.53/RamseyTheoryRL/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.682498 RamseyTheoryRL-0.53/RamseyTheoryRL/data/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:29:43.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.682592 RamseyTheoryRL-0.53/RamseyTheoryRL/data/csv/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:34.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/csv/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.682692 RamseyTheoryRL-0.53/RamseyTheoryRL/data/csv/scaled/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:37.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/csv/scaled/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.682786 RamseyTheoryRL-0.53/RamseyTheoryRL/data/csv/unscaled/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:40.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/csv/unscaled/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.682889 RamseyTheoryRL-0.53/RamseyTheoryRL/data/found_counters/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:45.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/found_counters/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.683001 RamseyTheoryRL-0.53/RamseyTheoryRL/data/found_counters/scaled_dnn/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:48.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/found_counters/scaled_dnn/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.683123 RamseyTheoryRL-0.53/RamseyTheoryRL/data/isomorphic_by_n/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:34:05.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/isomorphic_by_n/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.683251 RamseyTheoryRL-0.53/RamseyTheoryRL/data/time/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:34:20.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/data/time/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.683357 RamseyTheoryRL-0.53/RamseyTheoryRL/src/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.684465 RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:29:39.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)    12523 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/gbfs.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3539 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1070 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/igraph_train_gen.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1157 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/isofile_checker.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3365 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/train_gen.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.685427 RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-07-03 03:24:44.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
--rw-r--r--   0 stevevott   (501) staff       (20)     9795 2023-07-03 03:26:34.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)     8240 2023-07-03 03:26:39.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)    11528 2023-07-03 03:26:46.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/test.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.686531 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/gfeatures.py
--rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/guseful.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.687301 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
--rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.688070 RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:09.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1401 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/datavis.py
--rw-r--r--   0 stevevott   (501) staff       (20)      827 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/param_plot.py
--rw-r--r--   0 stevevott   (501) staff       (20)      788 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/r39_graph.py
--rw-r--r--   0 stevevott   (501) staff       (20)      878 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/r46_graphs.py
--rw-r--r--   0 stevevott   (501) staff       (20)     2123 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/vis.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:35:28.682360 RamseyTheoryRL-0.53/RamseyTheoryRL.egg-info/
--rw-r--r--   0 stevevott   (501) staff       (20)     2826 2023-07-03 03:35:28.000000 RamseyTheoryRL-0.53/RamseyTheoryRL.egg-info/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)     1704 2023-07-03 03:35:28.000000 RamseyTheoryRL-0.53/RamseyTheoryRL.egg-info/SOURCES.txt
--rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:35:28.000000 RamseyTheoryRL-0.53/RamseyTheoryRL.egg-info/dependency_links.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 03:35:28.000000 RamseyTheoryRL-0.53/RamseyTheoryRL.egg-info/top_level.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 03:35:28.688528 RamseyTheoryRL-0.53/setup.cfg
--rw-r--r--   0 stevevott   (501) staff       (20)      796 2023-07-03 03:35:23.000000 RamseyTheoryRL-0.53/setup.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.604815 RamseyTheoryRL-0.54/
+-rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.54/LICENSE.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)     2826 2023-07-03 03:43:15.604685 RamseyTheoryRL-0.54/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     2161 2023-07-03 03:33:06.000000 RamseyTheoryRL-0.54/README.md
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.596414 RamseyTheoryRL-0.54/RamseyTheoryRL/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.595284 RamseyTheoryRL-0.54/RamseyTheoryRL/data/
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.597131 RamseyTheoryRL-0.54/RamseyTheoryRL/data/csv/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:34.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/csv/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.597232 RamseyTheoryRL-0.54/RamseyTheoryRL/data/csv/scaled/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:37.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/csv/scaled/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.597344 RamseyTheoryRL-0.54/RamseyTheoryRL/data/csv/unscaled/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:40.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/csv/unscaled/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.597448 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:45.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.599944 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:33:48.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)        4 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_3_5_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_6_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       42 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_7_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       28 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_8_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_8_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       10 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_10_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     1140 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_8_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     2053 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_9_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     1969 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_6_8_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       30 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_10_4_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       30 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_15_4_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    11973 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_4_12_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       20 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_8_3_isograph.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.600139 RamseyTheoryRL-0.54/RamseyTheoryRL/data/isomorphic_by_n/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:34:05.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/data/isomorphic_by_n/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.600244 RamseyTheoryRL-0.54/RamseyTheoryRL/src/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.601332 RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:29:39.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    12523 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/gbfs.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3539 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1070 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/igraph_train_gen.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1157 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/isofile_checker.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3365 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/train_gen.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.602279 RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-07-03 03:24:44.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     9795 2023-07-03 03:26:34.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     8240 2023-07-03 03:26:39.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    11528 2023-07-03 03:42:53.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/test.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.602810 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/gfeatures.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/guseful.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.603579 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.604382 RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:30:09.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1401 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/datavis.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      827 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/param_plot.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      788 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/r39_graph.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      878 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/r46_graphs.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     2123 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/vis.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:43:15.596997 RamseyTheoryRL-0.54/RamseyTheoryRL.egg-info/
+-rw-r--r--   0 stevevott   (501) staff       (20)     2826 2023-07-03 03:43:15.000000 RamseyTheoryRL-0.54/RamseyTheoryRL.egg-info/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     2478 2023-07-03 03:43:15.000000 RamseyTheoryRL-0.54/RamseyTheoryRL.egg-info/SOURCES.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:43:15.000000 RamseyTheoryRL-0.54/RamseyTheoryRL.egg-info/dependency_links.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 03:43:15.000000 RamseyTheoryRL-0.54/RamseyTheoryRL.egg-info/top_level.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 03:43:15.604857 RamseyTheoryRL-0.54/setup.cfg
+-rw-r--r--   0 stevevott   (501) staff       (20)     1054 2023-07-03 03:43:13.000000 RamseyTheoryRL-0.54/setup.py
```

### Comparing `RamseyTheoryRL-0.53/LICENSE.txt` & `RamseyTheoryRL-0.54/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/PKG-INFO` & `RamseyTheoryRL-0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.53
+Version: 0.54
 Summary: Ramsey Number Explorer
 Home-page: https://github.com/aLehav/RamseyTheoryRL
 Author: Adam Lehavi, Steve Vott
 Author-email: svott03@gmail.com, alehavi@usc.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.53 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.54 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
 Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
 MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
```

### Comparing `RamseyTheoryRL-0.53/README.md` & `RamseyTheoryRL-0.54/README.md`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/gbfs.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/gbfs.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/heuristic.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/heuristic.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/igraph_train_gen.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/igraph_train_gen.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/isofile_checker.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/isofile_checker.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/models/train_gen.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/models/train_gen.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/ramsey_checker/test.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/ramsey_checker/test.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/gfeatures.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/gfeatures.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/guseful.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/guseful.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/datavis.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/datavis.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/param_plot.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/param_plot.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/r39_graph.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/r39_graph.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/r46_graphs.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/r46_graphs.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL/src/visuals/vis.py` & `RamseyTheoryRL-0.54/RamseyTheoryRL/src/visuals/vis.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.53/RamseyTheoryRL.egg-info/PKG-INFO` & `RamseyTheoryRL-0.54/RamseyTheoryRL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.53
+Version: 0.54
 Summary: Ramsey Number Explorer
 Home-page: https://github.com/aLehav/RamseyTheoryRL
 Author: Adam Lehavi, Steve Vott
 Author-email: svott03@gmail.com, alehavi@usc.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.53 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.54 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
 Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
 MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
```

