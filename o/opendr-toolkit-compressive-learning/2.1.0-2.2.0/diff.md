# Comparing `tmp/opendr-toolkit-compressive-learning-2.1.0.tar.gz` & `tmp/opendr-toolkit-compressive-learning-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-compressive-learning-2.1.0.tar", last modified: Wed Feb 22 08:10:25 2023, max compression
+gzip compressed data, was "opendr-toolkit-compressive-learning-2.2.0.tar", last modified: Mon Jul  3 13:34:47 2023, max compression
```

## Comparing `opendr-toolkit-compressive-learning-2.1.0.tar` & `opendr-toolkit-compressive-learning-2.2.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.847794 opendr-toolkit-compressive-learning-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-02-22 08:10:25.000000 opendr-toolkit-compressive-learning-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-02-22 08:10:25.847794 opendr-toolkit-compressive-learning-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-compressive-learning-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:25.847794 opendr-toolkit-compressive-learning-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-02-22 08:10:25.000000 opendr-toolkit-compressive-learning-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.839794 opendr-toolkit-compressive-learning-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/dependencies.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_allcnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     7370 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_densenet.py
--rw-r--r--   0 runner    (1001) docker     (122)     9872 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5088 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_vgg.py
--rw-r--r--   0 runner    (1001) docker     (122)     4842 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_densenet.py
--rw-r--r--   0 runner    (1001) docker     (122)     4388 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3718 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5347 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    17637 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/trainers.py
--rw-r--r--   0 runner    (1001) docker     (122)    28993 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/multilinear_compressive_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.843794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.847794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.847794 opendr-toolkit-compressive-learning-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:25.847794 opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-02-22 08:10:25.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-02-22 08:10:25.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:25.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-02-22 08:10:25.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:25.000000 opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.686795 opendr-toolkit-compressive-learning-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-03 13:34:47.000000 opendr-toolkit-compressive-learning-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-compressive-learning-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:47.686795 opendr-toolkit-compressive-learning-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-03 13:34:47.000000 opendr-toolkit-compressive-learning-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.678795 opendr-toolkit-compressive-learning-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.678795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.678795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/dependencies.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_allcnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7370 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9872 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5088 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4912 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4526 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3859 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5347 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17637 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28993 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/multilinear_compressive_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:47.682795 opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-07-03 13:34:47.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-07-03 13:34:47.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:47.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-03 13:34:47.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:47.000000 opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-compressive-learning-2.1.0/.clang-format` & `opendr-toolkit-compressive-learning-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/.gitignore` & `opendr-toolkit-compressive-learning-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/CHANGELOG.md` & `opendr-toolkit-compressive-learning-2.2.0/CHANGELOG.md`

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

### Comparing `opendr-toolkit-compressive-learning-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-compressive-learning-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/Dockerfile` & `opendr-toolkit-compressive-learning-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/Dockerfile-cuda` & `opendr-toolkit-compressive-learning-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/Dockerfile-embedded` & `opendr-toolkit-compressive-learning-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/LICENSE` & `opendr-toolkit-compressive-learning-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/Makefile` & `opendr-toolkit-compressive-learning-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/PKG-INFO` & `opendr-toolkit-compressive-learning-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-compressive-learning
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/compressive_learning)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-compressive-learning-2.1.0/README.md` & `opendr-toolkit-compressive-learning-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/description.txt` & `opendr-toolkit-compressive-learning-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/packages.txt` & `opendr-toolkit-compressive-learning-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/_version.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/constants.py`

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

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/_version.py`

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

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/__init__.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/__init__.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_allcnn.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_allcnn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_densenet.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_densenet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_resnet.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_resnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_vgg.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/cifar_vgg.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_densenet.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_densenet.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch.nn as nn
 import torchvision.models.densenet as densenet_models
 import re
 
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
+
 getters = {'densenet121': densenet_models.densenet121,
            'densenet161': densenet_models.densenet161,
            'densenet169': densenet_models.densenet169,
            'densenet201': densenet_models.densenet201,
            }
 
 
