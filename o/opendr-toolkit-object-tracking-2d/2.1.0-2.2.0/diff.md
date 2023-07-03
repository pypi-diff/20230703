# Comparing `tmp/opendr-toolkit-object-tracking-2d-2.1.0.tar.gz` & `tmp/opendr-toolkit-object-tracking-2d-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-object-tracking-2d-2.1.0.tar", last modified: Wed Feb 22 08:10:29 2023, max compression
+gzip compressed data, was "opendr-toolkit-object-tracking-2d-2.2.0.tar", last modified: Mon Jul  3 13:34:51 2023, max compression
```

## Comparing `opendr-toolkit-object-tracking-2d-2.1.0.tar` & `opendr-toolkit-object-tracking-2d-2.2.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.651859 opendr-toolkit-object-tracking-2d-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-02-22 08:10:29.000000 opendr-toolkit-object-tracking-2d-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-02-22 08:10:29.651859 opendr-toolkit-object-tracking-2d-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-object-tracking-2d-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:29.651859 opendr-toolkit-object-tracking-2d-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-02-22 08:10:29.000000 opendr-toolkit-object-tracking-2d-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.623859 opendr-toolkit-object-tracking-2d-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.627859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.627859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.627859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.627859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.627859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.627859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/market1501_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    45273 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/mot_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/otb_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.635859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/
--rw-r--r--   0 runner    (1001) docker     (122)   394093 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.10k.val
--rw-r--r--   0 runner    (1001) docker     (122)  1061896 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.all
--rw-r--r--   0 runner    (1001) docker     (122)  1054487 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.train
--rw-r--r--   0 runner    (1001) docker     (122)  1178127 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.val
--rw-r--r--   0 runner    (1001) docker     (122)   177486 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.train
--rw-r--r--   0 runner    (1001) docker     (122)    30956 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.val
--rw-r--r--   0 runner    (1001) docker     (122)   778820 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.train
--rw-r--r--   0 runner    (1001) docker     (122)   218219 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.val
--rw-r--r--   0 runner    (1001) docker     (122)   295563 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.train
--rw-r--r--   0 runner    (1001) docker     (122)    53809 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.val
--rw-r--r--   0 runner    (1001) docker     (122)    80184 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/eth.train
--rw-r--r--   0 runner    (1001) docker     (122)   254738 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot15.train
--rw-r--r--   0 runner    (1001) docker     (122)   233904 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot16.train
--rw-r--r--   0 runner    (1001) docker     (122)    42576 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.emb
--rw-r--r--   0 runner    (1001) docker     (122)   127536 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.half
--rw-r--r--   0 runner    (1001) docker     (122)   255168 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.train
--rw-r--r--   0 runner    (1001) docker     (122)   127632 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.val
--rw-r--r--   0 runner    (1001) docker     (122)   392964 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot20.train
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/nano_mot20.train
--rw-r--r--   0 runner    (1001) docker     (122)   153927 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.train
--rw-r--r--   0 runner    (1001) docker     (122)    54000 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.val
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.635859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/checkpoint/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/original_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4168 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     8117 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/track.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/tracker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort_tracker.py
--rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    12074 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    19264 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/object_tracking_2d_deep_sort_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/dependencies.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.639859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_crowd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_mot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.643859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.643859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5249 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/decode.py
--rw-r--r--   0 runner    (1001) docker     (122)     9568 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.643859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.643859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/default.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w18.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w32.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    23904 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/dlav0.py
--rw-r--r--   0 runner    (1001) docker     (122)    18269 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)    18551 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_dcn.py
--rw-r--r--   0 runner    (1001) docker     (122)    20111 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_hrnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_dcn.py
--rw-r--r--   0 runner    (1001) docker     (122)    10625 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_fpn_dcn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.643859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (122)     4722 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)    15434 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/multitracker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.643859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3756 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/nms.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/parse_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (122)    16157 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.643859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/base_trainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/mot.py
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/train_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.647859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7707 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/post_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     6589 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     4424 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/run.py
--rw-r--r--   0 runner    (1001) docker     (122)    24133 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/object_tracking_2d_fair_mot_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.647859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/
--rw-r--r--   0 runner    (1001) docker     (122)     2276 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.647859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/otb.py
--rw-r--r--   0 runner    (1001) docker     (122)    26245 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/siamrpn_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.647859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.647859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.647859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:29.647859 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-02-22 08:10:29.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20265 2023-02-22 08:10:29.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:29.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-02-22 08:10:29.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:29.000000 opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.818877 opendr-toolkit-object-tracking-2d-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-03 13:34:51.000000 opendr-toolkit-object-tracking-2d-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-07-03 13:34:51.818877 opendr-toolkit-object-tracking-2d-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-object-tracking-2d-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:51.818877 opendr-toolkit-object-tracking-2d-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-03 13:34:51.000000 opendr-toolkit-object-tracking-2d-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.790877 opendr-toolkit-object-tracking-2d-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.794877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.794877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.794877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.794877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.794877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.794877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/market1501_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45273 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/mot_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/otb_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.802877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/
+-rw-r--r--   0 runner    (1001) docker     (122)   394093 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.10k.val
+-rw-r--r--   0 runner    (1001) docker     (122)  1061896 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.all
+-rw-r--r--   0 runner    (1001) docker     (122)  1054487 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.train
+-rw-r--r--   0 runner    (1001) docker     (122)  1178127 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.val
+-rw-r--r--   0 runner    (1001) docker     (122)   177486 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.train
+-rw-r--r--   0 runner    (1001) docker     (122)    30956 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.val
+-rw-r--r--   0 runner    (1001) docker     (122)   778820 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.train
+-rw-r--r--   0 runner    (1001) docker     (122)   218219 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.val
+-rw-r--r--   0 runner    (1001) docker     (122)   295563 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.train
+-rw-r--r--   0 runner    (1001) docker     (122)    53809 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.val
+-rw-r--r--   0 runner    (1001) docker     (122)    80184 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/eth.train
+-rw-r--r--   0 runner    (1001) docker     (122)   254738 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot15.train
+-rw-r--r--   0 runner    (1001) docker     (122)   233904 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot16.train
+-rw-r--r--   0 runner    (1001) docker     (122)    42576 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.emb
+-rw-r--r--   0 runner    (1001) docker     (122)   127536 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.half
+-rw-r--r--   0 runner    (1001) docker     (122)   255168 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.train
+-rw-r--r--   0 runner    (1001) docker     (122)   127632 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.val
+-rw-r--r--   0 runner    (1001) docker     (122)   392964 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot20.train
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/nano_mot20.train
+-rw-r--r--   0 runner    (1001) docker     (122)   153927 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.train
+-rw-r--r--   0 runner    (1001) docker     (122)    54000 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.val
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.802877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/checkpoint/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/original_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4168 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8117 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12074 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19256 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/object_tracking_2d_deep_sort_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/dependencies.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.806877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_crowd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_mot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.810877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.810877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5249 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/decode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9568 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.810877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.810877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w18.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w32.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    23904 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/dlav0.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18269 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18551 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_dcn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20111 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_dcn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10625 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_fpn_dcn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.810877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4722 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15434 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/multitracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.810877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3756 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16157 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.810877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/base_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/mot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/train_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.814877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7707 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6589 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4424 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24390 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/object_tracking_2d_fair_mot_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.814877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/
+-rw-r--r--   0 runner    (1001) docker     (122)     2276 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.814877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/otb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26245 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/siamrpn_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.814877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.814877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.814877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:51.814877 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-07-03 13:34:51.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20265 2023-07-03 13:34:51.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:51.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-07-03 13:34:51.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:51.000000 opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/.clang-format` & `opendr-toolkit-object-tracking-2d-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/.gitignore` & `opendr-toolkit-object-tracking-2d-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/CHANGELOG.md` & `opendr-toolkit-object-tracking-2d-2.2.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # OpenDR Toolkit Change Log
 
