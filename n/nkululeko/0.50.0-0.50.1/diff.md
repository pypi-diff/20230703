# Comparing `tmp/nkululeko-0.50.0.tar.gz` & `tmp/nkululeko-0.50.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.50.0.tar", last modified: Thu Jun 29 12:06:41 2023, max compression
+gzip compressed data, was "nkululeko-0.50.1.tar", last modified: Mon Jul  3 11:44:40 2023, max compression
```

## Comparing `nkululeko-0.50.0.tar` & `nkululeko-0.50.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-29 12:06:41.921223 nkululeko-0.50.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6757 2023-06-29 11:58:53.000000 nkululeko-0.50.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.50.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18483 2023-06-29 12:06:41.921223 nkululeko-0.50.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.50.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-29 12:06:41.921223 nkululeko-0.50.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.50.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2404 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.50.0/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.50.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-29 11:57:42.000000 nkululeko-0.50.0/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21705 2023-06-23 11:40:37.000000 nkululeko-0.50.0/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.50.0/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.50.0/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.50.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.50.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21183 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.50.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.50.0/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.50.0/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.50.0/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.50.0/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.50.0/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.50.0/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.50.0/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.50.0/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.50.0/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.50.0/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.50.0/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.50.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.50.0/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.50.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.50.0/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.50.0/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.50.0/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10587 2023-06-29 11:42:43.000000 nkululeko-0.50.0/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.50.0/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.50.0/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.50.0/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.50.0/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.50.0/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.50.0/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.50.0/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.50.0/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.50.0/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.50.0/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.50.0/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.50.0/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.50.0/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-06-23 11:40:37.000000 nkululeko-0.50.0/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.50.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.50.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2659 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.50.0/nkululeko/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.50.0/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.50.0/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-06-23 11:40:37.000000 nkululeko-0.50.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.50.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.50.0/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.50.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.50.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9644 2023-06-29 11:29:44.000000 nkululeko-0.50.0/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-29 12:06:41.921223 nkululeko-0.50.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18483 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-29 12:06:41.000000 nkululeko-0.50.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.50.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-29 12:06:41.921223 nkululeko-0.50.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.50.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-03 11:44:40.815566 nkululeko-0.50.1/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6852 2023-07-03 11:14:52.000000 nkululeko-0.50.1/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.50.1/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18652 2023-07-03 11:44:40.815566 nkululeko-0.50.1/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.50.1/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-03 11:44:40.815566 nkululeko-0.50.1/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.50.1/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.50.1/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.50.1/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.50.1/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.50.1/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-03 11:13:30.000000 nkululeko-0.50.1/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21714 2023-07-03 11:06:03.000000 nkululeko-0.50.1/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.50.1/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.50.1/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.50.1/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.50.1/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21195 2023-07-03 11:05:03.000000 nkululeko-0.50.1/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.50.1/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.50.1/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.50.1/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.50.1/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.50.1/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.50.1/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.50.1/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.50.1/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.50.1/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.50.1/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.50.1/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.50.1/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.50.1/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.50.1/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.50.1/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3643 2023-07-03 11:42:57.000000 nkululeko-0.50.1/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.50.1/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.50.1/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.50.1/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.50.1/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.50.1/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.50.1/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.50.1/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.50.1/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.50.1/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.50.1/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.50.1/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.50.1/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.50.1/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.50.1/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.50.1/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.50.1/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.50.1/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.50.1/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.50.1/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6561 2023-07-03 11:09:57.000000 nkululeko-0.50.1/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.50.1/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.50.1/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.50.1/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.50.1/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.50.1/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.50.1/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.50.1/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.50.1/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.50.1/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9800 2023-07-03 11:04:05.000000 nkululeko-0.50.1/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-03 11:44:40.815566 nkululeko-0.50.1/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18652 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.50.1/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-07-03 11:44:40.815566 nkululeko-0.50.1/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.50.1/setup.py
```

### Comparing `nkululeko-0.50.0/CHANGELOG.md` & `nkululeko-0.50.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.50.1
+--------------
+* added caller information for debug and error messages in Util
+
 Version 0.50.0
 --------------
 * removed loso and added pre-selected logo (leave-one-group-out), aka folds
 
 Version 0.49.1
 --------------
 * bugfix: samples selection for augmentation didn't work
