# Comparing `tmp/tslearn-0.5.3.2.tar.gz` & `tmp/tslearn-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tslearn-0.5.3.2.tar", last modified: Fri Jan 20 13:25:37 2023, max compression
+gzip compressed data, was "tslearn-0.6.0.tar", last modified: Mon Jul  3 19:34:58 2023, max compression
```

## Comparing `tslearn-0.5.3.2.tar` & `tslearn-0.6.0.tar`

### file list

```diff
@@ -1,95 +1,101 @@
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:37.031531 tslearn-0.5.3.2/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1320 2017-06-28 16:18:01.000000 tslearn-0.5.3.2/LICENSE
--rw-r--r--   0 tavenard_r   (504) staff       (20)      254 2021-01-25 14:47:09.634369 tslearn-0.5.3.2/MANIFEST.in
--rw-r--r--   0 tavenard_r   (504) staff       (20)    14102 2023-01-20 13:25:37.034350 tslearn-0.5.3.2/PKG-INFO
--rw-r--r--   0 tavenard_r   (504) staff       (20)    13632 2021-08-16 07:05:25.718129 tslearn-0.5.3.2/README.md
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1166 2020-05-25 20:30:29.832352 tslearn-0.5.3.2/conftest.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)       59 2023-01-20 12:41:18.658875 tslearn-0.5.3.2/pyproject.toml
--rw-r--r--   0 tavenard_r   (504) staff       (20)      234 2020-05-25 20:30:29.833775 tslearn-0.5.3.2/setup.cfg
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1463 2023-01-20 12:45:16.795366 tslearn-0.5.3.2/setup.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.864072 tslearn-0.5.3.2/tslearn/
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.865476 tslearn-0.5.3.2/tslearn/.cached_datasets/
--rw-r--r--   0 tavenard_r   (504) staff       (20)   442330 2017-06-22 13:28:03.000000 tslearn-0.5.3.2/tslearn/.cached_datasets/Trace.npz
--rw-r--r--   0 tavenard_r   (504) staff       (20)      759 2023-01-20 13:20:23.242795 tslearn-0.5.3.2/tslearn/__init__.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.887216 tslearn-0.5.3.2/tslearn/barycenters/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1160 2021-01-05 10:39:33.337401 tslearn-0.5.3.2/tslearn/barycenters/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    26086 2021-01-06 07:38:50.170547 tslearn-0.5.3.2/tslearn/barycenters/dba.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1095 2023-01-20 12:41:18.661707 tslearn-0.5.3.2/tslearn/barycenters/euclidean.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3647 2023-01-20 12:41:18.662160 tslearn-0.5.3.2/tslearn/barycenters/softdtw.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)      285 2021-01-05 10:39:33.339083 tslearn-0.5.3.2/tslearn/barycenters/utils.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.889628 tslearn-0.5.3.2/tslearn/bases/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      120 2021-01-05 10:39:33.340758 tslearn-0.5.3.2/tslearn/bases/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     7807 2021-01-05 10:39:33.447118 tslearn-0.5.3.2/tslearn/bases/bases.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.922681 tslearn-0.5.3.2/tslearn/clustering/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      696 2023-01-20 12:41:18.662444 tslearn-0.5.3.2/tslearn/clustering/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    32544 2021-01-22 13:15:17.472749 tslearn-0.5.3.2/tslearn/clustering/kmeans.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     9994 2021-01-07 10:45:54.581839 tslearn-0.5.3.2/tslearn/clustering/kshape.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8445 2023-01-20 12:41:18.662711 tslearn-0.5.3.2/tslearn/clustering/utils.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.937269 tslearn-0.5.3.2/tslearn/datasets/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      359 2023-01-20 12:41:18.662963 tslearn-0.5.3.2/tslearn/datasets/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2843 2021-01-05 10:39:33.344441 tslearn-0.5.3.2/tslearn/datasets/cached.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2274 2021-01-05 10:39:33.344827 tslearn-0.5.3.2/tslearn/datasets/datasets.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    13805 2023-01-20 12:41:18.663303 tslearn-0.5.3.2/tslearn/datasets/ucr_uea.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.938300 tslearn-0.5.3.2/tslearn/early_classification/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      525 2021-01-05 10:39:33.346065 tslearn-0.5.3.2/tslearn/early_classification/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    21713 2021-01-05 10:39:33.440889 tslearn-0.5.3.2/tslearn/early_classification/early_classification.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.939280 tslearn-0.5.3.2/tslearn/generators/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      210 2021-01-05 10:39:33.348452 tslearn-0.5.3.2/tslearn/generators/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3556 2021-01-05 10:39:33.440389 tslearn-0.5.3.2/tslearn/generators/generators.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.948731 tslearn-0.5.3.2/tslearn/hdftools/
--rw-r--r--   0 tavenard_r   (504) staff       (20)       81 2021-01-05 10:39:33.349590 tslearn-0.5.3.2/tslearn/hdftools/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     4488 2023-01-20 12:41:18.663583 tslearn-0.5.3.2/tslearn/hdftools/hdftools.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.951098 tslearn-0.5.3.2/tslearn/matrix_profile/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      361 2021-01-05 10:39:33.350226 tslearn-0.5.3.2/tslearn/matrix_profile/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8825 2021-01-05 10:39:33.439263 tslearn-0.5.3.2/tslearn/matrix_profile/matrix_profile.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.966249 tslearn-0.5.3.2/tslearn/metrics/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2119 2023-01-20 12:41:18.664125 tslearn-0.5.3.2/tslearn/metrics/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    13515 2021-01-07 10:45:54.582432 tslearn-0.5.3.2/tslearn/metrics/ctw.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)   375335 2021-01-06 07:40:59.972248 tslearn-0.5.3.2/tslearn/metrics/cycc.c
--rw-r--r--   0 tavenard_r   (504) staff       (20)     4103 2023-01-20 12:41:18.664293 tslearn-0.5.3.2/tslearn/metrics/cycc.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)   423280 2021-01-06 07:41:00.252084 tslearn-0.5.3.2/tslearn/metrics/cysax.c
--rw-r--r--   0 tavenard_r   (504) staff       (20)     7323 2023-01-20 12:41:18.664522 tslearn-0.5.3.2/tslearn/metrics/cysax.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    65764 2023-01-20 12:41:18.665210 tslearn-0.5.3.2/tslearn/metrics/dtw_variants.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2177 2023-01-20 12:41:18.665620 tslearn-0.5.3.2/tslearn/metrics/sax.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)   281647 2021-01-06 07:41:00.441314 tslearn-0.5.3.2/tslearn/metrics/soft_dtw_fast.c
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3079 2023-01-20 12:41:18.665907 tslearn-0.5.3.2/tslearn/metrics/soft_dtw_fast.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    21767 2023-01-20 12:41:18.666321 tslearn-0.5.3.2/tslearn/metrics/softdtw_variants.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3320 2023-01-20 12:41:18.666655 tslearn-0.5.3.2/tslearn/metrics/utils.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.968276 tslearn-0.5.3.2/tslearn/neighbors/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      348 2023-01-20 12:41:18.666986 tslearn-0.5.3.2/tslearn/neighbors/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    28740 2021-01-05 10:39:33.422420 tslearn-0.5.3.2/tslearn/neighbors/neighbors.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.971526 tslearn-0.5.3.2/tslearn/neural_network/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      415 2021-01-05 10:39:33.362297 tslearn-0.5.3.2/tslearn/neural_network/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     5509 2021-01-05 10:39:33.421725 tslearn-0.5.3.2/tslearn/neural_network/neural_network.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.972696 tslearn-0.5.3.2/tslearn/piecewise/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      419 2021-01-05 10:39:33.363393 tslearn-0.5.3.2/tslearn/piecewise/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    24187 2023-01-20 12:41:18.667327 tslearn-0.5.3.2/tslearn/piecewise/piecewise.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.981055 tslearn-0.5.3.2/tslearn/preprocessing/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      318 2021-01-05 10:39:33.365690 tslearn-0.5.3.2/tslearn/preprocessing/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8690 2021-01-05 10:39:33.419089 tslearn-0.5.3.2/tslearn/preprocessing/preprocessing.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.984208 tslearn-0.5.3.2/tslearn/shapelets/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      565 2023-01-20 12:41:18.667731 tslearn-0.5.3.2/tslearn/shapelets/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    38104 2023-01-20 12:41:18.668210 tslearn-0.5.3.2/tslearn/shapelets/shapelets.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:36.987791 tslearn-0.5.3.2/tslearn/svm/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      340 2021-01-05 10:39:33.368177 tslearn-0.5.3.2/tslearn/svm/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    22178 2023-01-20 12:41:18.668648 tslearn-0.5.3.2/tslearn/svm/svm.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:37.028752 tslearn-0.5.3.2/tslearn/tests/
--rw-r--r--   0 tavenard_r   (504) staff       (20)        0 2020-05-25 20:30:29.875851 tslearn-0.5.3.2/tslearn/tests/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    25004 2023-01-20 12:41:18.669171 tslearn-0.5.3.2/tslearn/tests/sklearn_patches.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3983 2020-05-25 20:30:29.876986 tslearn-0.5.3.2/tslearn/tests/test_barycenters.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8032 2021-01-05 10:39:33.369380 tslearn-0.5.3.2/tslearn/tests/test_clustering.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8099 2023-01-20 12:41:18.669582 tslearn-0.5.3.2/tslearn/tests/test_estimators.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)      721 2020-06-15 19:11:12.798796 tslearn-0.5.3.2/tslearn/tests/test_matrixprofile.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    17118 2023-01-20 12:41:18.669971 tslearn-0.5.3.2/tslearn/tests/test_metrics.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1994 2021-01-05 10:39:33.370832 tslearn-0.5.3.2/tslearn/tests/test_neighbors.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3698 2020-06-02 06:20:08.173618 tslearn-0.5.3.2/tslearn/tests/test_piecewise.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)      508 2021-01-05 10:39:33.372803 tslearn-0.5.3.2/tslearn/tests/test_preprocessing.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     7777 2021-01-05 10:39:33.373545 tslearn-0.5.3.2/tslearn/tests/test_serialize_models.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     4205 2020-06-15 13:06:56.005238 tslearn-0.5.3.2/tslearn/tests/test_shapelets.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1187 2020-06-18 15:51:30.510806 tslearn-0.5.3.2/tslearn/tests/test_svm.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3005 2021-01-05 10:39:33.374191 tslearn-0.5.3.2/tslearn/tests/test_utils.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3620 2020-06-11 08:08:55.932129 tslearn-0.5.3.2/tslearn/tests/test_variablelength.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-01-20 13:25:37.031459 tslearn-0.5.3.2/tslearn/utils/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1605 2023-01-20 12:41:18.670358 tslearn-0.5.3.2/tslearn/utils/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    23572 2023-01-20 12:41:18.670786 tslearn-0.5.3.2/tslearn/utils/cast.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    21071 2023-01-20 12:41:18.671217 tslearn-0.5.3.2/tslearn/utils/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:58.022307 tslearn-0.6.0/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1320 2017-06-28 16:18:01.000000 tslearn-0.6.0/LICENSE
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      254 2021-01-25 14:47:09.634369 tslearn-0.6.0/MANIFEST.in
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    14218 2023-07-03 19:34:58.022631 tslearn-0.6.0/PKG-INFO
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    13726 2023-07-03 19:27:41.054001 tslearn-0.6.0/README.md
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1166 2020-05-25 20:30:29.832352 tslearn-0.6.0/conftest.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)       59 2023-01-20 12:41:18.658875 tslearn-0.6.0/pyproject.toml
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      234 2020-05-25 20:30:29.833775 tslearn-0.6.0/setup.cfg
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1494 2023-07-03 19:27:41.069213 tslearn-0.6.0/setup.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.760754 tslearn-0.6.0/tslearn/
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.764247 tslearn-0.6.0/tslearn/.cached_datasets/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   442330 2017-06-22 13:28:03.000000 tslearn-0.6.0/tslearn/.cached_datasets/Trace.npz
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      757 2023-07-03 19:30:24.909402 tslearn-0.6.0/tslearn/__init__.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.800317 tslearn-0.6.0/tslearn/backend/
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)      387 2023-07-03 19:27:41.069966 tslearn-0.6.0/tslearn/backend/__init__.py
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)     5097 2023-07-03 19:27:41.070559 tslearn-0.6.0/tslearn/backend/backend.py
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)     3909 2023-07-03 19:27:41.070918 tslearn-0.6.0/tslearn/backend/numpy_backend.py
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)     7737 2023-07-03 19:27:41.071513 tslearn-0.6.0/tslearn/backend/pytorch_backend.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.832884 tslearn-0.6.0/tslearn/barycenters/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1160 2021-01-05 10:39:33.337401 tslearn-0.6.0/tslearn/barycenters/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    26086 2021-01-06 07:38:50.170547 tslearn-0.6.0/tslearn/barycenters/dba.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1095 2023-01-20 12:41:18.661707 tslearn-0.6.0/tslearn/barycenters/euclidean.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3647 2023-01-20 12:41:18.662160 tslearn-0.6.0/tslearn/barycenters/softdtw.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      285 2021-01-05 10:39:33.339083 tslearn-0.6.0/tslearn/barycenters/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.845351 tslearn-0.6.0/tslearn/bases/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      120 2021-01-05 10:39:33.340758 tslearn-0.6.0/tslearn/bases/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     7807 2021-01-05 10:39:33.447118 tslearn-0.6.0/tslearn/bases/bases.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.851216 tslearn-0.6.0/tslearn/clustering/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      611 2023-07-03 19:27:41.072334 tslearn-0.6.0/tslearn/clustering/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    31792 2023-07-03 19:27:41.072990 tslearn-0.6.0/tslearn/clustering/kmeans.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     9994 2021-01-07 10:45:54.581839 tslearn-0.6.0/tslearn/clustering/kshape.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8445 2023-01-20 12:41:18.662711 tslearn-0.6.0/tslearn/clustering/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.856207 tslearn-0.6.0/tslearn/datasets/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      359 2023-01-20 12:41:18.662963 tslearn-0.6.0/tslearn/datasets/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2843 2021-01-05 10:39:33.344441 tslearn-0.6.0/tslearn/datasets/cached.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2274 2021-01-05 10:39:33.344827 tslearn-0.6.0/tslearn/datasets/datasets.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    13833 2023-07-03 18:23:27.324761 tslearn-0.6.0/tslearn/datasets/ucr_uea.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.858847 tslearn-0.6.0/tslearn/early_classification/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      525 2021-01-05 10:39:33.346065 tslearn-0.6.0/tslearn/early_classification/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    21713 2021-01-05 10:39:33.440889 tslearn-0.6.0/tslearn/early_classification/early_classification.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.862117 tslearn-0.6.0/tslearn/generators/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      210 2021-01-05 10:39:33.348452 tslearn-0.6.0/tslearn/generators/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3556 2021-01-05 10:39:33.440389 tslearn-0.6.0/tslearn/generators/generators.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.870667 tslearn-0.6.0/tslearn/hdftools/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)       81 2021-01-05 10:39:33.349590 tslearn-0.6.0/tslearn/hdftools/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     4488 2023-01-20 12:41:18.663583 tslearn-0.6.0/tslearn/hdftools/hdftools.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.873036 tslearn-0.6.0/tslearn/matrix_profile/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      361 2021-01-05 10:39:33.350226 tslearn-0.6.0/tslearn/matrix_profile/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8825 2021-01-05 10:39:33.439263 tslearn-0.6.0/tslearn/matrix_profile/matrix_profile.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.950061 tslearn-0.6.0/tslearn/metrics/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2200 2023-07-03 19:27:41.073788 tslearn-0.6.0/tslearn/metrics/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    14019 2023-07-03 19:27:41.075224 tslearn-0.6.0/tslearn/metrics/ctw.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   375335 2021-01-06 07:40:59.972248 tslearn-0.6.0/tslearn/metrics/cycc.c
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     4103 2023-01-20 12:41:18.664293 tslearn-0.6.0/tslearn/metrics/cycc.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   423280 2021-01-06 07:41:00.252084 tslearn-0.6.0/tslearn/metrics/cysax.c
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     7323 2023-01-20 12:41:18.664522 tslearn-0.6.0/tslearn/metrics/cysax.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    82613 2023-07-03 19:27:41.076292 tslearn-0.6.0/tslearn/metrics/dtw_variants.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2183 2023-07-03 19:27:41.076866 tslearn-0.6.0/tslearn/metrics/sax.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   281647 2021-01-06 07:41:00.441314 tslearn-0.6.0/tslearn/metrics/soft_dtw_fast.c
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8199 2023-07-03 19:27:41.077390 tslearn-0.6.0/tslearn/metrics/soft_dtw_fast.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     5245 2023-07-03 19:27:41.077789 tslearn-0.6.0/tslearn/metrics/soft_dtw_loss_pytorch.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    26296 2023-07-03 19:27:41.078376 tslearn-0.6.0/tslearn/metrics/softdtw_variants.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3319 2023-07-03 19:27:41.079312 tslearn-0.6.0/tslearn/metrics/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.956267 tslearn-0.6.0/tslearn/neighbors/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      348 2023-01-20 12:41:18.666986 tslearn-0.6.0/tslearn/neighbors/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    28740 2021-01-05 10:39:33.422420 tslearn-0.6.0/tslearn/neighbors/neighbors.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.961028 tslearn-0.6.0/tslearn/neural_network/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      415 2021-01-05 10:39:33.362297 tslearn-0.6.0/tslearn/neural_network/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     5509 2021-01-05 10:39:33.421725 tslearn-0.6.0/tslearn/neural_network/neural_network.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.968274 tslearn-0.6.0/tslearn/piecewise/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      419 2021-01-05 10:39:33.363393 tslearn-0.6.0/tslearn/piecewise/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    24187 2023-01-20 12:41:18.667327 tslearn-0.6.0/tslearn/piecewise/piecewise.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.972110 tslearn-0.6.0/tslearn/preprocessing/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      318 2021-01-05 10:39:33.365690 tslearn-0.6.0/tslearn/preprocessing/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8690 2021-01-05 10:39:33.419089 tslearn-0.6.0/tslearn/preprocessing/preprocessing.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.976615 tslearn-0.6.0/tslearn/shapelets/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      509 2023-07-03 19:27:41.080084 tslearn-0.6.0/tslearn/shapelets/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    33169 2023-07-03 19:27:41.080848 tslearn-0.6.0/tslearn/shapelets/shapelets.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.979601 tslearn-0.6.0/tslearn/svm/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      340 2021-01-05 10:39:33.368177 tslearn-0.6.0/tslearn/svm/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    20958 2023-07-03 19:27:41.081441 tslearn-0.6.0/tslearn/svm/svm.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:58.018719 tslearn-0.6.0/tslearn/tests/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)        0 2020-05-25 20:30:29.875851 tslearn-0.6.0/tslearn/tests/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    25004 2023-01-20 12:41:18.669171 tslearn-0.6.0/tslearn/tests/sklearn_patches.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3983 2020-05-25 20:30:29.876986 tslearn-0.6.0/tslearn/tests/test_barycenters.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8032 2021-01-05 10:39:33.369380 tslearn-0.6.0/tslearn/tests/test_clustering.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     7926 2023-07-03 19:27:41.081939 tslearn-0.6.0/tslearn/tests/test_estimators.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      721 2020-06-15 19:11:12.798796 tslearn-0.6.0/tslearn/tests/test_matrixprofile.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    24535 2023-07-03 19:27:41.082645 tslearn-0.6.0/tslearn/tests/test_metrics.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1994 2021-01-05 10:39:33.370832 tslearn-0.6.0/tslearn/tests/test_neighbors.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3698 2020-06-02 06:20:08.173618 tslearn-0.6.0/tslearn/tests/test_piecewise.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      508 2021-01-05 10:39:33.372803 tslearn-0.6.0/tslearn/tests/test_preprocessing.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     7750 2023-07-03 19:27:41.083347 tslearn-0.6.0/tslearn/tests/test_serialize_models.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     4205 2020-06-15 13:06:56.005238 tslearn-0.6.0/tslearn/tests/test_shapelets.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      806 2023-07-03 19:27:41.084192 tslearn-0.6.0/tslearn/tests/test_svm.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3005 2021-01-05 10:39:33.374191 tslearn-0.6.0/tslearn/tests/test_utils.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3620 2020-06-11 08:08:55.932129 tslearn-0.6.0/tslearn/tests/test_variablelength.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:58.022204 tslearn-0.6.0/tslearn/utils/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1605 2023-01-20 12:41:18.670358 tslearn-0.6.0/tslearn/utils/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    23572 2023-01-20 12:41:18.670786 tslearn-0.6.0/tslearn/utils/cast.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    21371 2023-07-03 19:27:41.085116 tslearn-0.6.0/tslearn/utils/utils.py
```

### Comparing `tslearn-0.5.3.2/LICENSE` & `tslearn-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/PKG-INFO` & `tslearn-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tslearn
-Version: 0.5.3.2
+Version: 0.6.0
 Summary: A machine learning toolkit dedicated to time-series data
 Home-page: http://tslearn.readthedocs.io/
 Author: Romain Tavenard
 Author-email: romain.tavenard@univ-rennes2.fr
 License: BSD-2-Clause
 Project-URL: Source, https://github.com/tslearn-team/tslearn
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+Provides-Extra: pytorch
 License-File: LICENSE
 
 <!-- Our title -->
 <div align="center">
   <h3>tslearn </h3>
 </div>
 
@@ -106,15 +107,15 @@
 >>> from tslearn.neighbors import KNeighborsTimeSeriesClassifier
 >>> knn = KNeighborsTimeSeriesClassifier(n_neighbors=1)
 >>> knn.fit(X_scaled, y)
 >>> print(knn.predict(X_scaled))
 [0 1 1]
 ```
 
-As can be seen, the models in tslearn follow the same API as those of the well-known scikit-learn. Moreover, they are fully compatible with it, allowing to use different scikit-learn utilities such as [hyper-parameter tuning and pipelines](https://tslearn.readthedocs.io/en/stable/auto_examples/plot_knnts_sklearn.html#sphx-glr-auto-examples-plot-knnts-sklearn-py).
+As can be seen, the models in tslearn follow the same API as those of the well-known scikit-learn. Moreover, they are fully compatible with it, allowing to use different scikit-learn utilities such as [hyper-parameter tuning and pipelines](https://tslearn.readthedocs.io/en/stable/auto_examples/neighbors/plot_knnts_sklearn.html).
 
 ### 4. More analyses
 
 tslearn further allows to perform all different types of analysis. Examples include [calculating barycenters](https://tslearn.readthedocs.io/en/stable/gen_modules/tslearn.barycenters.html#module-tslearn.barycenters) of a group of time series or calculate the distances between time series using a [variety of distance metrics](https://tslearn.readthedocs.io/en/stable/gen_modules/tslearn.metrics.html#module-tslearn.metrics).
 
 ## Available features
 
@@ -151,10 +152,10 @@
   number  = {118},
   pages   = {1-6},
   url     = {http://jmlr.org/papers/v21/20-091.html}
 }
 ```
 
 #### Acknowledgments
