# Comparing `tmp/opendr-toolkit-facial-expression-recognition-2.1.0.tar.gz` & `tmp/opendr-toolkit-facial-expression-recognition-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-facial-expression-recognition-2.1.0.tar", last modified: Wed Feb 22 08:10:26 2023, max compression
+gzip compressed data, was "opendr-toolkit-facial-expression-recognition-2.2.0.tar", last modified: Mon Jul  3 13:34:48 2023, max compression
```

## Comparing `opendr-toolkit-facial-expression-recognition-2.1.0.tar` & `opendr-toolkit-facial-expression-recognition-2.2.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.767817 opendr-toolkit-facial-expression-recognition-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-02-22 08:10:26.000000 opendr-toolkit-facial-expression-recognition-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-02-22 08:10:26.767817 opendr-toolkit-facial-expression-recognition-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-facial-expression-recognition-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:26.767817 opendr-toolkit-facial-expression-recognition-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-02-22 08:10:26.000000 opendr-toolkit-facial-expression-recognition-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.755817 opendr-toolkit-facial-expression-recognition-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.759817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.759817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.759817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.759817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.759817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.759817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.759817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4259 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/cbam.py
--rw-r--r--   0 runner    (1001) docker     (122)     8309 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/diversified_esr.py
--rw-r--r--   0 runner    (1001) docker     (122)     7711 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/esr_9.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16899 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/diversity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (122)     6320 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)    43666 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/facial_emotion_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/AFEW_data_gen.py
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/AFEW_labels.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CASIA_CK_data_gen.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CASIA_labels.csv
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CK+_labels.csv
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/data_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/frame_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/gen_facial_muscles_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/landmark_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2215 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5997 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/pstbln.py
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)    49108 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/progressive_spatio_temporal_bln_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.763817 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-02-22 08:10:26.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9390 2023-02-22 08:10:26.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:26.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-02-22 08:10:26.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:26.000000 opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-03 13:34:48.000000 opendr-toolkit-facial-expression-recognition-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-facial-expression-recognition-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-03 13:34:48.000000 opendr-toolkit-facial-expression-recognition-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.646814 opendr-toolkit-facial-expression-recognition-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4259 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/cbam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8309 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/diversified_esr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7711 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/esr_9.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.650814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16899 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6320 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    43721 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/facial_emotion_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/AFEW_data_gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/AFEW_labels.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CASIA_CK_data_gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CASIA_labels.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CK+_labels.csv
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/data_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/frame_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/gen_facial_muscles_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/landmark_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2215 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5997 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/pstbln.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    49100 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/progressive_spatio_temporal_bln_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.654814 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-07-03 13:34:48.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9390 2023-07-03 13:34:48.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:48.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-03 13:34:48.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:48.000000 opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/.clang-format` & `opendr-toolkit-facial-expression-recognition-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/.gitignore` & `opendr-toolkit-facial-expression-recognition-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/CHANGELOG.md` & `opendr-toolkit-facial-expression-recognition-2.2.0/CHANGELOG.md`

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

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-facial-expression-recognition-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/Dockerfile` & `opendr-toolkit-facial-expression-recognition-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/Dockerfile-cuda` & `opendr-toolkit-facial-expression-recognition-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/Dockerfile-embedded` & `opendr-toolkit-facial-expression-recognition-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/LICENSE` & `opendr-toolkit-facial-expression-recognition-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/Makefile` & `opendr-toolkit-facial-expression-recognition-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/PKG-INFO` & `opendr-toolkit-facial-expression-recognition-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-facial-expression-recognition
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/facial_expression_recognition)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/README.md` & `opendr-toolkit-facial-expression-recognition-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/description.txt` & `opendr-toolkit-facial-expression-recognition-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/packages.txt` & `opendr-toolkit-facial-expression-recognition-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/_version.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/constants.py`

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

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/_version.py`

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

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/__init__.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/README.md` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/__init__.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/cbam.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/cbam.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/diversified_esr.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/diversified_esr.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/esr_9.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/model/esr_9.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/datasets.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/diversity.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/diversity.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/image_processing.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/image_processing.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/plotting.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/algorithm/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/facial_emotion_learner.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/image_based_facial_emotion_estimation/facial_emotion_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 """
 
 # External Libraries
 from torch.utils.data import DataLoader
 from torchvision import transforms
 import torch.optim as optim
 import torch.nn as nn
-import PIL
 import numpy as np
 import zipfile
 import torch
 import os
 from os import path, makedirs
 import onnxruntime
 import shutil
 import json
 from urllib.request import urlretrieve
+from torchvision.transforms import InterpolationMode
 
 # OpenDR engine imports
 from opendr.engine.learners import Learner
 from opendr.engine.target import Category
 from opendr.engine.constants import OPENDR_SERVER_URL
 from opendr.perception.facial_expression_recognition.image_based_facial_emotion_estimation.algorithm.model.esr_9 \
     import ESR
@@ -168,15 +168,15 @@
             makedirs(path.join(self.base_path_experiment, self.name_experiment))
         # Define data transforms
         data_transforms = [transforms.ColorJitter(brightness=0.5, contrast=0.5),
                            transforms.RandomHorizontalFlip(p=0.5),
                            transforms.RandomAffine(degrees=30,
                                                    translate=(.1, .1),
                                                    scale=(1.0, 1.25),
-                                                   resample=PIL.Image.BILINEAR)]
+                                                   interpolation=InterpolationMode.BILINEAR)]
         if verbose:
             print("Starting: {}".format(str(self.name_experiment)))
             print("Running on {}".format(self.device))
 
         # Train a new model on AffectNet_Categorical from scratch
         if self.categorical_train:
             self.model = None
```

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/README.md` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/AFEW_data_gen.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/AFEW_data_gen.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CASIA_CK_data_gen.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/CASIA_CK_data_gen.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/data_augmentation.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/frame_extractor.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/frame_extractor.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/gen_facial_muscles_data.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/gen_facial_muscles_data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/landmark_extractor.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/datasets/landmark_extractor.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/feeder.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/pstbln.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/algorithm/models/pstbln.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/progressive_spatio_temporal_bln_learner.py` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr/perception/facial_expression_recognition/landmark_based_facial_expression_recognition/progressive_spatio_temporal_bln_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,15 +649,15 @@
         else:
             onnx_input = Variable(onnx_input.float(), requires_grad=False)
         # Export the model
         torch.onnx.export(self.model,  # model being run
                           onnx_input,  # model input (or a tuple for multiple inputs)
                           output_name,  # where to save the model (can be a file or file-like object)
                           verbose=verbose,
-                          enable_onnx_checker=True,
+                          opset_version=11,
                           do_constant_folding=do_constant_folding,
                           input_names=['onnx_input'],  # the model's input names
                           output_names=['onnx_output'],  # the model's output names
                           dynamic_axes={'onnx_input': {0: 'n'},  # variable lenght axes
                                         'onnx_output': {0: 'n'}})
 
         # This is a hack due to https://github.com/pytorch/pytorch/issues/72175 (see above)
```

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/PKG-INFO` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-facial-expression-recognition
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/facial_expression_recognition)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-facial-expression-recognition-2.1.0/src/opendr_toolkit_facial_expression_recognition.egg-info/SOURCES.txt` & `opendr-toolkit-facial-expression-recognition-2.2.0/src/opendr_toolkit_facial_expression_recognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