+## Version 2.2.0
+Released on July, 3rd, 2023.
+
+  - Dependency Updates ([#431](https://github.com/opendr-eu/opendr/pull/431)):
+    - Updated PyTorch version from 1.9.0 to 1.13.1.
+    - Updated Torchvision version from 0.10.0 to 0.14.1.
+    - Updated Torchaudio version from 0.9.0 to 0.13.1.
+    - Downgraded wheel version to 0.38.4 due to bug in recent version.
+
 ## Version 2.1.0
 Released on February, 22nd, 2023.
 
   - New Features:
-    - Added YOLOv5 as an inference-only tool ([#360](https://github.com/opendr-eu/opendr/pull/360)).
     - Added Efficient LiDAR Panoptic Segmentation ([#359](https://github.com/opendr-eu/opendr/pull/359)).
     - Added Nanodet 2D Object Detection tool ([#352](https://github.com/opendr-eu/opendr/pull/352)).
     - Added C API implementations of NanoDet 2D Object Detection tool ([#352](https://github.com/opendr-eu/opendr/pull/352)).
     - Added C API implementations of forward pass of DETR 2D Object Detection tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
     - Added C API implementations of forward pass of DeepSORT 2D Object Tracking tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
     - Added C API implementations of forward pass of Lightweight OpenPose, Pose Estimator tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
     - Added C API implementations of forward pass of X3D 2D Activity Recognition tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-object-tracking-2d-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/Dockerfile` & `opendr-toolkit-object-tracking-2d-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/Dockerfile-cuda` & `opendr-toolkit-object-tracking-2d-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/Dockerfile-embedded` & `opendr-toolkit-object-tracking-2d-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/LICENSE` & `opendr-toolkit-object-tracking-2d-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/Makefile` & `opendr-toolkit-object-tracking-2d-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/PKG-INFO` & `opendr-toolkit-object-tracking-2d-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-object-tracking-2d
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/object_tracking_2d)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/README.md` & `opendr-toolkit-object-tracking-2d-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/description.txt` & `opendr-toolkit-object-tracking-2d-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/packages.txt` & `opendr-toolkit-object-tracking-2d-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/_version.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.1.0"
+OPENDR_SERVER_URL = "ftp://opendrdata.csd.auth.gr/"
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/_version.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-OPENDR_SERVER_URL = "ftp://opendrdata.csd.auth.gr/"
+__version__ = "2.2.0"
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/__init__.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/market1501_dataset.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/market1501_dataset.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/mot_dataset.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/mot_dataset.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/otb_dataset.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/otb_dataset.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.10k.val` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.10k.val`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.all` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.all`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.val` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/caltech.val`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.val` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/citypersons.val`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.val` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/crowdhuman.val`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.val` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/cuhksysu.val`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/eth.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/eth.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot15.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot15.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot16.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot16.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.emb` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.emb`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.half` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.half`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.val` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot17.val`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot20.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/mot20.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.train` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.train`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.val` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/datasets/splits/prw.val`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/LICENSE` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/feature_extractor.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/model.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/model.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/original_model.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep/original_model.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep_sort.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/deep_sort.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/detection.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/detection.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/iou_matching.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/iou_matching.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/kalman_filter.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/linear_assignment.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/nn_matching.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/nn_matching.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/preprocessing.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/track.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/track.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/tracker.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort/sort/tracker.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort_tracker.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/deep_sort_tracker.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/run.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/run.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/draw.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/draw.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/evaluation.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/io.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/io.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/json_logger.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/parser.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/parser.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/tools.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/algorithm/utils/tools.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/deep_sort/object_tracking_2d_deep_sort_learner.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/deep_sort/object_tracking_2d_deep_sort_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,15 @@
 
     def __convert_to_onnx(self, input_shape, output_name, do_constant_folding=False, verbose=False):
         inp = torch.randn(input_shape).to(self.device)
         input_names = ["data"]
         output_names = ["output"]
 
         torch.onnx.export(
-            self.tracker.deepsort.extractor.net, inp, output_name, verbose=verbose, enable_onnx_checker=True,
+            self.tracker.deepsort.extractor.net, inp, output_name, verbose=verbose, opset_version=11,
             do_constant_folding=do_constant_folding, input_names=input_names, output_names=output_names,
             dynamic_axes={"data": {0: "batch"}},
         )
 
     def __load_from_onnx(self, path):
         """
         This method loads an ONNX model from the path provided into an onnxruntime inference session.
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_crowd.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_crowd.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_mot.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/gen_labels_mot.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/logger.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/logger.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/data_parallel.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/data_parallel.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/decode.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/decode.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/losses.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/losses.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/model.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/model.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/default.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/default.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w18.yaml` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w18.yaml`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w32.yaml` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/config/hrnet_w32.yaml`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/dlav0.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/dlav0.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_conv.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_dcn.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_dla_dcn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_hrnet.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/pose_hrnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_dcn.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_dcn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_fpn_dcn.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/networks/resnet_fpn_dcn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/scatter_gather.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/utils.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/models/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/basetrack.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/matching.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/multitracker.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracker/multitracker.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/evaluation.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/io.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/io.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/kalman_filter.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/parse_config.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/parse_config.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/timer.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/timer.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/utils.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/visualization.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/tracking_utils/visualization.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/base_trainer.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/base_trainer.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/mot.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/trains/mot.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/image.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/image.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/post_process.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/post_process.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/utils.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/lib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/load.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/load.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/run.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/algorithm/run.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/fair_mot/object_tracking_2d_fair_mot_learner.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/fair_mot/object_tracking_2d_fair_mot_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -519,15 +519,15 @@
 
     def __convert_to_onnx(self, input_shape, output_name, do_constant_folding=False, verbose=False):
         inp = torch.randn(input_shape).to(self.device)
         input_names = ["data"]
         output_names = self.heads.keys()
 
         torch.onnx.export(
-            self.model, inp, output_name, verbose=verbose, enable_onnx_checker=True,
+            self.model, inp, output_name, verbose=verbose, opset_version=11,
             do_constant_folding=do_constant_folding, input_names=input_names, output_names=output_names
         )
 
     def __load_from_onnx(self, path):
         """
         This method loads an ONNX model from the path provided into an onnxruntime inference session.
 
@@ -545,14 +545,20 @@
         # onnx.checker.check_model(self.model)
         #
         # # Print a human readable representation of the graph
         # onnx.helper.printable_graph(self.model.graph)
 
     def __load_from_pth(self, model, path, use_original_dict=False):
         all_params = torch.load(path, map_location=self.device)
+        state_dict = all_params['state_dict']
+        new_dict = dict()
+        for name, tensor in state_dict.items():
+            new_name = name.replace('offset_mask', 'offset')
+            new_dict[new_name] = tensor
+        all_params['state_dict'] = new_dict
         model.load_state_dict(all_params if use_original_dict else all_params["state_dict"])
 
     def _prepare_datasets(
         self,
         dataset,
         val_dataset,
         train_split_paths,
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/logger.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/logger.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/README.md` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/otb.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/data_utils/otb.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr/perception/object_tracking_2d/siamrpn/siamrpn_learner.py` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr/perception/object_tracking_2d/siamrpn/siamrpn_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/PKG-INFO` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-object-tracking-2d
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/object_tracking_2d)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-object-tracking-2d-2.1.0/src/opendr_toolkit_object_tracking_2d.egg-info/SOURCES.txt` & `opendr-toolkit-object-tracking-2d-2.2.0/src/opendr_toolkit_object_tracking_2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

