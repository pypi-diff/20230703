# Comparing `tmp/PJYoloVision-0.0.1.tar.gz` & `tmp/PJYoloVision-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PJYoloVision-0.0.1.tar", last modified: Sun Jul  2 17:45:33 2023, max compression
+gzip compressed data, was "PJYoloVision-0.0.3.tar", last modified: Mon Jul  3 11:31:34 2023, max compression
```

## Comparing `PJYoloVision-0.0.1.tar` & `PJYoloVision-0.0.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    35149 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/LICENCE.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.521211 PJYoloVision-0.0.1/PJYoloVision/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4906 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/nn/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/nn/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5599 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/nn/autobackend.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    10975 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/nn/autoshape.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      867 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/nn/modules.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17463 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/nn/tasks.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/tracker/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      162 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1594 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/track.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      131 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1085 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/basetrack.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4858 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/bot_sort.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13185 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/byte_tracker.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11965 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/gmc.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18422 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/kalman_filter.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7634 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/matching.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/cfg/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11774 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/cfg/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/core/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    35343 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/exporter.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9784 2023-07-02 17:45:18.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/model.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13012 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/predictor.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12519 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/results.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    29828 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/trainer.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9205 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/validator.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/data/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      444 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    31854 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/augment.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8963 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/base.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7658 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/build.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12613 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/stream_loaders.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17533 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5augmentations.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    46519 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5loader.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11030 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1359 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset_wrappers.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/data/scripts/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/scripts/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18817 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17619 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3175 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/autobatch.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4043 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/benchmarks.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3842 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/base.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2205 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/clearml.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2162 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/comet.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3040 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/hub.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1323 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/tensorboard.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9837 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/checks.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2424 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/dist.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6474 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/downloads.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2556 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/files.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11762 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/instance.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2326 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/loss.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    28016 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/metrics.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    19809 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/ops.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    15709 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/plotting.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    10646 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/tal.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18671 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/torch_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      122 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      318 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2649 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5479 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2237 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      190 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4193 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8474 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11661 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      208 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4940 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7299 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12004 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2906 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       13 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4441 2023-07-02 16:30:14.000000 PJYoloVision-0.0.1/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      607 2023-07-02 16:19:19.000000 PJYoloVision-0.0.1/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-07-02 17:45:29.000000 PJYoloVision-0.0.1/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    35149 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/LICENCE.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.445521 PJYoloVision-0.0.3/PJYoloVision/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4906 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/nn/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/nn/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5600 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/nn/autobackend.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10977 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/nn/autoshape.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      867 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/nn/modules.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17501 2023-07-03 09:58:58.000000 PJYoloVision-0.0.3/PJYoloVision/nn/tasks.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/tracker/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      162 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1594 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/track.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      131 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1085 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/basetrack.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4858 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/bot_sort.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13185 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/byte_tracker.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/tracker/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11965 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/utils/gmc.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18422 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/utils/kalman_filter.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7634 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/tracker/utils/matching.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/yolo/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/yolo/cfg/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11778 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/cfg/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/yolo/core/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/core/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    35345 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/core/exporter.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10046 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/core/model.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31279 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/core/predictor.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12519 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/core/results.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    32074 2023-07-03 08:53:54.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/core/trainer.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9207 2023-07-03 08:54:33.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/core/validator.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/yolo/data/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      444 2023-07-03 08:59:14.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31969 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/augment.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8997 2023-07-03 08:59:14.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/base.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7673 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/build.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 08:59:14.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12715 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/stream_loaders.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17579 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/v5augmentations.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    46738 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/v5loader.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11047 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataset.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1427 2023-07-03 08:59:14.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataset_wrappers.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.449521 PJYoloVision-0.0.3/PJYoloVision/yolo/data/scripts/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 08:59:14.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/scripts/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18817 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/data/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17619 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3175 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/autobatch.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4044 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/benchmarks.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3842 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/base.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2205 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/clearml.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2162 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/comet.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3040 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/hub.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1323 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/tensorboard.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9838 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/checks.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2424 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/dist.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6474 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/downloads.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2556 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/files.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11762 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/instance.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2326 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/loss.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    28016 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/metrics.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    19809 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/ops.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    15709 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/plotting.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10646 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/tal.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18673 2023-07-03 09:00:22.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/utils/torch_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      122 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      318 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2649 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5481 2023-07-03 09:00:48.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2223 2023-07-03 09:01:01.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      190 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4193 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10758 2023-07-03 09:01:52.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11661 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      208 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4940 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7300 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12005 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 11:31:34.445521 PJYoloVision-0.0.3/PJYoloVision.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-03 11:31:34.000000 PJYoloVision-0.0.3/PJYoloVision.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2906 2023-07-03 11:31:34.000000 PJYoloVision-0.0.3/PJYoloVision.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-03 11:31:34.000000 PJYoloVision-0.0.3/PJYoloVision.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-03 11:31:34.000000 PJYoloVision-0.0.3/PJYoloVision.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       13 2023-07-03 11:31:34.000000 PJYoloVision-0.0.3/PJYoloVision.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4441 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      607 2023-07-03 07:22:50.000000 PJYoloVision-0.0.3/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-03 11:31:34.453521 PJYoloVision-0.0.3/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-07-03 11:23:59.000000 PJYoloVision-0.0.3/setup.py
```

### Comparing `PJYoloVision-0.0.1/LICENCE.md` & `PJYoloVision-0.0.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/__init__.py` & `PJYoloVision-0.0.3/PJYoloVision/__init__.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/nn/autobackend.py` & `PJYoloVision-0.0.3/PJYoloVision/nn/autobackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             names = {k: map[v] for k, v in names.items()}
     return names
 
 
 class SmartLoad(nn.Module):
 
     def __init__(self,
-                 weights='YOLOvisionn.pt',
+                 weights='PJYoloVision.pt',
                  device=torch.device('cpu'),
                  dnn=False,
                  data=None,
                  fp16=False,
                  fuse=True,
                  detail=True, *args, **kwargs):
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/nn/autoshape.py` & `PJYoloVision-0.0.3/PJYoloVision/nn/autoshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,8 +216,8 @@
     def __len__(self):  # override len(results)
         return self.n
 
     def __str__(self, *args, **kwargs):  # override print(results)
         return self._run(pprint=True)  # print results
 
     def __repr__(self, *args, **kwargs):
-        return f'YOLOvision {self.__class__} instance\n' + self.__str__()
+        return f'PJYoloVision {self.__class__} instance\n' + self.__str__()
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/nn/modules.py` & `PJYoloVision-0.0.3/PJYoloVision/nn/modules.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/nn/tasks.py` & `PJYoloVision-0.0.3/PJYoloVision/nn/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 
 import thop
 import re
 import torch
 import torch.nn as nn
 
-from PJYoloVision.nn.modules import (C1, C2, C3, C3TR, SPP, SPPF, Bottleneck, BottleneckCSP, C2f, C3Ghost, C3x, Classify,
+from PJYoloVision.nn.modules import (C1, C2, C3, C3TR, SPP, SPPF, Bottleneck, BottleneckCSP, C2f, C3Ghost, C3x,
+                                     Classify,
                                      Concat, Conv, ConvTranspose, Detect, DWConv, DWConvTranspose2d, Ensemble, Focus,
                                      GhostBottleneck, GhostConv, Segment)
 from PJYoloVision.yolo.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, colorstr, emojis, yaml_load
 from PJYoloVision.yolo.utils.checks import check_suffix, check_yaml
 from PJYoloVision.yolo.utils.torch_utils import (fuse_conv_and_bn, fuse_deconv_and_bn, initialize_weights,
                                                  intersect_dicts, make_divisible, model_info, scale_img, time_sync)
 
@@ -89,15 +90,15 @@
         csd = model.float().state_dict()
         csd = intersect_dicts(csd, self.state_dict())
         self.load_state_dict(csd, strict=False)
 
 
 class DetectionModel(BaseModel):
 
-    def __init__(self, cfg='YOLOvisionn.yaml', ch=3, nc=None, detail=False, *args, **kwargs):
+    def __init__(self, cfg='PJYoloVision.yaml', ch=3, nc=None, detail=False, *args, **kwargs):
         super().__init__()
         self.yaml = cfg if isinstance(cfg, dict) else yaml_model_load(cfg)
 
         # Define model
         ch = self.yaml['ch'] = self.yaml.get('ch', ch)  # input channels
         if nc and nc != self.yaml['nc']:
             LOGGER.info(f"Overriding model.yaml nc={self.yaml['nc']} with nc={nc}")
@@ -162,15 +163,15 @@
         i = (spa[-1].shape[-1] // g) * sum(4 ** (nl - 1 - x) for x in range(e))  # indices
         spa[-1] = spa[-1][..., i:]  # small
         return spa
 
 
 class SegmentationModel(DetectionModel):
     #
-    def __init__(self, cfg='YOLOvisionn-seg.yaml', ch=3, nc=None, detail=True, *args, **kwargs):
+    def __init__(self, cfg='PJYoloVision-seg.yaml', ch=3, nc=None, detail=True, *args, **kwargs):
         super().__init__(cfg, ch, nc, detail)
 
     def _forward_augment(self, x, *args, **kwargs):
         raise NotImplementedError
 
 
 class ClassificationModel(BaseModel):
@@ -287,15 +288,14 @@
         setattr(ensemble, k, getattr(ensemble[0], k))
     ensemble.stride = ensemble[torch.argmax(torch.tensor([m.stride.max() for m in ensemble])).int()].stride
     assert all(ensemble[0].nc == m.nc for m in ensemble), f'Models differ in class counts: {[m.nc for m in ensemble]}'
     return ensemble
 
 
 def attempt_load_one_weight(weight, device=None, inplace=True, fuse=False, *args, **kwargs):
-
     ckpt, weight = torch_safe_load(weight)
     args = {**DEFAULT_CFG_DICT, **ckpt['train_args']}
     model = (ckpt.get('ema') or ckpt['model']).to(device).float()
 
     model.args = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}
     model.pt_path = weight
     model.task = get_model_task_from_cfg(model)
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/tracker/track.py` & `PJYoloVision-0.0.3/PJYoloVision/tracker/track.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/basetrack.py` & `PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/bot_sort.py` & `PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/byte_tracker.py` & `PJYoloVision-0.0.3/PJYoloVision/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/tracker/utils/gmc.py` & `PJYoloVision-0.0.3/PJYoloVision/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/tracker/utils/kalman_filter.py` & `PJYoloVision-0.0.3/PJYoloVision/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/tracker/utils/matching.py` & `PJYoloVision-0.0.3/PJYoloVision/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/cfg/__init__.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/cfg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                  'save_conf', 'save_crop', 'hide_labels', 'hide_conf', 'visualize', 'augment', 'agnostic_nms',
                  'retina_masks', 'boxes', 'keras', 'optimize', 'int8', 'dynamic', 'simplify', 'nms', 'v5loader')
 
 # Define valid tasks and modes
 MODES = 'train', 'val', 'predict', 'export', 'track', 'benchmark'
 TASKS = 'detection', 'segmentation', 'classify'
 TASK2DATA = {'detection': 'coco128.yaml', 'segmentation': 'coco128-seg.yaml', 'classify': 'imagenet100'}
-TASK2MODEL = {'detection': 'YOLOvisionn.pt', 'segmentation': 'YOLOvisionn-seg.pt', 'classify': 'YOLOvisionn-cls.pt'}
+TASK2MODEL = {'detection': 'PJYoloVision.pt', 'segmentation': 'PJYoloVision-seg.pt', 'classify': 'PJYoloVision-cls.pt'}
 
 
 def cfg2dict(cfg, *args, **kwargs):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Inputs:
@@ -206,15 +206,15 @@
             raise ValueError(f"Invalid 'task={task}'. Valid tasks are {TASKS}.\n{CLI_HELP_MSG}")
         if 'model' not in overrides:
             overrides['model'] = TASK2MODEL[task]
 
     # Model
     model = overrides.pop('model', DEFAULT_CFG.model)
     if model is None:
-        model = 'YOLOvisionn.pt'
+        model = 'PJYoloVision.pt'
         LOGGER.warning(f" Opps Wait  'model' is missing. Using default 'model={model}'.")
     from PJYoloVision.yolo.core.model import YOLO
     overrides['model'] = model
     model = YOLO(model, task=task)
     if isinstance(overrides.get('pretrained'), str):
         model.load(overrides['pretrained'])
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/core/exporter.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/core/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,21 +732,21 @@
 
     def run_callbacks(self, event: str):
         for callback in self.callbacks.get(event, []):
             callback(self)
 
 
 def export(cfg=DEFAULT_CFG, *args, **kwargs):
