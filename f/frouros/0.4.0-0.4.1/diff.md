# Comparing `tmp/frouros-0.4.0.tar.gz` & `tmp/frouros-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.4.0.tar", last modified: Wed Jun 21 12:19:19 2023, max compression
+gzip compressed data, was "frouros-0.4.1.tar", last modified: Mon Jul  3 08:22:15 2023, max compression
```

## Comparing `frouros-0.4.0.tar` & `frouros-0.4.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.294962 frouros-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-21 12:19:04.000000 frouros-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-21 12:19:04.000000 frouros-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    23091 2023-06-21 12:19:19.294962 frouros-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21470 2023-06-21 12:19:04.000000 frouros-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/batch/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.286962 frouros-0.4.0/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14974 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.290962 frouros-0.4.0/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.294962 frouros-0.4.0/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-06-21 12:19:04.000000 frouros-0.4.0/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 12:19:19.282962 frouros-0.4.0/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    23091 2023-06-21 12:19:18.000000 frouros-0.4.0/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4865 2023-06-21 12:19:19.000000 frouros-0.4.0/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 12:19:18.000000 frouros-0.4.0/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 12:19:18.000000 frouros-0.4.0/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-21 12:19:19.000000 frouros-0.4.0/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-21 12:19:19.000000 frouros-0.4.0/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-21 12:19:04.000000 frouros-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 12:19:19.294962 frouros-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-21 12:19:04.000000 frouros-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.023203 frouros-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-03 08:22:02.000000 frouros-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-03 08:22:02.000000 frouros-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    23090 2023-07-03 08:22:15.023203 frouros-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21469 2023-07-03 08:22:02.000000 frouros-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.011202 frouros-0.4.1/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.011202 frouros-0.4.1/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14974 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.023203 frouros-0.4.1/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.023203 frouros-0.4.1/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.011202 frouros-0.4.1/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    23090 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4865 2023-07-03 08:22:15.000000 frouros-0.4.1/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-03 08:22:02.000000 frouros-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 08:22:15.023203 frouros-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-07-03 08:22:02.000000 frouros-0.4.1/setup.py
```

### Comparing `frouros-0.4.0/LICENSE` & `frouros-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/PKG-INFO` & `frouros-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.4.0
+Version: 0.4.1
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
@@ -447,16 +447,16 @@
 
 ## 💬 Citation
 
 Although Frouros paper is still in preprint, if you want to cite it you can use the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the paper once is published).
 
 ```bibtex
 @article{cespedes2022frouros,
-  title={Frouros: A Python library for drift detection in Machine Learning problems},
-  author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+  title={Frouros: A Python library for drift detection in machine learning systems},
+  author={C{\'e}spedes-Sisniega, Jaime and L{\'o}pez-Garc{\'\i}a, {\'A}lvaro },
   journal={arXiv preprint arXiv:2208.06868},
   year={2022}
 }
 ```
 
 ## 📝 License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.4.0 Summary: An open-source
+Metadata-Version: 2.1 Name: frouros Version: 0.4.1 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
@@ -140,14 +140,14 @@
 machine learning pipelines: * [AI4EOSC](https://ai4eosc.eu). * [iMagine](https:
 //imagine-ai.eu). If you want your project listed here, do not hesitate to send
 us a pull request. ## ð Contributing Check out the [contribution](https://
 github.com/IFCA/frouros/blob/main/CONTRIBUTING.md) section. ## ð¬ Citation
 Although Frouros paper is still in preprint, if you want to cite it you can use
 the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the
 paper once is published). ```bibtex @article{cespedes2022frouros, title=
-{Frouros: A Python library for drift detection in Machine Learning problems},
-author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+{Frouros: A Python library for drift detection in machine learning systems},
+author={C{\'e}spedes-Sisniega, Jaime and L{\'o}pez-Garc{\'\i}a, {\'A}lvaro },
 journal={arXiv preprint arXiv:2208.06868}, year={2022} } ``` ## ð License
 Frouros is an open-source software licensed under the [BSD-3-Clause license]
 (https://github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements
 Frouros has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad
 de Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
```

### Comparing `frouros-0.4.0/README.md` & `frouros-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -411,16 +411,16 @@
 
 ## 💬 Citation
 
 Although Frouros paper is still in preprint, if you want to cite it you can use the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the paper once is published).
 
 ```bibtex
 @article{cespedes2022frouros,
-  title={Frouros: A Python library for drift detection in Machine Learning problems},
-  author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+  title={Frouros: A Python library for drift detection in machine learning systems},
+  author={C{\'e}spedes-Sisniega, Jaime and L{\'o}pez-Garc{\'\i}a, {\'A}lvaro },
   journal={arXiv preprint arXiv:2208.06868},
   year={2022}
 }
 ```
 
 ## 📝 License