-Authors would like to thank Mathieu Blondel for providing code for [Kernel k-means](https://gist.github.com/mblondel/6230787) and [Soft-DTW](https://github.com/mblondel/soft-dtw).
+Authors would like to thank Mathieu Blondel for providing code for [Kernel k-means](https://gist.github.com/mblondel/6230787) and [Soft-DTW](https://github.com/mblondel/soft-dtw), and to Mehran Maghoumi for his [`torch`-compatible implementation of SoftDTW](https://github.com/Maghoumi/pytorch-softdtw-cuda).
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: tslearn Version: 0.5.3.2 Summary: A machine
-learning toolkit dedicated to time-series data Home-page: http://
-tslearn.readthedocs.io/ Author: Romain Tavenard Author-email:
-romain.tavenard@univ-rennes2.fr License: BSD-2-Clause Project-URL: Source,
-https://github.com/tslearn-team/tslearn Platform: UNKNOWN Classifier: License
-:: OSI Approved :: BSD License Description-Content-Type: text/markdown
-Provides-Extra: tests License-File: LICENSE
+Metadata-Version: 2.1 Name: tslearn Version: 0.6.0 Summary: A machine learning
+toolkit dedicated to time-series data Home-page: http://tslearn.readthedocs.io/
+Author: Romain Tavenard Author-email: romain.tavenard@univ-rennes2.fr License:
+BSD-2-Clause Project-URL: Source, https://github.com/tslearn-team/tslearn
+Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
+pytorch License-File: LICENSE
                                **** tslearn ****
         The machine learning toolkit for time series analysis in Python
     [PyPI] [Documentation] [Build_(Azure_Pipelines)] [Codecov] [Downloads]
 
 ===============================================================================
  | Section | Description | |-|-| | [Installation](#installation) | Installing
 the dependencies and tslearn | | [Getting started](#getting-started) | A quick
@@ -63,37 +63,36 @@
 //tslearn.readthedocs.io/en/stable/auto_examples/index.html). ```python3 >>>
 from tslearn.neighbors import KNeighborsTimeSeriesClassifier >>> knn =
 KNeighborsTimeSeriesClassifier(n_neighbors=1) >>> knn.fit(X_scaled, y) >>>
 print(knn.predict(X_scaled)) [0 1 1] ``` As can be seen, the models in tslearn
 follow the same API as those of the well-known scikit-learn. Moreover, they are
 fully compatible with it, allowing to use different scikit-learn utilities such
 as [hyper-parameter tuning and pipelines](https://tslearn.readthedocs.io/en/
-stable/auto_examples/plot_knnts_sklearn.html#sphx-glr-auto-examples-plot-knnts-
-sklearn-py). ### 4. More analyses tslearn further allows to perform all
-different types of analysis. Examples include [calculating barycenters](https:/
-/tslearn.readthedocs.io/en/stable/gen_modules/tslearn.barycenters.html#module-
-tslearn.barycenters) of a group of time series or calculate the distances
-between time series using a [variety of distance metrics](https://
-tslearn.readthedocs.io/en/stable/gen_modules/tslearn.metrics.html#module-
-tslearn.metrics). ## Available features | data | processing | clustering |
-classification | regression | metrics | |--------------------------------------
+stable/auto_examples/neighbors/plot_knnts_sklearn.html). ### 4. More analyses
+tslearn further allows to perform all different types of analysis. Examples
+include [calculating barycenters](https://tslearn.readthedocs.io/en/stable/
+gen_modules/tslearn.barycenters.html#module-tslearn.barycenters) of a group of
+time series or calculate the distances between time series using a [variety of
+distance metrics](https://tslearn.readthedocs.io/en/stable/gen_modules/
+tslearn.metrics.html#module-tslearn.metrics). ## Available features | data |
+processing | clustering | classification | regression | metrics | |------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------|-----
 -------------------------------------------------------------------------------
--------------------------------------|-----------------------------------------
+--------------------|----------------------------------------------------------
+---------------------------------------------------------------|---------------
+-------------------------------------------------------------------------------
+--------------------------------------------------------------------|----------
 -------------------------------------------------------------------------------
-------------------------------------------|------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------------------|--------
+-----------------|-------------------------------------------------------------
 -------------------------------------------------------------------------------
+------------------------------------------|------------------------------------
 -------------------------------------------------------------------------------
-----------------|--------------------------------------------------------------
-------------------------------------------------------------------------| |
-[UCR Datasets](https://tslearn.readthedocs.io/en/stable/gen_modules/
-tslearn.datasets.html#module-tslearn.datasets) | [Scaling](https://
+-------------------| | [UCR Datasets](https://tslearn.readthedocs.io/en/stable/
+gen_modules/tslearn.datasets.html#module-tslearn.datasets) | [Scaling](https://
 tslearn.readthedocs.io/en/stable/gen_modules/tslearn.preprocessing.html#module-
 tslearn.preprocessing) | [TimeSeriesKMeans](https://tslearn.readthedocs.io/en/
 stable/gen_modules/clustering/
 tslearn.clustering.TimeSeriesKMeans.html#tslearn.clustering.TimeSeriesKMeans) |
 [KNN Classifier](https://tslearn.readthedocs.io/en/stable/gen_modules/
 neighbors/
 tslearn.neighbors.KNeighborsTimeSeriesClassifier.html#tslearn.neighbors.KNeighborsTimeSeriesClassifier)
@@ -145,8 +144,10 @@
 and Felix Divo and Guillaume Androz and Chester Holtz and Marie Payne and Roman
 Yurchak and Marc Ru{\ss}wurm and Kushal Kolar and Eli Woods}, title = {Tslearn,
 A Machine Learning Toolkit for Time Series Data}, journal = {Journal of Machine
 Learning Research}, year = {2020}, volume = {21}, number = {118}, pages = {1-
 6}, url = {http://jmlr.org/papers/v21/20-091.html} } ``` #### Acknowledgments
 Authors would like to thank Mathieu Blondel for providing code for [Kernel k-
 means](https://gist.github.com/mblondel/6230787) and [Soft-DTW](https://
-github.com/mblondel/soft-dtw).
+github.com/mblondel/soft-dtw), and to Mehran Maghoumi for his [`torch`-
+compatible implementation of SoftDTW](https://github.com/Maghoumi/pytorch-
+softdtw-cuda).
```

### Comparing `tslearn-0.5.3.2/README.md` & `tslearn-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 >>> from tslearn.neighbors import KNeighborsTimeSeriesClassifier
 >>> knn = KNeighborsTimeSeriesClassifier(n_neighbors=1)
 >>> knn.fit(X_scaled, y)
 >>> print(knn.predict(X_scaled))
 [0 1 1]
 ```
 
-As can be seen, the models in tslearn follow the same API as those of the well-known scikit-learn. Moreover, they are fully compatible with it, allowing to use different scikit-learn utilities such as [hyper-parameter tuning and pipelines](https://tslearn.readthedocs.io/en/stable/auto_examples/plot_knnts_sklearn.html#sphx-glr-auto-examples-plot-knnts-sklearn-py).
+As can be seen, the models in tslearn follow the same API as those of the well-known scikit-learn. Moreover, they are fully compatible with it, allowing to use different scikit-learn utilities such as [hyper-parameter tuning and pipelines](https://tslearn.readthedocs.io/en/stable/auto_examples/neighbors/plot_knnts_sklearn.html).
 
 ### 4. More analyses
 
 tslearn further allows to perform all different types of analysis. Examples include [calculating barycenters](https://tslearn.readthedocs.io/en/stable/gen_modules/tslearn.barycenters.html#module-tslearn.barycenters) of a group of time series or calculate the distances between time series using a [variety of distance metrics](https://tslearn.readthedocs.io/en/stable/gen_modules/tslearn.metrics.html#module-tslearn.metrics).
 
 ## Available features
 
@@ -136,8 +136,8 @@
   number  = {118},
   pages   = {1-6},
   url     = {http://jmlr.org/papers/v21/20-091.html}
 }
 ```
 
 #### Acknowledgments
-Authors would like to thank Mathieu Blondel for providing code for [Kernel k-means](https://gist.github.com/mblondel/6230787) and [Soft-DTW](https://github.com/mblondel/soft-dtw).
+Authors would like to thank Mathieu Blondel for providing code for [Kernel k-means](https://gist.github.com/mblondel/6230787) and [Soft-DTW](https://github.com/mblondel/soft-dtw), and to Mehran Maghoumi for his [`torch`-compatible implementation of SoftDTW](https://github.com/Maghoumi/pytorch-softdtw-cuda).
```

#### html2text {}

```diff
@@ -56,37 +56,36 @@
 //tslearn.readthedocs.io/en/stable/auto_examples/index.html). ```python3 >>>
 from tslearn.neighbors import KNeighborsTimeSeriesClassifier >>> knn =
 KNeighborsTimeSeriesClassifier(n_neighbors=1) >>> knn.fit(X_scaled, y) >>>
 print(knn.predict(X_scaled)) [0 1 1] ``` As can be seen, the models in tslearn
 follow the same API as those of the well-known scikit-learn. Moreover, they are
 fully compatible with it, allowing to use different scikit-learn utilities such
 as [hyper-parameter tuning and pipelines](https://tslearn.readthedocs.io/en/
-stable/auto_examples/plot_knnts_sklearn.html#sphx-glr-auto-examples-plot-knnts-
-sklearn-py). ### 4. More analyses tslearn further allows to perform all
-different types of analysis. Examples include [calculating barycenters](https:/
-/tslearn.readthedocs.io/en/stable/gen_modules/tslearn.barycenters.html#module-
-tslearn.barycenters) of a group of time series or calculate the distances
-between time series using a [variety of distance metrics](https://
-tslearn.readthedocs.io/en/stable/gen_modules/tslearn.metrics.html#module-
-tslearn.metrics). ## Available features | data | processing | clustering |
-classification | regression | metrics | |--------------------------------------
+stable/auto_examples/neighbors/plot_knnts_sklearn.html). ### 4. More analyses
+tslearn further allows to perform all different types of analysis. Examples
+include [calculating barycenters](https://tslearn.readthedocs.io/en/stable/
+gen_modules/tslearn.barycenters.html#module-tslearn.barycenters) of a group of
+time series or calculate the distances between time series using a [variety of
+distance metrics](https://tslearn.readthedocs.io/en/stable/gen_modules/
+tslearn.metrics.html#module-tslearn.metrics). ## Available features | data |
+processing | clustering | classification | regression | metrics | |------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------|-----
 -------------------------------------------------------------------------------
--------------------------------------|-----------------------------------------
+--------------------|----------------------------------------------------------
+---------------------------------------------------------------|---------------
+-------------------------------------------------------------------------------
+--------------------------------------------------------------------|----------
 -------------------------------------------------------------------------------
-------------------------------------------|------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------------------|--------
+-----------------|-------------------------------------------------------------
 -------------------------------------------------------------------------------
+------------------------------------------|------------------------------------
 -------------------------------------------------------------------------------
-----------------|--------------------------------------------------------------
-------------------------------------------------------------------------| |
-[UCR Datasets](https://tslearn.readthedocs.io/en/stable/gen_modules/
-tslearn.datasets.html#module-tslearn.datasets) | [Scaling](https://
+-------------------| | [UCR Datasets](https://tslearn.readthedocs.io/en/stable/
+gen_modules/tslearn.datasets.html#module-tslearn.datasets) | [Scaling](https://
 tslearn.readthedocs.io/en/stable/gen_modules/tslearn.preprocessing.html#module-
 tslearn.preprocessing) | [TimeSeriesKMeans](https://tslearn.readthedocs.io/en/
 stable/gen_modules/clustering/
 tslearn.clustering.TimeSeriesKMeans.html#tslearn.clustering.TimeSeriesKMeans) |
 [KNN Classifier](https://tslearn.readthedocs.io/en/stable/gen_modules/
 neighbors/
 tslearn.neighbors.KNeighborsTimeSeriesClassifier.html#tslearn.neighbors.KNeighborsTimeSeriesClassifier)
@@ -138,8 +137,10 @@
 and Felix Divo and Guillaume Androz and Chester Holtz and Marie Payne and Roman
 Yurchak and Marc Ru{\ss}wurm and Kushal Kolar and Eli Woods}, title = {Tslearn,
 A Machine Learning Toolkit for Time Series Data}, journal = {Journal of Machine
 Learning Research}, year = {2020}, volume = {21}, number = {118}, pages = {1-
 6}, url = {http://jmlr.org/papers/v21/20-091.html} } ``` #### Acknowledgments
 Authors would like to thank Mathieu Blondel for providing code for [Kernel k-
 means](https://gist.github.com/mblondel/6230787) and [Soft-DTW](https://
-github.com/mblondel/soft-dtw).
+github.com/mblondel/soft-dtw), and to Mehran Maghoumi for his [`torch`-
+compatible implementation of SoftDTW](https://github.com/Maghoumi/pytorch-
+softdtw-cuda).
```

### Comparing `tslearn-0.5.3.2/conftest.py` & `tslearn-0.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/setup.py` & `tslearn-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     classifiers=[
             "License :: OSI Approved :: BSD License"
     ],
     include_dirs=[numpy.get_include()],
     packages=find_packages(),
     package_data={"tslearn": [".cached_datasets/Trace.npz"]},
     install_requires=['numpy', 'scipy', 'scikit-learn', 'numba', 'joblib'],
-    extras_require={'tests': ['pytest']},
+    extras_require={'tests': ['pytest', 'torch'], 'pytorch': ['torch']},
     version=VERSION,
     url="http://tslearn.readthedocs.io/",
     project_urls={
         "Source": "https://github.com/tslearn-team/tslearn",
     },
     author="Romain Tavenard",
     author_email="romain.tavenard@univ-rennes2.fr",
```

### Comparing `tslearn-0.5.3.2/tslearn/.cached_datasets/Trace.npz` & `tslearn-0.6.0/tslearn/.cached_datasets/Trace.npz`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/__init__.py` & `tslearn-0.6.0/tslearn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 __author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
-__version__ = "0.5.3.2"
+__version__ = "0.6.0"
 __bibtex__ = r"""@article{JMLR:v21:20-091,
   author  = {Romain Tavenard and Johann Faouzi and Gilles Vandewiele and
              Felix Divo and Guillaume Androz and Chester Holtz and
              Marie Payne and Roman Yurchak and Marc Ru{\ss}wurm and
              Kushal Kolar and Eli Woods},
   title   = {Tslearn, A Machine Learning Toolkit for Time Series Data},
   journal = {Journal of Machine Learning Research},
```

### Comparing `tslearn-0.5.3.2/tslearn/barycenters/__init__.py` & `tslearn-0.6.0/tslearn/barycenters/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/barycenters/dba.py` & `tslearn-0.6.0/tslearn/barycenters/dba.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/barycenters/euclidean.py` & `tslearn-0.6.0/tslearn/barycenters/euclidean.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/barycenters/softdtw.py` & `tslearn-0.6.0/tslearn/barycenters/softdtw.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/bases/bases.py` & `tslearn-0.6.0/tslearn/bases/bases.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/clustering/__init__.py` & `tslearn-0.6.0/tslearn/clustering/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 
 **User guide:** See the :ref:`Clustering <clustering>` section for further 
  details.
 """
 from .kshape import KShape
 from .utils import (EmptyClusterError, silhouette_score,
                     TimeSeriesCentroidBasedClusteringMixin)
-from .kmeans import (TimeSeriesKMeans, KernelKMeans,
-                     GlobalAlignmentKernelKMeans)
+from .kmeans import (TimeSeriesKMeans, KernelKMeans)
 
 
 __author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
 
 
 __all__ = [
     "KShape",
 
     "EmptyClusterError", "silhouette_score",
     "TimeSeriesCentroidBasedClusteringMixin",
 
-    "TimeSeriesKMeans", "KernelKMeans",
-    "GlobalAlignmentKernelKMeans"
+    "TimeSeriesKMeans", "KernelKMeans"
 ]
```

### Comparing `tslearn-0.5.3.2/tslearn/clustering/kmeans.py` & `tslearn-0.6.0/tslearn/clustering/kmeans.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,69 @@
+import warnings
+
+import numpy
+import sklearn
+from scipy.spatial.distance import cdist
 from sklearn.base import ClusterMixin, TransformerMixin
 from sklearn.metrics.pairwise import pairwise_kernels
-
 from sklearn.utils import check_random_state
 from sklearn.utils.extmath import stable_cumsum
 from sklearn.utils.validation import _check_sample_weight
-from scipy.spatial.distance import cdist
-import numpy
-import warnings
 
 try:
     from sklearn.cluster._kmeans import _kmeans_plusplus
+
+    SKLEARN_VERSION_GREATER_THAN_OR_EQUAL_TO_1_3_0 = sklearn.__version__ >= "1.3.0"
 except:
     try:
         from sklearn.cluster._kmeans import _k_init
+
         warnings.warn(
-            "Scikit-learn <0.24 will be deprecated in a "
-            "future release of tslearn"
+            "Scikit-learn <0.24 will be deprecated in a " "future release of tslearn"
         )
     except:
         from sklearn.cluster.k_means_ import _k_init
+
         warnings.warn(
-            "Scikit-learn <0.24 will be deprecated in a "
-            "future release of tslearn"
+            "Scikit-learn <0.24 will be deprecated in a " "future release of tslearn"
         )
     # sklearn < 0.24: _k_init only returns centroids, not indices
     # So we need to add a second (fake) return value to make it match
     # _kmeans_plusplus' signature
     def _kmeans_plusplus(*args, **kwargs):
         return _k_init(*args, **kwargs), None
 
-from tslearn.metrics import cdist_gak, cdist_dtw, cdist_soft_dtw, sigma_gak
-from tslearn.barycenters import euclidean_barycenter, \
-    dtw_barycenter_averaging, softdtw_barycenter
+
 from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
-from tslearn.utils import (to_time_series_dataset, to_sklearn_dataset,
-                           check_dims)
+
+from tslearn.barycenters import (
+    dtw_barycenter_averaging,
+    euclidean_barycenter,
+    softdtw_barycenter,
+)
 from tslearn.bases import BaseModelPackage, TimeSeriesBaseEstimator
+from tslearn.metrics import cdist_dtw, cdist_gak, cdist_soft_dtw, sigma_gak
+from tslearn.utils import check_dims, to_sklearn_dataset, to_time_series_dataset
 
-from .utils import (EmptyClusterError, _check_initial_guess,
-                    _check_no_empty_cluster, _check_full_length,
-                    TimeSeriesCentroidBasedClusteringMixin, _compute_inertia)
+from .utils import (
+    EmptyClusterError,
+    TimeSeriesCentroidBasedClusteringMixin,
+    _check_full_length,
+    _check_initial_guess,
+    _check_no_empty_cluster,
+    _compute_inertia,
+)
 
-__author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
+__author__ = "Romain Tavenard romain.tavenard[at]univ-rennes2.fr"
 # Kernel k-means is derived from https://gist.github.com/mblondel/6230787 by
 # Mathieu Blondel, under BSD 3 clause license
 
 
-def _k_init_metric(X, n_clusters, cdist_metric, random_state,
-                   n_local_trials=None):
+def _k_init_metric(X, n_clusters, cdist_metric, random_state, n_local_trials=None):
     """Init n_clusters seeds according to k-means++ with a custom distance
     metric.
 
     Parameters
     ----------
     X : array, shape (n_samples, n_timestamps, n_features)
         The data to pick seeds for.
@@ -80,16 +91,15 @@
     on Discrete algorithms. 2007
 
     Version adapted from scikit-learn for use with a custom metric in place of
     Euclidean distance.
     """
     n_samples, n_timestamps, n_features = X.shape
 
-    centers = numpy.empty((n_clusters, n_timestamps, n_features),
-                          dtype=X.dtype)
+    centers = numpy.empty((n_clusters, n_timestamps, n_features), dtype=X.dtype)
 
     # Set the number of local seeding trials if none is given
     if n_local_trials is None:
         # This is what Arthur/Vassilvitskii tried, but did not report
         # specific results for other than mentioning in the conclusion
         # that it helped.
         n_local_trials = 2 + int(numpy.log(n_clusters))
@@ -103,26 +113,25 @@
     current_pot = closest_dist_sq.sum()
 
     # Pick the remaining n_clusters-1 points
     for c in range(1, n_clusters):
         # Choose center candidates by sampling with probability proportional
         # to the squared distance to the closest existing center
         rand_vals = random_state.random_sample(n_local_trials) * current_pot
-        candidate_ids = numpy.searchsorted(stable_cumsum(closest_dist_sq),
-                                           rand_vals)
+        candidate_ids = numpy.searchsorted(stable_cumsum(closest_dist_sq), rand_vals)
         # XXX: numerical imprecision can result in a candidate_id out of range
-        numpy.clip(candidate_ids, None, closest_dist_sq.size - 1,
-                   out=candidate_ids)
+        numpy.clip(candidate_ids, None, closest_dist_sq.size - 1, out=candidate_ids)
 
         # Compute distances to center candidates
         distance_to_candidates = cdist_metric(X[candidate_ids], X) ** 2
 
         # update closest distances squared and potential for each candidate
-        numpy.minimum(closest_dist_sq, distance_to_candidates,
-                      out=distance_to_candidates)
+        numpy.minimum(
+            closest_dist_sq, distance_to_candidates, out=distance_to_candidates
+        )
         candidates_pot = distance_to_candidates.sum(axis=1)
 
         # Decide which candidate is the best
         best_candidate = numpy.argmin(candidates_pot)
         current_pot = candidates_pot[best_candidate]
         closest_dist_sq = distance_to_candidates[best_candidate]
         best_candidate = candidate_ids[best_candidate]
@@ -161,40 +170,30 @@
         Number of time the k-means algorithm will be run with different
         centroid seeds. The final results will be the
         best output of n_init consecutive runs in terms of inertia.
 
     kernel_params : dict or None (default: None)
         Kernel parameters to be passed to the kernel function.
         None means no kernel parameter is set.
-        For Global Alignment Kernel, the only parameter of interest is `sigma`. 
-        If set to 'auto', it is computed based on a sampling of the training 
+        For Global Alignment Kernel, the only parameter of interest is `sigma`.
+        If set to 'auto', it is computed based on a sampling of the training
         set
         (cf :ref:`tslearn.metrics.sigma_gak <fun-tslearn.metrics.sigma_gak>`).
         If no specific value is set for `sigma`, its defaults to 1.
 
-    sigma : float or "auto" (default: "auto")
-        Bandwidth parameter for the Global Alignment kernel. If set to 'auto',
-        it is computed based on a sampling of the training set
-        (cf :ref:`tslearn.metrics.sigma_gak <fun-tslearn.metrics.sigma_gak>`)
-
-        .. deprecated:: 0.4
-            Setting `sigma` directly as a parameter for KernelKMeans and 
-            GlobalAlignmentKernelKMeans is deprecated in version 0.4 and will 
-            be removed in 0.6. Use `kernel_params` instead.
-
     n_jobs : int or None, optional (default=None)
         The number of jobs to run in parallel for GAK cross-similarity matrix
         computations.
         ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
         ``-1`` means using all processors. See scikit-learns'
         `Glossary <https://scikit-learn.org/stable/glossary.html#term-n-jobs>`_
         for more details.
 
     verbose : int (default: 0)
-        If nonzero, joblib progress messages are printed.  
+        If nonzero, joblib progress messages are printed.
 
     random_state : integer or numpy.RandomState, optional
         Generator used to initialize the centers. If an integer is given, it
         fixes the seed. Defaults to the global
         numpy random number generator.
 
     Attributes
@@ -232,62 +231,74 @@
     ----------
     .. [1] Kernel k-means, Spectral Clustering and Normalized Cuts.
            Inderjit S. Dhillon, Yuqiang Guan, Brian Kulis. KDD 2004.
 
     .. [2] Fast Global Alignment Kernels. Marco Cuturi. ICML 2011.
     """
 
-    def __init__(self, n_clusters=3, kernel="gak", max_iter=50, tol=1e-6,
-                 n_init=1, kernel_params=None, sigma=1., n_jobs=None,
-                 verbose=0, random_state=None):
+    def __init__(
+        self,
+        n_clusters=3,
+        kernel="gak",
+        max_iter=50,
+        tol=1e-6,
+        n_init=1,
+        kernel_params=None,
+        n_jobs=None,
+        verbose=0,
+        random_state=None,
+    ):
         self.n_clusters = n_clusters
         self.kernel = kernel
         self.max_iter = max_iter
         self.tol = tol
         self.n_init = n_init
         self.kernel_params = kernel_params
-        self.sigma = sigma
         self.n_jobs = n_jobs
         self.verbose = verbose
         self.random_state = random_state
 
     def _is_fitted(self):
-        check_is_fitted(self, '_X_fit')
+        check_is_fitted(self, "_X_fit")
         return True
 
     def _get_model_params(self):
         params = super()._get_model_params()
-        params.update({'_X_fit': self._X_fit})
+        params.update({"_X_fit": self._X_fit})
         return params
 
     def _get_kernel_params(self):
         if self.kernel_params is None:
             kernel_params = {}
         else:
             kernel_params = self.kernel_params
         if self.kernel == "gak":
             if hasattr(self, "sigma_gak_"):
                 kernel_params["sigma"] = self.sigma_gak_
-            elif "sigma" not in kernel_params.keys():
-                kernel_params["sigma"] = self.sigma
         return kernel_params
 
     def _get_kernel(self, X, Y=None):
         kernel_params = self._get_kernel_params()
         if self.kernel == "gak":
-            return cdist_gak(X, Y, n_jobs=self.n_jobs, verbose=self.verbose,
-                             **kernel_params)
+            return cdist_gak(
+                X, Y, n_jobs=self.n_jobs, verbose=self.verbose, **kernel_params
+            )
         else:
             X_sklearn = to_sklearn_dataset(X)
             if Y is not None:
                 Y_sklearn = to_sklearn_dataset(Y)
             else:
                 Y_sklearn = Y
-            return pairwise_kernels(X_sklearn, Y_sklearn, metric=self.kernel,
-                                    n_jobs=self.n_jobs, **kernel_params)
+            return pairwise_kernels(
+                X_sklearn,
+                Y_sklearn,
+                metric=self.kernel,
+                n_jobs=self.n_jobs,
+                **kernel_params
+            )
 
     def _fit_one_init(self, K, rs):
         n_samples = K.shape[0]
 
         self.labels_ = rs.randint(self.n_clusters, size=n_samples)
 
         dist = numpy.empty((n_samples, self.n_clusters))
@@ -322,31 +333,24 @@
 
         y
             Ignored
         sample_weight : array-like of shape=(n_ts, ) or None (default: None)
             Weights to be given to time series in the learning process. By
             default, all time series weights are equal.
         """
-        if self.sigma != 1.:
-            warnings.warn(
-                "Setting `sigma` directly as a parameter for KernelKMeans "
-                "and GlobalAlignmentKernelKMeans is deprecated in version "
-                "0.4 and will be removed in 0.6. Use `kernel_params` "
-                "instead.",
-                DeprecationWarning, stacklevel=2)
 
         X = check_array(X, allow_nd=True, force_all_finite=False)
         X = check_dims(X)
 
         sample_weight = _check_sample_weight(sample_weight=sample_weight, X=X)
 
         max_attempts = max(self.n_init, 10)
         kernel_params = self._get_kernel_params()
         if self.kernel == "gak":
-            self.sigma_gak_ = kernel_params.get("sigma", 1.)
+            self.sigma_gak_ = kernel_params.get("sigma", 1.0)
             if self.sigma_gak_ == "auto":
                 self.sigma_gak_ = sigma_gak(X)
         else:
             self.sigma_gak_ = None
 
         self.labels_ = None
         self.inertia_ = None
@@ -354,16 +358,15 @@
         self._X_fit = None
         # n_iter_ will contain the number of iterations the most
         # successful run required.
         self.n_iter_ = 0
 
         n_samples = X.shape[0]
         K = self._get_kernel(X)
-        sw = (sample_weight if sample_weight is not None
-              else numpy.ones(n_samples))
+        sw = sample_weight if sample_weight is not None else numpy.ones(n_samples)
         self.sample_weight_ = sw
         rs = check_random_state(self.random_state)
 
         last_correct_labels = None
         min_inertia = numpy.inf
         n_attempts = 0
         n_successful = 0
@@ -389,24 +392,26 @@
 
     def _compute_dist(self, K, dist):
         """Compute a n_samples x n_clusters distance matrix using the kernel
         trick."""
         sw = self.sample_weight_
 
         for j in range(self.n_clusters):
-            mask = (self.labels_ == j)
+            mask = self.labels_ == j
 
             if numpy.sum(mask) == 0:
-                raise EmptyClusterError("try smaller n_cluster or better "
-                                        "kernel parameters")
+                raise EmptyClusterError(
+                    "try smaller n_cluster or better " "kernel parameters"
+                )
 
             # NB: we use a normalized kernel so k(x,x) = 1 for all x
             # (including the centroid)
-            dist[:, j] = 2 - 2 * numpy.sum(sw[mask] * K[:, mask],
-                                           axis=1) / sw[mask].sum()
+            dist[:, j] = (
+                2 - 2 * numpy.sum(sw[mask] * K[:, mask], axis=1) / sw[mask].sum()
+            )
 
     @staticmethod
     def _compute_inertia(dist_sq):
         return dist_sq.min(axis=1).sum()
 
     def fit_predict(self, X, y=None):
         """Fit kernel k-means clustering using X and then predict the closest
@@ -440,41 +445,33 @@
 
         Returns
         -------
         labels : array of shape=(n_ts, )
             Index of the cluster each sample belongs to.
         """
         X = check_array(X, allow_nd=True, force_all_finite=False)
-        check_is_fitted(self, '_X_fit')
-        X = check_dims(X, X_fit_dims=self._X_fit.shape,
-                       check_n_features_only=True)
+        check_is_fitted(self, "_X_fit")
+        X = check_dims(X, X_fit_dims=self._X_fit.shape, check_n_features_only=True)
         K = self._get_kernel(X, self._X_fit)
         n_samples = X.shape[0]
         dist = numpy.zeros((n_samples, self.n_clusters))
         self._compute_dist(K, dist)
         return dist.argmin(axis=1)
 
     def _more_tags(self):
-        return {'allow_nan': True, 'allow_variable_length': True}
-
-
-class GlobalAlignmentKernelKMeans(KernelKMeans):
-    def __init__(self, **kwargs):
-        warnings.warn(
-            "`GlobalAlignmentKernelKMeans` is deprecated in version "
-            "0.4 and will be removed in 0.6. Use `KernelKMeans` "
-            "instead.",
-            DeprecationWarning, stacklevel=2)
-        super().__init__(**kwargs)
-        self.kernel = "gak"
+        return {"allow_nan": True, "allow_variable_length": True}
 
 
-class TimeSeriesKMeans(TransformerMixin, ClusterMixin,
-                       TimeSeriesCentroidBasedClusteringMixin,
-                       BaseModelPackage, TimeSeriesBaseEstimator):
+class TimeSeriesKMeans(
+    TransformerMixin,
+    ClusterMixin,
+    TimeSeriesCentroidBasedClusteringMixin,
+    BaseModelPackage,
+    TimeSeriesBaseEstimator,
+):
     """K-means clustering for time-series data.
 
     Parameters
     ----------
     n_clusters : int (default: 3)
         Number of clusters to form.
 
@@ -518,15 +515,15 @@
         for more details.
 
     dtw_inertia: bool (default: False)
         Whether to compute DTW inertia even if DTW is not the chosen metric.
 
     verbose : int (default: 0)
         If nonzero, print information about the inertia while learning
-        the model and joblib progress messages are printed.  
+        the model and joblib progress messages are printed.
 
     random_state : integer or numpy.RandomState, optional
         Generator used to initialize the centers. If an integer is given, it
         fixes the seed. Defaults to the global
         numpy random number generator.
 
     init : {'k-means++', 'random' or an ndarray} (default: 'k-means++')
@@ -585,80 +582,108 @@
     ...                                 [2, 5, 6, 7, 8, 9]])
     >>> km = TimeSeriesKMeans(n_clusters=2, max_iter=5,
     ...                       metric="dtw", random_state=0).fit(X_bis)
     >>> km.cluster_centers_.shape
     (2, 6, 1)
     """
 
-    def __init__(self, n_clusters=3, max_iter=50, tol=1e-6, n_init=1,
-                 metric="euclidean", max_iter_barycenter=100,
-                 metric_params=None, n_jobs=None, dtw_inertia=False,
-                 verbose=0, random_state=None, init='k-means++'):
+    def __init__(
+        self,
+        n_clusters=3,
+        max_iter=50,
+        tol=1e-6,
+        n_init=1,
+        metric="euclidean",
+        max_iter_barycenter=100,
+        metric_params=None,
+        n_jobs=None,
+        dtw_inertia=False,
+        verbose=0,
+        random_state=None,
+        init="k-means++",
+    ):
         self.n_clusters = n_clusters
         self.max_iter = max_iter
         self.tol = tol
         self.n_init = n_init
         self.metric = metric
         self.max_iter_barycenter = max_iter_barycenter
         self.metric_params = metric_params
         self.n_jobs = n_jobs
         self.dtw_inertia = dtw_inertia
         self.verbose = verbose
         self.random_state = random_state
         self.init = init
 
     def _is_fitted(self):
-        check_is_fitted(self, ['cluster_centers_'])
+        check_is_fitted(self, ["cluster_centers_"])
         return True
 
     def _get_metric_params(self):
         if self.metric_params is None:
             metric_params = {}
         else:
             metric_params = self.metric_params.copy()
         if "n_jobs" in metric_params.keys():
             del metric_params["n_jobs"]
         return metric_params
 
     def _fit_one_init(self, X, x_squared_norms, rs):
         metric_params = self._get_metric_params()
         n_ts, sz, d = X.shape
-        if hasattr(self.init, '__array__'):
+        if hasattr(self.init, "__array__"):
             self.cluster_centers_ = self.init.copy()
         elif isinstance(self.init, str) and self.init == "k-means++":
             if self.metric == "euclidean":
-                self.cluster_centers_ = _kmeans_plusplus(
-                    X.reshape((n_ts, -1)),
-                    self.n_clusters,
-                    x_squared_norms=x_squared_norms,
-                    random_state=rs
-                )[0].reshape((-1, sz, d))
+                if SKLEARN_VERSION_GREATER_THAN_OR_EQUAL_TO_1_3_0:
+                    sample_weight = _check_sample_weight(None, X, dtype=X.dtype)
+                    self.cluster_centers_ = _kmeans_plusplus(
+                        X.reshape((n_ts, -1)),
+                        self.n_clusters,
+                        x_squared_norms=x_squared_norms,
+                        sample_weight=sample_weight,
+                        random_state=rs,
+                    )[0].reshape((-1, sz, d))
+                else:
+                    self.cluster_centers_ = _kmeans_plusplus(
+                        X.reshape((n_ts, -1)),
+                        self.n_clusters,
+                        x_squared_norms=x_squared_norms,
+                        random_state=rs,
+                    )[0].reshape((-1, sz, d))
             else:
                 if self.metric == "dtw":
+
                     def metric_fun(x, y):
-                        return cdist_dtw(x, y, n_jobs=self.n_jobs,
-                                         verbose=self.verbose, **metric_params)
+                        return cdist_dtw(
+                            x,
+                            y,
+                            n_jobs=self.n_jobs,
+                            verbose=self.verbose,
+                            **metric_params
+                        )
 
                 elif self.metric == "softdtw":
+
                     def metric_fun(x, y):
                         return cdist_soft_dtw(x, y, **metric_params)
+
                 else:
                     raise ValueError(
                         "Incorrect metric: %s (should be one of 'dtw', "
                         "'softdtw', 'euclidean')" % self.metric
                     )
-                self.cluster_centers_ = _k_init_metric(X, self.n_clusters,
-                                                       cdist_metric=metric_fun,
-                                                       random_state=rs)
+                self.cluster_centers_ = _k_init_metric(
+                    X, self.n_clusters, cdist_metric=metric_fun, random_state=rs
+                )
         elif self.init == "random":
             indices = rs.choice(X.shape[0], self.n_clusters)
             self.cluster_centers_ = X[indices].copy()
         else:
-            raise ValueError("Value %r for parameter 'init'"
-                             "is invalid" % self.init)
+            raise ValueError("Value %r for parameter 'init'" "is invalid" % self.init)
         self.cluster_centers_ = _check_full_length(self.cluster_centers_)
         old_inertia = numpy.inf
 
         for it in range(self.max_iter):
             self._assign(X)
             if self.verbose:
                 print("%.3f" % self.inertia_, end=" --> ")
@@ -673,101 +698,117 @@
         self._iter = it + 1
 
         return self
 
     def _transform(self, X):
         metric_params = self._get_metric_params()
         if self.metric == "euclidean":
-            return cdist(X.reshape((X.shape[0], -1)),
-                         self.cluster_centers_.reshape((self.n_clusters, -1)),
-                         metric="euclidean")
+            return cdist(
+                X.reshape((X.shape[0], -1)),
+                self.cluster_centers_.reshape((self.n_clusters, -1)),
+                metric="euclidean",
+            )
         elif self.metric == "dtw":
-            return cdist_dtw(X, self.cluster_centers_, n_jobs=self.n_jobs,
-                             verbose=self.verbose, **metric_params)
+            return cdist_dtw(
+                X,
+                self.cluster_centers_,
+                n_jobs=self.n_jobs,
+                verbose=self.verbose,
+                **metric_params
+            )
         elif self.metric == "softdtw":
             return cdist_soft_dtw(X, self.cluster_centers_, **metric_params)
         else:
-            raise ValueError("Incorrect metric: %s (should be one of 'dtw', "
-                             "'softdtw', 'euclidean')" % self.metric)
+            raise ValueError(
+                "Incorrect metric: %s (should be one of 'dtw', "
+                "'softdtw', 'euclidean')" % self.metric
+            )
 
     def _assign(self, X, update_class_attributes=True):
         dists = self._transform(X)
         matched_labels = dists.argmin(axis=1)
         if update_class_attributes:
             self.labels_ = matched_labels
             _check_no_empty_cluster(self.labels_, self.n_clusters)
             if self.dtw_inertia and self.metric != "dtw":
-                inertia_dists = cdist_dtw(X, self.cluster_centers_,
-                                          n_jobs=self.n_jobs,
-                                          verbose=self.verbose)
+                inertia_dists = cdist_dtw(
+                    X, self.cluster_centers_, n_jobs=self.n_jobs, verbose=self.verbose
+                )
             else:
                 inertia_dists = dists
-            self.inertia_ = _compute_inertia(inertia_dists,
-                                             self.labels_,
-                                             self._squared_inertia)
+            self.inertia_ = _compute_inertia(
+                inertia_dists, self.labels_, self._squared_inertia
+            )
         return matched_labels
 
     def _update_centroids(self, X):
         metric_params = self._get_metric_params()
         for k in range(self.n_clusters):
             if self.metric == "dtw":
                 self.cluster_centers_[k] = dtw_barycenter_averaging(
                     X=X[self.labels_ == k],
                     barycenter_size=None,
                     init_barycenter=self.cluster_centers_[k],
                     metric_params=metric_params,
-                    verbose=False)
+                    verbose=False,
+                )
             elif self.metric == "softdtw":
                 self.cluster_centers_[k] = softdtw_barycenter(
                     X=X[self.labels_ == k],
                     max_iter=self.max_iter_barycenter,
                     init=self.cluster_centers_[k],
-                    **metric_params)
+                    **metric_params
+                )
             else:
-                self.cluster_centers_[k] = euclidean_barycenter(
-                    X=X[self.labels_ == k])
+                self.cluster_centers_[k] = euclidean_barycenter(X=X[self.labels_ == k])
 
     def fit(self, X, y=None):
         """Compute k-means clustering.
 
         Parameters
         ----------
         X : array-like of shape=(n_ts, sz, d)
             Time series dataset.
 
         y
             Ignored
         """
 
-        X = check_array(X, allow_nd=True, force_all_finite='allow-nan')
+        X = check_array(X, allow_nd=True, force_all_finite="allow-nan")
 
-        if hasattr(self.init, '__array__'):
-            X = check_dims(X, X_fit_dims=self.init.shape,
-                           extend=True,
-                           check_n_features_only=(self.metric != "euclidean"))
+        if hasattr(self.init, "__array__"):
+            X = check_dims(
+                X,
+                X_fit_dims=self.init.shape,
+                extend=True,
+                check_n_features_only=(self.metric != "euclidean"),
+            )
 
         self.labels_ = None
         self.inertia_ = numpy.inf
         self.cluster_centers_ = None
         self._X_fit = None
         self._squared_inertia = True
 
         self.n_iter_ = 0
 
         max_attempts = max(self.n_init, 10)
 
         X_ = to_time_series_dataset(X)
         rs = check_random_state(self.random_state)
 
-        if isinstance(self.init, str) and self.init == "k-means++" and \
-                        self.metric == "euclidean":
+        if (
+            isinstance(self.init, str)
+            and self.init == "k-means++"
+            and self.metric == "euclidean"
+        ):
             n_ts, sz, d = X_.shape
-            x_squared_norms = cdist(X_.reshape((n_ts, -1)),
-                                    numpy.zeros((1, sz * d)),
-                                    metric="sqeuclidean").reshape((1, -1))
+            x_squared_norms = cdist(
+                X_.reshape((n_ts, -1)), numpy.zeros((1, sz * d)), metric="sqeuclidean"
+            ).reshape((1, -1))
         else:
             x_squared_norms = None
         _check_initial_guess(self.init, self.n_clusters)
 
         best_correct_centroids = None
         min_inertia = numpy.inf
         n_successful = 0
@@ -805,15 +846,15 @@
             Ignored
 
         Returns
         -------
         labels : array of shape=(n_ts, )
             Index of the cluster each sample belongs to.
         """
-        X = check_array(X, allow_nd=True, force_all_finite='allow-nan')
+        X = check_array(X, allow_nd=True, force_all_finite="allow-nan")
         return self.fit(X, y).labels_
 
     def predict(self, X):
         """Predict the closest cluster each time series in X belongs to.
 
         Parameters
         ----------
@@ -821,39 +862,45 @@
             Time series dataset to predict.
 
         Returns
         -------
         labels : array of shape=(n_ts, )
             Index of the cluster each sample belongs to.
         """
-        X = check_array(X, allow_nd=True, force_all_finite='allow-nan')
-        check_is_fitted(self, 'cluster_centers_')
-        X = check_dims(X, X_fit_dims=self.cluster_centers_.shape,
-                       extend=True,
-                       check_n_features_only=(self.metric != "euclidean"))
+        X = check_array(X, allow_nd=True, force_all_finite="allow-nan")
+        check_is_fitted(self, "cluster_centers_")
+        X = check_dims(
+            X,
+            X_fit_dims=self.cluster_centers_.shape,
+            extend=True,
+            check_n_features_only=(self.metric != "euclidean"),
+        )
         return self._assign(X, update_class_attributes=False)
 
     def transform(self, X):
         """Transform X to a cluster-distance space.
 
-        In the new space, each dimension is the distance to the cluster 
+        In the new space, each dimension is the distance to the cluster
         centers.
 
         Parameters
         ----------
         X : array-like of shape=(n_ts, sz, d)
             Time series dataset
 
         Returns
         -------
         distances : array of shape=(n_ts, n_clusters)
             Distances to cluster centers
         """
-        X = check_array(X, allow_nd=True, force_all_finite='allow-nan')
-        check_is_fitted(self, 'cluster_centers_')
-        X = check_dims(X, X_fit_dims=self.cluster_centers_.shape,
-                       extend=True,
-                       check_n_features_only=(self.metric != "euclidean"))
+        X = check_array(X, allow_nd=True, force_all_finite="allow-nan")
+        check_is_fitted(self, "cluster_centers_")
+        X = check_dims(
+            X,
+            X_fit_dims=self.cluster_centers_.shape,
+            extend=True,
+            check_n_features_only=(self.metric != "euclidean"),
+        )
         return self._transform(X)
 
     def _more_tags(self):
-        return {'allow_nan': True, 'allow_variable_length': True}
+        return {"allow_nan": True, "allow_variable_length": True}
```

### Comparing `tslearn-0.5.3.2/tslearn/clustering/kshape.py` & `tslearn-0.6.0/tslearn/clustering/kshape.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/clustering/utils.py` & `tslearn-0.6.0/tslearn/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/datasets/cached.py` & `tslearn-0.6.0/tslearn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/datasets/datasets.py` & `tslearn-0.6.0/tslearn/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/datasets/ucr_uea.py` & `tslearn-0.6.0/tslearn/datasets/ucr_uea.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self._data_dir = os.path.expanduser(os.path.join(
             "~", ".tslearn", "datasets", "UCR_UEA"
         ))
         os.makedirs(self._data_dir, exist_ok=True)
 
         try:
             url_multivariate = ("https://www.timeseriesclassification.com/"
-                                "Downloads/Archives/summaryMultivariate.csv")
+                                "ClassificationDownloads/Archives/summaryMultivariate.csv")
             self._list_multivariate_filename = os.path.join(
                 self._data_dir, os.path.basename(url_multivariate)
             )
             urlretrieve(url_multivariate, self._list_multivariate_filename)
             url_baseline = ("https://www.timeseriesclassification.com/"
                             "singleTrainTest.csv")
             self._baseline_scores_filename = os.path.join(
@@ -263,15 +263,15 @@
             except FileNotFoundError:
                 pass  # nothing to do here, already deleted
             except IsADirectoryError:
                 # we then need this function to recursively remove the directory:
                 shutil.rmtree(full_path, ignore_errors=True)
             # else, actually raise the error!
 
-            url = ("https://www.timeseriesclassification.com/Downloads/%s.zip"
+            url = ("https://www.timeseriesclassification.com/ClassificationDownloads/%s.zip"
                    % dataset_name)
             success = extract_from_zip_url(url, target_dir=full_path)
             if not success:
                 warnings.warn("dataset \"%s\" could not be downloaded or "
                               "extracted" % dataset_name,
                               category=RuntimeWarning, stacklevel=2)
                 return None, None, None, None
```

### Comparing `tslearn-0.5.3.2/tslearn/early_classification/__init__.py` & `tslearn-0.6.0/tslearn/early_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/early_classification/early_classification.py` & `tslearn-0.6.0/tslearn/early_classification/early_classification.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/generators/generators.py` & `tslearn-0.6.0/tslearn/generators/generators.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/hdftools/hdftools.py` & `tslearn-0.6.0/tslearn/hdftools/hdftools.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/matrix_profile/matrix_profile.py` & `tslearn-0.6.0/tslearn/matrix_profile/matrix_profile.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/metrics/__init__.py` & `tslearn-0.6.0/tslearn/metrics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .ctw import ctw_path, ctw, cdist_ctw
 from .sax import cdist_sax
 from .softdtw_variants import (cdist_soft_dtw, cdist_gak,
                                cdist_soft_dtw_normalized, gak, soft_dtw,
                                soft_dtw_alignment,
                                sigma_gak, gamma_soft_dtw, SquaredEuclidean,
                                SoftDTW)
+from .soft_dtw_loss_pytorch import SoftDTWLossPyTorch
 from .cycc import cdist_normalized_cc, y_shifted_sbd_vec
 
 __author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
 
 TSLEARN_VALID_METRICS = ["ctw", "dtw", "gak", "sax", "softdtw", "lcss"]
 VARIABLE_LENGTH_METRICS = ["ctw", "dtw", "gak", "sax", "softdtw", "lcss"]
 
@@ -45,9 +46,11 @@
 
     "cdist_sax",
 
     "cdist_soft_dtw", "cdist_gak",
     "cdist_soft_dtw_normalized", "gak", "soft_dtw", "soft_dtw_alignment",
     "sigma_gak", "gamma_soft_dtw", "SquaredEuclidean", "SoftDTW",
 
+    "SoftDTWLossPyTorch",
+
     "cdist_normalized_cc", "y_shifted_sbd_vec"
 ]
```

### Comparing `tslearn-0.5.3.2/tslearn/metrics/ctw.py` & `tslearn-0.6.0/tslearn/metrics/ctw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,241 +1,258 @@
+import numpy as np
 from sklearn.cross_decomposition import CCA
+
+from tslearn.backend import instantiate_backend
+
+from ..utils import to_time_series
 from .dtw_variants import dtw_path
 from .utils import _cdist_generic
-from ..utils import to_time_series
-import numpy as np
 
-def _get_warp_matrices(warp_path):
+
+def _get_warp_matrices(warp_path, be):
     """
     Convert warping path sequence to matrices.
 
     Parameters
     ----------
-    warp_path = first output of the dtw_path function = list of tuple of two 
-    indices that are matched together.
+    warp_path : list of tuple of two indices that are matched together
+        First output of the dtw_path function.
+    be : Backend object or string
+        Backend.
 
     Returns
     -------
-    two 2D matrices of size m x T (m = number of step to match the two 
-    sequences
-
+    two 2D matrices of size m x T (m = number of step to match the two
+        sequences
     """
-
+    be = instantiate_backend(be, warp_path[0][0])
     # number of indices for the alignment
     m = len(warp_path)
     # number of frame of each sequence
     # (for DTW, the last two indices are matched)
     nx = warp_path[-1][0] + 1
     ny = warp_path[-1][1] + 1
-    Wx = np.zeros((m, nx))
-    Wy = np.zeros((m, ny))
+    Wx = be.zeros((m, nx), dtype=be.float64)
+    Wy = be.zeros((m, ny), dtype=be.float64)
 
     for i, match in enumerate(warp_path):
         Wx[i, match[0]] = 1
         Wy[i, match[1]] = 1
 
     return Wx, Wy
 
 
-def ctw_path(s1, s2, max_iter=100, n_components=None,
-             global_constraint=None, sakoe_chiba_radius=None,
-             itakura_max_slope=None, verbose=False):
+def ctw_path(
+    s1,
+    s2,
+    max_iter=100,
+    n_components=None,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    verbose=False,
+    be=None,
+):
     """Compute Canonical Time Warping (CTW) similarity measure between
     (possibly multidimensional) time series and return the alignment path, the
     canonical correlation analysis (sklearn) object and the similarity.
-    
-    Canonical Time Warping is a method to align time series under rigid 
+
+    Canonical Time Warping is a method to align time series under rigid
     registration of the feature space.
     It should not be confused with Dynamic Time Warping (DTW), though CTW uses
     DTW.
 
-    It is not required that both time series share the same size, nor the same 
-    dimension (CTW will find a subspace that best aligns feature spaces). 
+    It is not required that both time series share the same size, nor the same
+    dimension (CTW will find a subspace that best aligns feature spaces).
     CTW was originally presented in [1]_.
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-        
     max_iter : int (default: 100)
         Number of iterations for the CTW algorithm. Each iteration
-    
     n_components : int (default: None)
         Number of components to be used for Canonical Correlation Analysis.
-        If None, the lower minimum number of features between s1 and s2 is 
-        used. 
-
+        If None, the lower minimum number of features between s1 and s2 is
+        used.
     global_constraint : {"itakura", "sakoe_chiba"} or None (default: None)
         Global constraint to restrict admissible paths for DTW calls.
-
     sakoe_chiba_radius : int or None (default: None)
         Radius to be used for Sakoe-Chiba band global constraint.
         If None and `global_constraint` is set to "sakoe_chiba", a radius of
         1 is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     itakura_max_slope : float or None (default: None)
         Maximum slope for the Itakura parallelogram constraint.
         If None and `global_constraint` is set to "itakura", a maximum slope
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-        
     verbose : bool (default: True)
         If True, scores are printed at each iteration of the algorithm.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     list of integer pairs
         Matching path represented as a list of index pairs. In each pair, the
         first index corresponds to s1 and the second one corresponds to s2
-        
     sklearn.decomposition.CCA
         The Canonical Correlation Analysis object used to align time series
         at convergence.
-
     float
         Similarity score
 
     Examples
     --------
     >>> path, cca, dist = ctw_path([1, 2, 3], [1., 2., 2., 3.])
     >>> path
     [(0, 0), (1, 1), (1, 2), (2, 3)]
     >>> type(cca)  # doctest: +ELLIPSIS
     <class 'sklearn.cross_decomposition...CCA'>
     >>> dist
     0.0
-    >>> path, cca, dist = ctw_path([1, 2, 3], 
+    >>> path, cca, dist = ctw_path([1, 2, 3],
     ...                            [[1., 1.], [2., 2.], [2., 2.], [3., 3.]])
     >>> dist
     0.0
 
     See Also
     --------
     ctw : Get only the similarity score for CTW
 
     References
     ----------
-    .. [1] F. Zhou and F. Torre, "Canonical time warping for alignment of 
+    .. [1] F. Zhou and F. Torre, "Canonical time warping for alignment of
        human behavior". NIPS 2009.
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
+    s1, s2 = be.array(s1, dtype=be.float64), be.array(s2, dtype=be.float64)
 
     if n_components is None:
         n_components = min(s1.shape[-1], s2.shape[-1])
 
     cca = CCA(n_components=n_components)
 
     # first iteration :
     # identity matrices, this relates to apply first a dtw on the
     # (possibly truncated to a fixed number of features) inputs
-    seq1_tr = s1.dot(np.eye(s1.shape[1], n_components))
-    seq2_tr = s2.dot(np.eye(s2.shape[1], n_components))
-    current_path, score_match = dtw_path(seq1_tr, seq2_tr,
-                                         global_constraint=global_constraint,
-                                         sakoe_chiba_radius=sakoe_chiba_radius,
-                                         itakura_max_slope=itakura_max_slope)
+    seq1_tr = s1 @ be.eye(s1.shape[1], n_components, dtype=be.float64)
+    seq2_tr = s2 @ be.eye(s2.shape[1], n_components, dtype=be.float64)
+    current_path, score_match = dtw_path(
+        seq1_tr,
+        seq2_tr,
+        global_constraint=global_constraint,
+        sakoe_chiba_radius=sakoe_chiba_radius,
+        itakura_max_slope=itakura_max_slope,
+        be=be,
+    )
     current_score = score_match
 
     if verbose:
         print("Iteration 0, score={}".format(current_score))
 
-    for it in range(max_iter-1):
-        Wx, Wy = _get_warp_matrices(current_path)
+    for it in range(max_iter - 1):
+        Wx, Wy = _get_warp_matrices(current_path, be=be)
 
-        cca.fit(Wx.dot(s1), Wy.dot(s2))
+        cca.fit(Wx @ s1, Wy @ s2)
         seq1_tr, seq2_tr = cca.transform(s1, s2)
 
         current_path, score_match = dtw_path(
-            seq1_tr, seq2_tr,
+            seq1_tr,
+            seq2_tr,
             global_constraint=global_constraint,
             sakoe_chiba_radius=sakoe_chiba_radius,
-            itakura_max_slope=itakura_max_slope
+            itakura_max_slope=itakura_max_slope,
+            be=be,
         )
 
         if np.array_equal(current_path, current_path):
             break
 
         current_score = score_match
 
         if verbose:
             print("Iteration {}, score={}".format(it + 1, current_score))
 
     return current_path, cca, current_score
 
 
-def ctw(s1, s2, max_iter=100, n_components=None,
-        global_constraint=None, sakoe_chiba_radius=None,
-        itakura_max_slope=None, verbose=False):
+def ctw(
+    s1,
+    s2,
+    max_iter=100,
+    n_components=None,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    verbose=False,
+    be=None,
+):
     """Compute Canonical Time Warping (CTW) similarity measure between
     (possibly multidimensional) time series and return the similarity.
-    
-    Canonical Time Warping is a method to align time series under rigid 
+
+    Canonical Time Warping is a method to align time series under rigid
     registration of the feature space.
     It should not be confused with Dynamic Time Warping (DTW), though CTW uses
     DTW.
 
-    It is not required that both time series share the same size, nor the same 
-    dimension (CTW will find a subspace that best aligns feature spaces). 
+    It is not required that both time series share the same size, nor the same
+    dimension (CTW will find a subspace that best aligns feature spaces).
     CTW was originally presented in [1]_.
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-        
     max_iter : int (default: 100)
         Number of iterations for the CTW algorithm. Each iteration
-    
     n_components : int (default: None)
         Number of components to be used for Canonical Correlation Analysis.
-        If None, the lower minimum number of features between seq1 and seq2 is 
-        used. 
-
+        If None, the lower minimum number of features between seq1 and seq2 is
+        used.
     global_constraint : {"itakura", "sakoe_chiba"} or None (default: None)
         Global constraint to restrict admissible paths for DTW calls.
-
     sakoe_chiba_radius : int or None (default: None)
         Radius to be used for Sakoe-Chiba band global constraint.
         If None and `global_constraint` is set to "sakoe_chiba", a radius of
         1 is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     itakura_max_slope : float or None (default: None)
         Maximum slope for the Itakura parallelogram constraint.
         If None and `global_constraint` is set to "itakura", a maximum slope
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-        
     verbose : bool (default: True)
         If True, scores are printed at each iteration of the algorithm.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Similarity score
 
     Examples
@@ -247,118 +264,136 @@
 
     See Also
     --------
     ctw : Get only the similarity score for CTW
 
     References
     ----------
-    .. [1] F. Zhou and F. Torre, "Canonical time warping for alignment of 
+    .. [1] F. Zhou and F. Torre, "Canonical time warping for alignment of
        human behavior". NIPS 2009.
     """
-    return ctw_path(s1=s1, s2=s2, max_iter=max_iter,
-                    n_components=n_components,
-                    global_constraint=global_constraint,
-                    sakoe_chiba_radius=sakoe_chiba_radius,
-                    itakura_max_slope=itakura_max_slope, verbose=verbose)[-1]
-
-
-def cdist_ctw(dataset1, dataset2=None, max_iter=100, n_components=None,
-              global_constraint=None, sakoe_chiba_radius=None,
-              itakura_max_slope=None, n_jobs=None, verbose=0):
+    be = instantiate_backend(be, s1)
+    return ctw_path(
+        s1=s1,
+        s2=s2,
+        max_iter=max_iter,
+        n_components=n_components,
+        global_constraint=global_constraint,
+        sakoe_chiba_radius=sakoe_chiba_radius,
+        itakura_max_slope=itakura_max_slope,
+        verbose=verbose,
+        be=be,
+    )[-1]
+
+
+def cdist_ctw(
+    dataset1,
+    dataset2=None,
+    max_iter=100,
+    n_components=None,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    n_jobs=None,
+    verbose=0,
+    be=None,
+):
     r"""Compute cross-similarity matrix using Canonical Time Warping (CTW)
     similarity measure.
-    
-    Canonical Time Warping is a method to align time series under rigid 
+
+    Canonical Time Warping is a method to align time series under rigid
     registration of the feature space.
     It should not be confused with Dynamic Time Warping (DTW), though CTW uses
     DTW.
 
-    It is not required that both time series share the same size, nor the same 
-    dimension (CTW will find a subspace that best aligns feature spaces). 
+    It is not required that both time series share the same size, nor the same
+    dimension (CTW will find a subspace that best aligns feature spaces).
     CTW was originally presented in [1]_.
 
     Parameters
     ----------
     dataset1 : array-like
         A dataset of time series
-
     dataset2 : array-like (default: None)
         Another dataset of time series. If `None`, self-similarity of
         `dataset1` is returned.
-        
     max_iter : int (default: 100)
         Number of iterations for the CTW algorithm. Each iteration
-    
     n_components : int (default: None)
         Number of components to be used for Canonical Correlation Analysis.
-        If None, the lower minimum number of features between seq1 and seq2 is 
-        used. 
-
+        If None, the lower minimum number of features between seq1 and seq2 is
+        used.
     global_constraint : {"itakura", "sakoe_chiba"} or None (default: None)
         Global constraint to restrict admissible paths for DTW calls.
-
     sakoe_chiba_radius : int or None (default: None)
         Radius to be used for Sakoe-Chiba band global constraint.
         If None and `global_constraint` is set to "sakoe_chiba", a radius of
         1 is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     itakura_max_slope : float or None (default: None)
         Maximum slope for the Itakura parallelogram constraint.
         If None and `global_constraint` is set to "itakura", a maximum slope
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     n_jobs : int or None, optional (default=None)
         The number of jobs to run in parallel.
         ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
         ``-1`` means using all processors. See scikit-learns'
         `Glossary <https://scikit-learn.org/stable/glossary.html#term-n-jobs>`__
         for more details.
-
     verbose : int, optional (default=0)
         The verbosity level: if non zero, progress messages are printed.
         Above 50, the output is sent to stdout.
         The frequency of the messages increases with the verbosity level.
         If it more than 10, all iterations are reported.
         `Glossary <https://joblib.readthedocs.io/en/latest/parallel.html#parallel-reference-documentation>`__
         for more details.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     cdist : numpy.ndarray
         Cross-similarity matrix
 
     Examples
     --------
     >>> cdist_ctw([[1, 2, 2, 3], [1., 2., 3., 4.]])
     array([[0., 1.],
            [1., 0.]])
-    >>> cdist_ctw([[1, 2, 2, 3], [1., 2., 3., 4.]], 
+    >>> cdist_ctw([[1, 2, 2, 3], [1., 2., 3., 4.]],
     ...           [[[1, 1], [2, 2], [3, 3]], [[2, 2], [3, 3], [4, 4], [5, 5]]])
     array([[0.        , 2.44948974],
            [1.        , 1.41421356]])
 
     See Also
     --------
     ctw : Get CTW similarity score
 
     References
     ----------
-    .. [1] F. Zhou and F. Torre, "Canonical time warping for alignment of 
+    .. [1] F. Zhou and F. Torre, "Canonical time warping for alignment of
        human behavior". NIPS 2009.
     """  # noqa: E501
-    return _cdist_generic(dist_fun=ctw, dataset1=dataset1, dataset2=dataset2,
-                          n_jobs=n_jobs, verbose=verbose,
-                          compute_diagonal=False,
-                          max_iter=max_iter, n_components=n_components,
-                          global_constraint=global_constraint,
-                          sakoe_chiba_radius=sakoe_chiba_radius,
-                          itakura_max_slope=itakura_max_slope)
+    be = instantiate_backend(be, dataset1)
+    return _cdist_generic(
+        dist_fun=ctw,
+        dataset1=dataset1,
+        dataset2=dataset2,
+        n_jobs=n_jobs,
+        verbose=verbose,
+        compute_diagonal=False,
+        max_iter=max_iter,
+        n_components=n_components,
+        global_constraint=global_constraint,
+        sakoe_chiba_radius=sakoe_chiba_radius,
+        itakura_max_slope=itakura_max_slope,
+        be=be,
+    )
```

### Comparing `tslearn-0.5.3.2/tslearn/metrics/cycc.c` & `tslearn-0.6.0/tslearn/metrics/cycc.c`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/metrics/cycc.py` & `tslearn-0.6.0/tslearn/metrics/cycc.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/metrics/cysax.c` & `tslearn-0.6.0/tslearn/metrics/cysax.c`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/metrics/cysax.py` & `tslearn-0.6.0/tslearn/metrics/cysax.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/metrics/dtw_variants.py` & `tslearn-0.6.0/tslearn/metrics/dtw_variants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import warnings
 
 import numpy
 from numba import njit, prange
-from sklearn.metrics.pairwise import pairwise_distances
 
+from tslearn.backend import instantiate_backend
 from tslearn.utils import to_time_series
+
 from .utils import _cdist_generic
 
-__author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
+__author__ = "Romain Tavenard romain.tavenard[at]univ-rennes2.fr"
 
 GLOBAL_CONSTRAINT_CODE = {None: 0, "": 0, "itakura": 1, "sakoe_chiba": 2}
 
 
 @njit()
-def _local_squared_dist(x, y):
-    dist = 0.
+def _njit_local_squared_dist(x, y):
+    dist = 0.0
     for di in range(x.shape[0]):
-        diff = (x[di] - y[di])
+        diff = x[di] - y[di]
+        dist += diff * diff
+    return dist
+
+
+def _local_squared_dist(x, y, be=None):
+    be = instantiate_backend(be, x)
+    dist = 0.0
+    for di in range(be.shape(x)[0]):
+        diff = x[di] - y[di]
         dist += diff * diff
     return dist
 
 
 @njit()
 def njit_accumulated_matrix(s1, s2, mask):
     """Compute the accumulated cost matrix score between two time series.
@@ -41,28 +51,64 @@
     mat : array, shape = (sz1, sz2)
         Accumulated cost matrix.
 
     """
     l1 = s1.shape[0]
     l2 = s2.shape[0]
     cum_sum = numpy.full((l1 + 1, l2 + 1), numpy.inf)
-    cum_sum[0, 0] = 0.
+    cum_sum[0, 0] = 0.0
 
     for i in range(l1):
         for j in range(l2):
             if numpy.isfinite(mask[i, j]):
-                cum_sum[i + 1, j + 1] = _local_squared_dist(s1[i], s2[j])
-                cum_sum[i + 1, j + 1] += min(cum_sum[i, j + 1],
-                                             cum_sum[i + 1, j],
-                                             cum_sum[i, j])
+                cum_sum[i + 1, j + 1] = _njit_local_squared_dist(s1[i], s2[j])
+                cum_sum[i + 1, j + 1] += min(
+                    cum_sum[i, j + 1], cum_sum[i + 1, j], cum_sum[i, j]
+                )
+    return cum_sum[1:, 1:]
+
+
+def accumulated_matrix(s1, s2, mask, be=None):
+    """Compute the accumulated cost matrix score between two time series.
+
+    Parameters
+    ----------
+    s1 : array, shape = (sz1,)
+        First time series.
+    s2 : array, shape = (sz2,)
+        Second time series
+    mask : array, shape = (sz1, sz2)
+        Mask. Unconsidered cells must have infinite values.
+    be : Backend object or string or None
+        Backend.
+
+    Returns
+    -------
+    mat : array, shape = (sz1, sz2)
+        Accumulated cost matrix.
+
+    """
+    be = instantiate_backend(be, s1)
+    l1 = be.shape(s1)[0]
+    l2 = be.shape(s2)[0]
+    cum_sum = be.full((l1 + 1, l2 + 1), be.inf)
+    cum_sum[0, 0] = 0.0
+
+    for i in range(l1):
+        for j in range(l2):
+            if be.isfinite(mask[i, j]):
+                cum_sum[i + 1, j + 1] = _local_squared_dist(s1[i], s2[j], be=be)
+                cum_sum[i + 1, j + 1] += min(
+                    cum_sum[i, j + 1], cum_sum[i + 1, j], cum_sum[i, j]
+                )
     return cum_sum[1:, 1:]
 
 
 @njit(nogil=True)
-def njit_dtw(s1, s2, mask):
+def _njit_dtw(s1, s2, mask):
     """Compute the dynamic time warping score between two time series.
 
     Parameters
     ----------
     s1 : array, shape = (sz1,)
         First time series.
 
@@ -78,40 +124,103 @@
         Dynamic Time Warping score between both time series.
 
     """
     cum_sum = njit_accumulated_matrix(s1, s2, mask)
     return numpy.sqrt(cum_sum[-1, -1])
 
 
+def _dtw(s1, s2, mask, be=None):
+    """Compute the dynamic time warping score between two time series.
+
+    Parameters
+    ----------
+    s1 : array, shape = (sz1,)
+        First time series.
+    s2 : array, shape = (sz2,)
+        Second time series
+    mask : array, shape = (sz1, sz2)
+        Mask. Unconsidered cells must have infinite values.
+    be : Backend object or string or None
+        Backend.
+
+    Returns
+    -------
+    dtw_score : float
+        Dynamic Time Warping score between both time series.
+
+    """
+    be = instantiate_backend(be, s1)
+    cum_sum = accumulated_matrix(s1, s2, mask, be=be)
+    return be.sqrt(cum_sum[-1, -1])
+
+
 @njit()
-def _return_path(acc_cost_mat):
+def _njit_return_path(acc_cost_mat):
     sz1, sz2 = acc_cost_mat.shape
     path = [(sz1 - 1, sz2 - 1)]
     while path[-1] != (0, 0):
         i, j = path[-1]
         if i == 0:
             path.append((0, j - 1))
         elif j == 0:
             path.append((i - 1, 0))
         else:
-            arr = numpy.array([acc_cost_mat[i - 1][j - 1],
-                               acc_cost_mat[i - 1][j],
-                               acc_cost_mat[i][j - 1]])
+            arr = numpy.array(
+                [
+                    acc_cost_mat[i - 1][j - 1],
+                    acc_cost_mat[i - 1][j],
+                    acc_cost_mat[i][j - 1],
+                ]
+            )
             argmin = numpy.argmin(arr)
             if argmin == 0:
                 path.append((i - 1, j - 1))
             elif argmin == 1:
                 path.append((i - 1, j))
             else:
                 path.append((i, j - 1))
     return path[::-1]
 
 
-def dtw_path(s1, s2, global_constraint=None, sakoe_chiba_radius=None,
-             itakura_max_slope=None):
+def _return_path(acc_cost_mat, be=None):
+    be = instantiate_backend(be, acc_cost_mat)
+    sz1, sz2 = be.shape(acc_cost_mat)
+    path = [(sz1 - 1, sz2 - 1)]
+    while path[-1] != (0, 0):
+        i, j = path[-1]
+        if i == 0:
+            path.append((0, j - 1))
+        elif j == 0:
+            path.append((i - 1, 0))
+        else:
+            arr = be.array(
+                [
+                    acc_cost_mat[i - 1][j - 1],
+                    acc_cost_mat[i - 1][j],
+                    acc_cost_mat[i][j - 1],
+                ]
+            )
+            argmin = be.argmin(arr)
+            if argmin == 0:
+                path.append((i - 1, j - 1))
+            elif argmin == 1:
+                path.append((i - 1, j))
+            else:
+                path.append((i, j - 1))
+    return path[::-1]
+
+
+def dtw_path(
+    s1,
+    s2,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    be=None,
+):
     r"""Compute Dynamic Time Warping (DTW) similarity measure between
     (possibly multidimensional) time series and return both the path and the
     similarity.
 
     DTW is computed as the Euclidean distance between aligned time series,
     i.e., if :math:`\pi` is the alignment path:
 
@@ -123,40 +232,38 @@
     be the same dimension. DTW was originally presented in [1]_ and is
     discussed in more details in our :ref:`dedicated user-guide page <dtw>`.
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-
     global_constraint : {"itakura", "sakoe_chiba"} or None (default: None)
         Global constraint to restrict admissible paths for DTW.
-
     sakoe_chiba_radius : int or None (default: None)
         Radius to be used for Sakoe-Chiba band global constraint.
         If None and `global_constraint` is set to "sakoe_chiba", a radius of
         1 is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     itakura_max_slope : float or None (default: None)
         Maximum slope for the Itakura parallelogram constraint.
         If None and `global_constraint` is set to "itakura", a maximum slope
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     list of integer pairs
         Matching path represented as a list of index pairs. In each pair, the
         first index corresponds to s1 and the second one corresponds to s2
 
@@ -182,31 +289,41 @@
     References
     ----------
     .. [1] H. Sakoe, S. Chiba, "Dynamic programming algorithm optimization for
            spoken word recognition," IEEE Transactions on Acoustics, Speech and
            Signal Processing, vol. 26(1), pp. 43--49, 1978.
 
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
 
     if len(s1) == 0 or len(s2) == 0:
         raise ValueError(
-            "One of the input time series contains only nans or has zero length.")
+            "One of the input time series contains only nans or has zero length."
+        )
 
-    if s1.shape[1] != s2.shape[1]:
+    if be.shape(s1)[1] != be.shape(s2)[1]:
         raise ValueError("All input time series must have the same feature size.")
 
     mask = compute_mask(
-        s1, s2, GLOBAL_CONSTRAINT_CODE[global_constraint],
-        sakoe_chiba_radius, itakura_max_slope
+        s1,
+        s2,
+        GLOBAL_CONSTRAINT_CODE[global_constraint],
+        sakoe_chiba_radius,
+        itakura_max_slope,
+        be=be,
     )
-    acc_cost_mat = njit_accumulated_matrix(s1, s2, mask=mask)
-    path = _return_path(acc_cost_mat)
-    return path, numpy.sqrt(acc_cost_mat[-1, -1])
+    if be.is_numpy:
+        acc_cost_mat = njit_accumulated_matrix(s1, s2, mask=mask)
+        path = _njit_return_path(acc_cost_mat)
+    else:
+        acc_cost_mat = accumulated_matrix(s1, s2, mask=mask, be=be)
+        path = _return_path(acc_cost_mat, be=be)
+    return path, be.sqrt(acc_cost_mat[-1, -1])
 
 
 @njit()
 def njit_accumulated_matrix_from_dist_matrix(dist_matrix, mask):
     """Compute the accumulated cost matrix score between two time series using
     a precomputed distance matrix.
 
@@ -222,29 +339,68 @@
     -------
     mat : array, shape = (sz1, sz2)
         Accumulated cost matrix.
 
     """
     l1, l2 = dist_matrix.shape
     cum_sum = numpy.full((l1 + 1, l2 + 1), numpy.inf)
-    cum_sum[0, 0] = 0.
+    cum_sum[0, 0] = 0.0
 
     for i in prange(l1):
         for j in prange(l2):
             if numpy.isfinite(mask[i, j]):
                 cum_sum[i + 1, j + 1] = dist_matrix[i, j]
-                cum_sum[i + 1, j + 1] += min(cum_sum[i, j + 1],
-                                             cum_sum[i + 1, j],
-                                             cum_sum[i, j])
+                cum_sum[i + 1, j + 1] += min(
+                    cum_sum[i, j + 1], cum_sum[i + 1, j], cum_sum[i, j]
+                )
+    return cum_sum[1:, 1:]
+
+
+def accumulated_matrix_from_dist_matrix(dist_matrix, mask, be=None):
+    """Compute the accumulated cost matrix score between two time series using
+    a precomputed distance matrix.
+
+    Parameters
+    ----------
+    dist_matrix : array, shape = (sz1, sz2)
+        Array containing the pairwise distances.
+    mask : array, shape = (sz1, sz2)
+        Mask. Unconsidered cells must have infinite values.
+    be : Backend object or string or None
+        Backend.
+    Returns
+    -------
+    mat : array, shape = (sz1, sz2)
+        Accumulated cost matrix.
+    """
+    be = instantiate_backend(be, dist_matrix)
+    l1, l2 = be.shape(dist_matrix)
+    cum_sum = be.full((l1 + 1, l2 + 1), be.inf)
+    cum_sum[0, 0] = 0.0
+
+    for i in range(l1):
+        for j in range(l2):
+            if be.isfinite(mask[i, j]):
+                cum_sum[i + 1, j + 1] = dist_matrix[i, j]
+                cum_sum[i + 1, j + 1] += min(
+                    cum_sum[i, j + 1], cum_sum[i + 1, j], cum_sum[i, j]
+                )
     return cum_sum[1:, 1:]
 
 
-def dtw_path_from_metric(s1, s2=None, metric="euclidean",
-                         global_constraint=None, sakoe_chiba_radius=None,
-                         itakura_max_slope=None, **kwds):
+def dtw_path_from_metric(
+    s1,
+    s2=None,
+    metric="euclidean",
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    be=None,
+    **kwds
+):
     r"""Compute Dynamic Time Warping (DTW) similarity measure between
     (possibly multidimensional) time series using a distance metric defined by
     the user and return both the path and the similarity.
 
     Similarity is computed as the cumulative cost along the aligned time
     series.
 
@@ -298,14 +454,17 @@
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
 
+    be : Backend object or string or None
+        Backend.
+
     **kwds
         Additional arguments to pass to sklearn pairwise_distances to compute
         the pairwise distances.
 
     Returns
     -------
     list of integer pairs
@@ -363,37 +522,57 @@
     .. _pairwise_distances: https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise_distances.html
 
     .. _scikit: https://scikit-learn.org/stable/modules/metrics.html
 
     .. _scipy: https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.pdist.html
 
     """  # noqa: E501
+    be = instantiate_backend(be, s1)
     if metric == "precomputed":  # Pairwise distance given as input
-        sz1, sz2 = s1.shape
+        sz1, sz2 = be.shape(s1)
         mask = compute_mask(
-            sz1, sz2, GLOBAL_CONSTRAINT_CODE[global_constraint],
-            sakoe_chiba_radius, itakura_max_slope
+            sz1,
+            sz2,
+            GLOBAL_CONSTRAINT_CODE[global_constraint],
+            sakoe_chiba_radius,
+            itakura_max_slope,
+            be=be,
         )
         dist_mat = s1
     else:
-        s1 = to_time_series(s1, remove_nans=True)
-        s2 = to_time_series(s2, remove_nans=True)
+        s1 = to_time_series(s1, remove_nans=True, be=be)
+        s2 = to_time_series(s2, remove_nans=True, be=be)
         mask = compute_mask(
-            s1, s2, GLOBAL_CONSTRAINT_CODE[global_constraint],
-            sakoe_chiba_radius, itakura_max_slope
+            s1,
+            s2,
+            GLOBAL_CONSTRAINT_CODE[global_constraint],
+            sakoe_chiba_radius,
+            itakura_max_slope,
+            be=be,
         )
-        dist_mat = pairwise_distances(s1, s2, metric=metric, **kwds)
+        dist_mat = be.pairwise_distances(s1, s2, metric=metric, **kwds)
 
-    acc_cost_mat = njit_accumulated_matrix_from_dist_matrix(dist_mat, mask)
-    path = _return_path(acc_cost_mat)
+    if be.is_numpy:
+        acc_cost_mat = njit_accumulated_matrix_from_dist_matrix(dist_mat, mask)
+        path = _njit_return_path(acc_cost_mat)
+    else:
+        dist_mat = be.array(dist_mat)
+        acc_cost_mat = accumulated_matrix_from_dist_matrix(dist_mat, mask, be=be)
+        path = _return_path(acc_cost_mat, be=be)
     return path, acc_cost_mat[-1, -1]
 
 
-def dtw(s1, s2, global_constraint=None, sakoe_chiba_radius=None,
-        itakura_max_slope=None):
+def dtw(
+    s1,
+    s2,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    be=None,
+):
     r"""Compute Dynamic Time Warping (DTW) similarity measure between
     (possibly multidimensional) time series and return it.
 
     DTW is computed as the Euclidean distance between aligned time series,
     i.e., if :math:`\pi` is the optimal alignment path:
 
     .. math::
@@ -433,14 +612,17 @@
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
 
+    be : Backend object or string or None
+        Backend.
+
     Returns
     -------
     float
         Similarity score
 
     Examples
     --------
@@ -457,30 +639,37 @@
     References
     ----------
     .. [1] H. Sakoe, S. Chiba, "Dynamic programming algorithm optimization for
            spoken word recognition," IEEE Transactions on Acoustics, Speech and
            Signal Processing, vol. 26(1), pp. 43--49, 1978.
 
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
 
     if len(s1) == 0 or len(s2) == 0:
         raise ValueError(
-            "One of the input time series contains only nans or has zero length.")
+            "One of the input time series contains only nans or has zero length."
+        )
 
-    if s1.shape[1] != s2.shape[1]:
+    if be.shape(s1)[1] != be.shape(s2)[1]:
         raise ValueError("All input time series must have the same feature size.")
 
     mask = compute_mask(
-        s1, s2,
+        s1,
+        s2,
         GLOBAL_CONSTRAINT_CODE[global_constraint],
         sakoe_chiba_radius=sakoe_chiba_radius,
-        itakura_max_slope=itakura_max_slope)
-    return njit_dtw(s1, s2, mask=mask)
+        itakura_max_slope=itakura_max_slope,
+        be=be,
+    )
+    if be.is_numpy:
+        return _njit_dtw(s1, s2, mask=mask)
+    return _dtw(s1, s2, mask=mask, be=be)
 
 
 def _max_steps(i, j, max_length, length_1, length_2):
     """Maximum number of steps required in a L-DTW process to reach a given
     cell.
 
     Parameters
@@ -506,65 +695,66 @@
         Number of steps
     """
     candidate_1 = i + j
     candidate_2 = max_length - max(length_1 - i - 1, length_2 - j - 1)
     return min(candidate_1, candidate_2)
 
 
-def _limited_warping_length_cost(s1, s2, max_length):
+def _limited_warping_length_cost(s1, s2, max_length, be=None):
     r"""Compute accumulated scores necessary fo L-DTW.
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-
     max_length : int
         Maximum allowed warping path length. Should be an integer between
         XXX and YYY.  # TODO
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     dict
         Accumulated scores. This dict associates (i, j) pairs (keys) to
         dictionnaries with desired length as key and associated score as value.
     """
+    be = instantiate_backend(be, s1)
     dict_costs = {}
     for i in range(s1.shape[0]):
         for j in range(s2.shape[0]):
             dict_costs[i, j] = {}
 
     # Init
-    dict_costs[0, 0][0] = _local_squared_dist(s1[0], s2[0])
+    dict_costs[0, 0][0] = _local_squared_dist(s1[0], s2[0], be=be)
     for i in range(1, s1.shape[0]):
         pred = dict_costs[i - 1, 0][i - 1]
-        dict_costs[i, 0][i] = pred + _local_squared_dist(s1[i], s2[0])
+        dict_costs[i, 0][i] = pred + _local_squared_dist(s1[i], s2[0], be=be)
     for j in range(1, s2.shape[0]):
         pred = dict_costs[0, j - 1][j - 1]
-        dict_costs[0, j][j] = pred + _local_squared_dist(s1[0], s2[j])
+        dict_costs[0, j][j] = pred + _local_squared_dist(s1[0], s2[j], be=be)
 
     # Main loop
     for i in range(1, s1.shape[0]):
         for j in range(1, s2.shape[0]):
             min_s = max(i, j)
             max_s = _max_steps(i, j, max_length - 1, s1.shape[0], s2.shape[0])
             for s in range(min_s, max_s + 1):
-                dict_costs[i, j][s] = _local_squared_dist(s1[i], s2[j])
+                dict_costs[i, j][s] = _local_squared_dist(s1[i], s2[j], be=be)
                 dict_costs[i, j][s] += min(
-                    dict_costs[i, j - 1].get(s - 1, numpy.inf),
-                    dict_costs[i - 1, j].get(s - 1, numpy.inf),
-                    dict_costs[i - 1, j - 1].get(s - 1, numpy.inf)
+                    dict_costs[i, j - 1].get(s - 1, be.inf),
+                    dict_costs[i - 1, j].get(s - 1, be.inf),
+                    dict_costs[i - 1, j - 1].get(s - 1, be.inf),
                 )
     return dict_costs
 
 
-def dtw_limited_warping_length(s1, s2, max_length):
+def dtw_limited_warping_length(s1, s2, max_length, be=None):
     r"""Compute Dynamic Time Warping (DTW) similarity measure between
     (possibly multidimensional) time series under an upper bound constraint on
     the resulting path length and return the similarity cost.
 
     DTW is computed as the Euclidean distance between aligned time series,
     i.e., if :math:`\pi` is the optimal alignment path:
 
@@ -580,24 +770,24 @@
     Both bariants are
     discussed in more details in our :ref:`dedicated user-guide page <dtw>`
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-
     max_length : int
         Maximum allowed warping path length.
         If greater than len(s1) + len(s2), then it is equivalent to
         unconstrained DTW.
         If lower than max(len(s1), len(s2)), no path can be found and a
         ValueError is raised.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Similarity score
 
     Examples
@@ -618,55 +808,62 @@
     .. [1] H. Sakoe, S. Chiba, "Dynamic programming algorithm optimization for
            spoken word recognition," IEEE Transactions on Acoustics, Speech and
            Signal Processing, vol. 26(1), pp. 43--49, 1978.
     .. [2] Z. Zhang, R. Tavenard, A. Bailly, X. Tang, P. Tang, T. Corpetti
            Dynamic time warping under limited warping path length.
            Information Sciences, vol. 393, pp. 91--107, 2017.
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
 
     if max_length < max(s1.shape[0], s2.shape[0]):
-        raise ValueError("Cannot find a path of length {} to align given "
-                         "time series.".format(max_length))
+        raise ValueError(
+            "Cannot find a path of length {} to align given "
+            "time series.".format(max_length)
+        )
 
-    accumulated_costs = _limited_warping_length_cost(s1, s2, max_length)
+    accumulated_costs = _limited_warping_length_cost(s1, s2, max_length, be=be)
     idx_pair = (s1.shape[0] - 1, s2.shape[0] - 1)
     optimal_cost = min(accumulated_costs[idx_pair].values())
-    return numpy.sqrt(optimal_cost)
+    return be.sqrt(optimal_cost)
 
 
-def _return_path_limited_warping_length(accum_costs, target_indices,
-                                        optimal_length):
+def _return_path_limited_warping_length(
+    accum_costs, target_indices, optimal_length, be=None
+):
+    be = instantiate_backend(be, accum_costs)
     path = [target_indices]
     cur_length = optimal_length
     while path[-1] != (0, 0):
         i, j = path[-1]
         if i == 0:
             path.append((0, j - 1))
         elif j == 0:
             path.append((i - 1, 0))
         else:
-            arr = numpy.array(
-                [accum_costs[i - 1, j - 1].get(cur_length - 1, numpy.inf),
-                 accum_costs[i - 1, j].get(cur_length - 1, numpy.inf),
-                 accum_costs[i, j - 1].get(cur_length - 1, numpy.inf)]
+            arr = be.array(
+                [
+                    accum_costs[i - 1, j - 1].get(cur_length - 1, be.inf),
+                    accum_costs[i - 1, j].get(cur_length - 1, be.inf),
+                    accum_costs[i, j - 1].get(cur_length - 1, be.inf),
+                ]
             )
-            argmin = numpy.argmin(arr)
+            argmin = be.argmin(arr)
             if argmin == 0:
                 path.append((i - 1, j - 1))
             elif argmin == 1:
                 path.append((i - 1, j))
             else:
                 path.append((i, j - 1))
             cur_length -= 1
     return path[::-1]
 
 
-def dtw_path_limited_warping_length(s1, s2, max_length):
+def dtw_path_limited_warping_length(s1, s2, max_length, be=None):
     r"""Compute Dynamic Time Warping (DTW) similarity measure between
     (possibly multidimensional) time series under an upper bound constraint on
     the resulting path length and return the path as well as the similarity
     cost.
 
     DTW is computed as the Euclidean distance between aligned time series,
     i.e., if :math:`\pi` is the optimal alignment path:
@@ -683,30 +880,29 @@
     Both variants are
     discussed in more details in our :ref:`dedicated user-guide page <dtw>`
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-
     max_length : int
         Maximum allowed warping path length.
         If greater than len(s1) + len(s2), then it is equivalent to
         unconstrained DTW.
         If lower than max(len(s1), len(s2)), no path can be found and a
         ValueError is raised.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     list of integer pairs
         Optimal path
-
     float
         Similarity score
 
     Examples
     --------
     >>> path, cost = dtw_path_limited_warping_length([1, 2, 3],
     ...                                              [1., 2., 2., 3.], 5)
@@ -732,106 +928,163 @@
     .. [1] H. Sakoe, S. Chiba, "Dynamic programming algorithm optimization for
            spoken word recognition," IEEE Transactions on Acoustics, Speech and
            Signal Processing, vol. 26(1), pp. 43--49, 1978.
     .. [2] Z. Zhang, R. Tavenard, A. Bailly, X. Tang, P. Tang, T. Corpetti
            Dynamic time warping under limited warping path length.
            Information Sciences, vol. 393, pp. 91--107, 2017.
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
 
     if max_length < max(s1.shape[0], s2.shape[0]):
-        raise ValueError("Cannot find a path of length {} to align given "
-                         "time series.".format(max_length))
+        raise ValueError(
+            "Cannot find a path of length {} to align given "
+            "time series.".format(max_length)
+        )
 
-    accumulated_costs = _limited_warping_length_cost(s1, s2, max_length)
+    accumulated_costs = _limited_warping_length_cost(s1, s2, max_length, be=be)
     idx_pair = (s1.shape[0] - 1, s2.shape[0] - 1)
     optimal_length = -1
-    optimal_cost = numpy.inf
+    optimal_cost = be.inf
     for k, v in accumulated_costs[idx_pair].items():
         if v < optimal_cost:
             optimal_cost = v
             optimal_length = k
-    path = _return_path_limited_warping_length(accumulated_costs,
-                                               idx_pair,
-                                               optimal_length)
-    return path, numpy.sqrt(optimal_cost)
+    path = _return_path_limited_warping_length(
+        accumulated_costs, idx_pair, optimal_length, be=be
+    )
+    return path, be.sqrt(optimal_cost)
 
 
 @njit()
-def _subsequence_cost_matrix(subseq, longseq):
+def _njit_subsequence_cost_matrix(subseq, longseq):
     l1 = subseq.shape[0]
     l2 = longseq.shape[0]
     cum_sum = numpy.full((l1 + 1, l2 + 1), numpy.inf)
-    cum_sum[0, :] = 0.
+    cum_sum[0, :] = 0.0
+
+    for i in range(l1):
+        for j in range(l2):
+            cum_sum[i + 1, j + 1] = _njit_local_squared_dist(subseq[i], longseq[j])
+            cum_sum[i + 1, j + 1] += min(
+                cum_sum[i, j + 1], cum_sum[i + 1, j], cum_sum[i, j]
+            )
+    return cum_sum[1:, 1:]
+
+
+def _subsequence_cost_matrix(subseq, longseq, be=None):
+    be = instantiate_backend(be, subseq)
+    l1 = subseq.shape[0]
+    l2 = longseq.shape[0]
+    cum_sum = be.full((l1 + 1, l2 + 1), be.inf)
+    cum_sum[0, :] = 0.0
 
     for i in range(l1):
         for j in range(l2):
-            cum_sum[i + 1, j + 1] = _local_squared_dist(subseq[i], longseq[j])
-            cum_sum[i + 1, j + 1] += min(cum_sum[i, j + 1],
-                                         cum_sum[i + 1, j],
-                                         cum_sum[i, j])
+            cum_sum[i + 1, j + 1] = _local_squared_dist(subseq[i], longseq[j], be=be)
+            cum_sum[i + 1, j + 1] += min(
+                cum_sum[i, j + 1], cum_sum[i + 1, j], cum_sum[i, j]
+            )
     return cum_sum[1:, 1:]
 
 
-def subsequence_cost_matrix(subseq, longseq):
+def subsequence_cost_matrix(subseq, longseq, be=None):
     """Compute the accumulated cost matrix score between a subsequence and
     a reference time series.
 
     Parameters
     ----------
     subseq : array, shape = (sz1, d)
         Subsequence time series.
-
     longseq : array, shape = (sz2, d)
         Reference time series
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     mat : array, shape = (sz1, sz2)
         Accumulated cost matrix.
     """
-    return _subsequence_cost_matrix(subseq, longseq)
+    be = instantiate_backend(be, subseq)
+    if be.is_numpy:
+        return _njit_subsequence_cost_matrix(subseq, longseq)
+    return _subsequence_cost_matrix(subseq, longseq, be=be)
 
 
 @njit()
-def _subsequence_path(acc_cost_mat, idx_path_end):
+def _njit_subsequence_path(acc_cost_mat, idx_path_end):
     sz1, sz2 = acc_cost_mat.shape
     path = [(sz1 - 1, idx_path_end)]
     while path[-1][0] != 0:
         i, j = path[-1]
         if i == 0:
             path.append((0, j - 1))
         elif j == 0:
             path.append((i - 1, 0))
         else:
-            arr = numpy.array([acc_cost_mat[i - 1][j - 1],
-                               acc_cost_mat[i - 1][j],
-                               acc_cost_mat[i][j - 1]])
+            arr = numpy.array(
+                [
+                    acc_cost_mat[i - 1][j - 1],
+                    acc_cost_mat[i - 1][j],
+                    acc_cost_mat[i][j - 1],
+                ]
+            )
             argmin = numpy.argmin(arr)
             if argmin == 0:
                 path.append((i - 1, j - 1))
             elif argmin == 1:
                 path.append((i - 1, j))
             else:
                 path.append((i, j - 1))
     return path[::-1]
 
 
-def subsequence_path(acc_cost_mat, idx_path_end):
+def _subsequence_path(acc_cost_mat, idx_path_end, be=None):
+    be = instantiate_backend(be, acc_cost_mat)
+    sz1, sz2 = acc_cost_mat.shape
+    path = [(sz1 - 1, idx_path_end)]
+    while path[-1][0] != 0:
+        i, j = path[-1]
+        if i == 0:
+            path.append((0, j - 1))
+        elif j == 0:
+            path.append((i - 1, 0))
+        else:
+            arr = be.array(
+                [
+                    acc_cost_mat[i - 1][j - 1],
+                    acc_cost_mat[i - 1][j],
+                    acc_cost_mat[i][j - 1],
+                ]
+            )
+            argmin = be.argmin(arr)
+            if argmin == 0:
+                path.append((i - 1, j - 1))
+            elif argmin == 1:
+                path.append((i - 1, j))
+            else:
+                path.append((i, j - 1))
+    return path[::-1]
+
+
+def subsequence_path(acc_cost_mat, idx_path_end, be=None):
     r"""Compute the optimal path through a accumulated cost matrix given the
     endpoint of the sequence.
 
     Parameters
     ----------
     acc_cost_mat: array, shape = (sz1, sz2)
         The accumulated cost matrix comparing subsequence from a longer
         sequence.
     idx_path_end: int
         The end position of the matched subsequence in the longer sequence.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     path: list of tuples of integer pairs
         Matching path represented as a list of index pairs. In each pair, the
         first index corresponds to `subseq` and the second one corresponds to
         `longseq`. The startpoint of the Path is :math:`P_0 = (0, ?)` and it
@@ -850,18 +1103,21 @@
 
     See Also
     --------
     dtw_subsequence_path : Get the similarity score for DTW
     subsequence_cost_matrix: Calculate the required cost matrix
 
     """
-    return _subsequence_path(acc_cost_mat, idx_path_end)
+    be = instantiate_backend(be, acc_cost_mat)
+    if be.is_numpy:
+        return _njit_subsequence_path(acc_cost_mat, idx_path_end)
+    return _subsequence_path(acc_cost_mat, idx_path_end, be=be)
 
 
-def dtw_subsequence_path(subseq, longseq):
+def dtw_subsequence_path(subseq, longseq, be=None):
     r"""Compute sub-sequence Dynamic Time Warping (DTW) similarity measure
     between a (possibly multidimensional) query and a long time series and
     return both the path and the similarity.
 
     DTW is computed as the Euclidean distance between aligned time series,
     i.e., if :math:`\pi` is the alignment path:
 
@@ -880,14 +1136,16 @@
 
     Parameters
     ----------
     subseq : array, shape = (sz1, d)
         A query time series.
     longseq : array, shape = (sz2, d)
         A reference (supposed to be longer than `subseq`) time series.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     list of integer pairs
         Matching path represented as a list of index pairs. In each pair, the
         first index corresponds to `subseq` and the second one corresponds to
         `longseq`.
@@ -904,77 +1162,127 @@
 
     See Also
     --------
     dtw : Get the similarity score for DTW
     subsequence_cost_matrix: Calculate the required cost matrix
     subsequence_path: Calculate a matching path manually
     """
-    subseq = to_time_series(subseq)
-    longseq = to_time_series(longseq)
-    acc_cost_mat = subsequence_cost_matrix(subseq=subseq,
-                                           longseq=longseq)
-    global_optimal_match = numpy.argmin(acc_cost_mat[-1, :])
-    path = subsequence_path(acc_cost_mat, global_optimal_match)
-    return path, numpy.sqrt(acc_cost_mat[-1, :][global_optimal_match])
+    be = instantiate_backend(be, subseq)
+    subseq = to_time_series(subseq, be=be)
+    longseq = to_time_series(longseq, be=be)
+    acc_cost_mat = subsequence_cost_matrix(subseq=subseq, longseq=longseq, be=be)
+    global_optimal_match = be.argmin(acc_cost_mat[-1, :])
+    path = subsequence_path(acc_cost_mat, global_optimal_match, be=be)
+    return path, be.sqrt(acc_cost_mat[-1, :][global_optimal_match])
 
 
 @njit()
-def sakoe_chiba_mask(sz1, sz2, radius=1):
+def njit_sakoe_chiba_mask(sz1, sz2, radius=1):
     """Compute the Sakoe-Chiba mask.
 
     Parameters
     ----------
     sz1 : int
         The size of the first time series
-
     sz2 : int
         The size of the second time series.
-
     radius : int
         The radius of the band.
 
     Returns
     -------
     mask : array, shape = (sz1, sz2)
         Sakoe-Chiba mask.
 
     Examples
     --------
-    >>> sakoe_chiba_mask(4, 4, 1)
+    >>> njit_sakoe_chiba_mask(4, 4, 1)
     array([[ 0.,  0., inf, inf],
            [ 0.,  0.,  0., inf],
            [inf,  0.,  0.,  0.],
            [inf, inf,  0.,  0.]])
-    >>> sakoe_chiba_mask(7, 3, 1)
+    >>> njit_sakoe_chiba_mask(7, 3, 1)
     array([[ 0.,  0., inf],
            [ 0.,  0.,  0.],
            [ 0.,  0.,  0.],
            [ 0.,  0.,  0.],
            [ 0.,  0.,  0.],
            [ 0.,  0.,  0.],
            [inf,  0.,  0.]])
     """
     mask = numpy.full((sz1, sz2), numpy.inf)
     if sz1 > sz2:
         width = sz1 - sz2 + radius
         for i in prange(sz2):
             lower = max(0, i - radius)
             upper = min(sz1, i + width) + 1
-            mask[lower:upper, i] = 0.
+            mask[lower:upper, i] = 0.0
     else:
         width = sz2 - sz1 + radius
         for i in prange(sz1):
             lower = max(0, i - radius)
             upper = min(sz2, i + width) + 1
-            mask[i, lower:upper] = 0.
+            mask[i, lower:upper] = 0.0
+    return mask
+
+
+def sakoe_chiba_mask(sz1, sz2, radius=1, be=None):
+    """Compute the Sakoe-Chiba mask.
+
+    Parameters
+    ----------
+    sz1 : int
+        The size of the first time series
+    sz2 : int
+        The size of the second time series.
+    radius : int
+        The radius of the band.
+    be : Backend object or string or None
+        Backend.
+
+    Returns
+    -------
+    mask : array, shape = (sz1, sz2)
+        Sakoe-Chiba mask.
+
+    Examples
+    --------
+    >>> sakoe_chiba_mask(4, 4, 1)
+    array([[ 0.,  0., inf, inf],
+           [ 0.,  0.,  0., inf],
+           [inf,  0.,  0.,  0.],
+           [inf, inf,  0.,  0.]])
+    >>> sakoe_chiba_mask(7, 3, 1)
+    array([[ 0.,  0., inf],
+           [ 0.,  0.,  0.],
+           [ 0.,  0.,  0.],
+           [ 0.,  0.,  0.],
+           [ 0.,  0.,  0.],
+           [ 0.,  0.,  0.],
+           [inf,  0.,  0.]])
+    """
+    be = instantiate_backend(be, "numpy")
+    mask = be.full((sz1, sz2), be.inf)
+    if sz1 > sz2:
+        width = sz1 - sz2 + radius
+        for i in range(sz2):
+            lower = max(0, i - radius)
+            upper = min(sz1, i + width) + 1
+            mask[lower:upper, i] = 0.0
+    else:
+        width = sz2 - sz1 + radius
+        for i in range(sz1):
+            lower = max(0, i - radius)
+            upper = min(sz2, i + width) + 1
+            mask[i, lower:upper] = 0.0
     return mask
 
 
 @njit()
-def _njit_itakura_mask(sz1, sz2, max_slope=2.):
+def _njit_itakura_mask(sz1, sz2, max_slope=2.0):
     """Compute the Itakura mask without checking that the constraints
     are feasible. In most cases, you should use itakura_mask instead.
 
     Parameters
     ----------
     sz1 : int
         The size of the first time series
@@ -987,56 +1295,104 @@
 
     Returns
     -------
     mask : array, shape = (sz1, sz2)
         Itakura mask.
     """
     min_slope = 1 / float(max_slope)
-    max_slope *= (float(sz1) / float(sz2))
-    min_slope *= (float(sz1) / float(sz2))
+    max_slope *= float(sz1) / float(sz2)
+    min_slope *= float(sz1) / float(sz2)
 
     lower_bound = numpy.empty((2, sz2))
     lower_bound[0] = min_slope * numpy.arange(sz2)
-    lower_bound[1] = ((sz1 - 1) - max_slope * (sz2 - 1)
-                      + max_slope * numpy.arange(sz2))
+    lower_bound[1] = (sz1 - 1) - max_slope * (sz2 - 1) + max_slope * numpy.arange(sz2)
     lower_bound_ = numpy.empty(sz2)
     for i in prange(sz2):
-        lower_bound_[i] = max(round(lower_bound[0, i], 2),
-                              round(lower_bound[1, i], 2))
+        lower_bound_[i] = max(round(lower_bound[0, i], 2), round(lower_bound[1, i], 2))
     lower_bound_ = numpy.ceil(lower_bound_)
 
     upper_bound = numpy.empty((2, sz2))
     upper_bound[0] = max_slope * numpy.arange(sz2)
-    upper_bound[1] = ((sz1 - 1) - min_slope * (sz2 - 1)
-                      + min_slope * numpy.arange(sz2))
+    upper_bound[1] = (sz1 - 1) - min_slope * (sz2 - 1) + min_slope * numpy.arange(sz2)
     upper_bound_ = numpy.empty(sz2)
     for i in prange(sz2):
-        upper_bound_[i] = min(round(upper_bound[0, i], 2),
-                              round(upper_bound[1, i], 2))
+        upper_bound_[i] = min(round(upper_bound[0, i], 2), round(upper_bound[1, i], 2))
     upper_bound_ = numpy.floor(upper_bound_ + 1)
 
     mask = numpy.full((sz1, sz2), numpy.inf)
     for i in prange(sz2):
-        mask[int(lower_bound_[i]):int(upper_bound_[i]), i] = 0.
+        mask[int(lower_bound_[i]) : int(upper_bound_[i]), i] = 0.0
     return mask
 
 
-def itakura_mask(sz1, sz2, max_slope=2.):
-    """Compute the Itakura mask.
+def _itakura_mask(sz1, sz2, max_slope=2.0, be=None):
+    """Compute the Itakura mask without checking that the constraints
+    are feasible. In most cases, you should use itakura_mask instead.
 
     Parameters
     ----------
     sz1 : int
         The size of the first time series
-
     sz2 : int
         The size of the second time series.
+    max_slope : float (default = 2)
+        The maximum slope of the parallelogram.
+    be : Backend object or string or None
+        Backend.
 
+    Returns
+    -------
+    mask : array, shape = (sz1, sz2)
+        Itakura mask.
+    """
+    min_slope = 1 / float(max_slope)
+    max_slope *= float(sz1) / float(sz2)
+    min_slope *= float(sz1) / float(sz2)
+
+    lower_bound = be.empty((2, sz2))
+    lower_bound[0] = min_slope * be.arange(sz2)
+    lower_bound[1] = (sz1 - 1) - max_slope * (sz2 - 1) + max_slope * be.arange(sz2)
+    lower_bound_ = be.empty(sz2)
+    for i in range(sz2):
+        lower_bound_[i] = max(
+            be.round(lower_bound[0, i], decimals=2),
+            be.round(lower_bound[1, i], decimals=2),
+        )
+    lower_bound_ = be.ceil(lower_bound_)
+
+    upper_bound = be.empty((2, sz2))
+    upper_bound[0] = max_slope * be.arange(sz2)
+    upper_bound[1] = (sz1 - 1) - min_slope * (sz2 - 1) + min_slope * be.arange(sz2)
+    upper_bound_ = be.empty(sz2)
+    for i in range(sz2):
+        upper_bound_[i] = min(
+            be.round(upper_bound[0, i], decimals=2),
+            be.round(upper_bound[1, i], decimals=2),
+        )
+    upper_bound_ = be.floor(upper_bound_ + 1)
+
+    mask = be.full((sz1, sz2), be.inf)
+    for i in range(sz2):
+        mask[int(lower_bound_[i]) : int(upper_bound_[i]), i] = 0.0
+    return mask
+
+
+def itakura_mask(sz1, sz2, max_slope=2.0, be=None):
+    """Compute the Itakura mask.
+
+    Parameters
+    ----------
+    sz1 : int
+        The size of the first time series
+    sz2 : int
+        The size of the second time series.
     max_slope : float (default = 2)
         The maximum slope of the parallelogram.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     mask : array, shape = (sz1, sz2)
         Itakura mask.
 
     Examples
@@ -1045,122 +1401,151 @@
     array([[ 0., inf, inf, inf, inf, inf],
            [inf,  0.,  0., inf, inf, inf],
            [inf,  0.,  0.,  0., inf, inf],
            [inf, inf,  0.,  0.,  0., inf],
            [inf, inf, inf,  0.,  0., inf],
            [inf, inf, inf, inf, inf,  0.]])
     """
-    mask = _njit_itakura_mask(sz1, sz2, max_slope=max_slope)
+    be = instantiate_backend(be, "numpy")
+
+    if be.is_numpy:
+        mask = _njit_itakura_mask(sz1, sz2, max_slope=max_slope)
+    else:
+        mask = _itakura_mask(sz1, sz2, max_slope=max_slope, be=be)
 
     # Post-check
     raise_warning = False
-    for i in prange(sz1):
-        if not numpy.any(numpy.isfinite(mask[i])):
+    for i in range(sz1):
+        if not be.any(be.isfinite(mask[i])):
             raise_warning = True
             break
     if not raise_warning:
-        for j in prange(sz2):
-            if not numpy.any(numpy.isfinite(mask[:, j])):
+        for j in range(sz2):
+            if not be.any(be.isfinite(mask[:, j])):
                 raise_warning = True
                 break
     if raise_warning:
-        warnings.warn("'itakura_max_slope' constraint is unfeasible "
-                      "(ie. leads to no admissible path) for the "
-                      "provided time series sizes",
-                      RuntimeWarning)
+        warnings.warn(
+            "'itakura_max_slope' constraint is unfeasible "
+            "(ie. leads to no admissible path) for the "
+            "provided time series sizes",
+            RuntimeWarning,
+        )
 
     return mask
 
 
-def compute_mask(s1, s2, global_constraint=0,
-                 sakoe_chiba_radius=None, itakura_max_slope=None):
+def compute_mask(
+    s1,
+    s2,
+    global_constraint=0,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    be=None,
+):
     """Compute the mask (region constraint).
 
     Parameters
     ----------
     s1 : array
         A time series or integer.
-
     s2: array
         Another time series or integer.
-
     global_constraint : {0, 1, 2} (default: 0)
         Global constraint to restrict admissible paths for DTW:
         - "itakura" if 1
         - "sakoe_chiba" if 2
         - no constraint otherwise
-
     sakoe_chiba_radius : int or None (default: None)
         Radius to be used for Sakoe-Chiba band global constraint.
         If None and `global_constraint` is set to 2 (sakoe-chiba), a radius of
         1 is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     itakura_max_slope : float or None (default: None)
         Maximum slope for the Itakura parallelogram constraint.
         If None and `global_constraint` is set to 1 (itakura), a maximum slope
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     mask : array
         Constraint region.
     """
+    be = instantiate_backend(be, s1)
     # The output mask will be of shape (sz1, sz2)
     if isinstance(s1, int) and isinstance(s2, int):
         sz1, sz2 = s1, s2
     else:
-        sz1 = s1.shape[0]
-        sz2 = s2.shape[0]
-    if (global_constraint == 0 and sakoe_chiba_radius is not None
-            and itakura_max_slope is not None):
-        raise RuntimeWarning("global_constraint is not set for DTW, but both "
-                             "sakoe_chiba_radius and itakura_max_slope are "
-                             "set, hence global_constraint cannot be inferred "
-                             "and no global constraint will be used.")
-    if global_constraint == 2 or (global_constraint == 0
-                                  and sakoe_chiba_radius is not None):
+        sz1 = be.shape(s1)[0]
+        sz2 = be.shape(s2)[0]
+    if (
+        global_constraint == 0
+        and sakoe_chiba_radius is not None
+        and itakura_max_slope is not None
+    ):
+        raise RuntimeWarning(
+            "global_constraint is not set for DTW, but both "
+            "sakoe_chiba_radius and itakura_max_slope are "
+            "set, hence global_constraint cannot be inferred "
+            "and no global constraint will be used."
+        )
+    if global_constraint == 2 or (
+        global_constraint == 0 and sakoe_chiba_radius is not None
+    ):
         if sakoe_chiba_radius is None:
             sakoe_chiba_radius = 1
-        mask = sakoe_chiba_mask(sz1, sz2, radius=sakoe_chiba_radius)
-    elif global_constraint == 1 or (global_constraint == 0
-                                    and itakura_max_slope is not None):
+        if be.is_numpy:
+            mask = njit_sakoe_chiba_mask(sz1, sz2, radius=sakoe_chiba_radius)
+        else:
+            mask = sakoe_chiba_mask(sz1, sz2, radius=sakoe_chiba_radius, be=be)
+    elif global_constraint == 1 or (
+        global_constraint == 0 and itakura_max_slope is not None
+    ):
         if itakura_max_slope is None:
-            itakura_max_slope = 2.
-        mask = itakura_mask(sz1, sz2, max_slope=itakura_max_slope)
+            itakura_max_slope = 2.0
+        mask = itakura_mask(sz1, sz2, max_slope=itakura_max_slope, be=be)
     else:
-        mask = numpy.zeros((sz1, sz2))
+        mask = be.zeros((sz1, sz2))
     return mask
 
 
-def cdist_dtw(dataset1, dataset2=None, global_constraint=None,
-              sakoe_chiba_radius=None, itakura_max_slope=None, n_jobs=None,
-              verbose=0):
+def cdist_dtw(
+    dataset1,
+    dataset2=None,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    n_jobs=None,
+    verbose=0,
+    be=None,
+):
     r"""Compute cross-similarity matrix using Dynamic Time Warping (DTW)
     similarity measure.
 
     DTW is computed as the Euclidean distance between aligned time series,
     i.e., if :math:`\pi` is the alignment path:
 
     .. math::
 
         DTW(X, Y) = \sqrt{\sum_{(i, j) \in \pi} \|X_{i} - Y_{j}\|^2}
 
     Note that this formula is still valid for the multivariate case.
 
-    It is not required that time series share the same size, but they 
+    It is not required that time series share the same size, but they
     must be the same dimension.
     DTW was originally presented in [1]_ and is
     discussed in more details in our :ref:`dedicated user-guide page <dtw>`.
 
     Parameters
     ----------
     dataset1 : array-like
@@ -1204,14 +1589,17 @@
         The verbosity level: if non zero, progress messages are printed.
         Above 50, the output is sent to stdout.
         The frequency of the messages increases with the verbosity level.
         If it more than 10, all iterations are reported.
         `Glossary <https://joblib.readthedocs.io/en/latest/parallel.html#parallel-reference-documentation>`__
         for more details.
 
+    be : Backend object or string or None
+        Backend.
+
     Returns
     -------
     cdist : numpy.ndarray
         Cross-similarity matrix
 
     Examples
     --------
@@ -1228,20 +1616,27 @@
 
     References
     ----------
     .. [1] H. Sakoe, S. Chiba, "Dynamic programming algorithm optimization for
            spoken word recognition," IEEE Transactions on Acoustics, Speech and
            Signal Processing, vol. 26(1), pp. 43--49, 1978.
     """  # noqa: E501
-    return _cdist_generic(dist_fun=dtw, dataset1=dataset1, dataset2=dataset2,
-                          n_jobs=n_jobs, verbose=verbose,
-                          compute_diagonal=False,
-                          global_constraint=global_constraint,
-                          sakoe_chiba_radius=sakoe_chiba_radius,
-                          itakura_max_slope=itakura_max_slope)
+    be = instantiate_backend(be, dataset1)
+    return _cdist_generic(
+        dist_fun=dtw,
+        dataset1=dataset1,
+        dataset2=dataset2,
+        n_jobs=n_jobs,
+        verbose=verbose,
+        compute_diagonal=False,
+        global_constraint=global_constraint,
+        sakoe_chiba_radius=sakoe_chiba_radius,
+        itakura_max_slope=itakura_max_slope,
+        be=be,
+    )
 
 
 def lb_keogh(ts_query, ts_candidate=None, radius=1, envelope_candidate=None):
     r"""Compute LB_Keogh.
 
     LB_Keogh was originally presented in [1]_.
 
@@ -1297,30 +1692,33 @@
     .. [1] Keogh, E. Exact indexing of dynamic time warping. In International
        Conference on Very Large Data Bases, 2002. pp 406-417.
     """
     if ts_candidate is None:
         envelope_down, envelope_up = envelope_candidate
     else:
         ts_candidate = to_time_series(ts_candidate)
-        assert ts_candidate.shape[1] == 1, \
-            "LB_Keogh is available only for monodimensional time series"
+        assert (
+            ts_candidate.shape[1] == 1
+        ), "LB_Keogh is available only for monodimensional time series"
         envelope_down, envelope_up = lb_envelope(ts_candidate, radius)
     ts_query = to_time_series(ts_query)
-    assert ts_query.shape[1] == 1, \
-        "LB_Keogh is available only for monodimensional time series"
+    assert (
+        ts_query.shape[1] == 1
+    ), "LB_Keogh is available only for monodimensional time series"
     indices_up = ts_query[:, 0] > envelope_up[:, 0]
     indices_down = ts_query[:, 0] < envelope_down[:, 0]
-    return numpy.sqrt(numpy.linalg.norm(ts_query[indices_up, 0] -
-                                        envelope_up[indices_up, 0]) ** 2 +
-                      numpy.linalg.norm(ts_query[indices_down, 0] -
-                                        envelope_down[indices_down, 0]) ** 2)
+    return numpy.sqrt(
+        numpy.linalg.norm(ts_query[indices_up, 0] - envelope_up[indices_up, 0]) ** 2
+        + numpy.linalg.norm(ts_query[indices_down, 0] - envelope_down[indices_down, 0])
+        ** 2
+    )
 
 
 @njit()
-def njit_lb_envelope(time_series, radius):
+def _njit_lb_envelope(time_series, radius):
     sz, d = time_series.shape
     enveloppe_up = numpy.empty((sz, d))
     enveloppe_down = numpy.empty((sz, d))
 
     for i in prange(sz):
         min_idx = i - radius
         max_idx = i + radius + 1
@@ -1331,28 +1729,50 @@
         for di in prange(d):
             enveloppe_down[i, di] = numpy.min(time_series[min_idx:max_idx, di])
             enveloppe_up[i, di] = numpy.max(time_series[min_idx:max_idx, di])
 
     return enveloppe_down, enveloppe_up
 
 
-def lb_envelope(ts, radius=1):
+def _lb_envelope(time_series, radius, be=None):
+    be = instantiate_backend(be, time_series)
+    sz, d = be.shape(time_series)
+    enveloppe_up = be.empty((sz, d))
+    enveloppe_down = be.empty((sz, d))
+
+    for i in range(sz):
+        min_idx = i - radius
+        max_idx = i + radius + 1
+        if min_idx < 0:
+            min_idx = 0
+        if max_idx > sz:
+            max_idx = sz
+        for di in range(d):
+            enveloppe_down[i, di] = be.min(time_series[min_idx:max_idx, di])
+            enveloppe_up[i, di] = be.max(time_series[min_idx:max_idx, di])
+
+    return enveloppe_down, enveloppe_up
+
+
+def lb_envelope(ts, radius=1, be=None):
     r"""Compute time-series envelope as required by LB_Keogh.
 
     LB_Keogh was originally presented in [1]_.
 
     Parameters
     ----------
     ts : array-like
         Time-series for which the envelope should be computed.
     radius : int (default: 1)
         Radius to be used for the envelope generation (the envelope at time
         index i will be generated based on
         all observations from the time series at indices comprised between
         i-radius and i+radius).
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     array-like
         Lower-side of the envelope.
     array-like
         Upper-side of the envelope.
@@ -1379,15 +1799,18 @@
     lb_keogh : Compute LB_Keogh similarity
 
     References
     ----------
     .. [1] Keogh, E. Exact indexing of dynamic time warping. In International
        Conference on Very Large Data Bases, 2002. pp 406-417.
     """
-    return njit_lb_envelope(to_time_series(ts), radius=radius)
+    be = instantiate_backend(be, ts)
+    if be.is_numpy:
+        return _njit_lb_envelope(to_time_series(ts), radius=radius)
+    return _lb_envelope(to_time_series(ts, be=be), radius=radius, be=be)
 
 
 @njit(nogil=True)
 def njit_lcss_accumulated_matrix(s1, s2, eps, mask):
     """Compute the longest common subsequence similarity score between
     two time series.
 
@@ -1414,25 +1837,70 @@
     l1 = s1.shape[0]
     l2 = s2.shape[0]
     acc_cost_mat = numpy.full((l1 + 1, l2 + 1), 0)
 
     for i in range(1, l1 + 1):
         for j in range(1, l2 + 1):
             if numpy.isfinite(mask[i - 1, j - 1]):
-                if numpy.sqrt(_local_squared_dist(s1[i - 1], s2[j - 1])) <= eps:
+                if numpy.sqrt(_njit_local_squared_dist(s1[i - 1], s2[j - 1])) <= eps:
                     acc_cost_mat[i][j] = 1 + acc_cost_mat[i - 1][j - 1]
                 else:
-                    acc_cost_mat[i][j] = max(acc_cost_mat[i][j - 1],
-                                             acc_cost_mat[i - 1][j])
+                    acc_cost_mat[i][j] = max(
+                        acc_cost_mat[i][j - 1], acc_cost_mat[i - 1][j]
+                    )
+
+    return acc_cost_mat
+
+
+def lcss_accumulated_matrix(s1, s2, eps, mask, be=None):
+    """Compute the longest common subsequence similarity score between
+    two time series.
+
+    Parameters
+    ----------
+    s1 : array, shape = (sz1,)
+        First time series.
+    s2 : array, shape = (sz2,)
+        Second time series.
+    eps : float
+        Matching threshold.
+    mask : array, shape = (sz1, sz2)
+        Mask. Unconsidered cells must have infinite values.
+    be : Backend object or string or None
+        Backend.
+
+    Returns
+    -------
+    lcss_score : float
+        Longest Common Subsequence similarity score between both time series.
+    """
+    be = instantiate_backend(be, s1)
+    l1 = s1.shape[0]
+    l2 = s2.shape[0]
+    acc_cost_mat = be.full((l1 + 1, l2 + 1), 0)
+
+    for i in range(1, l1 + 1):
+        for j in range(1, l2 + 1):
+            if be.isfinite(mask[i - 1, j - 1]):
+                if be.is_numpy:
+                    squared_dist = _njit_local_squared_dist(s1[i - 1], s2[j - 1])
+                else:
+                    squared_dist = _local_squared_dist(s1[i - 1], s2[j - 1], be=be)
+                if be.sqrt(squared_dist) <= eps:
+                    acc_cost_mat[i][j] = 1 + acc_cost_mat[i - 1][j - 1]
+                else:
+                    acc_cost_mat[i][j] = max(
+                        acc_cost_mat[i][j - 1], acc_cost_mat[i - 1][j]
+                    )
 
     return acc_cost_mat
 
 
 @njit(nogil=True)
-def njit_lcss(s1, s2, eps, mask):
+def _njit_lcss(s1, s2, eps, mask):
     """Compute the longest common subsequence score between two time series.
 
     Parameters
     ----------
     s1 : array, shape = (sz1,)
         First time series.
 
@@ -1453,16 +1921,52 @@
     l1 = s1.shape[0]
     l2 = s2.shape[0]
     acc_cost_mat = njit_lcss_accumulated_matrix(s1, s2, eps, mask)
 
     return float(acc_cost_mat[-1][-1]) / min([l1, l2])
 
 
-def lcss(s1, s2, eps=1., global_constraint=None, sakoe_chiba_radius=None,
-         itakura_max_slope=None):
+def _lcss(s1, s2, eps, mask, be=None):
+    """Compute the longest common subsequence score between two time series.
+
+    Parameters
+    ----------
+    s1 : array, shape = (sz1,)
+        First time series.
+    s2 : array, shape = (sz2,)
+        Second time series
+    eps : float (default: 1.)
+        Maximum matching distance threshold.
+    mask : array, shape = (sz1, sz2)
+        Mask. Unconsidered cells must have infinite values.
+    be : Backend object or string or None
+        Backend.
+
+    Returns
+    -------
+    lcss_score : float
+        Longest Common Subsquence score between both time series.
+    """
+    be = instantiate_backend(be, s1)
+    l1 = s1.shape[0]
+    l2 = s2.shape[0]
+    acc_cost_mat = lcss_accumulated_matrix(s1, s2, eps, mask, be=be)
+
+    return float(acc_cost_mat[-1][-1]) / min([l1, l2])
+
+
+def lcss(
+    s1,
+    s2,
+    eps=1.0,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    be=None,
+):
     r"""Compute the Longest Common Subsequence (LCSS) similarity measure
     between (possibly multidimensional) time series and return the
     similarity.
 
     LCSS is computed by matching indexes that are met up until the eps
     threshold, so it leaves some points unmatched and focuses on the
     similar parts of two sequences. The matching can occur even if the
@@ -1483,43 +1987,40 @@
     ----
     Contrary to Dynamic Time Warping and variants, an LCSS path does not need to be contiguous.
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-
     eps : float (default: 1.)
         Maximum matching distance threshold.
-
     global_constraint : {"itakura", "sakoe_chiba"} or None (default: None)
         Global constraint to restrict admissible paths for LCSS.
-
     sakoe_chiba_radius : int or None (default: None)
         Radius to be used for Sakoe-Chiba band global constraint.
         If None and `global_constraint` is set to "sakoe_chiba", a radius of
         1 is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     itakura_max_slope : float or None (default: None)
         Maximum slope for the Itakura parallelogram constraint.
         If None and `global_constraint` is set to "itakura", a maximum slope
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Similarity score
 
     Examples
@@ -1541,62 +2042,116 @@
     ----------
     .. [1] M. Vlachos, D. Gunopoulos, and G. Kollios. 2002. "Discovering
             Similar Multidimensional Trajectories", In Proceedings of the
             18th International Conference on Data Engineering (ICDE '02).
             IEEE Computer Society, USA, 673.
 
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
 
     mask = compute_mask(
-        s1, s2,
+        s1,
+        s2,
         GLOBAL_CONSTRAINT_CODE[global_constraint],
         sakoe_chiba_radius=sakoe_chiba_radius,
-        itakura_max_slope=itakura_max_slope)
-
-    return njit_lcss(s1, s2, eps, mask)
+        itakura_max_slope=itakura_max_slope,
+        be=be,
+    )
+    if be.is_numpy:
+        return _njit_lcss(s1, s2, eps, mask)
+    return _lcss(s1, s2, eps, mask, be=be)
 
 
 @njit()
-def _return_lcss_path(s1, s2, eps, mask, acc_cost_mat, sz1, sz2):
+def _njit_return_lcss_path(s1, s2, eps, mask, acc_cost_mat, sz1, sz2):
     i, j = (sz1, sz2)
     path = []
 
     while i > 0 and j > 0:
         if numpy.isfinite(mask[i - 1, j - 1]):
-            if numpy.sqrt(_local_squared_dist(s1[i - 1], s2[j - 1])) <= eps:
+            if numpy.sqrt(_njit_local_squared_dist(s1[i - 1], s2[j - 1])) <= eps:
                 path.append((i - 1, j - 1))
                 i, j = (i - 1, j - 1)
-            elif acc_cost_mat[i - 1][j] > acc_cost_mat[i][j-1]:
+            elif acc_cost_mat[i - 1][j] > acc_cost_mat[i][j - 1]:
+                i = i - 1
+            else:
+                j = j - 1
+    return path[::-1]
+
+
+def _return_lcss_path(s1, s2, eps, mask, acc_cost_mat, sz1, sz2, be=None):
+    be = instantiate_backend(be, s1)
+    i, j = (sz1, sz2)
+    path = []
+
+    while i > 0 and j > 0:
+        if be.isfinite(mask[i - 1, j - 1]):
+            if be.is_numpy:
+                squared_dist = _njit_local_squared_dist(s1[i - 1], s2[j - 1])
+            else:
+                squared_dist = _local_squared_dist(s1[i - 1], s2[j - 1])
+            if be.sqrt(squared_dist) <= eps:
+                path.append((i - 1, j - 1))
+                i, j = (i - 1, j - 1)
+            elif acc_cost_mat[i - 1][j] > acc_cost_mat[i][j - 1]:
                 i = i - 1
             else:
                 j = j - 1
     return path[::-1]
 
 
 @njit()
-def _return_lcss_path_from_dist_matrix(dist_matrix, eps, mask, acc_cost_mat, sz1, sz2):
+def _njit_return_lcss_path_from_dist_matrix(
+    dist_matrix, eps, mask, acc_cost_mat, sz1, sz2
+):
     i, j = (sz1, sz2)
     path = []
 
     while i > 0 and j > 0:
         if numpy.isfinite(mask[i - 1, j - 1]):
             if dist_matrix[i - 1, j - 1] <= eps:
                 path.append((i - 1, j - 1))
                 i, j = (i - 1, j - 1)
-            elif acc_cost_mat[i - 1][j] > acc_cost_mat[i][j-1]:
+            elif acc_cost_mat[i - 1][j] > acc_cost_mat[i][j - 1]:
+                i = i - 1
+            else:
+                j = j - 1
+    return path[::-1]
+
+
+def _return_lcss_path_from_dist_matrix(
+    dist_matrix, eps, mask, acc_cost_mat, sz1, sz2, be=None
+):
+    be = instantiate_backend(be, dist_matrix)
+    i, j = (sz1, sz2)
+    path = []
+
+    while i > 0 and j > 0:
+        if be.isfinite(mask[i - 1, j - 1]):
+            if dist_matrix[i - 1, j - 1] <= eps:
+                path.append((i - 1, j - 1))
+                i, j = (i - 1, j - 1)
+            elif acc_cost_mat[i - 1][j] > acc_cost_mat[i][j - 1]:
                 i = i - 1
             else:
                 j = j - 1
     return path[::-1]
 
 
-def lcss_path(s1, s2, eps=1, global_constraint=None, sakoe_chiba_radius=None,
-              itakura_max_slope=None):
+def lcss_path(
+    s1,
+    s2,
+    eps=1,
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    be=None,
+):
     r"""Compute the Longest Common Subsequence (LCSS) similarity measure
     between (possibly multidimensional) time series and return both the
     path and the similarity.
 
     LCSS is computed by matching indexes that are met up until the eps
     threshold, so it leaves some points unmatched and focuses on the
     similar parts of two sequences. The matching can occur even if the
@@ -1618,43 +2173,40 @@
     ----
     Contrary to Dynamic Time Warping and variants, an LCSS path does not need to be contiguous.
 
     Parameters
     ----------
     s1
         A time series.
-
     s2
         Another time series.
-
     eps : float (default: 1.)
         Maximum matching distance threshold.
-
     global_constraint : {"itakura", "sakoe_chiba"} or None (default: None)
        Global constraint to restrict admissible paths for LCSS.
-
     sakoe_chiba_radius : int or None (default: None)
        Radius to be used for Sakoe-Chiba band global constraint.
        If None and `global_constraint` is set to "sakoe_chiba", a radius of
        1 is used.
        If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
        `global_constraint` is used to infer which constraint to use among the
        two. In this case, if `global_constraint` corresponds to no global
        constraint, a `RuntimeWarning` is raised and no global constraint is
        used.
-
     itakura_max_slope : float or None (default: None)
        Maximum slope for the Itakura parallelogram constraint.
        If None and `global_constraint` is set to "itakura", a maximum slope
        of 2. is used.
        If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
        `global_constraint` is used to infer which constraint to use among the
        two. In this case, if `global_constraint` corresponds to no global
        constraint, a `RuntimeWarning` is raised and no global constraint is
        used.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     list of integer pairs
         Matching path represented as a list of index pairs. In each pair, the
         first index corresponds to s1 and the second one corresponds to s2
 
@@ -1680,31 +2232,40 @@
     ----------
     .. [1] M. Vlachos, D. Gunopoulos, and G. Kollios. 2002. "Discovering
             Similar Multidimensional Trajectories", In Proceedings of the
             18th International Conference on Data Engineering (ICDE '02).
             IEEE Computer Society, USA, 673.
 
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
 
     mask = compute_mask(
-        s1, s2,
+        s1,
+        s2,
         GLOBAL_CONSTRAINT_CODE[global_constraint],
-        sakoe_chiba_radius, itakura_max_slope)
+        sakoe_chiba_radius,
+        itakura_max_slope,
+        be=be,
+    )
 
     l1 = s1.shape[0]
     l2 = s2.shape[0]
 
-    acc_cost_mat = njit_lcss_accumulated_matrix(s1, s2, eps, mask)
-    path = _return_lcss_path(s1, s2, eps, mask, acc_cost_mat, l1, l2)
+    if be.is_numpy:
+        acc_cost_mat = njit_lcss_accumulated_matrix(s1, s2, eps, mask)
+    else:
+        acc_cost_mat = lcss_accumulated_matrix(s1, s2, eps, mask, be=be)
+    path = _return_lcss_path(s1, s2, eps, mask, acc_cost_mat, l1, l2, be=be)
 
     return path, float(acc_cost_mat[-1][-1]) / min([l1, l2])
 
 
+@njit()
 def njit_lcss_accumulated_matrix_from_dist_matrix(dist_matrix, eps, mask):
     """Compute the accumulated cost matrix score between two time series using
     a precomputed distance matrix.
 
     Parameters
     ----------
     dist_matrix : array, shape = (sz1, sz2)
@@ -1727,23 +2288,69 @@
 
     for i in range(1, l1 + 1):
         for j in range(1, l2 + 1):
             if numpy.isfinite(mask[i - 1, j - 1]):
                 if dist_matrix[i - 1, j - 1] <= eps:
                     acc_cost_mat[i][j] = 1 + acc_cost_mat[i - 1][j - 1]
                 else:
-                    acc_cost_mat[i][j] = max(acc_cost_mat[i][j - 1],
-                                             acc_cost_mat[i - 1][j])
+                    acc_cost_mat[i][j] = max(
+                        acc_cost_mat[i][j - 1], acc_cost_mat[i - 1][j]
+                    )
 
     return acc_cost_mat
 
 
-def lcss_path_from_metric(s1, s2=None, eps=1, metric="euclidean",
-                          global_constraint=None, sakoe_chiba_radius=None,
-                          itakura_max_slope=None, **kwds):
+def lcss_accumulated_matrix_from_dist_matrix(dist_matrix, eps, mask, be=None):
+    """Compute the accumulated cost matrix score between two time series using
+    a precomputed distance matrix.
+
+    Parameters
+    ----------
+    dist_matrix : array, shape = (sz1, sz2)
+        Array containing the pairwise distances.
+    eps : float (default: 1.)
+        Maximum matching distance threshold.
+    mask : array, shape = (sz1, sz2)
+        Mask. Unconsidered cells must have infinite values.
+    be : Backend object or string or None
+        Backend.
+
+    Returns
+    -------
+    mat : array, shape = (sz1, sz2)
+        Accumulated cost matrix.
+    """
+    be = instantiate_backend(be, dist_matrix)
+    l1, l2 = dist_matrix.shape
+    acc_cost_mat = be.full((l1 + 1, l2 + 1), 0)
+
+    for i in range(1, l1 + 1):
+        for j in range(1, l2 + 1):
+            if be.isfinite(mask[i - 1, j - 1]):
+                if dist_matrix[i - 1, j - 1] <= eps:
+                    acc_cost_mat[i][j] = 1 + acc_cost_mat[i - 1][j - 1]
+                else:
+                    acc_cost_mat[i][j] = max(
+                        acc_cost_mat[i][j - 1], acc_cost_mat[i - 1][j]
+                    )
+
+    return acc_cost_mat
+
+
+def lcss_path_from_metric(
+    s1,
+    s2=None,
+    eps=1,
+    metric="euclidean",
+    global_constraint=None,
+    sakoe_chiba_radius=None,
+    itakura_max_slope=None,
+    be=None,
+    **kwds
+):
     r"""Compute the Longest Common Subsequence (LCSS) similarity measure between
     (possibly multidimensional) time series using a distance metric defined by
     the user and return both the path and the similarity.
 
     Having the length of the longest commom subsequence between two time-series,
     the similarity is computed as the percentage of that value regarding the
     length of the shortest time series.
@@ -1757,68 +2364,59 @@
     pairwise distances. See `scikit`_ and `scipy`_ documentations for more
     information about the available metrics.
 
     Parameters
     ----------
     s1 : array, shape = (sz1, d) if metric!="precomputed", (sz1, sz2) otherwise
         A time series or an array of pairwise distances between samples.
-
     s2 : array, shape = (sz2, d), optional (default: None)
         A second time series, only allowed if metric != "precomputed".
-
     eps : float (default: 1.)
         Maximum matching distance threshold.
-
     metric : string or callable (default: "euclidean")
         Function used to compute the pairwise distances between each points of
         `s1` and `s2`.
-
         If metric is "precomputed", `s1` is assumed to be a distance matrix.
-
         If metric is an other string, it must be one of the options compatible
         with sklearn.metrics.pairwise_distances.
-
         Alternatively, if metric is a callable function, it is called on pairs
         of rows of `s1` and `s2`. The callable should take two 1 dimensional
         arrays as input and return a value indicating the distance between
         them.
-
     global_constraint : {"itakura", "sakoe_chiba"} or None (default: None)
         Global constraint to restrict admissible paths for LCSS.
-
     sakoe_chiba_radius : int or None (default: None)
         Radius to be used for Sakoe-Chiba band global constraint.
         If None and `global_constraint` is set to "sakoe_chiba", a radius of
         1 is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
     itakura_max_slope : float or None (default: None)
         Maximum slope for the Itakura parallelogram constraint.
         If None and `global_constraint` is set to "itakura", a maximum slope
         of 2. is used.
         If both `sakoe_chiba_radius` and `itakura_max_slope` are set,
         `global_constraint` is used to infer which constraint to use among the
         two. In this case, if `global_constraint` corresponds to no global
         constraint, a `RuntimeWarning` is raised and no global constraint is
         used.
-
+    be : Backend object or string or None
+        Backend.
     **kwds
         Additional arguments to pass to sklearn pairwise_distances to compute
         the pairwise distances.
 
     Returns
     -------
     list of integer pairs
         Matching path represented as a list of index pairs. In each pair, the
         first index corresponds to s1 and the second one corresponds to s2.
-
     float
         Similarity score.
 
     Examples
     --------
     Lets create 2 numpy arrays to wrap:
 
@@ -1846,15 +2444,15 @@
     >>> lcss_path_from_metric(dist_matrix,
     ...                      metric="precomputed")  # doctest: +ELLIPSIS
     ([(0, 1), (1, 2), (2, 3), (3, 4), (4, 5)], 1.0)
 
     Notes
     --------
     By using a squared euclidean distance metric as shown above, the output
-    path and similarity is the same as the one obtained by using lcss_path 
+    path and similarity is the same as the one obtained by using lcss_path
     (which uses the euclidean distance) simply because with the sum of squared
     distances the matching threshold is still not reached.
     Also, contrary to Dynamic Time Warping and variants, an LCSS path does not need to be contiguous.
 
     See Also
     --------
     lcss: Get only the similarity score for LCSS
@@ -1870,31 +2468,50 @@
     .. _pairwise_distances: https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise_distances.html
 
     .. _scikit: https://scikit-learn.org/stable/modules/metrics.html
 
     .. _scipy: https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.pdist.html
 
     """  # noqa: E501
+    be = instantiate_backend(be, s1)
     if metric == "precomputed":  # Pairwise distance given as input
         sz1, sz2 = s1.shape
         mask = compute_mask(
-            sz1, sz2, GLOBAL_CONSTRAINT_CODE[global_constraint],
-            sakoe_chiba_radius, itakura_max_slope
+            sz1,
+            sz2,
+            GLOBAL_CONSTRAINT_CODE[global_constraint],
+            sakoe_chiba_radius,
+            itakura_max_slope,
+            be=be,
         )
         dist_mat = s1
     else:
-        s1 = to_time_series(s1, remove_nans=True)
-        s2 = to_time_series(s2, remove_nans=True)
+        s1 = to_time_series(s1, remove_nans=True, be=be)
+        s2 = to_time_series(s2, remove_nans=True, be=be)
         sz1 = s1.shape[0]
         sz2 = s2.shape[0]
         mask = compute_mask(
-            s1, s2, GLOBAL_CONSTRAINT_CODE[global_constraint],
-            sakoe_chiba_radius, itakura_max_slope
+            s1,
+            s2,
+            GLOBAL_CONSTRAINT_CODE[global_constraint],
+            sakoe_chiba_radius,
+            itakura_max_slope,
+            be=be,
         )
-        dist_mat = pairwise_distances(s1, s2, metric=metric, **kwds)
+        dist_mat = be.array(be.pairwise_distances(s1, s2, metric=metric, **kwds))
 
-    acc_cost_mat = njit_lcss_accumulated_matrix_from_dist_matrix(
-        dist_mat, eps, mask)
-    path = _return_lcss_path_from_dist_matrix(
-        dist_mat, eps, mask, acc_cost_mat, sz1, sz2)
+    if be.is_numpy:
+        acc_cost_mat = njit_lcss_accumulated_matrix_from_dist_matrix(
+            dist_mat, eps, mask
+        )
+        path = _njit_return_lcss_path_from_dist_matrix(
+            dist_mat, eps, mask, acc_cost_mat, sz1, sz2
+        )
+    else:
+        acc_cost_mat = lcss_accumulated_matrix_from_dist_matrix(
+            dist_mat, eps, mask, be=be
+        )
+        path = _return_lcss_path_from_dist_matrix(
+            dist_mat, eps, mask, acc_cost_mat, sz1, sz2, be=be
+        )
 
     return path, float(acc_cost_mat[-1][-1]) / min([sz1, sz2])
```

### Comparing `tslearn-0.5.3.2/tslearn/metrics/sax.py` & `tslearn-0.6.0/tslearn/metrics/sax.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,8 +51,8 @@
     ----------
     .. [1] Lin, Jessica, et al. "Experiencing SAX: a novel symbolic
            representation of time series." Data Mining and knowledge
            discovery 15.2 (2007): 107-144.
 
     """  # noqa: E501
     return _cdist_generic(cydist_sax, dataset1, dataset2, n_jobs, verbose,
-                          False, int, breakpoints_avg, size_fitted)
+                          False, int, None, breakpoints_avg, size_fitted)
```

### Comparing `tslearn-0.5.3.2/tslearn/metrics/soft_dtw_fast.c` & `tslearn-0.6.0/tslearn/metrics/soft_dtw_fast.c`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/metrics/softdtw_variants.py` & `tslearn-0.6.0/tslearn/metrics/softdtw_variants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,81 @@
-import numpy
+import numpy as np
 from joblib import Parallel, delayed
 from numba import njit
-from scipy.spatial.distance import cdist, pdist
-from sklearn.metrics.pairwise import euclidean_distances
 from sklearn.utils import check_random_state
 
+from tslearn.backend import instantiate_backend
 from tslearn.utils import (
     check_equal_size,
     to_time_series,
     to_time_series_dataset,
     ts_size,
 )
 
 from .dtw_variants import dtw, dtw_path
-from .soft_dtw_fast import _jacobian_product_sq_euc, _soft_dtw, _soft_dtw_grad
+from .soft_dtw_fast import (
+    _jacobian_product_sq_euc,
+    _njit_jacobian_product_sq_euc,
+    _njit_soft_dtw,
+    _njit_soft_dtw_grad,
+    _soft_dtw,
+    _soft_dtw_grad,
+)
 from .utils import _cdist_generic
 
 __author__ = "Romain Tavenard romain.tavenard[at]univ-rennes2.fr"
 
 GLOBAL_CONSTRAINT_CODE = {None: 0, "": 0, "itakura": 1, "sakoe_chiba": 2}
 TSLEARN_VALID_METRICS = ["dtw", "gak", "softdtw", "sax"]
 VARIABLE_LENGTH_METRICS = ["dtw", "gak", "softdtw", "sax"]
 
 
+def _gak(s1, s2, gram, be=None):
+    be = instantiate_backend(be, s1)
+    l1 = s1.shape[0]
+    l2 = s2.shape[0]
+
+    cum_sum = be.zeros((l1 + 1, l2 + 1))
+    cum_sum[0, 0] = 1.0
+
+    for i in range(l1):
+        for j in range(l2):
+            cum_sum[i + 1, j + 1] = (
+                cum_sum[i, j + 1] + cum_sum[i + 1, j] + cum_sum[i, j]
+            ) * gram[i, j]
+
+    return cum_sum[l1, l2]
+
+
 @njit(nogil=True)
-def njit_gak(s1, s2, gram):
+def _njit_gak(s1, s2, gram):
     l1 = s1.shape[0]
     l2 = s2.shape[0]
 
-    cum_sum = numpy.zeros((l1 + 1, l2 + 1))
+    cum_sum = np.zeros((l1 + 1, l2 + 1))
     cum_sum[0, 0] = 1.0
 
     for i in range(l1):
         for j in range(l2):
             cum_sum[i + 1, j + 1] = (
                 cum_sum[i, j + 1] + cum_sum[i + 1, j] + cum_sum[i, j]
             ) * gram[i, j]
 
     return cum_sum[l1, l2]
 
 
-def _gak_gram(s1, s2, sigma=1.0):
-    gram = -cdist(s1, s2, "sqeuclidean") / (2 * sigma**2)
-    gram -= numpy.log(2 - numpy.exp(gram))
-    return numpy.exp(gram)
+def _gak_gram(s1, s2, sigma=1.0, be=None):
+    be = instantiate_backend(be, s1)
+    gram = -be.cdist(s1, s2, "sqeuclidean") / (2 * sigma**2)
+    gram = be.array(gram)
+    gram -= be.log(2 - be.exp(gram))
+    return be.exp(gram)
 
 
-def unnormalized_gak(s1, s2, sigma=1.0):
+def unnormalized_gak(s1, s2, sigma=1.0, be=None):
     r"""Compute Global Alignment Kernel (GAK) between (possibly
     multidimensional) time series and return it.
 
     It is not required that both time series share the same size, but they must
     be the same dimension. GAK was
     originally presented in [1]_.
     This is an unnormalized version.
@@ -59,14 +84,16 @@
     ----------
     s1
         A time series
     s2
         Another time series
     sigma : float (default 1.)
         Bandwidth of the internal gaussian kernel used for GAK
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Kernel value
 
     Examples
@@ -84,24 +111,26 @@
     gak : normalized version of GAK that ensures that k(x,x) = 1
     cdist_gak : Compute cross-similarity matrix using Global Alignment kernel
 
     References
     ----------
     .. [1] M. Cuturi, "Fast global alignment kernels," ICML 2011.
     """
-    s1 = to_time_series(s1, remove_nans=True)
-    s2 = to_time_series(s2, remove_nans=True)
+    be = instantiate_backend(be, s1)
+    s1 = to_time_series(s1, remove_nans=True, be=be)
+    s2 = to_time_series(s2, remove_nans=True, be=be)
 
-    gram = _gak_gram(s1, s2, sigma=sigma)
+    gram = _gak_gram(s1, s2, sigma=sigma, be=be)
 
-    gak_val = njit_gak(s1, s2, gram)
-    return gak_val
+    if be.is_numpy:
+        return _njit_gak(s1, s2, gram)
+    return _gak(s1, s2, gram, be=be)
 
 
-def gak(s1, s2, sigma=1.0):  # TODO: better doc (formula for the kernel)
+def gak(s1, s2, sigma=1.0, be=None):  # TODO: better doc (formula for the kernel)
     r"""Compute Global Alignment Kernel (GAK) between (possibly
     multidimensional) time series and return it.
 
     It is not required that both time series share the same size, but they must
     be the same dimension. GAK was
     originally presented in [1]_.
     This is a normalized version that ensures that :math:`k(x,x)=1` for all
@@ -111,14 +140,16 @@
     ----------
     s1
         A time series
     s2
         Another time series
     sigma : float (default 1.)
         Bandwidth of the internal gaussian kernel used for GAK
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Kernel value
 
     Examples
@@ -132,21 +163,23 @@
     --------
     cdist_gak : Compute cross-similarity matrix using Global Alignment kernel
 
     References
     ----------
     .. [1] M. Cuturi, "Fast global alignment kernels," ICML 2011.
     """
-    denom = numpy.sqrt(
-        unnormalized_gak(s1, s1, sigma=sigma) * unnormalized_gak(s2, s2, sigma=sigma)
+    be = instantiate_backend(be, s1)
+    denom = be.sqrt(
+        unnormalized_gak(s1, s1, sigma=sigma, be=be)
+        * unnormalized_gak(s2, s2, sigma=sigma, be=be)
     )
-    return unnormalized_gak(s1, s2, sigma=sigma) / denom
+    return unnormalized_gak(s1, s2, sigma=sigma, be=be) / denom
 
 
-def cdist_gak(dataset1, dataset2=None, sigma=1.0, n_jobs=None, verbose=0):
+def cdist_gak(dataset1, dataset2=None, sigma=1.0, n_jobs=None, verbose=0, be=None):
     r"""Compute cross-similarity matrix using Global Alignment kernel (GAK).
 
     GAK was originally presented in [1]_.
 
     Parameters
     ----------
     dataset1
@@ -164,14 +197,16 @@
     verbose : int, optional (default=0)
         The verbosity level: if non zero, progress messages are printed.
         Above 50, the output is sent to stdout.
         The frequency of the messages increases with the verbosity level.
         If it more than 10, all iterations are reported.
         `Glossary <https://joblib.readthedocs.io/en/latest/parallel.html#parallel-reference-documentation>`__
         for more details.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     numpy.ndarray
         Cross-similarity matrix
 
     Examples
@@ -189,56 +224,61 @@
     --------
     gak : Compute Global Alignment kernel
 
     References
     ----------
     .. [1] M. Cuturi, "Fast global alignment kernels," ICML 2011.
     """  # noqa: E501
+    be = instantiate_backend(be, dataset1)
+
     unnormalized_matrix = _cdist_generic(
         dist_fun=unnormalized_gak,
         dataset1=dataset1,
         dataset2=dataset2,
         n_jobs=n_jobs,
         verbose=verbose,
         sigma=sigma,
         compute_diagonal=True,
+        be=be,
     )
-    dataset1 = to_time_series_dataset(dataset1)
+    dataset1 = to_time_series_dataset(dataset1, be=be)
     if dataset2 is None:
-        diagonal = numpy.diag(numpy.sqrt(1.0 / numpy.diag(unnormalized_matrix)))
+        diagonal = be.diag(be.sqrt(1.0 / be.diag(unnormalized_matrix)))
         diagonal_left = diagonal_right = diagonal
     else:
-        dataset2 = to_time_series_dataset(dataset2)
+        dataset2 = to_time_series_dataset(dataset2, be=be)
         diagonal_left = Parallel(n_jobs=n_jobs, prefer="threads", verbose=verbose)(
-            delayed(unnormalized_gak)(dataset1[i], dataset1[i], sigma=sigma)
+            delayed(unnormalized_gak)(dataset1[i], dataset1[i], sigma=sigma, be=be)
             for i in range(len(dataset1))
         )
         diagonal_right = Parallel(n_jobs=n_jobs, prefer="threads", verbose=verbose)(
-            delayed(unnormalized_gak)(dataset2[j], dataset2[j], sigma=sigma)
+            delayed(unnormalized_gak)(dataset2[j], dataset2[j], sigma=sigma, be=be)
             for j in range(len(dataset2))
         )
-        diagonal_left = numpy.diag(1.0 / numpy.sqrt(diagonal_left))
-        diagonal_right = numpy.diag(1.0 / numpy.sqrt(diagonal_right))
-    return (diagonal_left.dot(unnormalized_matrix)).dot(diagonal_right)
+        diagonal_left = be.diag(1.0 / be.sqrt(be.array(diagonal_left)))
+        diagonal_right = be.diag(1.0 / be.sqrt(be.array(diagonal_right)))
+    return diagonal_left @ unnormalized_matrix @ diagonal_right
 
 
-def sigma_gak(dataset, n_samples=100, random_state=None):
+def sigma_gak(dataset, n_samples=100, random_state=None, be=None):
     r"""Compute sigma value to be used for GAK.
 
     This method was originally presented in [1]_.
 
     Parameters
     ----------
     dataset
         A dataset of time series
     n_samples : int (default: 100)
         Number of samples on which median distance should be estimated
     random_state : integer or numpy.RandomState or None (default: None)
         The generator used to draw the samples. If an integer is given, it
         fixes the seed. Defaults to the global numpy random number generator.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Suggested bandwidth (:math:`\sigma`) for the Global Alignment kernel
 
     Examples
@@ -254,44 +294,49 @@
     gak : Compute Global Alignment kernel
     cdist_gak : Compute cross-similarity matrix using Global Alignment kernel
 
     References
     ----------
     .. [1] M. Cuturi, "Fast global alignment kernels," ICML 2011.
     """
+    be = instantiate_backend(be, dataset)
+
     random_state = check_random_state(random_state)
-    dataset = to_time_series_dataset(dataset)
-    n_ts, sz, d = dataset.shape
-    if not check_equal_size(dataset):
-        sz = numpy.min([ts_size(ts) for ts in dataset])
+    dataset = to_time_series_dataset(dataset, be=be)
+    n_ts, sz, d = be.shape(dataset)
+    if not check_equal_size(dataset, be=be):
+        sz = be.min([ts_size(ts) for ts in dataset])
     if n_ts * sz < n_samples:
         replace = True
     else:
         replace = False
     sample_indices = random_state.choice(n_ts * sz, size=n_samples, replace=replace)
-    dists = pdist(
-        dataset[:, :sz, :].reshape((-1, d))[sample_indices], metric="euclidean"
+    dists = be.pdist(
+        dataset[:, :sz, :].reshape((-1, d))[sample_indices],
+        metric="euclidean",
     )
-    return numpy.median(dists) * numpy.sqrt(sz)
+    return be.median(dists) * be.sqrt(sz)
 
 
-def gamma_soft_dtw(dataset, n_samples=100, random_state=None):
+def gamma_soft_dtw(dataset, n_samples=100, random_state=None, be=None):
     r"""Compute gamma value to be used for GAK/Soft-DTW.
 
     This method was originally presented in [1]_.
 
     Parameters
     ----------
     dataset
         A dataset of time series
     n_samples : int (default: 100)
         Number of samples on which median distance should be estimated
     random_state : integer or numpy.RandomState or None (default: None)
         The generator used to draw the samples. If an integer is given, it
         fixes the seed. Defaults to the global numpy random number generator.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Suggested :math:`\gamma` parameter for the Soft-DTW
 
     Examples
@@ -306,20 +351,25 @@
     --------
     sigma_gak : Compute sigma parameter for Global Alignment kernel
 
     References
     ----------
     .. [1] M. Cuturi, "Fast global alignment kernels," ICML 2011.
     """
-    return 2. * sigma_gak(dataset=dataset,
-                          n_samples=n_samples,
-                          random_state=random_state) ** 2
+    be = instantiate_backend(be, dataset)
+    return (
+        2.0
+        * sigma_gak(
+            dataset=dataset, n_samples=n_samples, random_state=random_state, be=be
+        )
+        ** 2
+    )
 
 
-def soft_dtw(ts1, ts2, gamma=1.0):
+def soft_dtw(ts1, ts2, gamma=1.0, be=None):
     r"""Compute Soft-DTW metric between two time series.
 
     Soft-DTW was originally presented in [1]_ and is
     discussed in more details in our
     :ref:`user-guide page on DTW and its variants<dtw>`.
 
     Soft-DTW is computed as:
@@ -340,14 +390,16 @@
     ----------
     ts1
         A time series
     ts2
         Another time series
     gamma : float (default 1.)
         Gamma parameter for Soft-DTW
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     float
         Similarity
 
     Examples
@@ -366,22 +418,25 @@
     cdist_soft_dtw : Cross similarity matrix between time series datasets
 
     References
     ----------
     .. [1] M. Cuturi, M. Blondel "Soft-DTW: a Differentiable Loss Function for
        Time-Series," ICML 2017.
     """
+    be = instantiate_backend(be, ts1)
     if gamma == 0.0:
-        return dtw(ts1, ts2) ** 2
+        return dtw(ts1, ts2, be=be) ** 2
     return SoftDTW(
-        SquaredEuclidean(ts1[: ts_size(ts1)], ts2[: ts_size(ts2)]), gamma=gamma
+        SquaredEuclidean(ts1[: ts_size(ts1)], ts2[: ts_size(ts2)], be=be),
+        gamma=gamma,
+        be=be,
     ).compute()
 
 
-def soft_dtw_alignment(ts1, ts2, gamma=1.0):
+def soft_dtw_alignment(ts1, ts2, gamma=1.0, be=None):
     r"""Compute Soft-DTW metric between two time series and return both the
     similarity measure and the alignment matrix.
 
     Soft-DTW was originally presented in [1]_ and is
     discussed in more details in our
     :ref:`user-guide page on DTW and its variants<dtw>`.
 
@@ -403,14 +458,16 @@
     ----------
     ts1
         A time series
     ts2
         Another time series
     gamma : float (default 1.)
         Gamma parameter for Soft-DTW
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     numpy.ndarray
         Soft-alignment matrix
     float
         Similarity
@@ -433,30 +490,33 @@
     soft_dtw : Returns soft-DTW score alone
 
     References
     ----------
     .. [1] M. Cuturi, M. Blondel "Soft-DTW: a Differentiable Loss Function for
        Time-Series," ICML 2017.
     """
+    be = instantiate_backend(be, ts1)
     if gamma == 0.0:
-        path, dist = dtw_path(ts1, ts2)
+        path, dist = dtw_path(ts1, ts2, be=be)
         dist_sq = dist**2
-        a = numpy.zeros((ts_size(ts1), ts_size(ts2)))
+        a = be.zeros((ts_size(ts1), ts_size(ts2)))
         for i, j in path:
             a[i, j] = 1.0
     else:
         sdtw = SoftDTW(
-            SquaredEuclidean(ts1[: ts_size(ts1)], ts2[: ts_size(ts2)]), gamma=gamma
+            SquaredEuclidean(ts1[: ts_size(ts1)], ts2[: ts_size(ts2)], be=be),
+            gamma=gamma,
+            be=be,
         )
         dist_sq = sdtw.compute()
         a = sdtw.grad()
     return a, dist_sq
 
 
-def cdist_soft_dtw(dataset1, dataset2=None, gamma=1.0):
+def cdist_soft_dtw(dataset1, dataset2=None, gamma=1.0, be=None):
     r"""Compute cross-similarity matrix using Soft-DTW metric.
 
     Soft-DTW was originally presented in [1]_ and is
     discussed in more details in our
     :ref:`user-guide page on DTW and its variants<dtw>`.
 
     Soft-DTW is computed as:
@@ -477,14 +537,16 @@
     ----------
     dataset1
         A dataset of time series
     dataset2
         Another dataset of time series
     gamma : float (default 1.)
         Gamma parameter for Soft-DTW
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     numpy.ndarray
         Cross-similarity matrix
 
     Examples
@@ -504,43 +566,48 @@
         datasets using a normalized version of Soft-DTW
 
     References
     ----------
     .. [1] M. Cuturi, M. Blondel "Soft-DTW: a Differentiable Loss Function for
        Time-Series," ICML 2017.
     """
-    dataset1 = to_time_series_dataset(dataset1, dtype=numpy.float64)
+    be = instantiate_backend(be, dataset1)
+    dataset1 = to_time_series_dataset(dataset1, dtype=be.float64, be=be)
+
     self_similarity = False
     if dataset2 is None:
         dataset2 = dataset1
         self_similarity = True
     else:
-        dataset2 = to_time_series_dataset(dataset2, dtype=numpy.float64)
-    dists = numpy.empty((dataset1.shape[0], dataset2.shape[0]))
-    equal_size_ds1 = check_equal_size(dataset1)
-    equal_size_ds2 = check_equal_size(dataset2)
+        dataset2 = to_time_series_dataset(dataset2, dtype=be.float64, be=be)
+
+    dists = be.empty((dataset1.shape[0], dataset2.shape[0]))
+
+    equal_size_ds1 = check_equal_size(dataset1, be=be)
+    equal_size_ds2 = check_equal_size(dataset2, be=be)
+
     for i, ts1 in enumerate(dataset1):
         if equal_size_ds1:
             ts1_short = ts1
         else:
             ts1_short = ts1[: ts_size(ts1)]
         for j, ts2 in enumerate(dataset2):
             if equal_size_ds2:
                 ts2_short = ts2
             else:
                 ts2_short = ts2[: ts_size(ts2)]
             if self_similarity and j < i:
                 dists[i, j] = dists[j, i]
             else:
-                dists[i, j] = soft_dtw(ts1_short, ts2_short, gamma=gamma)
+                dists[i, j] = soft_dtw(ts1_short, ts2_short, gamma=gamma, be=be)
 
     return dists
 
 
-def cdist_soft_dtw_normalized(dataset1, dataset2=None, gamma=1.0):
+def cdist_soft_dtw_normalized(dataset1, dataset2=None, gamma=1.0, be=None):
     r"""Compute cross-similarity matrix using a normalized version of the
     Soft-DTW metric.
 
     Soft-DTW was originally presented in [1]_ and is
     discussed in more details in our
     :ref:`user-guide page on DTW and its variants<dtw>`.
 
@@ -570,89 +637,112 @@
     and ensures that all returned values are positive and that
     :math:`\text{norm-soft-DTW}_{\gamma}(X, X) = 0`.
 
     Parameters
     ----------
     dataset1
         A dataset of time series
-
     dataset2
         Another dataset of time series
-
     gamma : float (default 1.)
         Gamma parameter for Soft-DTW
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     numpy.ndarray
         Cross-similarity matrix
 
     Examples
     --------
-    >>> time_series = numpy.random.randn(10, 15, 1)
-    >>> numpy.alltrue(cdist_soft_dtw_normalized(time_series) >= 0.)
+    >>> time_series = np.random.randn(10, 15, 1)
+    >>> np.alltrue(cdist_soft_dtw_normalized(time_series) >= 0.)
     True
 
     See Also
     --------
     soft_dtw : Compute Soft-DTW
     cdist_soft_dtw : Cross similarity matrix between time series
         datasets using the unnormalized version of Soft-DTW
 
     References
     ----------
     .. [1] M. Cuturi, M. Blondel "Soft-DTW: a Differentiable Loss Function for
        Time-Series," ICML 2017.
     """
-    dists = cdist_soft_dtw(dataset1, dataset2=dataset2, gamma=gamma)
-    d_ii = numpy.diag(dists)
-    dists -= 0.5 * (d_ii.reshape((-1, 1)) + d_ii.reshape((1, -1)))
+    be = instantiate_backend(be, dataset1)
+    dists = cdist_soft_dtw(dataset1, dataset2=dataset2, gamma=gamma, be=be)
+    d_ii = be.diag(dists)
+    dists -= 0.5 * (be.reshape(d_ii, (-1, 1)) + be.reshape(d_ii, (1, -1)))
     return dists
 
 
 class SoftDTW:
-    def __init__(self, D, gamma=1.0):
+    def __init__(self, D, gamma=1.0, be=None, compute_with_backend=False):
         """
         Parameters
         ----------
+        D : array-like, shape=[m, n], dtype=float64 or class computing distances with a method 'compute'
+            Distances. An example of class computing distance is 'SquaredEuclidean'.
         gamma: float
             Regularization parameter.
             Lower is less smoothed (closer to true DTW).
+        be : Backend object or string or None
+            Backend.
+        compute_with_backend : bool, default=False
+            This parameter has no influence when the NumPy backend is used.
+            When using a backend different from NumPy is used:
+            If `True`, the computation is done with the corresponding backend.
+            If `False`, a conversion to the NumPy backend can be used to accelerate the computation.
 
         Attributes
         ----------
         self.R_: array, shape = [m + 2, n + 2]
             Accumulated cost matrix (stored after calling `compute`).
         """
+        be = instantiate_backend(be, D)
+        self.be = be
+        self.compute_with_backend = compute_with_backend
         if hasattr(D, "compute"):
             self.D = D.compute()
         else:
             self.D = D
-        self.D = self.D.astype(numpy.float64)
+        self.D = self.be.cast(self.D, dtype=self.be.float64)
 
         # Allocate memory.
         # We need +2 because we use indices starting from 1
         # and to deal with edge cases in the backward recursion.
-        m, n = self.D.shape
-        self.R_ = numpy.zeros((m + 2, n + 2), dtype=numpy.float64)
+        m, n = self.be.shape(self.D)
+        self.R_ = self.be.zeros((m + 2, n + 2), dtype=self.be.float64)
         self.computed = False
 
-        self.gamma = numpy.float64(gamma)
+        self.gamma = self.be.array(gamma, dtype=self.be.float64)
 
     def compute(self):
         """Compute soft-DTW by dynamic programming.
 
         Returns
         -------
         sdtw: float
             soft-DTW discrepancy.
         """
-        m, n = self.D.shape
+        m, n = self.be.shape(self.D)
 
-        _soft_dtw(self.D, self.R_, gamma=self.gamma)
+        if self.be.is_numpy:
+            _njit_soft_dtw(self.D, self.R_, gamma=self.gamma)
+        elif not self.compute_with_backend:
+            _njit_soft_dtw(
+                self.be.to_numpy(self.D),
+                self.be.to_numpy(self.R_),
+                gamma=self.be.to_numpy(self.gamma),
+            )
+            self.R_ = self.be.array(self.R_)
+        else:
+            _soft_dtw(self.D, self.R_, gamma=self.gamma, be=self.be)
 
         self.computed = True
 
         return self.R_[m, n]
 
     def grad(self):
         """Compute gradient of soft-DTW w.r.t. D by dynamic programming.
@@ -661,61 +751,81 @@
         -------
         grad: array, shape = [m, n]
             Gradient w.r.t. D.
         """
         if not self.computed:
             raise ValueError("Needs to call compute() first.")
 
-        m, n = self.D.shape
+        m, n = self.be.shape(self.D)
 
         # Add an extra row and an extra column to D.
         # Needed to deal with edge cases in the recursion.
-        D = numpy.vstack((self.D, numpy.zeros(n)))
-        D = numpy.hstack((D, numpy.zeros((m + 1, 1))))
+        D = self.be.vstack((self.D, self.be.zeros(n)))
+        D = self.be.hstack((D, self.be.zeros((m + 1, 1))))
 
         # Allocate memory.
         # We need +2 because we use indices starting from 1
         # and to deal with edge cases in the recursion.
-        E = numpy.zeros((m + 2, n + 2), dtype=numpy.float64)
+        E = self.be.zeros((m + 2, n + 2), dtype=self.be.float64)
 
-        _soft_dtw_grad(D, self.R_, E, gamma=self.gamma)
+        if self.be.is_numpy:
+            _njit_soft_dtw_grad(D, self.R_, E, gamma=self.gamma)
+        elif not self.compute_with_backend:
+            _njit_soft_dtw_grad(
+                self.be.to_numpy(D),
+                self.be.to_numpy(self.R_),
+                self.be.to_numpy(E),
+                gamma=self.be.to_numpy(self.gamma),
+            )
+            self.R_ = self.be.array(self.R_)
+        else:
+            _soft_dtw_grad(D, self.R_, E, gamma=self.gamma, be=self.be)
 
         return E[1:-1, 1:-1]
 
 
 class SquaredEuclidean:
-    def __init__(self, X, Y):
+    def __init__(self, X, Y, be=None, compute_with_backend=False):
         """
         Parameters
         ----------
         X: array, shape = [m, d]
             First time series.
         Y: array, shape = [n, d]
             Second time series.
+        be : Backend object or string or None
+            Backend.
+        compute_with_backend : bool, default=False
+            This parameter has no influence when the NumPy backend is used.
+            When using a backend different from NumPy is used:
+            If `True`, the computation is done with the corresponding backend.
+            If `False`, a conversion to the NumPy backend can be used to accelerate the computation.
 
         Examples
         --------
         >>> SquaredEuclidean([1, 2, 2, 3], [1, 2, 3, 4]).compute()
         array([[0., 1., 4., 9.],
                [1., 0., 1., 4.],
                [1., 0., 1., 4.],
                [4., 1., 0., 1.]])
         """
-        self.X = to_time_series(X).astype(numpy.float64)
-        self.Y = to_time_series(Y).astype(numpy.float64)
+        self.be = instantiate_backend(be, X)
+        self.compute_with_backend = compute_with_backend
+        self.X = self.be.cast(to_time_series(X), dtype=self.be.float64)
+        self.Y = self.be.cast(to_time_series(Y), dtype=self.be.float64)
 
     def compute(self):
         """Compute distance matrix.
 
         Returns
         -------
         D: array, shape = [m, n]
             Distance matrix.
         """
-        return euclidean_distances(self.X, self.Y, squared=True)
+        return self.be.pairwise_euclidean_distances(self.X, self.Y) ** 2
 
     def jacobian_product(self, E):
         """Compute the product between the Jacobian
         (a linear map from m x d to m x n) and a matrix E.
 
         Parameters
         ----------
@@ -724,12 +834,25 @@
 
         Returns
         -------
         G: array, shape = [m, d]
             Product with Jacobian
             ([m x d, m x n] * [m x n] = [m x d]).
         """
-        G = numpy.zeros_like(self.X, dtype=numpy.float64)
+        G = self.be.zeros_like(self.X, dtype=self.be.float64)
 
-        _jacobian_product_sq_euc(self.X, self.Y, E.astype(numpy.float64), G)
+        if self.be.is_numpy:
+            _njit_jacobian_product_sq_euc(self.X, self.Y, E.astype(np.float64), G)
+        elif not self.compute_with_backend:
+            _njit_jacobian_product_sq_euc(
+                self.be.to_numpy(self.X),
+                self.be.to_numpy(self.Y),
+                self.be.to_numpy(E).astype(np.float64),
+                self.be.to_numpy(G),
+            )
+            G = self.be.array(G)
+        else:
+            _jacobian_product_sq_euc(
+                self.X, self.Y, self.be.cast(E, self.be.float64), G
+            )
 
         return G
```

### Comparing `tslearn-0.5.3.2/tslearn/metrics/utils.py` & `tslearn-0.6.0/tslearn/metrics/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,27 @@
-import numpy
 from joblib import Parallel, delayed
+
+from tslearn.backend import instantiate_backend
 from tslearn.utils import to_time_series_dataset
 
-__author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
+__author__ = "Romain Tavenard romain.tavenard[at]univ-rennes2.fr"
 
 
-def _cdist_generic(dist_fun, dataset1, dataset2, n_jobs, verbose,
-                   compute_diagonal=True, dtype=float, *args, **kwargs):
+def _cdist_generic(
+    dist_fun,
+    dataset1,
+    dataset2,
+    n_jobs,
+    verbose,
+    compute_diagonal=True,
+    dtype=float,
+    be=None,
+    *args,
+    **kwargs
+):
     """Compute cross-similarity matrix with joblib parallelization for a given
     similarity function.
 
     Parameters
     ----------
     dist_fun : function
         Similarity function to be used
@@ -33,53 +44,54 @@
         The verbosity level: if non zero, progress messages are printed.
         Above 50, the output is sent to stdout.
         The frequency of the messages increases with the verbosity level.
         If it more than 10, all iterations are reported.
         `Glossary <https://joblib.readthedocs.io/en/latest/parallel.html#parallel-reference-documentation>`__
         for more details.
 
+    be : Backend object or string or None
+        Backend.
+
     compute_diagonal : bool (default: True)
         Whether diagonal terms should be computed or assumed to be 0 in the
         self-similarity case. Used only if `dataset2` is `None`.
 
     *args and **kwargs :
         Optional additional parameters to be passed to the similarity function.
 
 
     Returns
     -------
     cdist : numpy.ndarray
         Cross-similarity matrix
     """  # noqa: E501
-    dataset1 = to_time_series_dataset(dataset1, dtype=dtype)
+    be = instantiate_backend(be, dataset1)
+    dataset1 = to_time_series_dataset(dataset1, dtype=dtype, be=be)
 
     if dataset2 is None:
         # Inspired from code by @GillesVandewiele:
         # https://github.com/rtavenar/tslearn/pull/128#discussion_r314978479
-        matrix = numpy.zeros((len(dataset1), len(dataset1)))
-        indices = numpy.triu_indices(len(dataset1),
-                                     k=0 if compute_diagonal else 1,
-                                     m=len(dataset1))
-        matrix[indices] = Parallel(n_jobs=n_jobs,
-                                   prefer="threads",
-                                   verbose=verbose)(
-            delayed(dist_fun)(
-                dataset1[i], dataset1[j],
-                *args, **kwargs
+        matrix = be.zeros((len(dataset1), len(dataset1)))
+        indices = be.triu_indices(
+            len(dataset1), k=0 if compute_diagonal else 1, m=len(dataset1)
+        )
+
+        matrix[indices] = be.array(
+            Parallel(n_jobs=n_jobs, prefer="threads", verbose=verbose)(
+                delayed(dist_fun)(dataset1[i], dataset1[j], *args, **kwargs)
+                for i in range(len(dataset1))
+                for j in range(i if compute_diagonal else i + 1, len(dataset1))
             )
-            for i in range(len(dataset1))
-            for j in range(i if compute_diagonal else i + 1,
-                           len(dataset1))
         )
-        indices = numpy.tril_indices(len(dataset1), k=-1, m=len(dataset1))
+
+        indices = be.tril_indices(len(dataset1), k=-1, m=len(dataset1))
         matrix[indices] = matrix.T[indices]
+
         return matrix
     else:
-        dataset2 = to_time_series_dataset(dataset2, dtype=dtype)
+        dataset2 = to_time_series_dataset(dataset2, dtype=dtype, be=be)
         matrix = Parallel(n_jobs=n_jobs, prefer="threads", verbose=verbose)(
-            delayed(dist_fun)(
-                dataset1[i], dataset2[j],
-                *args, **kwargs
-            )
-            for i in range(len(dataset1)) for j in range(len(dataset2))
+            delayed(dist_fun)(dataset1[i], dataset2[j], *args, **kwargs)
+            for i in range(len(dataset1))
+            for j in range(len(dataset2))
         )
-        return numpy.array(matrix).reshape((len(dataset1), -1))
+        return be.reshape(be.array(matrix), (len(dataset1), -1))
```

### Comparing `tslearn-0.5.3.2/tslearn/neighbors/neighbors.py` & `tslearn-0.6.0/tslearn/neighbors/neighbors.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/neural_network/neural_network.py` & `tslearn-0.6.0/tslearn/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/piecewise/piecewise.py` & `tslearn-0.6.0/tslearn/piecewise/piecewise.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/preprocessing/preprocessing.py` & `tslearn-0.6.0/tslearn/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/shapelets/shapelets.py` & `tslearn-0.6.0/tslearn/shapelets/shapelets.py`

 * *Files 10% similar despite different names*

```diff
@@ -579,15 +579,15 @@
         self._check_series_length(X)
 
         n_ts, sz, d = X.shape
         locations = self.locator_model_.predict(
             [X[:, :, di].reshape((n_ts, sz, 1)) for di in range(self.d_)],
             batch_size=self.batch_size, verbose=self.verbose
         )
-        return locations.astype(numpy.int)
+        return locations.astype(numpy.int_)
 
     def _check_series_length(self, X):
         """Ensures that time series in X matches the following requirements:
         
         - their length is greater than the size of the longest shapelet
         - (at predict time) their length is lower than the maximum allowed 
         length, as set by self.max_size
@@ -884,133 +884,7 @@
         # errors in the `transform` method, while sklearn performs checks
         # that requires the output of transform to have less than 1e-9
         # difference between outputs of same input.
         return {'allow_nan': True, 'allow_variable_length': True}
 
 
 ShapeletModel = LearningShapelets
-
-
-class SerializableShapeletModel(LearningShapelets):
-    """Serializable variant of the Learning Time-Series Shapelets model.
-
-
-    Learning Time-Series Shapelets was originally presented in [1]_.
-    
-    .. deprecated:: 0.4
-             `SerializableShapeletModel` is deprecated in version 0.4 and
-            will be removed in 0.6. Use `LearningShapelets` instead, which is
-            now fully serializable and clonable.
-
-    Parameters
-    ----------
-    n_shapelets_per_size: dict (default: None)
-        Dictionary giving, for each shapelet size (key),
-        the number of such shapelets to be trained (value)
-    max_iter: int (default: 10,000)
-        Number of training epochs.
-
-        .. versionchanged:: 0.3
-            default value for max_iter is set to 10,000 instead of 100
-
-    batch_size: int (default:256)
-        Batch size to be used.
-
-    verbose: {0, 1, 2} (default: 0)
-        `keras` verbose level.
-    learning_rate: float (default: 0.01)
-        Learning rate to be used for the SGD optimizer.
-    weight_regularizer: float or None (default: 0.)
-        Strength of the L2 regularizer to use for training the classification
-        (softmax) layer. If 0, no regularization is performed.
-    shapelet_length: float (default 0.15)
-        The length of the shapelets, expressed as a fraction of the ts length
-    total_lengths: int (default 3)
-        The number of different shapelet lengths. Will extract shapelets of
-        length i * shapelet_length for i in [1, total_lengths]
-    random_state : int or None, optional (default: None)
-        The seed of the pseudo random number generator to use when shuffling
-        the data.  If int, random_state is the seed used by the random number
-        generator; If None, the random number generator is the RandomState
-        instance used by `np.random`.
-
-    Attributes
-    ----------
-    shapelets_ : numpy.ndarray of objects, each object being a time series
-        Set of time-series shapelets.
-
-    shapelets_as_time_series_ : numpy.ndarray of shape (n_shapelets, sz_shp, \
-            d) where `sz_shp` is the maximum of all  shapelet sizes
-        Set of time-series shapelets formatted as a ``tslearn`` time series
-        dataset.
-
-    transformer_model_ : keras.Model
-        Transforms an input dataset of timeseries into distances to the
-        learned shapelets.
-
-    locator_model_ : keras.Model
-        Returns the indices where each of the shapelets can be found (minimal
-        distance) within each of the timeseries of the input dataset.
-
-    model_ : keras.Model
-        Directly predicts the class probabilities for the input timeseries.
-
-    Notes
-    -----
-        This implementation requires a dataset of equal-sized time series.
-
-    Examples
-    --------
-    >>> from tslearn.generators import random_walk_blobs
-    >>> X, y = random_walk_blobs(n_ts_per_blob=10, sz=16, d=2, n_blobs=3)
-    >>> clf = SerializableShapeletModel(n_shapelets_per_size={4: 5},
-    ...                                 max_iter=1, verbose=0,
-    ...                                 learning_rate=0.01)
-    >>> _ = clf.fit(X, y)
-    >>> clf.shapelets_.shape[0]
-    5
-    >>> clf.shapelets_[0].shape
-    (4, 2)
-    >>> clf.predict(X).shape
-    (30,)
-    >>> clf.predict_proba(X).shape
-    (30, 3)
-    >>> clf.transform(X).shape
-    (30, 5)
-
-    References
-    ----------
-    .. [1] J. Grabocka et al. Learning Time-Series Shapelets. SIGKDD 2014.
-    """
-    def __init__(self, n_shapelets_per_size=None,
-                 max_iter=10000,
-                 batch_size=256,
-                 verbose=0,
-                 learning_rate=0.01,
-                 weight_regularizer=0.,
-                 shapelet_length=0.3,
-                 total_lengths=3,
-                 random_state=None):
-        super().__init__(n_shapelets_per_size=n_shapelets_per_size,
-                             max_iter=max_iter,
-                             batch_size=batch_size,
-                             verbose=verbose,
-                             weight_regularizer=weight_regularizer,
-                             shapelet_length=shapelet_length,
-                             total_lengths=total_lengths,
-                             random_state=random_state)
-        self.learning_rate = learning_rate
-        warnings.warn(
-            "`SerializableShapeletModel` is deprecated in version 0.4 and "
-            "will be removed in 0.6. Use `LearningShapelets` instead, which is"
-            " now fully serializable and clonable.",
-            DeprecationWarning, stacklevel=2)
-
-    def _set_model_layers(self, X, ts_sz, d, n_classes):
-        super()._set_model_layers(X=X,
-                                  ts_sz=ts_sz,
-                                  d=d,
-                                  n_classes=n_classes)
-        K.set_value(self.model_.optimizer.lr, self.learning_rate)
-
-    def set_params(self, **params):
-        return super().set_params(**params)
```

### Comparing `tslearn-0.5.3.2/tslearn/svm/svm.py` & `tslearn-0.6.0/tslearn/svm/svm.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,26 +230,14 @@
 
     @property
     def n_iter_(self):
         warnings.warn('n_iter_ is always set to 1 for TimeSeriesSVC, since '
                       'it is non-trivial to access the underlying libsvm')
         return 1
 
-    @deprecated('The use of '
-                '`support_vectors_time_series_` is deprecated in '
-                'tslearn v0.4 and will be removed in v0.6. Use '
-                '`support_vectors_` property instead.')
-    def support_vectors_time_series_(self, X=None):
-        warnings.warn('The use of '
-                      '`support_vectors_time_series_` is deprecated in '
-                      'tslearn v0.4 and will be removed in v0.6. Use '
-                      '`support_vectors_` property instead.')
-        check_is_fitted(self, '_X_fit')
-        return self._X_fit[self.svm_estimator_.support_]
-
     @property
     def support_vectors_(self):
         check_is_fitted(self, '_X_fit')
         sv = []
         idx_start = 0
         for cl in range(len(self.svm_estimator_.n_support_)):
             idx_end = idx_start + self.svm_estimator_.n_support_[cl]
@@ -505,26 +493,14 @@
 
     @property
     def n_iter_(self):
         warnings.warn('n_iter_ is always set to 1 for TimeSeriesSVR, since '
                       'it is non-trivial to access the underlying libsvm')
         return 1
 
-    @deprecated('The use of '
-                '`support_vectors_time_series_` is deprecated in '
-                'tslearn v0.4 and will be removed in v0.6. Use '
-                '`support_vectors_` property instead.')
-    def support_vectors_time_series_(self, X=None):
-        warnings.warn('The use of '
-                      '`support_vectors_time_series_` is deprecated in '
-                      'tslearn v0.4 and will be removed in v0.6. Use '
-                      '`support_vectors_` property instead.')
-        check_is_fitted(self, '_X_fit')
-        return self._X_fit[self.svm_estimator_.support_]
-
     @property
     def support_vectors_(self):
         check_is_fitted(self, '_X_fit')
         return self._X_fit[self.svm_estimator_.support_]
 
     def fit(self, X, y, sample_weight=None):
         """Fit the SVM model according to the given training data.
```

### Comparing `tslearn-0.5.3.2/tslearn/tests/sklearn_patches.py` & `tslearn-0.6.0/tslearn/tests/sklearn_patches.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_barycenters.py` & `tslearn-0.6.0/tslearn/tests/test_barycenters.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_clustering.py` & `tslearn-0.6.0/tslearn/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_estimators.py` & `tslearn-0.6.0/tslearn/tests/test_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                              check_regressor_data_not_an_array,
                              check_classifier_data_not_an_array,
                              check_regressors_int_patched,
                              check_classifiers_cont_target,
                              check_pipeline_consistency,
                              yield_all_checks,
                              _create_large_ts_dataset)
-from tslearn.shapelets import LearningShapelets, SerializableShapeletModel
+from tslearn.shapelets import LearningShapelets
 import warnings
 import pytest
 
 
 # Patching some check functions to work on ts data instead of tabular data.
 checks = sklearn.utils.estimator_checks
 checks._yield_all_checks = yield_all_checks
@@ -173,16 +173,15 @@
         check_no_attributes_set_in_init(name, estimator)
     else:
         # got an instance
         estimator = Estimator
         name = type(estimator).__name__
 
     if hasattr(estimator, 'max_iter'):
-        if (isinstance(estimator, LearningShapelets) or
-                isinstance(estimator, SerializableShapeletModel)):
+        if isinstance(estimator, LearningShapelets):
             estimator.set_params(max_iter=100)
         else:
             estimator.set_params(max_iter=10)
     if hasattr(estimator, 'total_lengths'):
         estimator.set_params(total_lengths=1)
     if hasattr(estimator, 'probability'):
         estimator.set_params(probability=True)
@@ -204,12 +203,11 @@
 @pytest.mark.parametrize('name, Estimator', get_estimators('all'))
 def test_all_estimators(name, Estimator):
     """Test all the estimators in tslearn."""
     allow_nan = (hasattr(checks, 'ALLOW_NAN') and
                  Estimator().get_tags()["allow_nan"])
     if allow_nan:
         checks.ALLOW_NAN.append(name)
-    if name in ["GlobalAlignmentKernelKMeans", "ShapeletModel",
-                "SerializableShapeletModel"]:
+    if name in ["ShapeletModel"]:
         # Deprecated models
         return
     check_estimator(Estimator)
```

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_matrixprofile.py` & `tslearn-0.6.0/tslearn/tests/test_matrixprofile.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_neighbors.py` & `tslearn-0.6.0/tslearn/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_piecewise.py` & `tslearn-0.6.0/tslearn/tests/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_serialize_models.py` & `tslearn-0.6.0/tslearn/tests/test_serialize_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 from sklearn.exceptions import NotFittedError
 from tslearn import hdftools
 from tslearn.preprocessing import TimeSeriesScalerMeanVariance
 
 from tslearn.neighbors import KNeighborsTimeSeries, \
     KNeighborsTimeSeriesClassifier
-from tslearn.shapelets import LearningShapelets, SerializableShapeletModel
+from tslearn.shapelets import LearningShapelets
 from tslearn.clustering import KShape, TimeSeriesKMeans, \
     KernelKMeans
 from tslearn.generators import random_walks
 from tslearn.piecewise import PiecewiseAggregateApproximation, \
     SymbolicAggregateApproximation, OneD_SymbolicAggregateApproximation
```

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_shapelets.py` & `tslearn-0.6.0/tslearn/tests/test_shapelets.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_utils.py` & `tslearn-0.6.0/tslearn/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/tests/test_variablelength.py` & `tslearn-0.6.0/tslearn/tests/test_variablelength.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/utils/__init__.py` & `tslearn-0.6.0/tslearn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/utils/cast.py` & `tslearn-0.6.0/tslearn/utils/cast.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.5.3.2/tslearn/utils/utils.py` & `tslearn-0.6.0/tslearn/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 import numpy
 from sklearn.base import TransformerMixin
 from sklearn.utils import column_or_1d
 from sklearn.utils.validation import check_is_fitted
 
 try:
     from scipy.io import arff
+
     HAS_ARFF = True
 except:
     HAS_ARFF = False
 
 try:
     from sklearn.utils.estimator_checks import _NotAnArray as NotAnArray
 except ImportError:  # Old sklearn versions
     from sklearn.utils.estimator_checks import NotAnArray
+from tslearn.backend import instantiate_backend
 from tslearn.bases import TimeSeriesBaseEstimator
 
-__author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
+__author__ = "Romain Tavenard romain.tavenard[at]univ-rennes2.fr"
 
 
 def check_dims(X, X_fit_dims=None, extend=True, check_n_features_only=False):
     """Reshapes X to a 3-dimensional array of X.shape[0] univariate
     timeseries of length X.shape[1] if X is 2-dimensional and extend
     is True. Then checks whether the provided X_fit_dims and the
     dimensions of X (except for the first one), match.
@@ -78,51 +80,55 @@
     ------
     ValueError
         Will raise exception if X is None or (if X_fit_dims is provided) one
         of the dimensions of the provided data, except the first, does not
         match X_fit_dims.
     """
     if X is None:
-        raise ValueError('X is equal to None!')
+        raise ValueError("X is equal to None!")
 
     if extend and len(X.shape) == 2:
-        warnings.warn('2-Dimensional data passed. Assuming these are '
-                      '{} 1-dimensional timeseries'.format(X.shape[0]))
+        warnings.warn(
+            "2-Dimensional data passed. Assuming these are "
+            "{} 1-dimensional timeseries".format(X.shape[0])
+        )
         X = X.reshape((X.shape) + (1,))
 
     if X_fit_dims is not None:
         if check_n_features_only:
             if X_fit_dims[2] != X.shape[2]:
                 raise ValueError(
-                    'Number of features of the provided timeseries'
-                    '(last dimension) must match the one of the fitted data!'
-                    ' ({} and {} are passed shapes)'.format(X_fit_dims,
-                                                            X.shape))
+                    "Number of features of the provided timeseries"
+                    "(last dimension) must match the one of the fitted data!"
+                    " ({} and {} are passed shapes)".format(X_fit_dims, X.shape)
+                )
         else:
             if X_fit_dims[1:] != X.shape[1:]:
                 raise ValueError(
-                    'Dimensions of the provided timeseries'
-                    '(except first) must match those of the fitted data!'
-                    ' ({} and {} are passed shapes)'.format(X_fit_dims,
-                                                            X.shape))
+                    "Dimensions of the provided timeseries"
+                    "(except first) must match those of the fitted data!"
+                    " ({} and {} are passed shapes)".format(X_fit_dims, X.shape)
+                )
 
     return X
 
 
-def to_time_series(ts, remove_nans=False):
+def to_time_series(ts, remove_nans=False, be=None):
     """Transforms a time series so that it fits the format used in ``tslearn``
     models.
 
     Parameters
     ----------
     ts : array-like
         The time series to be transformed.
     remove_nans : bool (default: False)
         Whether trailing NaNs at the end of the time series should be removed
         or not
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     numpy.ndarray of shape (sz, d)
         The transformed time series. This is always guaraneteed to be a new
         time series and never just a view into the old one.
 
@@ -139,25 +145,26 @@
     array([[1.],
            [2.]])
 
     See Also
     --------
     to_time_series_dataset : Transforms a dataset of time series
     """
-    ts_out = numpy.array(ts, copy=True)
+    be = instantiate_backend(be, ts)
+    ts_out = be.array(ts)
     if ts_out.ndim <= 1:
-        ts_out = ts_out.reshape((-1, 1))
-    if ts_out.dtype != float:
-        ts_out = ts_out.astype(float)
+        ts_out = be.reshape(ts_out, (-1, 1))
+    if not be.is_float(ts_out):
+        ts_out = be.cast(ts_out, dtype=float)
     if remove_nans:
-        ts_out = ts_out[:ts_size(ts_out)]
+        ts_out = ts_out[: ts_size(ts_out, be=be)]
     return ts_out
 
 
-def to_time_series_dataset(dataset, dtype=float):
+def to_time_series_dataset(dataset, dtype=float, be=None):
     """Transforms a time series dataset so that it fits the format used in
     ``tslearn`` models.
 
     Parameters
     ----------
     dataset : array-like
         The dataset of time series to be transformed. A single time series will
@@ -189,35 +196,39 @@
     >>> to_time_series_dataset([]).shape
     (0, 0, 0)
 
     See Also
     --------
     to_time_series : Transforms a single time series
     """
+    be = instantiate_backend(be, dataset)
+
     try:
         import pandas as pd
+
         if isinstance(dataset, pd.DataFrame):
-            return to_time_series_dataset(numpy.array(dataset))
+            return to_time_series_dataset(be.array(dataset), be=be)
     except ImportError:
         pass
     if isinstance(dataset, NotAnArray):  # Patch to pass sklearn tests
-        return to_time_series_dataset(numpy.array(dataset))
+        return to_time_series_dataset(be.array(dataset), be=be)
     if len(dataset) == 0:
-        return numpy.zeros((0, 0, 0))
-    if numpy.array(dataset[0]).ndim == 0:
+        return be.zeros((0, 0, 0))
+    if be.ndim(be.array(dataset[0])) == 0:
         dataset = [dataset]
     n_ts = len(dataset)
-    max_sz = max([ts_size(to_time_series(ts, remove_nans=True))
-                  for ts in dataset])
-    d = to_time_series(dataset[0]).shape[1]
-    dataset_out = numpy.zeros((n_ts, max_sz, d), dtype=dtype) + numpy.nan
+    max_sz = max(
+        [ts_size(to_time_series(ts, remove_nans=True, be=be)) for ts in dataset]
+    )
+    d = be.shape(to_time_series(dataset[0], be=be))[1]
+    dataset_out = be.zeros((n_ts, max_sz, d), dtype=dtype) + be.nan
     for i in range(n_ts):
-        ts = to_time_series(dataset[i], remove_nans=True)
-        dataset_out[i, :ts.shape[0]] = ts
-    return dataset_out.astype(dtype)
+        ts = to_time_series(dataset[i], remove_nans=True, be=be)
+        dataset_out[i, : ts.shape[0]] = ts
+    return be.cast(dataset_out, dtype=dtype)
 
 
 def time_series_to_str(ts, fmt="%.18e"):
     """Transforms a time series to its representation as a string (used when
     saving time series to disk).
 
     Parameters
@@ -340,24 +351,23 @@
     >>> reloaded_dataset = load_time_series_txt("tmp-tslearn-test.txt")
 
     See Also
     --------
     save_time_series_txt : Save time series to disk
     """
     with open(fname, "r") as f:
-        return to_time_series_dataset([
-            str_to_time_series(row)
-            for row in f.readlines()
-        ])
+        return to_time_series_dataset(
+            [str_to_time_series(row) for row in f.readlines()]
+        )
 
 
 load_timeseries_txt = load_time_series_txt
 
 
-def check_equal_size(dataset):
+def check_equal_size(dataset, be=None):
     """Check if all time series in the dataset have the same size.
 
     Parameters
     ----------
     dataset: array-like
         The dataset to check.
 
@@ -371,33 +381,37 @@
     >>> check_equal_size([[1, 2, 3], [4, 5, 6], [5, 3, 2]])
     True
     >>> check_equal_size([[1, 2, 3, 4], [4, 5, 6], [5, 3, 2]])
     False
     >>> check_equal_size([])
     True
     """
-    dataset_ = to_time_series_dataset(dataset)
+    be = instantiate_backend(be, dataset)
+
+    dataset_ = to_time_series_dataset(dataset, be=be)
     if len(dataset_) == 0:
         return True
 
-    size = ts_size(dataset[0])
+    size = ts_size(dataset[0], be=be)
     return all(ts_size(ds) == size for ds in dataset_[1:])
 
 
-def ts_size(ts):
+def ts_size(ts, be=None):
     """Returns actual time series size.
 
     Final timesteps that have `NaN` values for all dimensions will be removed
     from the count. Infinity and negative infinity ar considered valid time
     series values.
 
     Parameters
     ----------
     ts : array-like
         A time series.
+    be : Backend object or string or None
+        Backend.
 
     Returns
     -------
     int
         Actual size of the time series.
 
     Examples
@@ -413,17 +427,18 @@
     ...          [3, 4],
     ...          [numpy.nan, 2],
     ...          [numpy.nan, numpy.nan]])
     4
     >>> ts_size([numpy.nan, 3, numpy.inf, numpy.nan])
     3
     """
-    ts_ = to_time_series(ts)
-    sz = ts_.shape[0]
-    while sz > 0 and numpy.all(numpy.isnan(ts_[sz - 1])):
+    be = instantiate_backend(be, ts)
+    ts_ = to_time_series(ts, be=be)
+    sz = be.shape(ts_)[0]
+    while sz > 0 and be.all(be.isnan(ts_[sz - 1])):
         sz -= 1
     return sz
 
 
 def ts_zeros(sz, d=1):
     """Returns a time series made of zero values.
 