-    cfg.model = cfg.model or 'YOLOvisionn.yaml'
+    cfg.model = cfg.model or 'PJYoloVision.yaml'
     cfg.format = cfg.format or 'torchscript'
 
     from PJYoloVision import YOLO
     model = YOLO(cfg.model)
     model.export(**vars(cfg))
 
 
 if __name__ == '__main__':
     """
     CLI:
-    yolo mode=export model=YOLOvisionn.yaml format=onnx
+    yolo mode=export model=PJYoloVision.yaml format=onnx
     """
     export()
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/core/model.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/core/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,22 @@
         self.model.args = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}
         self.model.task = self.task
 
     def _load_model(self, weights: str, task=None, *args, **kwargs):
         suffix = Path(weights).suffix
         if suffix == '.pt':
             self.model, self.ckpt = attempt_load_one_weight(weights)
-            self.task = task or self.model.args['train_args']['task']
+            # print(self.model.args)
+            try:
+                self.task = task or self.model.args['task']
+            except KeyError:
+                try:
+                    self.task = task or self.model.args['train_args']['task']
+                except KeyError:
+                    raise ValueError('no Task Found !')
             self.overrides = self.model.args = self._reset_ckpt_args(self.model.args)
             self.ckpt_path = self.model.pt_path
         else:
             weights = check_file(weights)
             self.model, self.ckpt = weights, None
             self.task = task or get_model_task_from_cfg(weights)
             self.ckpt_path = weights
@@ -96,15 +103,15 @@
             if hasattr(m, 'reset_parameters'):
                 m.reset_parameters()
         for p in self.model.parameters():
             p.requires_grad = True
         return self
 
     @smart_inference_mode()
-    def load(self, weights='YOLOvisionn.pt', *args, **kwargs):
+    def load(self, weights='PJYoloVision.pt', *args, **kwargs):
 
         if isinstance(weights, (str, Path)):
             weights, self.ckpt = attempt_load_one_weight(weights)
         self.model.load(weights)
         return self
 
     def info(self, detail=False, *args, **kwargs):
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/core/predictor.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/val.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,264 +1,237 @@
-"""
-Run prediction on images, videos, directories, globs, YouTube, webcam, streams, etc.
+ 
 
-Usage - sources:
-    $ yolo mode=predict model=YOLOvisionn.pt --source 0                               # webcam
-                                                  img.jpg                         # image
-                                                  vid.mp4                         # video
-                                                  screen                          # screenshot
-                                                  path/                           # directory
-                                                  list.txt                        # list of images
-                                                  list.streams                    # list of streams
-                                                  'path/*.jpg'                    # glob
-                                                  'https://youtu.be/Zgi9g1ksQHc'  # YouTube
-                                                  'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
-
-Usage - formats:
-    $ yolo mode=predict model=YOLOvisionn.pt                 # PyTorch
-                              YOLOvisionn.torchscript        # TorchScript
-                              YOLOvisionn.onnx               # ONNX Runtime or OpenCV DNN with dnn=True
-                              YOLOvisionn_openvino_model     # OpenVINO
-                              YOLOvisionn.core             # TensorRT
-                              YOLOvisionn.mlmodel            # CoreML (macOS-only)
-                              YOLOvisionn_saved_model        # TensorFlow SavedModel
-                              YOLOvisionn.pb                 # TensorFlow GraphDef
-                              YOLOvisionn.tflite             # TensorFlow Lite
-                              YOLOvisionn_edgetpu.tflite     # TensorFlow Edge TPU
-                              YOLOvisionn_paddle_model       # PaddlePaddle
-"""
-import os.path
-import pathlib
-import platform
-from collections import defaultdict
+import os
 from pathlib import Path
 
-import cv2
+import numpy as np
+import torch
 
-from PJYoloVision.nn.autobackend import SmartLoad
-from PJYoloVision.yolo.cfg import get_cfg
-from PJYoloVision.yolo.data import load_inference_source
-from PJYoloVision.yolo.data.augment import classify_transforms
-from PJYoloVision.yolo.utils import DEFAULT_CFG, LOGGER, SETTINGS, callbacks, colorstr, ops
-from PJYoloVision.yolo.utils.checks import check_imgsz, check_imshow
-from PJYoloVision.yolo.utils.files import increment_path
-from PJYoloVision.yolo.utils.torch_utils import select_device, smart_inference_mode
-
-STREAM_WARNING = """
-    Opps Wait  stream/video/webcam/dir predict source will accumulate results in RAM unless `stream=True` is passed,
-    causing potential out-of-memory errors for large sources or long-running streams/videos.
-
-    Usage:
-        results = model(source=..., stream=True)  # generator of Results objects
-        for r in results:
-            boxes = r.boxes  # Boxes object for bbox outputs
-            masks = r.masks  # Masks object for segmentation masks outputs
-            probs = r.probs  # Class probabilities for classification outputs
-"""
-
-
-class BasePredictor:
-
-    def __init__(self, cfg=DEFAULT_CFG, overrides=None, *args, **kwargs):
-
-        self.args = get_cfg(cfg, overrides)
-        project = self.args.project or Path(SETTINGS['runs_dir']) / self.args.task
-        name = self.args.name or f'{self.args.mode}'
-        self.save_dir = increment_path(Path(project) / name, exist_ok=self.args.exist_ok)
-        if self.args.conf is None:
-            self.args.conf = 0.25  # default conf=0.25
-        self.done_warmup = False
-        if self.args.show:
-            self.args.show = check_imshow(warn=True)
-
-        # Usable if setup is done
-        self.model = None
-        self.data = self.args.data  # data_dict
-        self.imgsz = None
-        self.device = None
-        self.dataset = None
-        self.vid_path, self.vid_writer = None, None
-        self.annotator = None
-        self.data_path = None
-        self.source_type = None
-        self.batch = None
-        self.callbacks = defaultdict(list, callbacks.default_callbacks)  # add callbacks
-        callbacks.add_integration_callbacks(self)
-
-    def preprocess(self, img, *args, **kwargs):
-        pass
-
-    def get_annotator(self, img, *args, **kwargs):
-        raise NotImplementedError('get_annotator function needs to be implemented')
-
-    def write_results(self, results, batch, print_string, *args, **kwargs):
-        raise NotImplementedError('print_results function needs to be implemented')
-
-    def postprocess(self, preds, img, orig_img, *args, **kwargs):
+from PJYoloVision.yolo.data import build_dataloader
+from PJYoloVision.yolo.data.dataloaders.v5loader import create_dataloader
+from PJYoloVision.yolo.core.validator import BaseValidator
+from PJYoloVision.yolo.utils import DEFAULT_CFG, LOGGER, colorstr, ops
+ 
+from PJYoloVision.yolo.utils.metrics import ConfusionMatrix, DetMetrics, box_iou
+from PJYoloVision.yolo.utils.plotting import output_to_target, plot_images
+from PJYoloVision.yolo.utils.torch_utils import de_parallel
+
+
+class DetectionValidator(BaseValidator):
+
+    def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, **kwargs):
+        super().__init__(dataloader, save_dir, pbar, args)
+        self.args.task = 'detection'
+        self.is_coco = False
+        self.class_map = None
+        self.metrics = DetMetrics(save_dir=self.save_dir)
+        self.iouv = torch.linspace(0.5, 0.95, 10)  # iou vector for mAP@0.5:0.95
+        self.niou = self.iouv.numel()
+
+    def preprocess(self, batch, *args, **kwargs):
+        batch['img'] = batch['img'].to(self.device, non_blocking=True)
+        batch['img'] = (batch['img'].half() if self.args.half else batch['img'].float()) / 255
+        for k in ['batch_idx', 'cls', 'bboxes']:
+            batch[k] = batch[k].to(self.device)
+
+        nb = len(batch['img'])
+        self.lb = [torch.cat([batch['cls'], batch['bboxes']], dim=-1)[batch['batch_idx'] == i]
+                   for i in range(nb)] if self.args.save_hybrid else []  # for autolabelling
+
+        return batch
+
+    def init_metrics(self, model, *args, **kwargs):
+        val = self.data.get(self.args.split, '')  # validation path
+        self.is_coco = isinstance(val, str) and val.endswith(f'coco{os.sep}val2017.txt')  # is COCO dataset
+        self.class_map = list(range(1000))
+        self.args.save_json |= self.is_coco and not self.training  # run on final val if training COCO
+        self.names = model.names
+        self.nc = len(model.names)
+        self.metrics.names = self.names
+        self.metrics.plot = self.args.plots
+        self.confusion_matrix = ConfusionMatrix(nc=self.nc)
+        self.seen = 0
+        self.jdict = []
+        self.stats = []
+
+    def get_desc(self, *args, **kwargs):
+        return ('%22s' + '%11s' * 6) % ('Class', 'Images', 'Instances', 'Box(P', 'R', 'mAP50', 'mAP50-95)')
+
+    def postprocess(self, preds, *args, **kwargs):
+        preds = ops.non_max_suppression(preds,
+                                        self.args.conf,
+                                        self.args.iou,
+                                        labels=self.lb,
+                                        multi_label=True,
+                                        agnostic=self.args.single_cls,
+                                        max_det=self.args.max_det)
         return preds
 