```

### Comparing `nkululeko-0.50.0/LICENSE` & `nkululeko-0.50.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/PKG-INFO` & `nkululeko-0.50.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.50.0
+Version: 0.50.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -142,17 +142,18 @@
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
  * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
-Here's a rough UML-like sketch of the framework.
+Here's a rough UML-like sketch of the framework (and [here's the real one done with pyreverse](meta/images/classes.png)).
 ![sketch](meta/images/class_diagram.png)
 
+
 Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
 
@@ -210,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.50.1
+--------------
+* added caller information for debug and error messages in Util
+
 Version 0.50.0
 --------------
 * removed loso and added pre-selected logo (leave-one-group-out), aka folds
 
 Version 0.49.1
 --------------
 * bugfix: samples selection for augmentation didn't work
```

### Comparing `nkululeko-0.50.0/README.md` & `nkululeko-0.50.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -126,17 +126,18 @@
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
  * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
-Here's a rough UML-like sketch of the framework.
+Here's a rough UML-like sketch of the framework (and [here's the real one done with pyreverse](meta/images/classes.png)).
 ![sketch](meta/images/class_diagram.png)
 
+
 Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
```

### Comparing `nkululeko-0.50.0/nkululeko/augment.py` & `nkululeko-0.50.1/nkululeko/augment.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         exit()
         
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     # create a new experiment
     expr = Experiment(config)
-    util = Util()
+    util = Util('augment')
     util.debug(f'running {expr.name}, nkululeko version {VERSION}')
 
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
```

### Comparing `nkululeko-0.50.0/nkululeko/augmenter.py` & `nkululeko-0.50.1/nkululeko/augmenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class Augmenter:
     """
         augmenting the train split
     """
     def __init__(self, df):
         self.df = df
-        self.util = Util()
+        self.util = Util('augmenter')
         # Define a standard transformation that randomly add augmentations to files
         self.audioment = Compose([
             AddGaussianNoise(min_amplitude=0.001, max_amplitude=0.015, p=0.5),
             TimeStretch(min_rate=0.8, max_rate=1.25, p=0.5),
             PitchShift(min_semitones=-4, max_semitones=4, p=0.5),
             Shift(min_fraction=-0.5, max_fraction=0.5, p=0.5),
         ])
```

### Comparing `nkululeko-0.50.0/nkululeko/cacheddataset.py` & `nkululeko-0.50.1/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/dataset.py` & `nkululeko-0.50.1/nkululeko/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     df_train = None # The training split
     df_test = None # The evaluation split
 
     def __init__(self, name):
         """Constructor setting up name and configuration"""
         self.name = name
         self.target = glob_conf.config['DATA']['target']
-        self.util = Util()
+        self.util = Util('dataset')
         self.plot = Plots()
         self.limit = int(self.util.config_val_data(self.name, 'limit', 0))
         self.start_fresh = eval(self.util.config_val('DATA', 'no_reuse', 'False'))
         self.is_labeled, self.got_speaker, self.got_gender, self.got_age = False, False, False, False 
 
 
     def _get_tables(self):
```

### Comparing `nkululeko-0.50.0/nkululeko/dataset_csv.py` & `nkululeko-0.50.1/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/dataset_ravdess.py` & `nkululeko-0.50.1/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/demo.py` & `nkululeko-0.50.1/nkululeko/demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     
     # create a new experiment
     expr = Experiment(config)
-    util = Util()
+    util = Util('demo')
     util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the experiment
     expr.load(f'{util.get_save_name()}')
     if args.file is None and args.list is None:
        expr.demo(None, False)
     else:
```

### Comparing `nkululeko-0.50.0/nkululeko/demo_predictor.py` & `nkululeko-0.50.1/nkululeko/demo_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         """Constructor setting up name and configuration"""
         self.model = model
         self.feature_extractor = feature_extractor
         self.label_encoder = label_encoder
         self.is_list = is_list
         self.sr = 16000
         self.target = glob_conf.config['DATA']['target']
-        self.util = Util()
+        self.util = Util('demo_predictor')
         self.file = file
 
     def run_demo(self):
         signal, sr = None, 0
         if self.file is not None:
             if not self.is_list:
                 sig, sr = audiofile.read(self.file)