```

#### html2text {}

```diff
@@ -118,14 +118,14 @@
 machine learning pipelines: * [AI4EOSC](https://ai4eosc.eu). * [iMagine](https:
 //imagine-ai.eu). If you want your project listed here, do not hesitate to send
 us a pull request. ## ð Contributing Check out the [contribution](https://
 github.com/IFCA/frouros/blob/main/CONTRIBUTING.md) section. ## ð¬ Citation
 Although Frouros paper is still in preprint, if you want to cite it you can use
 the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the
 paper once is published). ```bibtex @article{cespedes2022frouros, title=
-{Frouros: A Python library for drift detection in Machine Learning problems},
-author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+{Frouros: A Python library for drift detection in machine learning systems},
+author={C{\'e}spedes-Sisniega, Jaime and L{\'o}pez-Garc{\'\i}a, {\'A}lvaro },
 journal={arXiv preprint arXiv:2208.06868}, year={2022} } ``` ## ð License
 Frouros is an open-source software licensed under the [BSD-3-Clause license]
 (https://github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements
 Frouros has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad
 de Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
```

### Comparing `frouros-0.4.0/frouros/callbacks/base.py` & `frouros-0.4.1/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/callbacks/batch/base.py` & `frouros-0.4.1/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/callbacks/batch/permutation_test.py` & `frouros-0.4.1/frouros/callbacks/batch/permutation_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/callbacks/batch/reset.py` & `frouros-0.4.1/frouros/callbacks/batch/reset.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/callbacks/streaming/base.py` & `frouros-0.4.1/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/callbacks/streaming/history.py` & `frouros-0.4.1/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/callbacks/streaming/msprt.py` & `frouros-0.4.1/frouros/callbacks/streaming/msprt.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.4.1/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/datasets/base.py` & `frouros-0.4.1/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/datasets/real.py` & `frouros-0.4.1/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/datasets/synthetic.py` & `frouros-0.4.1/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/base.py` & `frouros-0.4.1/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/__init__.py` & `frouros-0.4.1/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/base.py` & `frouros-0.4.1/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/base.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/__init__.py` & `frouros-0.4.1/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/base.py` & `frouros-0.4.1/frouros/detectors/data_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/base.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.4.1/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/metrics/base.py` & `frouros-0.4.1/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/metrics/prequential_error.py` & `frouros-0.4.1/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/tests/conftest.py` & `frouros-0.4.1/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/tests/integration/test_callback.py` & `frouros-0.4.1/frouros/tests/integration/test_callback.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/tests/integration/test_concept_drift.py` & `frouros-0.4.1/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/tests/integration/test_data_drift.py` & `frouros-0.4.1/frouros/tests/integration/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/tests/integration/test_real.py` & `frouros-0.4.1/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/tests/integration/test_synthetic.py` & `frouros-0.4.1/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.4.1/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/utils/checks.py` & `frouros-0.4.1/frouros/utils/checks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/utils/data_structures.py` & `frouros-0.4.1/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros/utils/stats.py` & `frouros-0.4.1/frouros/utils/stats.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/frouros.egg-info/PKG-INFO` & `frouros-0.4.1/frouros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.4.0
+Version: 0.4.1
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
@@ -447,16 +447,16 @@
 
 ## 💬 Citation
 
 Although Frouros paper is still in preprint, if you want to cite it you can use the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the paper once is published).
 
 ```bibtex
 @article{cespedes2022frouros,
-  title={Frouros: A Python library for drift detection in Machine Learning problems},
-  author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+  title={Frouros: A Python library for drift detection in machine learning systems},
+  author={C{\'e}spedes-Sisniega, Jaime and L{\'o}pez-Garc{\'\i}a, {\'A}lvaro },
   journal={arXiv preprint arXiv:2208.06868},
   year={2022}
 }
 ```
 
 ## 📝 License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.4.0 Summary: An open-source