-    def __call__(self, source=None, model=None, stream=False, *args, **kwargs):
-        self.stream = stream
-        if stream:
-            return self.stream_inference(source, model)
-        else:
-            return list(self.stream_inference(source, model))  # merge list of Result into one
-
-    def predict_cli(self, source=None, model=None, *args, **kwargs):
-        # Method used for CLI prediction. It uses always generator as outputs as not required by CLI mode
-        gen = self.stream_inference(source, model)
-        for _ in gen:  # running CLI inference without accumulating any outputs (do not modify)
-            pass
-
-    def setup_source(self, source, *args, **kwargs):
-        self.imgsz = check_imgsz(self.args.imgsz, stride=self.model.stride, min_dim=2)  # check image size
-        if self.args.task == 'classify':
-            transforms = getattr(self.model.model, 'transforms', classify_transforms(self.imgsz[0]))
-        else:  # predict, segmentation
-            transforms = None
-        self.dataset = load_inference_source(source=source,
-                                             transforms=transforms,
-                                             imgsz=self.imgsz,
-                                             vid_stride=self.args.vid_stride,
-                                             stride=self.model.stride,
-                                             auto=self.model.pt)
-        self.source_type = self.dataset.source_type
-        if not getattr(self, 'stream', True) and (self.dataset.mode == 'stream' or  # streams
-                                                  len(self.dataset) > 1000 or  # images
-                                                  any(getattr(self.dataset, 'video_flag', [False]))):  # videos
-            LOGGER.warning(STREAM_WARNING)
-        self.vid_path, self.vid_writer = [None] * self.dataset.bs, [None] * self.dataset.bs
-
-    @smart_inference_mode()
-    def stream_inference(self, source=None, model=None, *args, **kwargs):
-        if self.args.detail:
-            LOGGER.info('')
-        if not os.path.exists(self.save_dir):
-            self.save_dir: pathlib.WindowsPath = self.save_dir
-            self.save_dir.mkdir(parents=True, exist_ok=True)
-            LOGGER.warning('Out Folder Created')
-        # setup model
-        if not self.model:
-            self.setup_model(model)
-        # setup source every time predict is called
-        self.setup_source(source if source is not None else self.args.source)
-
-        # check if save_dir/ label file exists
-        if self.args.save or self.args.save_txt:
-            (self.save_dir / 'labels' if self.args.save_txt else self.save_dir).mkdir(parents=True, exist_ok=True)
-        # warmup model
-        if not self.done_warmup:
-            self.model.warmup(imgsz=(1 if self.model.pt or self.model.triton else self.dataset.bs, 3, *self.imgsz))
-            self.done_warmup = True
-
-        self.seen, self.windows, self.dt, self.batch = 0, [], (ops.Profile(), ops.Profile(), ops.Profile()), None
-        self.run_callbacks('on_predict_start')
-        for batch in self.dataset:
-            self.run_callbacks('on_predict_batch_start')
-            self.batch = batch
-            path, im, im0s, vid_cap, s = batch
-            visualize = increment_path(self.save_dir / Path(path).stem, mkdir=True) if self.args.visualize else False
-
-            # preprocess
-            with self.dt[0]:
-                im = self.preprocess(im)
-                if len(im.shape) == 3:
-                    im = im[None]  # expand for batch dim
-
-            # inference
-            with self.dt[1]:
-                preds = self.model(im, augment=self.args.augment, visualize=visualize)
-
-            # postprocess
-            with self.dt[2]:
-                self.results = self.postprocess(preds, im, im0s)
-            self.run_callbacks('on_predict_postprocess_end')
-
-            # visualize, save, write results
-            n = len(im)
-            for i in range(n):
-                self.results[i].speed = {
-                    'preprocess': self.dt[0].dt * 1E3 / n,
-                    'inference': self.dt[1].dt * 1E3 / n,
-                    'postprocess': self.dt[2].dt * 1E3 / n}
-                if self.source_type.tensor:  # skip write, show and plot operations if input is raw tensor
-                    continue
-                p, im0 = (path[i], im0s[i].copy()) if self.source_type.webcam or self.source_type.from_img \
-                    else (path, im0s.copy())
-                p = Path(p)
-
-                if self.args.detail or self.args.save or self.args.save_txt or self.args.show:
-                    s += self.write_results(i, self.results, (p, im, im0))
-
-                if self.args.show:
-                    self.show(p)
-
-                if self.args.save:
-                    self.save_preds(vid_cap, i, str(self.save_dir / p.name))
-            self.run_callbacks('on_predict_batch_end')
-            yield from self.results
-
-            # Print time (inference-only)
-            if self.args.detail:
-                LOGGER.info(f'{s}{self.dt[1].dt * 1E3:.1f}ms')
-
-        # Release assets
-        if isinstance(self.vid_writer[-1], cv2.VideoWriter):
-            self.vid_writer[-1].release()  # release final video writer
-
-        # Print results
-        if self.args.detail and self.seen:
-            t = tuple(x.t / self.seen * 1E3 for x in self.dt)  # speeds per image
-            LOGGER.info(f'Speed: %.1fms preprocess, %.1fms inference, %.1fms postprocess per image at shape '
-                        f'{(1, 3, *self.imgsz)}' % t)
-        if self.args.save or self.args.save_txt or self.args.save_crop:
-            nl = len(list(self.save_dir.glob('labels/*.txt')))  # number of labels
-            s = f"\n{nl} label{'s' * (nl > 1)} saved to {self.save_dir / 'labels'}" if self.args.save_txt else ''
-            LOGGER.info(f"Results saved to {colorstr('bold', self.save_dir)}{s}")
-
-        self.run_callbacks('on_predict_end')
-
-    def setup_model(self, model, detail=True, *args, **kwargs):
-        device = select_device(self.args.device, detail=detail)
-        model = model or self.args.model
-        self.args.half &= device.type != 'cpu'  # half precision only supported on CUDA
-        self.model = SmartLoad(model,
-                               device=device,
-                               dnn=self.args.dnn,
-                               data=self.args.data,
-                               fp16=self.args.half,
-                               detail=detail)
-        self.device = device
-        self.model.eval()
-
-    def show(self, p, *args, **kwargs):
-        im0 = self.annotator.result()
-        if platform.system() == 'Linux' and p not in self.windows:
-            self.windows.append(p)
-            cv2.namedWindow(str(p), cv2.WINDOW_NORMAL | cv2.WINDOW_KEEPRATIO)  # allow window resize (Linux)
-            cv2.resizeWindow(str(p), im0.shape[1], im0.shape[0])
-        cv2.imshow(str(p), im0)
-        cv2.waitKey(500 if self.batch[4].startswith('image') else 1)  # 1 millisecond
-
-    def save_preds(self, vid_cap, idx, save_path, *args, **kwargs):
-        im0 = self.annotator.result()
-        # save imgs
-        if self.dataset.mode == 'image':
-            cv2.imwrite(save_path, im0)
-        else:  # 'video' or 'stream'
-            if self.vid_path[idx] != save_path:  # new video
-                self.vid_path[idx] = save_path
-                if isinstance(self.vid_writer[idx], cv2.VideoWriter, *args, **kwargs):
-                    self.vid_writer[idx].release()  # release previous video writer
-                if vid_cap:  # video
-                    fps = int(vid_cap.get(cv2.CAP_PROP_FPS))  # integer required, floats produce error in MP4 codec
-                    w = int(vid_cap.get(cv2.CAP_PROP_FRAME_WIDTH))
-                    h = int(vid_cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-                else:  # stream
-                    fps, w, h = 30, im0.shape[1], im0.shape[0]
-                save_path = str(Path(save_path).with_suffix('.mp4'))  # force *.mp4 suffix on results videos
-                self.vid_writer[idx] = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc(*'mp4v'), fps, (w, h))
-            self.vid_writer[idx].write(im0)
-
-    def run_callbacks(self, event: str):
-        for callback in self.callbacks.get(event, []):
-            callback(self)
+    def update_metrics(self, preds, batch, *args, **kwargs):
+        # Metrics
+        for si, pred in enumerate(preds):
+            idx = batch['batch_idx'] == si
+            cls = batch['cls'][idx]
+            bbox = batch['bboxes'][idx]
+            nl, npr = cls.shape[0], pred.shape[0]  # number of labels, predictions
+            shape = batch['ori_shape'][si]
+            correct_bboxes = torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device)  # init
+            self.seen += 1
+
+            if npr == 0:
+                if nl:
+                    self.stats.append((correct_bboxes, *torch.zeros((2, 0), device=self.device), cls.squeeze(-1)))
+                    if self.args.plots:
+                        self.confusion_matrix.process_batch(detections=None, labels=cls.squeeze(-1))
+                continue
+
+            # Predictions
+            if self.args.single_cls:
+                pred[:, 5] = 0
+            predn = pred.clone()
+            ops.scale_boxes(batch['img'][si].shape[1:], predn[:, :4], shape,
+                            ratio_pad=batch['ratio_pad'][si])  # native-space pred
+
+            # Evaluate
+            if nl:
+                height, width = batch['img'].shape[2:]
+                tbox = ops.xywh2xyxy(bbox) * torch.tensor(
+                    (width, height, width, height), device=self.device)  # target boxes
+                ops.scale_boxes(batch['img'][si].shape[1:], tbox, shape,
+                                ratio_pad=batch['ratio_pad'][si])  # native-space labels
+                labelsn = torch.cat((cls, tbox), 1)  # native-space labels
+                correct_bboxes = self._process_batch(predn, labelsn)
+                # TODO: maybe remove these `self.` arguments as they already are member variable
+                if self.args.plots:
+                    self.confusion_matrix.process_batch(predn, labelsn)
+            self.stats.append((correct_bboxes, pred[:, 4], pred[:, 5], cls.squeeze(-1)))  # (conf, pcls, tcls)
+
+            # Save
+            if self.args.save_json:
+                self.pred_to_json(predn, batch['im_file'][si])
+            if self.args.save_txt:
+                file = self.save_dir / 'labels' / f'{Path(batch["im_file"][si]).stem}.txt'
+                self.save_one_txt(predn, self.args.save_conf, shape, file)
+
+    def finalize_metrics(self, *args, **kwargs):
+        self.metrics.speed = self.speed
+        self.metrics.confusion_matrix = self.confusion_matrix
+
+    def get_stats(self, *args, **kwargs):
+        stats = [torch.cat(x, 0).cpu().numpy() for x in zip(*self.stats)]  # to numpy
+        if len(stats) and stats[0].any():
+            self.metrics.process(*stats)
+        self.nt_per_class = np.bincount(stats[-1].astype(int), minlength=self.nc)  # number of targets per class
+        return self.metrics.results_dict
+
+    def print_results(self, *args, **kwargs):
+        pf = '%22s' + '%11i' * 2 + '%11.3g' * len(self.metrics.keys)  # print format
+        LOGGER.info(pf % ('all', self.seen, self.nt_per_class.sum(), *self.metrics.mean_results()))
+        if self.nt_per_class.sum() == 0:
+            LOGGER.warning(
+                f'Opps Wait  no labels found in {self.args.task} set, can not compute metrics without labels')
+
+        # Print results per class
+        if self.args.detail and not self.training and self.nc > 1 and len(self.stats):
+            for i, c in enumerate(self.metrics.ap_class_index):
+                LOGGER.info(pf % (self.names[c], self.seen, self.nt_per_class[c], *self.metrics.class_result(i)))
+
+        if self.args.plots:
+            self.confusion_matrix.plot(save_dir=self.save_dir, names=list(self.names.values()))
+
+    def _process_batch(self, detections, labels, *args, **kwargs):
+
+        iou = box_iou(labels[:, 1:], detections[:, :4])
+        correct = np.zeros((detections.shape[0], self.iouv.shape[0])).astype(bool)
+        correct_class = labels[:, 0:1] == detections[:, 5]
+        for i in range(len(self.iouv)):
+            x = torch.where((iou >= self.iouv[i]) & correct_class)
+            if x[0].shape[0]:
+                matches = torch.cat((torch.stack(x, 1), iou[x[0], x[1]][:, None]),
+                                    1).cpu().numpy()
+                if x[0].shape[0] > 1:
+                    matches = matches[matches[:, 2].argsort()[::-1]]
+                    matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
+                    matches = matches[np.unique(matches[:, 0], return_index=True)[1]]
+                correct[matches[:, 1].astype(int), i] = True
+        return torch.tensor(correct, dtype=torch.bool, device=detections.device)
+
+    def get_dataloader(self, dataset_path, batch_size, *args, **kwargs):
+        # TODO: manage splits differently
+        # calculate stride - check if model is initialized
+        gs = max(int(de_parallel(self.model).stride if self.model else 0), 32)
+        return create_dataloader(path=dataset_path,
+                                 imgsz=self.args.imgsz,
+                                 batch_size=batch_size,
+                                 stride=gs,
+                                 hyp=vars(self.args),
+                                 cache=False,
+                                 pad=0.5,
+                                 rect=self.args.rect,
+                                 workers=self.args.workers,
+                                 prefix=colorstr(f'{self.args.mode}: '),
+                                 shuffle=False,
+                                 seed=self.args.seed)[0] if self.args.v5loader else \
+            build_dataloader(self.args, batch_size, img_path=dataset_path, stride=gs, names=self.data['names'],
+                             mode='val')[0]
+
+    def plot_val_samples(self, batch, ni, *args, **kwargs):
+        plot_images(batch['img'],
+                    batch['batch_idx'],
+                    batch['cls'].squeeze(-1),
+                    batch['bboxes'],
+                    paths=batch['im_file'],
+                    fname=self.save_dir / f'val_batch{ni}_labels.jpg',
+                    names=self.names)
+
+    def plot_predictions(self, batch, preds, ni, *args, **kwargs):
+        plot_images(batch['img'],
+                    *output_to_target(preds, max_det=15),
+                    paths=batch['im_file'],
+                    fname=self.save_dir / f'val_batch{ni}_pred.jpg',
+                    names=self.names)  # pred
+
+    def save_one_txt(self, predn, save_conf, shape, file, *args, **kwargs):
+        gn = torch.tensor(shape)[[1, 0, 1, 0]]  # normalization gain whwh
+        for *xyxy, conf, cls in predn.tolist():
+            xywh = (ops.xyxy2xywh(torch.tensor(xyxy).view(1, 4)) / gn).view(-1).tolist()  # normalized xywh
+            line = (cls, *xywh, conf) if save_conf else (cls, *xywh)  # label format
+            with open(file, 'a') as f:
+                f.write(('%g ' * len(line)).rstrip() % line + '\n')
+
+    def pred_to_json(self, predn, filename, *args, **kwargs):
+        stem = Path(filename).stem
+        image_id = int(stem) if stem.isnumeric() else stem
+        box = ops.xyxy2xywh(predn[:, :4])  # xywh
+        box[:, :2] -= box[:, 2:] / 2  # xy center to top-left corner
+        for p, b in zip(predn.tolist(), box.tolist()):
+            self.jdict.append({
+                'image_id': image_id,
+                'category_id': self.class_map[int(p[5])],
+                'bbox': [round(x, 3) for x in b],
+                'score': round(p[4], 5)})
+
+    def eval_json(self, stats, *args, **kwargs):
+        if self.args.save_json and self.is_coco and len(self.jdict):
+            anno_json = self.data['path'] / 'annotations/instances_val2017.json'  # annotations
+            pred_json = self.save_dir / 'predictions.json'  # predictions
+            LOGGER.info(f'\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...')
+            try:
+                 
+                from pycocotools.coco import COCO
+                from pycocotools.cocoeval import COCOeval  # noqa
+
+                for x in anno_json, pred_json:
+                    assert x.is_file(), f'{x} file not found'
+                anno = COCO(str(anno_json))  # init annotations api
+                pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
+                eval = COCOeval(anno, pred, 'bbox')
+                if self.is_coco:
+                    eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # images to eval
+                eval.evaluate()
+                eval.accumulate()
+                eval.summarize()
+                stats[self.metrics.keys[-1]], stats[self.metrics.keys[-2]] = eval.stats[:2]  # update mAP50-95 and mAP50
+            except Exception as e:
+                LOGGER.warning(f'pycocotools unable to run: {e}')
+        return stats
+
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/core/results.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/core/results.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/core/trainer.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/core/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,74 +1,134 @@
-
 import os
 import subprocess
 import time
 from collections import defaultdict
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
+from tarfile import is_tarfile
+from zipfile import is_zipfile
 
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from torch.cuda import amp
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim import lr_scheduler
 from tqdm import tqdm
 
+from PJYoloVision.nn.autobackend import check_class_names
 from PJYoloVision.nn.tasks import attempt_load_one_weight, attempt_load_weights
 from PJYoloVision.yolo.cfg import get_cfg