```

### Comparing `nkululeko-0.50.0/nkululeko/experiment.py` & `nkululeko-0.50.1/nkululeko/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Parameters
         ----------
         config_obj : a config parser object that sets the experiment parameters and being set as a global object.
         """
 
         self.set_globals(config_obj)
         self.name = glob_conf.config['EXP']['name']
-        self.util = Util()
+        self.util = Util('experiment')
         glob_conf.set_util(self.util)
         self.loso = self.util.config_val('MODEL', 'loso', False)
         self.logo = self.util.config_val('MODEL', 'logo', False)
         self.xfoldx = self.util.config_val('MODEL', 'k_fold_cross', False)
         self.start = time.process_time()
 
     def get_name(self):
```

### Comparing `nkululeko-0.50.0/nkululeko/explore.py` & `nkululeko-0.50.1/nkululeko/explore.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         exit()
         
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     # create a new experiment
     expr = Experiment(config)
-    util = Util()
+    util = Util('explore')
     util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
```

### Comparing `nkululeko-0.50.0/nkululeko/feats_analyser.py` & `nkululeko-0.50.1/nkululeko/feats_analyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sklearn.tree import DecisionTreeRegressor
 import matplotlib.pyplot as plt
 
 class FeatureAnalyser:
  
 
     def __init__(self, label, df_labels, df_features):
-        self.util = Util()
+        self.util = Util('feats_analyser')
         target = self.util.config_val('DATA', 'target', 'emotion')    
         self.y = df_labels[target]
         self.df_labels = df_labels
         self.X = df_features
         self.label = label
```

### Comparing `nkululeko-0.50.0/nkululeko/feats_audmodel.py` & `nkululeko-0.50.1/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.50.1/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feats_clap.py` & `nkululeko-0.50.1/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feats_import.py` & `nkululeko-0.50.1/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feats_mld.py` & `nkululeko-0.50.1/nkululeko/feats_mld.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import numpy as np
 from nkululeko.util import Util 
 import nkululeko.glob_conf as glob_conf
 
 class MLD_set(Featureset):
 
     def __init__(self, name, data_df):
-        self.name = name
-        self.data_df = data_df
-        self.util = Util()
+        super().__init__(name, data_df)   
         mld_path = self.util.config_val('FEATS', 'mld.model', None)
         sys.path.append(mld_path)
 
     def extract(self):
         store = self.util.get_path('store')
         storage = f'{store}{self.name}.pkl'
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
```

### Comparing `nkululeko-0.50.0/nkululeko/feats_opensmile.py` & `nkululeko-0.50.1/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feats_oxbow.py` & `nkululeko-0.50.1/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feats_praat.py` & `nkululeko-0.50.1/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feats_trill.py` & `nkululeko-0.50.1/nkululeko/feats_trill.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,15 @@
         
         :param name: Name of the class
         :type name: str
         :param data_df: Data of the class
         :type data_df: DataFrame
         :return: None
         """
-        self.name = name
-        self.data_df = data_df 
-        self.util = Util()
+        super().__init__(name, data_df)   
         # Load the model from the configured path
         model_path = self.util.config_val('FEATS', 'trill.model', \
             'https://tfhub.dev/google/nonsemantic-speech-benchmark/trill/3')
         self.module = hub.load(model_path)
 
 
     def extract(self):
```

### Comparing `nkululeko-0.50.0/nkululeko/feats_wav2vec2.py` & `nkululeko-0.50.1/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/feature_extractor.py` & `nkululeko-0.50.1/nkululeko/feature_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     df = None # pandas dataframe to store the features (and indexed with the data from the sets)
     data_df = None # dataframe to get audio paths
 
 # def __init__
     def set_data(self, data_df, data_name, feats_designation):
         self.data_df = data_df
         self.data_name = data_name
-        self.util = Util()
+        self.util = Util('feature_extractor')
         self.feats_designation = feats_designation
 
     def extract(self):
         strategy = self.util.config_val('DATA', 'strategy', 'traintest')
         feats_types = self.util.config_val_list('FEATS', 'type', ['os'])
         self.featExtractor = None
         self.feats= pd.DataFrame()
```

### Comparing `nkululeko-0.50.0/nkululeko/featureset.py` & `nkululeko-0.50.1/nkululeko/featureset.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     df = None # pandas dataframe to store the features (and indexed with the data from the sets)
     data_df = None # dataframe to get audio paths
 
 
     def __init__(self, name, data_df):
         self.name = name
         self.data_df = data_df