@@ -447,16 +462,17 @@
            [0., 0.]])
     >>> ts_zeros(5).shape
     (5, 1)
     """
     return numpy.zeros((sz, d))
 
 
-def check_dataset(X, force_univariate=False, force_equal_length=False,
-                  force_single_time_series=False):
+def check_dataset(
+    X, force_univariate=False, force_equal_length=False, force_single_time_series=False
+):
     """Check if X is a valid tslearn dataset, with possibly additional extra
     constraints.
 
     Parameters
     ----------
     X: array, shape = (n_ts, sz, d)
         Time series dataset.
@@ -508,24 +524,25 @@
     Traceback (most recent call last):
     ...
     ValueError: Array should be made of a single time series (3 here)
     """
     X_ = to_time_series_dataset(X)
     if force_univariate and X_.shape[2] != 1:
         raise ValueError(
-            "Array should be univariate and is of shape: {}".format(
-                X_.shape
-            )
+            "Array should be univariate and is of shape: {}".format(X_.shape)
         )
     if force_equal_length and not check_equal_size(X_):
-        raise ValueError("All the time series in the array should be of "
-                         "equal lengths")
+        raise ValueError(
+            "All the time series in the array should be of " "equal lengths"
+        )
     if force_single_time_series and X_.shape[0] != 1:
-        raise ValueError("Array should be made of a single time series "
-                         "({} here)".format(X_.shape[0]))
+        raise ValueError(
+            "Array should be made of a single time series "
+            "({} here)".format(X_.shape[0])
+        )
     return X_
 
 
 class LabelCategorizer(TransformerMixin, TimeSeriesBaseEstimator):
     """Transformer to transform indicator-based labels into categorical ones.
 
     Attributes