-from PJYoloVision.yolo.data.utils import check_cls_dataset, check_det_dataset
-from PJYoloVision.yolo.utils import (DEFAULT_CFG, LOGGER, ONLINE, RANK, ROOT, SETTINGS, TQDM_BAR_FORMAT, __version__,
-                                     callbacks, colorstr, emojis, yaml_save)
+
+from PJYoloVision.yolo.utils import (DEFAULT_CFG, LOGGER, RANK, SETTINGS, TQDM_BAR_FORMAT, __version__,
+                                     callbacks, colorstr, emojis, yaml_save, DATASETS_DIR, yaml_load)
 from PJYoloVision.yolo.utils.autobatch import check_train_batch_size
-from PJYoloVision.yolo.utils.checks import check_file, check_imgsz, print_args
+from PJYoloVision.yolo.utils.checks import check_file, check_imgsz, print_args, is_ascii, check_font
 from PJYoloVision.yolo.utils.dist import ddp_cleanup, generate_ddp_command
+from PJYoloVision.yolo.utils.downloads import safe_download
 from PJYoloVision.yolo.utils.files import get_latest_run, increment_path
 from PJYoloVision.yolo.utils.torch_utils import (EarlyStopping, ModelEMA, de_parallel, init_seeds, one_cycle,
                                                  select_device, strip_optimizer)
 
 
