# Comparing `tmp/opendr-toolkit-multimodal-human-centric-2.1.0.tar.gz` & `tmp/opendr-toolkit-multimodal-human-centric-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-multimodal-human-centric-2.1.0.tar", last modified: Wed Feb 22 08:10:26 2023, max compression
+gzip compressed data, was "opendr-toolkit-multimodal-human-centric-2.2.0.tar", last modified: Mon Jul  3 13:34:48 2023, max compression
```

## Comparing `opendr-toolkit-multimodal-human-centric-2.1.0.tar` & `opendr-toolkit-multimodal-human-centric-2.2.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-02-22 08:10:26.000000 opendr-toolkit-multimodal-human-centric-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-multimodal-human-centric-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-02-22 08:10:26.000000 opendr-toolkit-multimodal-human-centric-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.435809 opendr-toolkit-multimodal-human-centric-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.439809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.439809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.439809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.439809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.439809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.439809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/README.MD
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4108 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_modulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     5884 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12296 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/trainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/transformer_timm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    19501 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/avlearner.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/dependencies.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13344 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/densenet.py
--rw-r--r--   0 runner    (1001) docker     (122)    12597 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mnasnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     8971 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (122)    16168 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/vgg.py
--rw-r--r--   0 runner    (1001) docker     (122)     6608 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    20479 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/rgbd_hand_gesture_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:26.443809 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-02-22 08:10:26.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-02-22 08:10:26.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:26.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-02-22 08:10:26.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:26.000000 opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.314808 opendr-toolkit-multimodal-human-centric-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-07-03 13:34:48.000000 opendr-toolkit-multimodal-human-centric-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-07-03 13:34:48.314808 opendr-toolkit-multimodal-human-centric-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-multimodal-human-centric-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:48.314808 opendr-toolkit-multimodal-human-centric-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-03 13:34:48.000000 opendr-toolkit-multimodal-human-centric-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.306808 opendr-toolkit-multimodal-human-centric-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/README.MD
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4108 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_modulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5884 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12296 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/transformer_timm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19501 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/avlearner.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/dependencies.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13434 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12687 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mnasnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9060 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16257 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7038 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6608 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20479 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/rgbd_hand_gesture_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.310808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:48.314808 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-07-03 13:34:48.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-07-03 13:34:48.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:48.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-03 13:34:48.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:48.000000 opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/.clang-format` & `opendr-toolkit-multimodal-human-centric-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/.gitignore` & `opendr-toolkit-multimodal-human-centric-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/CHANGELOG.md` & `opendr-toolkit-multimodal-human-centric-2.2.0/CHANGELOG.md`

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

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-multimodal-human-centric-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/Dockerfile` & `opendr-toolkit-multimodal-human-centric-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/Dockerfile-cuda` & `opendr-toolkit-multimodal-human-centric-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/Dockerfile-embedded` & `opendr-toolkit-multimodal-human-centric-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/LICENSE` & `opendr-toolkit-multimodal-human-centric-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/Makefile` & `opendr-toolkit-multimodal-human-centric-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/PKG-INFO` & `opendr-toolkit-multimodal-human-centric-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-multimodal-human-centric
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/multimodal_human_centric)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/README.md` & `opendr-toolkit-multimodal-human-centric-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/description.txt` & `opendr-toolkit-multimodal-human-centric-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/packages.txt` & `opendr-toolkit-multimodal-human-centric-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/_version.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/constants.py`

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

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/_version.py`

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

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/__init__.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data_utils.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/data_utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_modulator.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_modulator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_utils.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/efficientface_utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/models.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/models.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/spatial_transforms.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/trainer.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/trainer.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/transformer_timm.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/transformer_timm.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/utils.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/avlearner.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/audiovisual_emotion_learner/avlearner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/README.md` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/__init__.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/__init__.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/densenet.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/densenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,21 @@
 
 import re
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint as cp
 from collections import OrderedDict
-from torchvision.models.utils import load_state_dict_from_url
 from torch import Tensor
 
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
+
 
 __all__ = ['DenseNet', 'densenet121', 'densenet169', 'densenet201', 'densenet161']
 
 model_urls = {
     'densenet121': 'https://download.pytorch.org/models/densenet121-a639ec97.pth',
     'densenet169': 'https://download.pytorch.org/models/densenet169-b2777c0a.pth',
     'densenet201': 'https://download.pytorch.org/models/densenet201-c1103571.pth',
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mnasnet.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mnasnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 import warnings
 import torch
 import torch.nn as nn
-from torchvision.models.utils import load_state_dict_from_url
+
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
 
 __all__ = ['MNASNet', 'mnasnet0_5', 'mnasnet0_75', 'mnasnet1_0', 'mnasnet1_3']
 
 model_urls = {
     "mnasnet0_5":
     "https://download.pytorch.org/models/mnasnet0.5_top1_67.823-3ffadce67e.pth",
     "mnasnet1_0":
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mobilenet.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/mobilenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 from torch import nn
-from torchvision.models.utils import load_state_dict_from_url
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
 
 
 __all__ = ['MobileNetV2', 'mobilenet_v2']
 
 
 model_urls = {
     'mobilenet_v2': 'https://download.pytorch.org/models/mobilenet_v2-b0353104.pth',
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/resnet.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,19 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 import torch
 import torch.nn as nn
-from torchvision.models.utils import load_state_dict_from_url
 
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
 
 __all__ = ['ResNet', 'resnet18', 'resnet34', 'resnet50', 'resnet101',
            'resnet152', 'resnext50_32x4d', 'resnext101_32x8d',
            'wide_resnet50_2', 'wide_resnet101_2']
 
 
 model_urls = {
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/vgg.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/architectures/vgg.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,21 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import torch.nn as nn
-from torchvision.models.utils import load_state_dict_from_url
 from torchvision.models.vgg import VGG, model_urls, cfgs
 
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
+
 
 def make_layers(cfg, batch_norm=False):
     layers = []
     in_channels = 4
     for v in cfg:
         if v == 'M':
             layers += [nn.MaxPool2d(kernel_size=2, stride=2)]
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/data.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/algorithm/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/rgbd_hand_gesture_learner.py` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr/perception/multimodal_human_centric/rgbd_hand_gesture_learner/rgbd_hand_gesture_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/PKG-INFO` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-multimodal-human-centric
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/multimodal_human_centric)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-multimodal-human-centric-2.1.0/src/opendr_toolkit_multimodal_human_centric.egg-info/SOURCES.txt` & `opendr-toolkit-multimodal-human-centric-2.2.0/src/opendr_toolkit_multimodal_human_centric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