@@ -565,16 +582,18 @@
     >>> lc.inverse_transform(lc.transform(y))
     array([-1.,  2., -1., -1.,  2.])
 
     References
     ----------
     .. [1] J. Grabocka et al. Learning Time-Series Shapelets. SIGKDD 2014.
     """
-    def __init__(self, single_column_if_binary=False, forward_match=None,
-                 backward_match=None):
+
+    def __init__(
+        self, single_column_if_binary=False, forward_match=None, backward_match=None
+    ):
         self.single_column_if_binary = single_column_if_binary
         self.forward_match = forward_match
         self.backward_match = backward_match
 
     def _init(self):
         self.forward_match = {}
         self.backward_match = []
@@ -585,33 +604,33 @@
         values = sorted(set(y))
         for i, v in enumerate(values):
             self.forward_match[v] = i
             self.backward_match.append(v)
         return self
 
     def transform(self, y):
-        check_is_fitted(self, ['backward_match', 'forward_match'])
+        check_is_fitted(self, ["backward_match", "forward_match"])
         y = column_or_1d(y, warn=True)
         n_classes = len(self.backward_match)
         n = len(y)
         y_out = numpy.zeros((n, n_classes))
         for i in range(n):
             y_out[i, self.forward_match[y[i]]] = 1
         if n_classes == 2 and self.single_column_if_binary:
             return y_out[:, 0].reshape((-1, 1))
         else:
             return y_out
 
     def inverse_transform(self, y):
-        check_is_fitted(self, ['backward_match', 'forward_match'])
+        check_is_fitted(self, ["backward_match", "forward_match"])
         y_ = numpy.array(y)
         n, n_c = y_.shape
         if n_c == 1 and self.single_column_if_binary:
             y_ = numpy.hstack((y_, 1 - y_))
-        y_out = numpy.zeros((n, ))
+        y_out = numpy.zeros((n,))
         for i in range(n):
             y_out[i] = self.backward_match[y_[i].argmax()]
         return y_out
 
     def get_params(self, deep=True):
         """Get parameters for this estimator.
         Parameters