-class BaseTrainer:
-    """
-    BaseTrainer
+def check_cls_dataset(dataset: str):
+    data_dir = (DATASETS_DIR / dataset).resolve()
+    if not data_dir.is_dir():
+        raise FileExistsError('dataset you provided is not exists ')
+
+    train_set = data_dir / 'train'
+    test_set = data_dir / 'test' if (data_dir / 'test').exists() else data_dir / 'val'  # data/test or data/val
+    nc = len([x for x in (data_dir / 'train').glob('*') if x.is_dir()])  # number of classes
+    names = [x.name for x in (data_dir / 'train').iterdir() if x.is_dir()]  # class names list
+    names = dict(enumerate(sorted(names)))
+    return {'train': train_set, 'val': test_set, 'nc': nc, 'names': names}
+
+
+def check_det_dataset(dataset, autodownload=True, *args, **kwargs):
+    # Download, check and/or unzip dataset if not found locally
+
+    data = check_file(dataset)
+
+    # Download (optional)
+    extract_dir = ''
+    if isinstance(data, (str, Path)) and (is_zipfile(data) or is_tarfile(data)):
+        new_dir = safe_download(data, dir=DATASETS_DIR, unzip=True, delete=False, curl=False)
+        data = next((DATASETS_DIR / new_dir).rglob('*.yaml'))
+        extract_dir, autodownload = data.parent, False
+
+    # Read yaml (optional)
+    if isinstance(data, (str, Path)):
+        data = yaml_load(data, append_filename=True)  # dictionary
+
+    # Checks
+    for k in 'train', 'val':
+        if k not in data:
+            raise SyntaxError(
+                emojis(f"{dataset} '{k}:' key missing ❌.\n'train' and 'val' are required in all data YAMLs."))
+    if 'names' not in data and 'nc' not in data:
+        raise SyntaxError(emojis(f"{dataset} key missing ❌.\n either 'names' or 'nc' are required in all data YAMLs."))
+    if 'names' in data and 'nc' in data and len(data['names']) != data['nc']:
+        raise SyntaxError(emojis(f"{dataset} 'names' length {len(data['names'])} and 'nc: {data['nc']}' must match."))
+    if 'names' not in data:
+        data['names'] = [f'class_{i}' for i in range(data['nc'])]
+    else:
+        data['nc'] = len(data['names'])
+
+    data['names'] = check_class_names(data['names'])
+    # Resolve paths
+    path = Path(extract_dir or data.get('path') or Path(data.get('yaml_file', '')).parent)  # dataset root
+
+    if not path.is_absolute():
+        path = (DATASETS_DIR / path).resolve()
+        data['path'] = path
+    for k in 'train', 'val', 'test':
+        if data.get(k):
+            if isinstance(data[k], str):
+                x = (path / data[k]).resolve()
+                if not x.exists() and data[k].startswith('../'):
+                    x = (path / data[k][3:]).resolve()
+
+                data[k] = str(x)
+            else:
+
+                data[k] = [str((path / x).resolve()) for x in data[k]]
+
+    # Parse yaml
+    train, val, test, s = (data.get(x) for x in ('train', 'val', 'test', 'download'))
+    if val:
+        val = [Path(x).resolve() for x in (val if isinstance(val, list) else [val])]  # val path
+
+        if not all(x.exists() for x in val):
+            m = f"\nDataset '{dataset}' images not found ⚠️, missing paths %s" % [str(x) for x in val if not x.exists()]
+
+            if s and autodownload:
+                LOGGER.warning(m)
+            else:
+
+                raise FileNotFoundError(m)
+            t = time.time()
+            if s.startswith('http') and s.endswith('.zip', *args, **kwargs):  # URL
+                safe_download(url=s, dir=DATASETS_DIR, delete=True)
+                r = None  # success
+            elif s.startswith('bash ', *args, **kwargs):  # bash script
+                LOGGER.info(f'Running {s} ...')
+                r = os.system(s)
+            else:  # python script
+                r = exec(s, {'yaml': data})  # return None
+            dt = f'({round(time.time() - t, 1)}s)'
+            s = f"success ✅ {dt}, saved to {colorstr('bold', DATASETS_DIR)}" if r in (0, None) else f'failure {dt} ❌'
+            LOGGER.info(f'Dataset download {s}\n')
+    check_font('Arial.ttf' if is_ascii(data['names']) else 'Arial.Unicode.ttf')  # download fonts
 
-    A base class for creating trainers.
+    return data  # dictionary
 
-    Attributes:
-        args (SimpleNamespace, *args, **kwargs): Configuration for the trainer.
-        check_resume (method, *args, **kwargs): Method to check if training should be resumed from a saved checkpoint.
-        validator (BaseValidator): Validator instance.
-        model (nn.Module ): Model instance.
-        callbacks (defaultdict, *args, **kwargs): Dictionary of callbacks.
-        save_dir (Path, *args, **kwargs): Directory to save results.
-        wdir (Path, *args, **kwargs): Directory to save downloads.
-        last (Path, *args, **kwargs): Path to last checkpoint.
-        best (Path, *args, **kwargs): Path to best checkpoint.
-        save_period (int, *args, **kwargs): Save checkpoint every x epochs (disabled if < 1).
-        batch_size (int, *args, **kwargs): Batch size for training.
-        epochs (int, *args, **kwargs): Number of epochs to train for.
-        start_epoch (int, *args, **kwargs): Starting epoch for training.
-        device (torch.device): Device to use for training.
-        amp (bool): Flag to enable AMP (Automatic Mixed Precision).
-        scaler (amp.GradScaler, *args, **kwargs): Gradient scaler for AMP.
-        data (str): Path to data.
-        trainset (torch.utils.data.Dataset): Training dataset.
-        testset (torch.utils.data.Dataset): Testing dataset.
-        ema (nn.Module ): EMA (Exponential Moving Average) of the model.
-        lf (nn.Module ): Loss function.
-        scheduler (torch.optim.lr_scheduler._LRScheduler, *args, **kwargs): Learning rate scheduler.
-        best_fitness (float): The best fitness value achieved.
-        fitness (float): Current fitness value.
-        loss (float): Current loss value.
-        tloss (float): Total loss value.
-        loss_names (list): List of loss names.
-        csv (Path, *args, **kwargs): Path to results CSV file.
-    """
+
+class BaseTrainer:
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, *args, **kwargs):
         """
         Initializes the BaseTrainer class.
 
         Args:
             cfg (str, optional, *args, **kwargs): Path to a configuration file. Defaults to DEFAULT_CFG.
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/core/validator.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/core/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 import torch
 from tqdm import tqdm
 
 from PJYoloVision.nn.autobackend import SmartLoad
 from PJYoloVision.yolo.cfg import get_cfg
-from PJYoloVision.yolo.data.utils import check_cls_dataset, check_det_dataset
+from PJYoloVision.yolo.core.trainer import check_det_dataset, check_cls_dataset
 from PJYoloVision.yolo.utils import DEFAULT_CFG, LOGGER, RANK, SETTINGS, TQDM_BAR_FORMAT, callbacks, colorstr, emojis
 from PJYoloVision.yolo.utils.checks import check_imgsz
 from PJYoloVision.yolo.utils.files import increment_path
 from PJYoloVision.yolo.utils.ops import Profile
 from PJYoloVision.yolo.utils.torch_utils import de_parallel, select_device, smart_inference_mode
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/augment.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/augment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
- 
-
 import math
 import random
 from copy import deepcopy
 
 import cv2
 import numpy as np
 import torch
@@ -73,22 +71,22 @@
 
     def __call__(self, labels, *args, **kwargs):
         if random.uniform(0, 1) > self.p:
             return labels
 
         # get index of one or three other images
         indexes = self.get_indexes()
-        if isinstance(indexes,int):
+        if isinstance(indexes, int):
             indexes = [indexes]
 
         # get images information will be used for Mosaic or MixUp
         mix_labels = [self.dataset.get_label_info(i) for i in indexes]
 
         if self.pre_transform is not None:
-            for i, data in enumerate(mix_labels):
+            for i, data in enumerate(mix_labels, *args, **kwargs):
                 mix_labels[i] = self.pre_transform(data)
         labels['mix_labels'] = mix_labels
 
         # Mosaic or MixUp
         labels = self._mix_transform(labels)
         labels.pop('mix_labels', None)
         return labels
@@ -120,15 +118,15 @@
 
     def _mix_transform(self, labels, *args, **kwargs):
         mosaic_labels = []
         assert labels.get('rect_shape', None) is None, 'rect and mosaic is exclusive.'
         assert len(labels.get('mix_labels', [])) > 0, 'There are no other images for mosaic augment.'
         s = self.imgsz
         yc, xc = (int(random.uniform(-x, 2 * s + x)) for x in self.border)  # mosaic center x, y
-        for i in range(4):
+        for i in range(4, *args, **kwargs):
             labels_patch = (labels if i == 0 else labels['mix_labels'][i - 1]).copy()
             # Load image
             img = labels_patch['img']
             h, w = labels_patch.pop('resized_shape')
 
             # place img in img4
             if i == 0:  # top left
@@ -356,15 +354,15 @@
         img, M, scale = self.affine_transform(img, border)
 
         bboxes = self.apply_bboxes(instances.bboxes, M)
 
         segments = instances.segments
         keypoints = instances.keypoints
         # update bboxes if there are segments.
-        if len(segments):
+        if len(segments, *args, **kwargs):
             bboxes, segments = self.apply_segments(segments, M)
 
         if keypoints is not None:
             keypoints = self.apply_keypoints(keypoints, M)
         new_instances = Instances(bboxes, segments, keypoints, bbox_format='xyxy', normalized=False)
         # clip
         new_instances.clip(*self.size)
@@ -377,15 +375,16 @@
                                 area_thr=0.01 if len(segments) else 0.10)
         labels['instances'] = new_instances[i]
         labels['cls'] = cls[i]
         labels['img'] = img
         labels['resized_shape'] = img.shape[:2]
         return labels
 
-    def box_candidates(self, box1, box2, wh_thr=2, ar_thr=100, area_thr=0.1, eps=1e-16, *args, **kwargs):  # box1(4,n), box2(4,n)
+    def box_candidates(self, box1, box2, wh_thr=2, ar_thr=100, area_thr=0.1, eps=1e-16, *args,
+                       **kwargs):  # box1(4,n), box2(4,n)
         # Compute box candidates: box1 before augment, box2 after augment, wh_thr (pixels), aspect_ratio_thr, area_ratio
         w1, h1 = box1[2] - box1[0], box1[3] - box1[1]
         w2, h2 = box2[2] - box2[0], box2[3] - box2[1]
         ar = np.maximum(w2 / (h2 + eps), h2 / (w2 + eps))  # aspect ratio
         return (w2 > wh_thr) & (h2 > wh_thr) & (w2 * h2 / (w1 * h1 + eps) > area_thr) & (ar < ar_thr)  # candidates
 
 
@@ -454,15 +453,15 @@
 
     def __call__(self, labels=None, image=None, *args, **kwargs):
         if labels is None:
             labels = {}
         img = labels.get('img') if image is None else image
         shape = img.shape[:2]  # current shape [height, width]
         new_shape = labels.pop('rect_shape', self.new_shape)
-        if isinstance(new_shape,int):
+        if isinstance(new_shape, int):
             new_shape = (new_shape, new_shape)
 
         # Scale ratio (new / old)
         r = min(new_shape[0] / shape[0], new_shape[1] / shape[1])
         if not self.scaleup:  # only scale down, do not scale up (for better val mAP)
             r = min(r, 1.0)
 
@@ -485,15 +484,15 @@
         if shape[::-1] != new_unpad:  # resize
             img = cv2.resize(img, new_unpad, interpolation=cv2.INTER_LINEAR)
         top, bottom = int(round(dh - 0.1)), int(round(dh + 0.1))
         left, right = int(round(dw - 0.1)), int(round(dw + 0.1))
         img = cv2.copyMakeBorder(img, top, bottom, left, right, cv2.BORDER_CONSTANT,
                                  value=(114, 114, 114))  # add border
 
-        if len(labels):
+        if len(labels, *args, **kwargs):
             labels = self._update_labels(labels, ratio, dw, dh)
             labels['img'] = img
             labels['resized_shape'] = new_shape
             return labels
         else:
             return img
 
@@ -515,15 +514,15 @@
         # Implement Copy-Paste augmentation https://arxiv.org/abs/2012.07177, labels as nx5 np.array(cls, xyxy)
         im = labels['img']
         cls = labels['cls']
         h, w = im.shape[:2]
         instances = labels.pop('instances')
         instances.convert_bbox(format='xyxy')
         instances.denormalize(w, h)
-        if self.p and len(instances.segments):
+        if self.p and len(instances.segments, *args, **kwargs):
             n = len(instances)
             _, w, _ = im.shape  # height, width, channels
             im_new = np.zeros(im.shape, np.uint8)
 
             # calculate ioa first then select indexes randomly
             ins_flip = deepcopy(instances)
             ins_flip.fliplr(w)
@@ -572,15 +571,15 @@
             pass
         except Exception as e:
             LOGGER.info(f'{prefix}{e}')
 
     def __call__(self, labels, *args, **kwargs):
         im = labels['img']
         cls = labels['cls']
-        if len(cls):
+        if len(cls, *args, **kwargs):
             labels['instances'].convert_bbox('xywh')
             labels['instances'].normalize(*im.shape[:2][::-1])
             bboxes = labels['instances'].bboxes
             # TODO: add supports of segments and keypoints
             if self.transform and random.random() < self.p:
                 new = self.transform(image=im, bboxes=bboxes, class_labels=cls)  # transformed
                 if len(new['class_labels']) > 0:  # skip update if no bbox in new im
@@ -680,33 +679,33 @@
         RandomFlip(direction='vertical', p=hyp.flipud),
         RandomFlip(direction='horizontal', p=hyp.fliplr)])  # transforms
 
 
 # Classification augmentations -----------------------------------------------------------------------------------------
 def classify_transforms(size=224, mean=(0.0, 0.0, 0.0), std=(1.0, 1.0, 1.0)):  # IMAGENET_MEAN, IMAGENET_STD
     # Transforms to apply if albumentations not installed
-    if not isinstance(size,int):
+    if not isinstance(size, int):
         raise TypeError(f'classify_transforms() size {size} must be integer, not (list, tuple)')
-    if any(mean) or any(std, *args, **kwargs):
+    if any(mean) or any(std):
         return T.Compose([CenterCrop(size), ToTensor(), T.Normalize(mean, std, inplace=True)])
     else:
         return T.Compose([CenterCrop(size), ToTensor()])
 
 
 def classify_albumentations(
         augment=True,
         size=224,
         scale=(0.08, 1.0),
         hflip=0.5,
         vflip=0.0,
         jitter=0.4,
-        mean=(0.0, 0.0, 0.0), 
+        mean=(0.0, 0.0, 0.0),
         std=(1.0, 1.0, 1.0),
         auto_aug=False
-, *args, **kwargs):
+        , *args, **kwargs):
     # PJYoloVision classification Albumentations (optional, only used if package is installed)
     prefix = colorstr('albumentations: ')
     try:
         import albumentations as A
         from albumentations.pytorch import ToTensorV2
 
         check_version(A.__version__, '1.0.3', hard=True)  # version requirement
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/base.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         irect = ar.argsort()
         self.im_files = [self.im_files[i] for i in irect]
         self.labels = [self.labels[i] for i in irect]
         ar = ar[irect]
 
         # Set training image shapes
         shapes = [[1, 1]] * nb
-        for i in range(nb):
+        for i in range(nb, *args, **kwargs):
             ari = ar[bi == i]
             mini, maxi = ari.min(), ari.max()
             if maxi < 1:
                 shapes[i] = [maxi, 1]
             elif mini > 1:
                 shapes[i] = [1, 1 / mini]
 
@@ -185,15 +185,15 @@
             label['resized_shape'][1] / label['ori_shape'][1],
         )  # for evaluation
         if self.rect:
             label['rect_shape'] = self.batch_shapes[self.batch[index]]
         label = self.update_labels_info(label)
         return label
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.labels)
 
     def update_labels_info(self, label, *args, **kwargs):
         """custom your label format here"""
         return label
 
     def build_transforms(self, hyp=None, *args, **kwargs):
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/build.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import torch
 from PIL import Image
 from torch.utils.data import DataLoader, dataloader, distributed
 
 from PJYoloVision.yolo.data.dataloaders.stream_loaders import (LOADERS, LoadImages, LoadPilAndNumpy,
-                                                               LoadStreams, LoadTensor, SourceTypes, autocast_list)
+                                                             LoadStreams, LoadTensor, SourceTypes, autocast_list)
 from PJYoloVision.yolo.data.utils import IMG_FORMATS, VID_FORMATS
 from PJYoloVision.yolo.utils.checks import check_file
 
 from ..utils import LOGGER, RANK, colorstr
 from ..utils.torch_utils import torch_distributed_zero_first
 from .dataset import ClassificationDataset, YOLODataset
 from .utils import PIN_MEMORY
@@ -27,15 +27,15 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         object.__setattr__(self, 'batch_sampler', _RepeatSampler(self.batch_sampler))
         self.iterator = super().__iter__()
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.batch_sampler.sampler)
 
     def __iter__(self, *args, **kwargs):
         for _ in range(len(self)):
             yield next(self.iterator)
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/stream_loaders.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/stream_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.imgsz = imgsz
         self.stride = stride
         self.vid_stride = vid_stride  # video frame-rate stride
         sources = Path(sources).read_text().rsplit() if os.path.isfile(sources) else [sources]
         n = len(sources)
         self.sources = [ops.clean_str(x) for x in sources]  # clean source names for later
         self.imgs, self.fps, self.frames, self.threads = [None] * n, [0] * n, [0] * n, [None] * n
-        for i, s in enumerate(sources):  # index, source
+        for i, s in enumerate(sources, *args, **kwargs):  # index, source
             # Start thread to read frames from video stream
             st = f'{i + 1}/{n}: {s}... '
             if urlparse(s).hostname in ('www.youtube.com', 'youtube.com', 'youtu.be'):
 
                  
                 import pafy  # noqa
                 s = pafy.new(s).getbest(preftype='mp4').url  # YouTube URL
@@ -111,15 +111,15 @@
         else:
             im = np.stack([LetterBox(self.imgsz, self.auto, stride=self.stride)(image=x) for x in im0])
             im = im[..., ::-1].transpose((0, 3, 1, 2))  # BGR to RGB, BHWC to BCHW
             im = np.ascontiguousarray(im)  # contiguous
 
         return self.sources, im, im0, None, ''
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.sources)  # 1E12 frames = 32 streams at 30 FPS for 30 years
 
 
 class LoadImages:
     # PJYoloVision image/video dataloader, i.e. `yolo predict source=image.jpg/vid.mp4`
     def __init__(self, path, imgsz=640, stride=32, auto=True, transforms=None, vid_stride=1, *args, **kwargs):
         if isinstance(path, str) and Path(path).suffix == '.txt':  # *.txt file with img/vid/dir on each line
@@ -167,15 +167,15 @@
         if self.count == self.nf:
             raise StopIteration
         path = self.files[self.count]
 
         if self.video_flag[self.count]:
             # Read video
             self.mode = 'video'
-            for _ in range(self.vid_stride):
+            for _ in range(self.vid_stride, *args, **kwargs):
                 self.cap.grab()
             success, im0 = self.cap.retrieve()
             while not success:
                 self.count += 1
                 self.cap.release()
                 if self.count == self.nf:  # last video
                     raise StopIteration
@@ -218,15 +218,15 @@
             return cv2.rotate(im, cv2.ROTATE_90_CLOCKWISE)
         elif self.orientation == 180:
             return cv2.rotate(im, cv2.ROTATE_90_COUNTERCLOCKWISE)
         elif self.orientation == 90:
             return cv2.rotate(im, cv2.ROTATE_180)
         return im
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return self.nf  # number of files
 
 
 class LoadPilAndNumpy:
 
     def __init__(self, im0, imgsz=640, stride=32, auto=True, transforms=None, *args, **kwargs):
         if not isinstance(im0, list):
@@ -256,15 +256,15 @@
             im = self.transforms(im)  # transforms
         else:
             im = LetterBox(self.imgsz, auto=auto, stride=self.stride)(image=im)
             im = im.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
             im = np.ascontiguousarray(im)  # contiguous
         return im
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.im0)
 
     def __next__(self, *args, **kwargs):
         if self.count == 1:  # loop only once as it's batch inference
             raise StopIteration
         auto = all(x.shape == self.im0[0].shape for x in self.im0) and self.auto
         im = [self._single_preprocess(im, auto) for im in self.im0]
@@ -290,15 +290,15 @@
 
     def __next__(self, *args, **kwargs):
         if self.count == 1:
             raise StopIteration
         self.count += 1
         return None, self.im0, self.im0, None, ''  # self.paths, im, self.im0, None, ''
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return self.bs
 
 
 def autocast_list(source, *args, **kwargs):
     """
     Merges a list of source of different types into a list of numpy arrays or PIL images
     """
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5augmentations.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/v5augmentations.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 def normalize(x, mean=IMAGENET_MEAN, std=IMAGENET_STD, inplace=False, *args, **kwargs):
     # Denormalize RGB images x per ImageNet stats in BCHW format, i.e. = (x - mean) / std
     return TF.normalize(x, mean, std, inplace=inplace)
 
 
 def denormalize(x, mean=IMAGENET_MEAN, std=IMAGENET_STD, *args, **kwargs):
     # Denormalize RGB images x per ImageNet stats in BCHW format, i.e. = x * std + mean
-    for i in range(3):
+    for i in range(3, *args, **kwargs):
         x[:, i] = x[:, i] * std[i] + mean[i]
     return x
 
 
 def augment_hsv(im, hgain=0.5, sgain=0.5, vgain=0.5, *args, **kwargs):
     # HSV color-space augmentation
     if hgain or sgain or vgain:
@@ -202,16 +202,16 @@
 
     # Transform label coordinates
     n = len(targets)
     if n:
         use_segments = any(x.any() for x in segments)
         new = np.zeros((n, 4))
         if use_segments:  # warp segments
-            segments = resample_segments(segments)
-            for i, segmentation in enumerate(segments):
+            segments = resample_segments(segments)  # upsample
+            for i, segmentation in enumerate(segments, *args, **kwargs):
                 xy = np.ones((len(segmentation), 3))
                 xy[:, :2] = segmentation
                 xy = xy @ M.T  # transform
                 xy = xy[:, :2] / xy[:, 2:3] if perspective else xy[:, :2]  # perspective rescale or affine
 
                 # clip
                 new[i] = segment2box(xy, width, height)
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5loader.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataloaders/v5loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import torch
 import torchvision
 from PIL import ExifTags, Image, ImageOps
 from torch.utils.data import DataLoader, Dataset, dataloader, distributed
 from tqdm import tqdm
 
 from PJYoloVision.yolo.utils import (DATASETS_DIR, LOGGER, NUM_THREADS, TQDM_BAR_FORMAT, is_colab, is_dir_writeable,
-                                     is_kaggle)
+                                   is_kaggle)
 
 from PJYoloVision.yolo.utils.ops import clean_str, segments2boxes, xyn2xy, xywh2xyxy, xywhn2xyxy, xyxy2xywhn
 from PJYoloVision.yolo.utils.torch_utils import torch_distributed_zero_first
 
 from .v5augmentations import (Albumentations, augment_hsv, classify_albumentations, classify_transforms, copy_paste,
                               letterbox, mixup, random_perspective)
 
@@ -149,15 +149,15 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         object.__setattr__(self, 'batch_sampler', _RepeatSampler(self.batch_sampler))
         self.iterator = super().__iter__()
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.batch_sampler.sampler)
 
     def __iter__(self, *args, **kwargs):
         for _ in range(len(self)):
             yield next(self.iterator)
 
 
@@ -221,15 +221,15 @@
         if self.count == self.nf:
             raise StopIteration
         path = self.files[self.count]
 
         if self.video_flag[self.count]:
             # Read video
             self.mode = 'video'
-            for _ in range(self.vid_stride):
+            for _ in range(self.vid_stride, *args, **kwargs):
                 self.cap.grab()
             ret_val, im0 = self.cap.retrieve()
             while not ret_val:
                 self.count += 1
                 self.cap.release()
                 if self.count == self.nf:  # last video
                     raise StopIteration
@@ -271,15 +271,15 @@
             return cv2.rotate(im, cv2.ROTATE_90_CLOCKWISE)
         elif self.orientation == 180:
             return cv2.rotate(im, cv2.ROTATE_90_COUNTERCLOCKWISE)
         elif self.orientation == 90:
             return cv2.rotate(im, cv2.ROTATE_180)
         return im
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return self.nf  # number of files
 
 
 class LoadStreams:
     # YOLOv5 streamloader, i.e. `python detection.py --source 'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP streams`
     def __init__(self, sources='file.streams', img_size=640, stride=32, auto=True, transforms=None, vid_stride=1, *args,
                  **kwargs):
@@ -288,15 +288,15 @@
         self.img_size = img_size
         self.stride = stride
         self.vid_stride = vid_stride  # video frame-rate stride
         sources = Path(sources).read_text().rsplit() if os.path.isfile(sources) else [sources]
         n = len(sources)
         self.sources = [clean_str(x) for x in sources]  # clean source names for later
         self.imgs, self.fps, self.frames, self.threads = [None] * n, [0] * n, [0] * n, [None] * n
-        for i, s in enumerate(sources):  # index, source
+        for i, s in enumerate(sources, *args, **kwargs):  # index, source
             # Start thread to read frames from video stream
             st = f'{i + 1}/{n}: {s}... '
             if urlparse(s).hostname in ('www.youtube.com', 'youtube.com', 'youtu.be'):
 
                 import pafy
                 s = pafy.new(s).getbest(preftype='mp4').url
             s = eval(s) if s.isnumeric() else s
@@ -357,15 +357,15 @@
         else:
             im = np.stack([letterbox(x, self.img_size, stride=self.stride, auto=self.auto)[0] for x in im0])  # resize
             im = im[..., ::-1].transpose((0, 3, 1, 2))  # BGR to RGB, BHWC to BCHW
             im = np.ascontiguousarray(im)  # contiguous
 
         return self.sources, im, im0, None, ''
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.sources)  # 1E12 frames = 32 streams at 30 FPS for 30 years
 
 
 def img2label_paths(img_paths, *args, **kwargs):
     # Define label paths as a function of image paths
     sa, sb = f'{os.sep}images{os.sep}', f'{os.sep}labels{os.sep}'  # /images/, /labels/ substrings
     return [sb.join(x.rsplit(sa, 1)).rsplit('.', 1)[0] + '.txt' for x in img_paths]
@@ -492,15 +492,15 @@
             self.labels = [self.labels[i] for i in irect]
             self.segments = [self.segments[i] for i in irect]
             self.shapes = s[irect]  # wh
             ar = ar[irect]
 
             # Set training image shapes
             shapes = [[1, 1]] * nb
-            for i in range(nb):
+            for i in range(nb, *args, **kwargs):
                 ari = ar[bi == i]
                 mini, maxi = ari.min(), ari.max()
                 if maxi < 1:
                     shapes[i] = [maxi, 1]
                 elif mini > 1:
                     shapes[i] = [1, 1 / mini]
 
@@ -527,15 +527,15 @@
                     pbar.desc = f'{prefix}Caching images ({b / gb:.1f}GB {cache_images})'
                 pbar.close()
 
     def check_cache_ram(self, safety_margin=0.1, prefix='', *args, **kwargs):
         # Check image caching requirements vs available memory
         b, gb = 0, 1 << 30  # bytes of cached images, bytes per gigabytes
         n = min(self.n, 30)  # extrapolate from 30 random images
-        for _ in range(n):
+        for _ in range(n, *args, **kwargs):
             im = cv2.imread(random.choice(self.im_files))  # sample image
             ratio = self.img_size / max(im.shape[0], im.shape[1])  # max(h, w)  # ratio
             b += im.nbytes * ratio ** 2
         mem_required = b * self.n / n  # GB required to cache dataset into RAM
         mem = psutil.virtual_memory()
         cache = mem_required * (1 + safety_margin) < mem.available  # to cache or not to cache, that is the question
         if not cache:
@@ -579,15 +579,15 @@
             np.save(str(path), x)  # save cache for next time
             path.with_suffix('.cache.npy').rename(path)  # remove .npy suffix
             LOGGER.info(f'{prefix}New cache created: {path}')
         else:
             LOGGER.warning(f'{prefix}Opps Wait  Cache directory {path.parent} is not writeable')  # not writeable
         return x
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.im_files)
 
     # def __iter__(self, *args, **kwargs):
     #     self.count = -1
     #     print('ran dataset iter')
     #     #self.shuffled_vector = np.random.permutation(self.nF) if self.augment else np.arange(self.nF)
     #     return self
@@ -692,15 +692,15 @@
     def load_mosaic(self, index, *args, **kwargs):
         # YOLOv5 4-mosaic loader. Loads 1 image + 3 random images into a 4-image mosaic
         labels4, segments4 = [], []
         s = self.img_size
         yc, xc = (int(random.uniform(-x, 2 * s + x)) for x in self.mosaic_border)  # mosaic center x, y
         indices = [index] + random.choices(self.indices, k=3)  # 3 additional image indices
         random.shuffle(indices)
-        for i, index in enumerate(indices):
+        for i, index in enumerate(indices, *args, **kwargs):
             # Load image
             img, _, (h, w) = self.load_image(index)
 
             # place img in img4
             if i == 0:  # top left
                 img4 = np.full((s * 2, s * 2, img.shape[2]), 114, dtype=np.uint8)  # base image with 4 tiles
                 x1a, y1a, x2a, y2a = max(xc - w, 0), max(yc - h, 0), xc, yc  # xmin, ymin, xmax, ymax (large image)
@@ -750,15 +750,15 @@
     def load_mosaic9(self, index, *args, **kwargs):
         # YOLOv5 9-mosaic loader. Loads 1 image + 8 random images into a 9-image mosaic
         labels9, segments9 = [], []
         s = self.img_size
         indices = [index] + random.choices(self.indices, k=8)  # 8 additional image indices
         random.shuffle(indices)
         hp, wp = -1, -1  # height, width previous
-        for i, index in enumerate(indices):
+        for i, index in enumerate(indices, *args, **kwargs):
             # Load image
             img, _, (h, w) = self.load_image(index)
 
             # place img in img9
             if i == 0:  # center
                 img9 = np.full((s * 3, s * 3, img.shape[2]), 114, dtype=np.uint8)  # base image with 4 tiles
                 h0, w0 = h, w
@@ -824,15 +824,15 @@
 
         return img9, labels9
 
     @staticmethod
     def collate_fn(batch, *args, **kwargs):
         # PJYoloVision collate function, outputs dict
         im, label, path, shapes = zip(*batch)  # transposed
-        for i, lb in enumerate(label):
+        for i, lb in enumerate(label, *args, **kwargs):
             lb[:, 0] = i  # add target image index for build_targets()
         batch_idx, cls, bboxes = torch.cat(label, 0).split((1, 1, 4), dim=1)
         return {
             'ori_shape': tuple((x[0] if x else None) for x in shapes),
             'ratio_pad': tuple((x[1] if x else None) for x in shapes),
             'im_file': path,
             'img': torch.stack(im, 0),
@@ -840,15 +840,15 @@
             'bboxes': bboxes,
             'batch_idx': batch_idx.view(-1)}
 
     @staticmethod
     def collate_fn_old(batch, *args, **kwargs):
         # YOLOv5 original collate function
         im, label, path, shapes = zip(*batch)  # transposed
-        for i, lb in enumerate(label):
+        for i, lb in enumerate(label, *args, **kwargs):
             lb[:, 0] = i  # add target image index for build_targets()
         return torch.stack(im, 0), torch.cat(label, 0), path, shapes
 
 
 # Ancillary functions --------------------------------------------------------------------------------------------------
 def flatten_recursive(path=DATASETS_DIR / 'coco128', *args, **kwargs):
     # Flatten a recursive directory by bringing all files to top level
@@ -874,15 +874,15 @@
 
             # labels
             lb_file = Path(img2label_paths([str(im_file)])[0])
             if Path(lb_file).exists():
                 with open(lb_file) as f:
                     lb = np.array([x.split() for x in f.read().strip().splitlines()], dtype=np.float32)  # labels
 
-                for j, x in enumerate(lb):
+                for j, x in enumerate(lb, *args, **kwargs):
                     c = int(x[0])  # class
                     f = (path / 'classifier') / f'{c}' / f'{path.stem}_{im_file.stem}_{j}.jpg'  # new filename
                     if not f.parent.is_dir():
                         f.parent.mkdir(parents=True)
 
                     b = x[1:] * [w, h, w, h]  # box
                     # b[2:] = b[2:].max()  # rectangle to square
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         return label
 
     @staticmethod
     def collate_fn(batch, *args, **kwargs):
         new_batch = {}
         keys = batch[0].keys()
         values = list(zip(*[list(b.values()) for b in batch]))
-        for i, k in enumerate(keys):
+        for i, k in enumerate(keys, *args, **kwargs):
             value = values[i]
             if k == 'img':
                 value = torch.stack(value, 0)
             if k in ['masks', 'keypoints', 'bboxes', 'cls']:
                 value = torch.cat(value, 0)
             new_batch[k] = value
         new_batch['batch_idx'] = list(new_batch['batch_idx'])
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset_wrappers.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/dataset_wrappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,26 @@
         transforms (Sequence[dict], *args, **kwargs): config dict to be composed.
     """
 
     def __init__(self, dataset, *args, **kwargs):
         self.dataset = dataset
         self.imgsz = dataset.imgsz
 