+Metadata-Version: 2.1 Name: frouros Version: 0.4.1 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
@@ -140,14 +140,14 @@
 machine learning pipelines: * [AI4EOSC](https://ai4eosc.eu). * [iMagine](https:
 //imagine-ai.eu). If you want your project listed here, do not hesitate to send
 us a pull request. ## ð Contributing Check out the [contribution](https://
 github.com/IFCA/frouros/blob/main/CONTRIBUTING.md) section. ## ð¬ Citation
 Although Frouros paper is still in preprint, if you want to cite it you can use
 the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the
 paper once is published). ```bibtex @article{cespedes2022frouros, title=
-{Frouros: A Python library for drift detection in Machine Learning problems},
-author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+{Frouros: A Python library for drift detection in machine learning systems},
+author={C{\'e}spedes-Sisniega, Jaime and L{\'o}pez-Garc{\'\i}a, {\'A}lvaro },
 journal={arXiv preprint arXiv:2208.06868}, year={2022} } ``` ## ð License
 Frouros is an open-source software licensed under the [BSD-3-Clause license]
 (https://github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements
 Frouros has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad
 de Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
```

### Comparing `frouros-0.4.0/frouros.egg-info/SOURCES.txt` & `frouros-0.4.1/frouros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frouros-0.4.0/pyproject.toml` & `frouros-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.4.0"
+version = "0.4.1"
 description = "An open-source Python library for drift detection in machine learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
@@ -32,33 +32,33 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 requires-python = ">=3.8,<3.12"
 dependencies = [
-    "matplotlib>=3.6.0,<3.7",
-    "numpy>=1.24.0,<1.25",
+    "matplotlib>=3.6.0,<3.8",
+    "numpy>=1.24.0,<1.26",
     "requests>=2.31.0,<2.32",
     "scipy>=1.10.0,<1.11",
     "tqdm>=4.65,<5",
 ]
 
 [project.optional-dependencies]
 docs = [
-    "sphinx>=5.3.0,<5.4",
+    "sphinx>=5.3.0,<7.1",
     "sphinx-book-theme>=1.0.0,<1.1",
     "sphinxcontrib-bibtex>=2.5.0,<2.6",
-    "myst-parser>=0.18.0,<0.19",
+    "myst-parser>=0.18.0,<2.1",
     "myst-nb>=0.17.0,<0.18",
 ]
 notebooks = [
-    "scikit-learn>=1.2.0,<1.3",
-    "torch>=1.13.0,<1.14",
-    "torchvision>=0.14.0,<0.15",
+    "scikit-learn>=1.2.0,<1.4",
+    "torch>=1.13.0,<2.1",
+    "torchvision>=0.14.0,<0.16",
     "ipywidgets>=8.0.0,<8.1",
 ]
 
 [project.urls]
 homepage = "https://frouros.readthedocs.io"
 repository = "https://github.com/IFCA/frouros"
 documentation = "https://frouros.readthedocs.io"
```

### Comparing `frouros-0.4.0/setup.py` & `frouros-0.4.1/setup.py`

 * *Files identical despite different names*