@@ -627,20 +646,20 @@
         out = TimeSeriesBaseEstimator.get_params(self, deep=deep)
         out["single_column_if_binary"] = self.single_column_if_binary
         out["forward_match"] = self.forward_match
         out["backward_match"] = self.backward_match
         return out
 
     def _more_tags(self):
-        return {'X_types': ['1dlabels']}
+        return {"X_types": ["1dlabels"]}
 
 
 def _load_arff_uea(dataset_path):
     """Load arff file for uni/multi variate dataset
-    
+
     Parameters
     ----------
     dataset_path: string of dataset_path
         Path to the ARFF file to be read
 
     Returns
     -------
@@ -652,16 +671,18 @@
     Raises
     ------
     ImportError: if the version of *Scipy* is too old (pre 1.3.0)
     Exception: on any failure, e.g. if the given file does not exist or is
                corrupted
     """
     if not HAS_ARFF:
-        raise ImportError("scipy 1.3.0 or newer is required to load "
-                          "time series datasets from arff format.")
+        raise ImportError(
+            "scipy 1.3.0 or newer is required to load "
+            "time series datasets from arff format."
+        )
     data, meta = arff.loadarff(dataset_path)
     names = meta.names()  # ["input", "class"] for multi-variate
 
     # firstly get y_train
     y_ = data[names[-1]]  # data["class"]
     y = numpy.array(y_).astype("str")
```