-        self.util = Util()
+        self.util = Util('featureset')
 
     def extract(self):
         pass
 
     def filter(self):
         # use only the features that are indexed in the target dataframes
         self.df = self.df[self.df.index.isin(self.data_df.index)]
```

### Comparing `nkululeko-0.50.0/nkululeko/feinberg_praat.py` & `nkululeko-0.50.1/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/filter_data.py` & `nkululeko-0.50.1/nkululeko/filter_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,58 @@
 import audformat
 import pandas as pd
 import nkululeko.glob_conf as glob_conf
+from nkululeko.util import Util
+
+class DataFilter:
+    def __init__(self, df):
+        self.util = Util('datafilter')
+        self.df = df.copy()
+
+    def limit_speakers(self, max=20):
+        """ limit number of samples per speaker
+            the samples are selected randomly          
+        """
+        df_ret = pd.DataFrame()
+        for s in self.df.speaker.unique():
+            s_df = self.df[self.df['speaker'].eq(s)]
+            if s_df.shape[0] < max:
+                df_ret = df_ret.append(s_df)
+            else:
+                df_ret = df_ret.append(s_df.sample(max))
+        return df_ret
+
+    def filter_min_dur(self, min_dur):
+        """remove all samples less than min_dur duration
+        """
+        if not isinstance(self.df.index, pd.MultiIndex):
+            glob_conf.util.debug('converting file index to multi index, this might take a while...')
+            self.df.index = audformat.utils.to_segmented_index(self.df.index, allow_nat=False)    
+        for i in self.df.index:
+            start = i[1]
+            end = i[2]
+            dur = (end - start).total_seconds()
+            if dur < float(min_dur):
+                self.df = self.df.drop(i, axis=0)
+        return self.df
+
+    def filter_max_dur(self, max_dur):
+        """remove all samples less than min_dur duration
+        """
+        if not isinstance(self.df.index, pd.MultiIndex):
+            glob_conf.util.debug('converting file index to multi index, this might take a while...')
+            self.df.index = audformat.utils.to_segmented_index(self.df.index, allow_nat=False)    
+        for i in self.df.index:
+            start = i[1]
+            end = i[2]
+            dur = (end - start).total_seconds()
+            if dur > float(max_dur):
+                df_ret = df_ret.drop(i, axis=0)
+        return self.df
+        
 
 def limit_speakers(df, max=20):
     """ limit number of samples per speaker
         the samples are selected randomly          
     """
     df_ret = pd.DataFrame()
     for s in df.speaker.unique():
```

### Comparing `nkululeko-0.50.0/nkululeko/loss_ccc.py` & `nkululeko-0.50.1/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/loss_softf1loss.py` & `nkululeko-0.50.1/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/model.py` & `nkululeko-0.50.1/nkululeko/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class Model:
     """Generic model class for linear (non-neural) algorithms"""
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes"""
         self.df_train, self.df_test, self.feats_train, self.feats_test = df_train, df_test, feats_train, feats_test
-        self.util = Util()
+        self.util = Util('model')
         self.target = self.util.config_val('DATA', 'target', 'emotion')
         self.run = 0
         self.epoch = 0
         self.logo = self.util.config_val('MODEL', 'logo', False)
         self.xfoldx = self.util.config_val('MODEL', 'k_fold_cross', False)
                 
     def set_testdata(self, data_df, feats_df):
```

### Comparing `nkululeko-0.50.0/nkululeko/model_cnn.py` & `nkululeko-0.50.1/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/model_gmm.py` & `nkululeko-0.50.1/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/model_knn.py` & `nkululeko-0.50.1/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/model_knn_reg.py` & `nkululeko-0.50.1/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/model_mlp.py` & `nkululeko-0.50.1/nkululeko/model_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 class MLP_model(Model):
     """MLP = multi layer perceptron"""
 
     is_classifier = True
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes"""
-        Model.__init__(self, df_train, df_test, feats_train, feats_test)
-        self.util = Util()
+        super().__init__(df_train, df_test, feats_train, feats_test)
         self.target = glob_conf.config['DATA']['target']
         labels = ast.literal_eval(glob_conf.config['DATA']['labels'])
         self.class_num = len(labels)
         # set up loss criterion
         criterion = self.util.config_val('MODEL', 'loss', 'cross')
         if criterion == 'cross':
             self.criterion = torch.nn.CrossEntropyLoss()