-    def __len__(self):
+    def __len__(self, *args, **kwargs):
         return len(self.dataset)
 
     def __getitem__(self, index, *args, **kwargs):
         labels = deepcopy(self.dataset[index])
         for transform in self.dataset.transforms.tolist():
             # mosaic and mixup
-            if hasattr(transform, 'get_indexes'):
+            if hasattr(transform, 'get_indexes', *args, **kwargs):
                 indexes = transform.get_indexes(self.dataset)
-                if not isinstance(indexes, collections.abc.Sequence):
+                if not isinstance(indexes, collections.abc.Sequence, *args, **kwargs):
                     indexes = [indexes]
                 mix_labels = [deepcopy(self.dataset[index]) for index in indexes]
                 labels['mix_labels'] = mix_labels
-            if self.dataset.rect and isinstance(transform, LetterBox):
+            if self.dataset.rect and isinstance(transform, LetterBox, *args, **kwargs):
                 transform.new_shape = self.dataset.batch_shapes[self.dataset.batch[index]]
             labels = transform(labels)
             if 'mix_labels' in labels:
                 labels.pop('mix_labels')
         return labels
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/data/utils.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/__init__.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/autobatch.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/benchmarks.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/benchmarks.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from PJYoloVision.yolo.utils import LINUX, LOGGER, MACOS, ROOT, SETTINGS
 from PJYoloVision.yolo.utils.checks import check_yolo
 from PJYoloVision.yolo.utils.downloads import download
 from PJYoloVision.yolo.utils.files import file_size
 from PJYoloVision.yolo.utils.torch_utils import select_device
 
 
-def benchmark(model=Path(SETTINGS['weights_dir']) / 'YOLOvisionn.pt', imgsz=160, half=False, device='cpu', hard_fail=False, *args, **kwargs):
+def benchmark(model=Path(SETTINGS['weights_dir']) / 'PJYoloVision.pt', imgsz=160, half=False, device='cpu', hard_fail=False, *args, **kwargs):
     import pandas as pd
     pd.options.display.max_columns = 10
     pd.options.display.width = 120
     device = select_device(device, detail=False)
     if isinstance(model, (str, Path)):
         model = YOLO(model)
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/base.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/clearml.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/comet.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/hub.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/tensorboard.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/checks.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     return check_version(platform.python_version(), minimum, name='Python ', hard=True)
 
 
 @TryExcept()
 def check_requirements(requirements=ROOT.parent / 'requirements.txt', exclude=(), install=True, cmds='', *args, **kwargs):
     pass
 
-def check_suffix(file='YOLOvisionn.pt', suffix='.pt', msg='', *args, **kwargs):
+def check_suffix(file='PJYoloVision.pt', suffix='.pt', msg='', *args, **kwargs):
     # Check file(s) for acceptable suffix
     if file and suffix:
         if isinstance(suffix, str):
             suffix = (suffix, )
         for f in file if isinstance(file, (list, tuple)) else [file]:
             s = Path(f).suffix.lower().strip()  # file suffix
             if len(s):
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/dist.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/downloads.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/files.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/instance.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/loss.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/metrics.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/ops.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/plotting.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/tal.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/torch_utils.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/utils/torch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return (torch.inference_mode if TORCH_1_9 else torch.no_grad)()(fn)
 
     return decorate
 
 
 def select_device(device='', batch=0, newline=False, detail=True, *args, **kwargs):
     # device = None or 'cpu' or 0 or '0' or '0,1,2,3'