@@ -50,16 +55,15 @@
         assert model_name in getters.keys()
         assert pretrained in ['', 'with_classifier', 'without_classifier']
 
         self.body = getters[model_name](pretrained=False, num_classes=n_class)
 
         if pretrained != '':
             # get pretrained weights
-            state_dict = densenet_models.load_state_dict_from_url(densenet_models.model_urls[model_name],
-                                                                  progress=False)
+            state_dict = load_state_dict_from_url(densenet_models.model_urls[model_name], progress=False)
 
             # fix naming issue
             # as in https://github.com/pytorch/vision/blob/master/torchvision/models/densenet.py
             pattern = re.compile(
                 r'^(.*denselayer\d+\.(?:norm|relu|conv))\.((?:[12])\.(?:weight|bias|running_mean|running_var))$')
 
             for key in list(state_dict.keys()):
```

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_resnet.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_resnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch.nn as nn
 import torchvision.models.resnet as resnet_models
 
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
+
 getters = {'resnet18': resnet_models.resnet18,
            'resnet34': resnet_models.resnet34,
            'resnet50': resnet_models.resnet50,
            'resnet101': resnet_models.resnet101,
            'resnet152': resnet_models.resnet152,
            'resnext50_32x4d': resnet_models.resnext50_32x4d,
            'resnext101_32x8d': resnet_models.resnext101_32x8d,
@@ -34,15 +39,15 @@
         assert model_name in getters.keys()
         assert pretrained in ['', 'with_classifier', 'without_classifier']
 
         self.body = getters[model_name](pretrained=False, num_classes=n_class)
 
         if pretrained != '':
             # get pretrained weights
-            state_dict = resnet_models.load_state_dict_from_url(resnet_models.model_urls[model_name], progress=False)
+            state_dict = load_state_dict_from_url(resnet_models.model_urls[model_name], progress=False)
 
             # remove the last classifier layer from pretrained weights
             if pretrained == 'without_classifier':
                 cur_state_dict = self.body.state_dict()
                 state_dict['fc.weight'] = cur_state_dict['fc.weight']
                 state_dict['fc.bias'] = cur_state_dict['fc.bias']
             else:
```

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_vgg.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/imagenet_vgg.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch.nn as nn
 import torchvision.models.vgg as vgg_models
 
+try:
+    from torch.hub import load_state_dict_from_url
+except ImportError:
+    from torch.utils.model_zoo import load_url as load_state_dict_from_url
+
 getters = {'vgg11': vgg_models.vgg11,
            'vgg11_bn': vgg_models.vgg11_bn,
            'vgg13': vgg_models.vgg13,
            'vgg13_bn': vgg_models.vgg13_bn,
            'vgg16': vgg_models.vgg16,
            'vgg16_bn': vgg_models.vgg16_bn,
            'vgg19': vgg_models.vgg19,
@@ -32,15 +37,15 @@
         assert model_name in getters.keys()
         assert pretrained in ['', 'with_classifier', 'without_classifier']
 
         self.body = getters[model_name](pretrained=False, num_classes=n_class)
 
         if pretrained != '':
             # get pretrained weights
-            state_dict = vgg_models.load_state_dict_from_url(vgg_models.model_urls[model_name], progress=False)
+            state_dict = load_state_dict_from_url(vgg_models.model_urls[model_name], progress=False)
 
             # remove the last classifier layer from pretrained weights
             if pretrained == 'without_classifier':
                 cur_state_dict = self.body.state_dict()
                 state_dict['classifier.6.weight'] = cur_state_dict['classifier.6.weight']
                 state_dict['classifier.6.bias'] = cur_state_dict['classifier.6.bias']
             else:
```

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/model_utils.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/backbones/model_utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/data.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/learner.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/trainers.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/algorithm/trainers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/multilinear_compressive_learner.py` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr/perception/compressive_learning/multilinear_compressive_learning/multilinear_compressive_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/PKG-INFO` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-compressive-learning
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/compressive_learning)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-compressive-learning-2.1.0/src/opendr_toolkit_compressive_learning.egg-info/SOURCES.txt` & `opendr-toolkit-compressive-learning-2.2.0/src/opendr_toolkit_compressive_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