```

### Comparing `nkululeko-0.50.0/nkululeko/model_mlp_regression.py` & `nkululeko-0.50.1/nkululeko/model_mlp_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 class MLP_Reg_model(Model):
     """MLP = multi layer perceptron"""
 
     is_classifier = False
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
         """Constructor taking the configuration and all dataframes"""
-        Model.__init__(self, df_train, df_test, feats_train, feats_test)
-        self.util = Util()
+        super().__init__(df_train, df_test, feats_train, feats_test)
         self.target = glob_conf.config['DATA']['target']
         labels = ast.literal_eval(glob_conf.config['DATA']['labels'])
         self.class_num = len(labels)
         # set up loss criterion
         criterion = self.util.config_val('MODEL', 'loss', 'mse')
         if criterion == 'mse':
             self.criterion = torch.nn.MSELoss()
```

### Comparing `nkululeko-0.50.0/nkululeko/model_svm.py` & `nkululeko-0.50.1/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/modelrunner.py` & `nkululeko-0.50.1/nkululeko/modelrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             Args:
                 df_train: train dataframe
                 df_test: test dataframe
                 feats_train: train features
                 feats_train: test features
         """
         self.df_train, self.df_test, self.feats_train, self.feats_test = df_train, df_test, feats_train, feats_test
-        self.util = Util()
+        self.util = Util('modelrunner')
         self.run = run
         self.target = glob_conf.config['DATA']['target']
         # intialize a new model
         model_type = glob_conf.config['MODEL']['type']
         self._select_model(model_type)
```

### Comparing `nkululeko-0.50.0/nkululeko/nkululeko.py` & `nkululeko-0.50.1/nkululeko/nkululeko.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     
     # create a new experiment
     expr = exp.Experiment(config)
-    util = Util()
+    util = Util('nkululeko')
     util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
```

### Comparing `nkululeko-0.50.0/nkululeko/plots.py` & `nkululeko-0.50.1/nkululeko/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import seaborn as sns
 import numpy as np
 
 class Plots():
     
     def __init__(self):
         """Initializing the util system"""
-        self.util = Util()
+        self.util = Util('plots')
         self.format = self.util.config_val('PLOT', 'format', 'png')
 
     def describe_df(self, name, df, target, filename):
         """Make a stacked barplot of samples and speakers per sex and target values. speaker, gender and target columns must be present"""
         fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
         sampl_num = df.shape[0]
         sex_col = 'gender'
```

### Comparing `nkululeko-0.50.0/nkululeko/randomsplicer.py` & `nkululeko-0.50.1/nkululeko/randomsplicer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class Randomsplicer:
     """
         augmenting the train split
     """
     def __init__(self, df):
         self.df = df
-        self.util = Util()
+        self.util = Util('randomsplicer')
 
     def changepath(self, fp, np):
         fullpath = os.path.dirname(fp)
         return fp.replace(fullpath, np)
 
     def run(self, sample_selection):
         """
```

### Comparing `nkululeko-0.50.0/nkululeko/randomsplicing.py` & `nkululeko-0.50.1/nkululeko/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/reporter.py` & `nkululeko-0.50.1/nkululeko/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             elif self.measure == 'ccc':
                 self.MEASURE = 'CCC'
                 self.result.measure = self.MEASURE
 
 
     def __init__(self, truths, preds, run, epoch):
         """Initialization with ground truth und predictions vector"""
-        self.util = Util()
+        self.util = Util('reporter')
         self.format = self.util.config_val('PLOT', 'format', 'png')
         self.truths = truths
         self.preds = preds
         self.result = Result(0, 0, 0, 'unknown')
         self.run = run
         self.epoch = epoch
         self.__set_measure()
