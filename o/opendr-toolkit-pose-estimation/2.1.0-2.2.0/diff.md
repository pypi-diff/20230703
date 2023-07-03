# Comparing `tmp/opendr-toolkit-pose-estimation-2.1.0.tar.gz` & `tmp/opendr-toolkit-pose-estimation-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-pose-estimation-2.1.0.tar", last modified: Wed Feb 22 08:10:25 2023, max compression
+gzip compressed data, was "opendr-toolkit-pose-estimation-2.2.0.tar", last modified: Mon Jul  3 13:34:47 2023, max compression
```

## Comparing `opendr-toolkit-pose-estimation-2.1.0.tar` & `opendr-toolkit-pose-estimation-2.2.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-02-22 08:10:25.000000 opendr-toolkit-pose-estimation-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-pose-estimation-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-02-22 08:10:25.000000 opendr-toolkit-pose-estimation-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.251782 opendr-toolkit-pose-estimation-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/dependencies.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/hr_pose_estimation/
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/hr_pose_estimation/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/hr_pose_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36318 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/hr_pose_estimation/high_resolution_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)     1870 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (122)    10002 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.255782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4932 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (122)     9714 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    15573 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_shufflenet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/get_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     8106 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (122)     1411 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/load_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/one_euro_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/make_val_subset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5932 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/prepare_train_labels.py
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/val.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/filtered_pose.py
--rw-r--r--   0 runner    (1001) docker     (122)    66998 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/lightweight_open_pose_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)     6476 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.259782 opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-02-22 08:10:25.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6152 2023-02-22 08:10:25.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:25.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-02-22 08:10:25.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:25.000000 opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-03 13:34:46.000000 opendr-toolkit-pose-estimation-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-pose-estimation-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-03 13:34:46.000000 opendr-toolkit-pose-estimation-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.062784 opendr-toolkit-pose-estimation-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/dependencies.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/hr_pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/hr_pose_estimation/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/hr_pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36318 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/hr_pose_estimation/high_resolution_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.066784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)     1870 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10002 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4932 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9714 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15573 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_shufflenet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/get_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8106 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1411 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/load_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/one_euro_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/make_val_subset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5932 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/prepare_train_labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/val.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/filtered_pose.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66990 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/lightweight_open_pose_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6476 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.070784 opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-07-03 13:34:47.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6152 2023-07-03 13:34:47.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:47.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-07-03 13:34:47.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:47.000000 opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-pose-estimation-2.1.0/.clang-format` & `opendr-toolkit-pose-estimation-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/.gitignore` & `opendr-toolkit-pose-estimation-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/CHANGELOG.md` & `opendr-toolkit-pose-estimation-2.2.0/CHANGELOG.md`

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

### Comparing `opendr-toolkit-pose-estimation-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-pose-estimation-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/Dockerfile` & `opendr-toolkit-pose-estimation-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/Dockerfile-cuda` & `opendr-toolkit-pose-estimation-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/Dockerfile-embedded` & `opendr-toolkit-pose-estimation-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/LICENSE` & `opendr-toolkit-pose-estimation-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/Makefile` & `opendr-toolkit-pose-estimation-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/PKG-INFO` & `opendr-toolkit-pose-estimation-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-pose-estimation
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/pose_estimation)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-pose-estimation-2.1.0/README.md` & `opendr-toolkit-pose-estimation-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/description.txt` & `opendr-toolkit-pose-estimation-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/packages.txt` & `opendr-toolkit-pose-estimation-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/_version.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/constants.py`

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

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/_version.py`

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

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/hr_pose_estimation/high_resolution_learner.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/hr_pose_estimation/high_resolution_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/README.md` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/coco.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/transformations.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/datasets/transformations.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet_v2.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_shufflenet.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/models/with_shufflenet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/conv.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/get_parameters.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/get_parameters.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/keypoints.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/keypoints.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/load_state.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/load_state.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/one_euro_filter.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/modules/one_euro_filter.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/make_val_subset.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/make_val_subset.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/prepare_train_labels.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/scripts/prepare_train_labels.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/val.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/algorithm/val.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/filtered_pose.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/filtered_pose.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/lightweight_open_pose_learner.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/lightweight_open_pose_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -853,15 +853,15 @@
             output_names = ['stage_0_output_1_heatmaps', 'stage_0_output_0_pafs',
                             'stage_1_output_1_heatmaps', 'stage_1_output_0_pafs',
                             'stage_2_output_1_heatmaps', 'stage_2_output_0_pafs']
 
         else:
             output_names = ['stage_0_output_1_heatmaps', 'stage_0_output_0_pafs']
 
-        torch.onnx.export(self.model, inp, output_name, verbose=verbose, enable_onnx_checker=True,
+        torch.onnx.export(self.model, inp, output_name, verbose=verbose, opset_version=11,
                           do_constant_folding=do_constant_folding, input_names=input_names, output_names=output_names,
                           dynamic_axes={"data": {3: "width"}})
 
     def optimize(self, do_constant_folding=False):
         """
         Optimize method converts the model to ONNX format and saves the
         model in the parent directory defined by self.temp_path. The ONNX model is then loaded.
```

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr/perception/pose_estimation/lightweight_open_pose/utilities.py` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr/perception/pose_estimation/lightweight_open_pose/utilities.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/PKG-INFO` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-pose-estimation
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/pose_estimation)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-pose-estimation-2.1.0/src/opendr_toolkit_pose_estimation.egg-info/SOURCES.txt` & `opendr-toolkit-pose-estimation-2.2.0/src/opendr_toolkit_pose_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