-    s = f'YOLOvision YOLOv{__version__} 🚀 Python-{platform.python_version()} torch-{torch.__version__} '
+    s = f'PJYoloVision YOLOv{__version__} 🚀 Python-{platform.python_version()} torch-{torch.__version__} '
     device = str(device).lower()
     for remove in 'cuda:', 'none', '(', ')', '[', ']', "'", ' ':
         device = device.replace(remove, '')  # to string, 'cuda:0' -> '0' and '(0, 1)' -> '0,1'
     cpu = device == 'cpu'
     mps = device == 'mps'  # Apple Metal Performance Shaders (MPS)
     if cpu or mps:
         os.environ['CUDA_VISIBLE_DEVICES'] = '-1'  # force torch.cuda.is_available() = False
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/predict.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/train.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
  
 
 import torch
 import torchvision
 
 from PJYoloVision.nn.tasks import ClassificationModel, attempt_load_one_weight
 from PJYoloVision.yolo import vision
-from PJYoloVision.yolo.data import build_classification_dataloader
+
+
 from PJYoloVision.yolo.core.trainer import BaseTrainer
+from PJYoloVision.yolo.data import build_classification_dataloader
 from PJYoloVision.yolo.utils import DEFAULT_CFG, LOGGER, RANK, colorstr
 from PJYoloVision.yolo.utils.torch_utils import is_parallel, strip_optimizer
 
 
 class ClassificationTrainer(BaseTrainer):
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, *args, **kwargs):
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/val.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/classify/val.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
- 
 
-from PJYoloVision.yolo.data import build_classification_dataloader
 from PJYoloVision.yolo.core.validator import BaseValidator
-from PJYoloVision.yolo.utils import DEFAULT_CFG, LOGGER
+from PJYoloVision.yolo.data import build_classification_dataloader
+from PJYoloVision.yolo.utils import  LOGGER
 from PJYoloVision.yolo.utils.metrics import ClassifyMetrics
 
 
 class ClassificationValidator(BaseValidator):
 
     def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, **kwargs):
         super().__init__(dataloader, save_dir, pbar, args)
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/predict.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/train.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/detection/train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,82 @@
+import os
 from copy import copy
 
 import numpy as np
 import torch
 import torch.nn as nn
+from torch.utils.data import DataLoader, distributed
 
 from PJYoloVision.nn.tasks import DetectionModel
 from PJYoloVision.yolo import vision
-from PJYoloVision.yolo.data import build_dataloader
-from PJYoloVision.yolo.data.dataloaders.v5loader import create_dataloader
+
+from PJYoloVision.yolo.core.predictor import PIN_MEMORY
 from PJYoloVision.yolo.core.trainer import BaseTrainer
+from PJYoloVision.yolo.data import build_dataloader
+from PJYoloVision.yolo.data.dataloaders.v5loader import LoadImagesAndLabels, InfiniteDataLoader, seed_worker
 from PJYoloVision.yolo.utils import RANK, colorstr
 from PJYoloVision.yolo.utils.loss import BboxLoss
 from PJYoloVision.yolo.utils.ops import xywh2xyxy
 from PJYoloVision.yolo.utils.plotting import plot_images, plot_labels, plot_results
 from PJYoloVision.yolo.utils.tal import TaskAlignedAssigner, dist2bbox, make_anchors
-from PJYoloVision.yolo.utils.torch_utils import de_parallel
+from PJYoloVision.yolo.utils.torch_utils import de_parallel, torch_distributed_zero_first
+
+
+def create_dataloader(path,
+                      imgsz,
+                      batch_size,
+                      stride,
+                      single_cls=False,
+                      hyp=None,
+                      augment=False,
+                      cache=False,
+                      pad=0.0,
+                      rect=False,
+                      rank=-1,
+                      workers=8,
+                      image_weights=False,
+                      close_mosaic=False,
+                      min_items=0,
+                      prefix='',
+                      shuffle=False,
+                      seed=0, *args, **kwargs):
+    if rect and shuffle:
+        shuffle = False
+    with torch_distributed_zero_first(rank):
+        dataset = LoadImagesAndLabels(
+            path,
+            imgsz,
+            batch_size,
+            augment=augment,  # augmentation
+            hyp=hyp,  # hyperparameters
+            rect=rect,  # rectangular batches
+            cache_images=cache,
+            single_cls=single_cls,
+            stride=int(stride),
+            pad=pad,
+            image_weights=image_weights,
+            min_items=min_items,
+            prefix=prefix)
+
+    batch_size = min(batch_size, len(dataset))
+    nd = torch.cuda.device_count()  # number of CUDA devices
+    nw = min([os.cpu_count() // max(nd, 1), batch_size if batch_size > 1 else 0, workers])  # number of workers
+    sampler = None if rank == -1 else distributed.DistributedSampler(dataset, shuffle=shuffle)
+    loader = DataLoader if image_weights or close_mosaic else InfiniteDataLoader  # DataLoader allows attribute updates
+    generator = torch.Generator()
+    generator.manual_seed(6148914691236517205 + seed + RANK)
+    return loader(dataset,
+                  batch_size=batch_size,
+                  shuffle=shuffle and sampler is None,
+                  num_workers=nw,
+                  sampler=sampler,
+                  pin_memory=PIN_MEMORY,
+                  collate_fn=LoadImagesAndLabels.collate_fn,
+                  worker_init_fn=seed_worker,
+                  generator=generator), dataset
 
 
 # BaseTrainer python usage
 class DetectionTrainer(BaseTrainer):
 
     def get_dataloader(self, dataset_path, batch_size, mode='train', rank=0):
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/val.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/val.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,83 @@
- 
-
-import os
+from multiprocessing.pool import ThreadPool
 from pathlib import Path
 
 import numpy as np
 import torch
+import torch.nn.functional as F
+
+from PJYoloVision.yolo.utils import DEFAULT_CFG, LOGGER, NUM_THREADS, ops
 
-from PJYoloVision.yolo.data import build_dataloader
-from PJYoloVision.yolo.data.dataloaders.v5loader import create_dataloader
-from PJYoloVision.yolo.core.validator import BaseValidator
-from PJYoloVision.yolo.utils import DEFAULT_CFG, LOGGER, colorstr, ops
- 
-from PJYoloVision.yolo.utils.metrics import ConfusionMatrix, DetMetrics, box_iou
+from PJYoloVision.yolo.utils.metrics import SegmentMetrics, box_iou, mask_iou
 from PJYoloVision.yolo.utils.plotting import output_to_target, plot_images
-from PJYoloVision.yolo.utils.torch_utils import de_parallel
+from PJYoloVision.yolo.vision.detection import DetectionValidator
 
 
-class DetectionValidator(BaseValidator):
+class SegmentationValidator(DetectionValidator):
 
     def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, **kwargs):
         super().__init__(dataloader, save_dir, pbar, args)
-        self.args.task = 'detection'
-        self.is_coco = False
-        self.class_map = None
-        self.metrics = DetMetrics(save_dir=self.save_dir)
-        self.iouv = torch.linspace(0.5, 0.95, 10)  # iou vector for mAP@0.5:0.95
-        self.niou = self.iouv.numel()
+        self.args.task = 'segmentation'
+        self.metrics = SegmentMetrics(save_dir=self.save_dir)
 
     def preprocess(self, batch, *args, **kwargs):
-        batch['img'] = batch['img'].to(self.device, non_blocking=True)
-        batch['img'] = (batch['img'].half() if self.args.half else batch['img'].float()) / 255
-        for k in ['batch_idx', 'cls', 'bboxes']:
-            batch[k] = batch[k].to(self.device)
-
-        nb = len(batch['img'])
-        self.lb = [torch.cat([batch['cls'], batch['bboxes']], dim=-1)[batch['batch_idx'] == i]
-                   for i in range(nb)] if self.args.save_hybrid else []  # for autolabelling
-
+        batch = super().preprocess(batch)
+        batch['masks'] = batch['masks'].to(self.device).float()
         return batch
 
     def init_metrics(self, model, *args, **kwargs):
-        val = self.data.get(self.args.split, '')  # validation path
-        self.is_coco = isinstance(val, str) and val.endswith(f'coco{os.sep}val2017.txt')  # is COCO dataset
-        self.class_map = list(range(1000))
-        self.args.save_json |= self.is_coco and not self.training  # run on final val if training COCO
-        self.names = model.names
-        self.nc = len(model.names)
-        self.metrics.names = self.names
-        self.metrics.plot = self.args.plots
-        self.confusion_matrix = ConfusionMatrix(nc=self.nc)
-        self.seen = 0
-        self.jdict = []
-        self.stats = []
+        super().init_metrics(model)
+        self.plot_masks = []
+        if self.args.save_json:
+
+            self.process = ops.process_mask_upsample  # more accurate
+        else:
+            self.process = ops.process_mask  # faster
 
     def get_desc(self, *args, **kwargs):
-        return ('%22s' + '%11s' * 6) % ('Class', 'Images', 'Instances', 'Box(P', 'R', 'mAP50', 'mAP50-95)')
+        return ('%22s' + '%11s' * 10) % ('Class', 'Images', 'Instances', 'Box(P', 'R', 'mAP50', 'mAP50-95)', 'Mask(P',
+                                         'R', 'mAP50', 'mAP50-95)')
 
     def postprocess(self, preds, *args, **kwargs):
-        preds = ops.non_max_suppression(preds,
-                                        self.args.conf,
-                                        self.args.iou,
-                                        labels=self.lb,
-                                        multi_label=True,
-                                        agnostic=self.args.single_cls,
-                                        max_det=self.args.max_det)
-        return preds
+        p = ops.non_max_suppression(preds[0],
+                                    self.args.conf,
+                                    self.args.iou,
+                                    labels=self.lb,
+                                    multi_label=True,
+                                    agnostic=self.args.single_cls,
+                                    max_det=self.args.max_det,
+                                    nc=self.nc)
+        proto = preds[1][-1] if len(preds[1]) == 3 else preds[1]  # second output is len 3 if pt, but only 1 if exported
+        return p, proto
 
     def update_metrics(self, preds, batch, *args, **kwargs):
         # Metrics
-        for si, pred in enumerate(preds):
+        for si, (pred, proto) in enumerate(zip(preds[0], preds[1])):
             idx = batch['batch_idx'] == si
             cls = batch['cls'][idx]
             bbox = batch['bboxes'][idx]
             nl, npr = cls.shape[0], pred.shape[0]  # number of labels, predictions
             shape = batch['ori_shape'][si]
+            correct_masks = torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device)  # init
             correct_bboxes = torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device)  # init
             self.seen += 1
 
             if npr == 0:
                 if nl:
-                    self.stats.append((correct_bboxes, *torch.zeros((2, 0), device=self.device), cls.squeeze(-1)))
+                    self.stats.append((correct_masks, correct_bboxes, *torch.zeros(
+                        (2, 0), device=self.device), cls.squeeze(-1)))
                     if self.args.plots:
                         self.confusion_matrix.process_batch(detections=None, labels=cls.squeeze(-1))
                 continue
 
+            # Masks
+            midx = [si] if self.args.overlap_mask else idx
+            gt_masks = batch['masks'][midx]
+            pred_masks = self.process(proto, pred[:, 6:], pred[:, :4], shape=batch['img'][si].shape[1:])
+
             # Predictions
             if self.args.single_cls:
                 pred[:, 5] = 0
             predn = pred.clone()
             ops.scale_boxes(batch['img'][si].shape[1:], predn[:, :4], shape,
                             ratio_pad=batch['ratio_pad'][si])  # native-space pred
 
@@ -97,141 +87,164 @@
                 tbox = ops.xywh2xyxy(bbox) * torch.tensor(
                     (width, height, width, height), device=self.device)  # target boxes
                 ops.scale_boxes(batch['img'][si].shape[1:], tbox, shape,
                                 ratio_pad=batch['ratio_pad'][si])  # native-space labels
                 labelsn = torch.cat((cls, tbox), 1)  # native-space labels
                 correct_bboxes = self._process_batch(predn, labelsn)
                 # TODO: maybe remove these `self.` arguments as they already are member variable
+                correct_masks = self._process_batch(predn,
+                                                    labelsn,
+                                                    pred_masks,
+                                                    gt_masks,
+                                                    overlap=self.args.overlap_mask,
+                                                    masks=True)
                 if self.args.plots:
                     self.confusion_matrix.process_batch(predn, labelsn)
-            self.stats.append((correct_bboxes, pred[:, 4], pred[:, 5], cls.squeeze(-1)))  # (conf, pcls, tcls)
+
+            # Append correct_masks, correct_boxes, pconf, pcls, tcls
+            self.stats.append((correct_masks, correct_bboxes, pred[:, 4], pred[:, 5], cls.squeeze(-1)))
+
+            pred_masks = torch.as_tensor(pred_masks, dtype=torch.uint8)
+            if self.args.plots and self.batch_i < 3:
+                self.plot_masks.append(pred_masks[:15].cpu())  # filter top 15 to plot
 
             # Save
             if self.args.save_json:
-                self.pred_to_json(predn, batch['im_file'][si])
-            if self.args.save_txt:
-                file = self.save_dir / 'labels' / f'{Path(batch["im_file"][si]).stem}.txt'
-                self.save_one_txt(predn, self.args.save_conf, shape, file)
+                pred_masks = ops.scale_image(batch['img'][si].shape[1:],
+                                             pred_masks.permute(1, 2, 0).contiguous().cpu().numpy(),
+                                             shape,
+                                             ratio_pad=batch['ratio_pad'][si])
+                self.pred_to_json(predn, batch['im_file'][si], pred_masks)
+            # if self.args.save_txt:
+            #    save_one_txt(predn, save_conf, shape, file=save_dir / 'labels' / f'{path.stem}.txt')
 
     def finalize_metrics(self, *args, **kwargs):
         self.metrics.speed = self.speed
         self.metrics.confusion_matrix = self.confusion_matrix
 
-    def get_stats(self, *args, **kwargs):
-        stats = [torch.cat(x, 0).cpu().numpy() for x in zip(*self.stats)]  # to numpy
-        if len(stats) and stats[0].any():
-            self.metrics.process(*stats)
-        self.nt_per_class = np.bincount(stats[-1].astype(int), minlength=self.nc)  # number of targets per class
-        return self.metrics.results_dict
-
-    def print_results(self, *args, **kwargs):
-        pf = '%22s' + '%11i' * 2 + '%11.3g' * len(self.metrics.keys)  # print format
-        LOGGER.info(pf % ('all', self.seen, self.nt_per_class.sum(), *self.metrics.mean_results()))
-        if self.nt_per_class.sum() == 0:
-            LOGGER.warning(
-                f'Opps Wait  no labels found in {self.args.task} set, can not compute metrics without labels')
-
-        # Print results per class
-        if self.args.detail and not self.training and self.nc > 1 and len(self.stats):
-            for i, c in enumerate(self.metrics.ap_class_index):
-                LOGGER.info(pf % (self.names[c], self.seen, self.nt_per_class[c], *self.metrics.class_result(i)))
-
-        if self.args.plots:
-            self.confusion_matrix.plot(save_dir=self.save_dir, names=list(self.names.values()))
+    def _process_batch(self, detections, labels, pred_masks=None, gt_masks=None, overlap=False, masks=False, *args,
+                       **kwargs):
+        """
+        Return correct prediction matrix
+        Arguments:
+            detections (array[N, 6]), x1, y1, x2, y2, conf, class
+            labels (array[M, 5]), class, x1, y1, x2, y2
+        Returns:
+            correct (array[N, 10]), for 10 IoU levels
+        """
+        if masks:
+            if overlap:
+                nl = len(labels)
+                index = torch.arange(nl, device=gt_masks.device).view(nl, 1, 1) + 1
+                gt_masks = gt_masks.repeat(nl, 1, 1)  # shape(1,640,640) -> (n,640,640)
+                gt_masks = torch.where(gt_masks == index, 1.0, 0.0)
+            if gt_masks.shape[1:] != pred_masks.shape[1:]:
+                gt_masks = F.interpolate(gt_masks[None], pred_masks.shape[1:], mode='bilinear', align_corners=False)[0]
+                gt_masks = gt_masks.gt_(0.5)
+            iou = mask_iou(gt_masks.view(gt_masks.shape[0], -1), pred_masks.view(pred_masks.shape[0], -1))
+        else:  # boxes
+            iou = box_iou(labels[:, 1:], detections[:, :4])
 
-    def _process_batch(self, detections, labels, *args, **kwargs):
-
-        iou = box_iou(labels[:, 1:], detections[:, :4])
         correct = np.zeros((detections.shape[0], self.iouv.shape[0])).astype(bool)
+        labels = labels.to(detections)
         correct_class = labels[:, 0:1] == detections[:, 5]
         for i in range(len(self.iouv)):
-            x = torch.where((iou >= self.iouv[i]) & correct_class)
+            x = torch.where((iou >= self.iouv[i]) & correct_class)  # IoU > threshold and classes match
             if x[0].shape[0]:
                 matches = torch.cat((torch.stack(x, 1), iou[x[0], x[1]][:, None]),
-                                    1).cpu().numpy()
+                                    1).cpu().numpy()  # [label, detection, iou]
                 if x[0].shape[0] > 1:
                     matches = matches[matches[:, 2].argsort()[::-1]]
                     matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
+                    # matches = matches[matches[:, 2].argsort()[::-1]]
                     matches = matches[np.unique(matches[:, 0], return_index=True)[1]]
                 correct[matches[:, 1].astype(int), i] = True
         return torch.tensor(correct, dtype=torch.bool, device=detections.device)
 
-    def get_dataloader(self, dataset_path, batch_size, *args, **kwargs):
-        # TODO: manage splits differently
-        # calculate stride - check if model is initialized
-        gs = max(int(de_parallel(self.model).stride if self.model else 0), 32)
-        return create_dataloader(path=dataset_path,
-                                 imgsz=self.args.imgsz,
-                                 batch_size=batch_size,
-                                 stride=gs,
-                                 hyp=vars(self.args),
-                                 cache=False,
-                                 pad=0.5,
-                                 rect=self.args.rect,
-                                 workers=self.args.workers,
-                                 prefix=colorstr(f'{self.args.mode}: '),
-                                 shuffle=False,
-                                 seed=self.args.seed)[0] if self.args.v5loader else \
-            build_dataloader(self.args, batch_size, img_path=dataset_path, stride=gs, names=self.data['names'],
-                             mode='val')[0]
-
     def plot_val_samples(self, batch, ni, *args, **kwargs):
         plot_images(batch['img'],
                     batch['batch_idx'],
                     batch['cls'].squeeze(-1),
                     batch['bboxes'],
+                    batch['masks'],
                     paths=batch['im_file'],
                     fname=self.save_dir / f'val_batch{ni}_labels.jpg',
                     names=self.names)
 
     def plot_predictions(self, batch, preds, ni, *args, **kwargs):
         plot_images(batch['img'],
-                    *output_to_target(preds, max_det=15),
+                    *output_to_target(preds[0], max_det=15),
+                    torch.cat(self.plot_masks, dim=0) if len(self.plot_masks) else self.plot_masks,
                     paths=batch['im_file'],
                     fname=self.save_dir / f'val_batch{ni}_pred.jpg',
                     names=self.names)  # pred
+        self.plot_masks.clear()
 
-    def save_one_txt(self, predn, save_conf, shape, file, *args, **kwargs):
-        gn = torch.tensor(shape)[[1, 0, 1, 0]]  # normalization gain whwh
-        for *xyxy, conf, cls in predn.tolist():
-            xywh = (ops.xyxy2xywh(torch.tensor(xyxy).view(1, 4)) / gn).view(-1).tolist()  # normalized xywh
-            line = (cls, *xywh, conf) if save_conf else (cls, *xywh)  # label format
-            with open(file, 'a') as f:
-                f.write(('%g ' * len(line)).rstrip() % line + '\n')
+    def pred_to_json(self, predn, filename, pred_masks):
+        # Save one JSON result
+        # Example result = {"image_id": 42, "category_id": 18, "bbox": [258.15, 41.29, 348.26, 243.78], "score": 0.236}
+        from pycocotools.mask import encode  # noqa
+
+        def single_encode(x, *args, **kwargs):
+            rle = encode(np.asarray(x[:, :, None], order='F', dtype='uint8'))[0]
+            rle['counts'] = rle['counts'].decode('utf-8')
+            return rle
 
-    def pred_to_json(self, predn, filename, *args, **kwargs):
         stem = Path(filename).stem
         image_id = int(stem) if stem.isnumeric() else stem
         box = ops.xyxy2xywh(predn[:, :4])  # xywh
         box[:, :2] -= box[:, 2:] / 2  # xy center to top-left corner
-        for p, b in zip(predn.tolist(), box.tolist()):
+        pred_masks = np.transpose(pred_masks, (2, 0, 1))
+        with ThreadPool(NUM_THREADS) as pool:
+            rles = pool.map(single_encode, pred_masks)
+        for i, (p, b) in enumerate(zip(predn.tolist(), box.tolist())):
             self.jdict.append({
                 'image_id': image_id,
                 'category_id': self.class_map[int(p[5])],
                 'bbox': [round(x, 3) for x in b],
-                'score': round(p[4], 5)})
+                'score': round(p[4], 5),
+                'segmentation': rles[i]})
 
     def eval_json(self, stats, *args, **kwargs):
         if self.args.save_json and self.is_coco and len(self.jdict):
             anno_json = self.data['path'] / 'annotations/instances_val2017.json'  # annotations
             pred_json = self.save_dir / 'predictions.json'  # predictions
             LOGGER.info(f'\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...')
             try:
-                 
-                from pycocotools.coco import COCO
+
+                from pycocotools.coco import COCO  # noqa
                 from pycocotools.cocoeval import COCOeval  # noqa
 
                 for x in anno_json, pred_json:
                     assert x.is_file(), f'{x} file not found'
                 anno = COCO(str(anno_json))  # init annotations api
                 pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
-                eval = COCOeval(anno, pred, 'bbox')
-                if self.is_coco:
-                    eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # images to eval
-                eval.evaluate()
-                eval.accumulate()
-                eval.summarize()
-                stats[self.metrics.keys[-1]], stats[self.metrics.keys[-2]] = eval.stats[:2]  # update mAP50-95 and mAP50
+                for i, eval in enumerate([COCOeval(anno, pred, 'bbox'), COCOeval(anno, pred, 'segm')]):
+                    if self.is_coco:
+                        eval.params.imgIds = [int(Path(x).stem)
+                                              for x in self.dataloader.dataset.im_files]  # images to eval
+                    eval.evaluate()
+                    eval.accumulate()
+                    eval.summarize()
+                    idx = i * 4 + 2
+                    stats[self.metrics.keys[idx + 1]], stats[
+                        self.metrics.keys[idx]] = eval.stats[:2]  # update mAP50-95 and mAP50
             except Exception as e:
                 LOGGER.warning(f'pycocotools unable to run: {e}')
         return stats
 
+
+def val(cfg=DEFAULT_CFG, use_python=False, *args, **kwargs):
+    model = cfg.model or 'PJYoloVision-seg.pt'
+    data = cfg.data or 'coco128-seg.yaml'
+
+    args = dict(model=model, data=data)
+    if use_python:
+        from PJYoloVision import YOLO
+        YOLO(model).val(**args)
+    else:
+        validator = SegmentationValidator(args=args)
+        validator(model=args['model'])
+
+
+if __name__ == '__main__':
+    val()
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/predict.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/train.py` & `PJYoloVision-0.0.3/PJYoloVision/yolo/vision/segmentation/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         # Mask loss for one image
         pred_mask = (pred @ proto.view(self.nm, -1)).view(-1, *proto.shape[1:])  # (n, 32) @ (32,80,80) -> (n,80,80)
         loss = F.binary_cross_entropy_with_logits(pred_mask, gt_mask, reduction='none')
         return (crop_mask(loss, xyxy).mean(dim=(1, 2)) / area).mean()
 
 
 def train(cfg=DEFAULT_CFG, use_python=False, *args, **kwargs):
-    model = cfg.model or 'YOLOvisionn-seg.pt'
+    model = cfg.model or 'PJYoloVision-seg.pt'
     data = cfg.data or 'coco128-seg.yaml'  # or yolo.ClassificationDataset("mnist")
     device = cfg.device if cfg.device is not None else ''
 
     args = dict(model=model, data=data, device=device)
     if use_python:
         from PJYoloVision import YOLO
         YOLO(model).train(**args)
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision.egg-info/PKG-INFO` & `PJYoloVision-0.0.3/PJYoloVision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYoloVision
-Version: 0.0.1
+Version: 0.0.3
 Summary: The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
 Home-page: https://github.com/erfanzar/PJYoloVision
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `PJYoloVision-0.0.1/PJYoloVision.egg-info/SOURCES.txt` & `PJYoloVision-0.0.3/PJYoloVision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/PKG-INFO` & `PJYoloVision-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYoloVision
-Version: 0.0.1
+Version: 0.0.3
 Summary: The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
 Home-page: https://github.com/erfanzar/PJYoloVision
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `PJYoloVision-0.0.1/README.md` & `PJYoloVision-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/pyproject.toml` & `PJYoloVision-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.1/setup.py` & `PJYoloVision-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PJYoloVision',
-    version='0.0.1',
+    version='0.0.3',
     author='Erfan Zare Chavoshi',
     author_email='erfanzare82@eyahoo.com',
     description="""
     The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
     These models can be trained to detect specific types of objects, such as cars, people, animals,
      or any other object of interest. The YOLO models are known for being fast and accurate, 
      making them a good choice for real-time applications.
```

