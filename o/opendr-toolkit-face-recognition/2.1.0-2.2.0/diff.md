# Comparing `tmp/opendr-toolkit-face-recognition-2.1.0.tar.gz` & `tmp/opendr-toolkit-face-recognition-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-face-recognition-2.1.0.tar", last modified: Wed Feb 22 08:10:24 2023, max compression
+gzip compressed data, was "opendr-toolkit-face-recognition-2.2.0.tar", last modified: Mon Jul  3 13:34:46 2023, max compression
```

## Comparing `opendr-toolkit-face-recognition-2.1.0.tar` & `opendr-toolkit-face-recognition-2.2.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-02-22 08:10:24.000000 opendr-toolkit-face-recognition-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-face-recognition-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-02-22 08:10:24.000000 opendr-toolkit-face-recognition-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.543779 opendr-toolkit-face-recognition-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.543779 opendr-toolkit-face-recognition-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.543779 opendr-toolkit-face-recognition-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.543779 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.543779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.543779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.543779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.547779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1848 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/align.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8064 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/align_trans.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5572 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/box_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4170 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/detector.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3020 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/first_stage.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5120 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/get_nets.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8320 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/matlab_cp2tform.py
--rwxr-xr-x   0 runner    (1001) docker     (122)  2345483 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/onet.npy
--rwxr-xr-x   0 runner    (1001) docker     (122)    41271 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/pnet.npy
--rwxr-xr-x   0 runner    (1001) docker     (122)   604651 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/rnet.npy
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7416 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/model_irse.py
--rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/model_mobilenet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5692 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/model_resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/head/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/head/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8630 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/head/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/loss/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/loss/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      444 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/loss/focal.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      602 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/iterator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10733 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5545 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/verification.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)    44670 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/face_recognition_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:24.551779 opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-02-22 08:10:24.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-02-22 08:10:24.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:24.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-02-22 08:10:24.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:24.000000 opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.346772 opendr-toolkit-face-recognition-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-07-03 13:34:46.000000 opendr-toolkit-face-recognition-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-face-recognition-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:46.346772 opendr-toolkit-face-recognition-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-07-03 13:34:46.000000 opendr-toolkit-face-recognition-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.334771 opendr-toolkit-face-recognition-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.334771 opendr-toolkit-face-recognition-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.334771 opendr-toolkit-face-recognition-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.338771 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.338771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.338771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.338771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1848 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/align.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8064 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/align_trans.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5572 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/box_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4170 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/detector.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3020 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/first_stage.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5120 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/get_nets.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8320 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/matlab_cp2tform.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)  2345483 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/onet.npy
+-rwxr-xr-x   0 runner    (1001) docker     (122)    41271 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/pnet.npy
+-rwxr-xr-x   0 runner    (1001) docker     (122)   604651 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/rnet.npy
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7416 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/model_irse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/model_mobilenet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5692 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/model_resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/head/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/head/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8630 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/head/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/loss/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/loss/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      444 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/loss/focal.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      602 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10733 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5545 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/verification.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    44654 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/face_recognition_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:46.342771 opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-07-03 13:34:46.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-07-03 13:34:46.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:46.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-07-03 13:34:46.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:46.000000 opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-face-recognition-2.1.0/.clang-format` & `opendr-toolkit-face-recognition-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/.gitignore` & `opendr-toolkit-face-recognition-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/CHANGELOG.md` & `opendr-toolkit-face-recognition-2.2.0/CHANGELOG.md`

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

### Comparing `opendr-toolkit-face-recognition-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-face-recognition-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/Dockerfile` & `opendr-toolkit-face-recognition-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/Dockerfile-cuda` & `opendr-toolkit-face-recognition-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/Dockerfile-embedded` & `opendr-toolkit-face-recognition-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/LICENSE` & `opendr-toolkit-face-recognition-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/Makefile` & `opendr-toolkit-face-recognition-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/PKG-INFO` & `opendr-toolkit-face-recognition-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-face-recognition
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/face_recognition)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-face-recognition-2.1.0/README.md` & `opendr-toolkit-face-recognition-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/description.txt` & `opendr-toolkit-face-recognition-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/packages.txt` & `opendr-toolkit-face-recognition-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/_version.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/constants.py`

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

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/_version.py`

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

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/README.md` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/align.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/align.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/align_trans.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/align_trans.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/box_utils.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/box_utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/detector.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/detector.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/first_stage.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/first_stage.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/get_nets.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/get_nets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/matlab_cp2tform.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/onet.npy` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/onet.npy`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/pnet.npy` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/pnet.npy`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/align/rnet.npy` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/align/rnet.npy`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/model_irse.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/model_irse.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/model_mobilenet.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/model_mobilenet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/backbone/model_resnet.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/backbone/model_resnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/head/losses.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/head/losses.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/iterator.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/iterator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/utils.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/algorithm/util/verification.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/algorithm/util/verification.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr/perception/face_recognition/face_recognition_learner.py` & `opendr-toolkit-face-recognition-2.2.0/src/opendr/perception/face_recognition/face_recognition_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -842,25 +842,25 @@
         if 'cuda' in self.device:
             inp = torch.randn(1, 3, self.input_size[0], self.input_size[1]).to(self.device)
         else:
             inp = torch.randn(1, 3, self.input_size[0], self.input_size[1])
         input_names = ['data']
         output_names = ['features']
         output_name = os.path.join(self.temp_path, 'onnx_' + self.backbone + '_backbone_model.onnx')
-        torch.onnx.export(self.backbone_model, inp, output_name, verbose=verbose, enable_onnx_checker=True,
+        torch.onnx.export(self.backbone_model, inp, output_name, verbose=verbose, opset_version=11,
                           input_names=input_names, output_names=output_names)
         if self.mode == 'full' and self.network_head == 'classifier':
             if 'cuda' in self.device:
                 inp = torch.randn(1, self.embedding_size).to(self.device)
             else:
                 inp = torch.randn(1, self.embedding_size)
             input_names = ['features']
             output_names = ['classes']
             output_name = os.path.join(self.temp_path, 'onnx_' + self.network_head + '_head_model.onnx')
-            torch.onnx.export(self.network_head_model, inp, output_name, verbose=verbose, enable_onnx_checker=True,
+            torch.onnx.export(self.network_head_model, inp, output_name, verbose=verbose, opset_version=11,
                               input_names=input_names, output_names=output_names)
 
     def optimize(self, do_constant_folding=False):
         """
         Optimize method converts the model to ONNX format and saves the
         model in the parent directory defined by self.temp_path. The ONNX model is then loaded.
         :param do_constant_folding: whether to optimize constants, defaults to 'False'
```

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/PKG-INFO` & `opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-face-recognition
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/face_recognition)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-face-recognition-2.1.0/src/opendr_toolkit_face_recognition.egg-info/SOURCES.txt` & `opendr-toolkit-face-recognition-2.2.0/src/opendr_toolkit_face_recognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