```

### Comparing `nkululeko-0.50.0/nkululeko/runmanager.py` & `nkululeko-0.50.1/nkululeko/runmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             feats_train: train features
             feats_train: test features
 
         Returns:
         
         """
         self.df_train, self.df_test, self.feats_train, self.feats_test = df_train, df_test, feats_train, feats_test
-        self.util = Util()
+        self.util = Util('runmanager')
         self.target = glob_conf.config['DATA']['target']
         # intialize a new model
         #model_type = glob_conf.config['MODEL']['type']
         #self._select_model(model_type)
```

### Comparing `nkululeko-0.50.0/nkululeko/scaler.py` & `nkululeko-0.50.1/nkululeko/scaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                         train_data_df (pd.DataFrame): The training dataframe with speakers.
                             only needed for speaker normalization
                         test_data_df (pd.DataFrame): The test dataframe with speakers
                             only needed for speaker normalization
                         train_feats (pd.DataFrame): The train features dataframe 
                         test_feats (pd.DataFrame): The test features dataframe (can be None) 
         '''
-        self.util = Util()
+        self.util = Util('scaler')
         if scaler_type == 'standard':
             self.scaler = StandardScaler()
         elif scaler_type == 'robust':
             self.scaler = RobustScaler()
         elif scaler_type == 'speaker':
             self.scaler = StandardScaler()
         else:
```

### Comparing `nkululeko-0.50.0/nkululeko/syllable_nuclei.py` & `nkululeko-0.50.1/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/nkululeko/test.py` & `nkululeko-0.50.1/nkululeko/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     
     # create a new experiment
     expr = Experiment(config)
-    util = Util()
+    util = Util('test')
     util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the experiment
     expr.load(f'{util.get_save_name()}')
     expr.fill_tests()
     expr.extract_test_feats()
     expr.predict_test_and_save(args.outfile)
```

### Comparing `nkululeko-0.50.0/nkululeko/test_predictor.py` & `nkululeko-0.50.1/nkululeko/test_predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def __init__(self, model, orig_df, labenc, name):
         """Constructor setting up name and configuration"""
         self.model = model
         self.orig_df = orig_df
         self.label_encoder = labenc
         self.target = glob_conf.config['DATA']['target']
-        self.util = Util()
+        self.util = Util('test_predictor')
         self.name = name
 
     def predict_and_store(self):
         label_data = self.util.config_val('DATA', 'label_data', False)
         if label_data:
             data = Dataset(label_data)
             data.load()
```

### Comparing `nkululeko-0.50.0/nkululeko/util.py` & `nkululeko-0.50.1/nkululeko/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 import audformat
 import pandas as pd
 
 class Util:
 
     stopvals = [False, 'False', 'classification', 'png']
 
-    def __init__(self):
+    def __init__(self, caller=None):
         self.got_data_roots = self.config_val('DATA', 'root_folders', False)
         if self.got_data_roots:
             # if there is a global data rootfolder file, read from there
             if not os.path.isfile(self.got_data_roots):
                 self.error(f'no such file: {self.got_data_roots}')
             self.data_roots = configparser.ConfigParser()
             self.data_roots.read(self.got_data_roots)
-        
+        if caller is not None:
+            self.caller = caller
+        else:  
+            self.caller = ''
+
     def get_path(self, entry):
         """
         This method allows the user to get the directory path for the given argument.
         """
         root = glob_conf.config['EXP']['root']
         name = glob_conf.config['EXP']['name']
         try:
@@ -169,22 +173,22 @@
     def exp_is_classification(self):
         type = self.config_val('EXP', 'type', 'classification')
         if type=='classification':
             return True
         return False
 
     def error(self, message):
-        print(f'ERROR: {message}')
+        print(f'ERROR {self.caller}: {message}')
         sys.exit()
 
     def warn(self, message):
-        print(f'WARNING: {message}')
+        print(f'WARNING {self.caller}: {message}')
 
     def debug(self, message):
-        print(f'DEBUG: {message}')
+        print(f'DEBUG {self.caller}: {message}')
 
     def set_config_val(self, section, key, value):
         try:
             # does the section already exists?
             glob_conf.config[section][key] = str(value)
         except KeyError:
             glob_conf.config.add_section(section)
```

### Comparing `nkululeko-0.50.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.50.1/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.50.0
+Version: 0.50.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -142,17 +142,18 @@
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
  * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
-Here's a rough UML-like sketch of the framework.
+Here's a rough UML-like sketch of the framework (and [here's the real one done with pyreverse](meta/images/classes.png)).
 ![sketch](meta/images/class_diagram.png)
 
+
 Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
 
@@ -210,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.50.1
+--------------
+* added caller information for debug and error messages in Util
+
 Version 0.50.0
 --------------
 * removed loso and added pre-selected logo (leave-one-group-out), aka folds
 
 Version 0.49.1
 --------------
 * bugfix: samples selection for augmentation didn't work
```

### Comparing `nkululeko-0.50.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.50.1/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.0/setup.cfg` & `nkululeko-0.50.1/setup.cfg`

 * *Files identical despite different names*

