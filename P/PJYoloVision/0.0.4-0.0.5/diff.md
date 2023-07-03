# Comparing `tmp/PJYoloVision-0.0.4.tar.gz` & `tmp/PJYoloVision-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PJYoloVision-0.0.4.tar", last modified: Mon Jul  3 13:16:19 2023, max compression
+gzip compressed data, was "PJYoloVision-0.0.5.tar", last modified: Mon Jul  3 13:22:52 2023, max compression
```

## Comparing `PJYoloVision-0.0.4.tar` & `PJYoloVision-0.0.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    35149 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/LICENCE.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4906 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/nn/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/nn/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5600 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/nn/autobackend.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    10977 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/nn/autoshape.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      867 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/nn/modules.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17501 2023-07-03 09:58:58.000000 PJYoloVision-0.0.4/PJYoloVision/nn/tasks.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/tracker/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      162 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1594 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/track.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      131 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1085 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/basetrack.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4858 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/bot_sort.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13185 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/byte_tracker.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/tracker/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11965 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/utils/gmc.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18422 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/utils/kalman_filter.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7634 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/tracker/utils/matching.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/yolo/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/yolo/cfg/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11778 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/cfg/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision/yolo/core/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/core/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    35345 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/core/exporter.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9182 2023-07-03 12:57:24.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/core/model.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13542 2023-07-03 13:11:21.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/core/predictor.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12519 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/core/results.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    32074 2023-07-03 08:53:54.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/core/trainer.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9207 2023-07-03 08:54:33.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/core/validator.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/data/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      444 2023-07-03 08:59:14.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    31969 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/augment.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8997 2023-07-03 08:59:14.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/base.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7673 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/build.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 08:59:14.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12715 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/stream_loaders.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17579 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/v5augmentations.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    46738 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/v5loader.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11047 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataset.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1427 2023-07-03 08:59:14.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataset_wrappers.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/data/scripts/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 08:59:14.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/scripts/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18817 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/data/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17619 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3175 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/autobatch.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4044 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/benchmarks.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3842 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/base.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2205 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/clearml.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2162 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/comet.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3040 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/hub.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1323 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/tensorboard.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9838 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/checks.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2424 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/dist.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6474 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/downloads.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2556 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/files.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11762 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/instance.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2326 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/loss.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    28016 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/metrics.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    19809 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/ops.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    15709 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/plotting.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    10646 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/tal.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18673 2023-07-03 09:00:22.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/utils/torch_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      125 2023-07-03 12:55:08.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      318 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2649 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5481 2023-07-03 09:00:48.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2223 2023-07-03 09:01:01.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      190 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4323 2023-07-03 13:00:03.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9431 2023-07-03 13:07:27.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11661 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      208 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4940 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7300 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12005 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:16:19.967985 PJYoloVision-0.0.4/PJYoloVision.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-03 13:16:19.000000 PJYoloVision-0.0.4/PJYoloVision.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2906 2023-07-03 13:16:19.000000 PJYoloVision-0.0.4/PJYoloVision.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-03 13:16:19.000000 PJYoloVision-0.0.4/PJYoloVision.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-03 13:16:19.000000 PJYoloVision-0.0.4/PJYoloVision.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       13 2023-07-03 13:16:19.000000 PJYoloVision-0.0.4/PJYoloVision.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4441 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      607 2023-07-03 07:22:50.000000 PJYoloVision-0.0.4/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-03 13:16:19.971985 PJYoloVision-0.0.4/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-07-03 13:15:50.000000 PJYoloVision-0.0.4/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    35149 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/LICENCE.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4906 2023-07-03 13:19:58.000000 PJYoloVision-0.0.5/PJYoloVision/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/nn/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/nn/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5600 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/nn/autobackend.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10977 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/nn/autoshape.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      867 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/nn/modules.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17501 2023-07-03 09:58:58.000000 PJYoloVision-0.0.5/PJYoloVision/nn/tasks.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/tracker/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      162 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1594 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/track.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      131 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1085 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/basetrack.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4858 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/bot_sort.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13185 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/byte_tracker.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/tracker/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11965 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/utils/gmc.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18422 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/utils/kalman_filter.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7634 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/tracker/utils/matching.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/yolo/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/yolo/cfg/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11778 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/cfg/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/yolo/core/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/core/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    35345 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/core/exporter.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9494 2023-07-03 13:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/core/model.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13542 2023-07-03 13:11:21.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/core/predictor.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12519 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/core/results.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    32074 2023-07-03 08:53:54.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/core/trainer.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9207 2023-07-03 08:54:33.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/core/validator.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/yolo/data/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      444 2023-07-03 08:59:14.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31969 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/augment.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8997 2023-07-03 08:59:14.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/base.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7673 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/build.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 08:59:14.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12715 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/stream_loaders.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17579 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/v5augmentations.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    46738 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/v5loader.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11047 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataset.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1427 2023-07-03 08:59:14.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataset_wrappers.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision/yolo/data/scripts/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-03 08:59:14.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/scripts/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18817 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/data/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17619 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3175 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/autobatch.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4044 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/benchmarks.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3842 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/base.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2205 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/clearml.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2162 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/comet.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3040 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/hub.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1323 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/tensorboard.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9838 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/checks.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2424 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/dist.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6474 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/downloads.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2556 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/files.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11762 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/instance.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2326 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/loss.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    28016 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/metrics.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    19809 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/ops.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    15709 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/plotting.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10646 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/tal.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18673 2023-07-03 09:00:22.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/utils/torch_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      125 2023-07-03 12:55:08.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      318 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2649 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5481 2023-07-03 09:00:48.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2223 2023-07-03 09:01:01.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      190 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4323 2023-07-03 13:00:03.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9431 2023-07-03 13:07:27.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11661 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      208 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4940 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7300 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12005 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-03 13:22:52.273925 PJYoloVision-0.0.5/PJYoloVision.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-03 13:22:52.000000 PJYoloVision-0.0.5/PJYoloVision.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2906 2023-07-03 13:22:52.000000 PJYoloVision-0.0.5/PJYoloVision.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-03 13:22:52.000000 PJYoloVision-0.0.5/PJYoloVision.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-03 13:22:52.000000 PJYoloVision-0.0.5/PJYoloVision.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       13 2023-07-03 13:22:52.000000 PJYoloVision-0.0.5/PJYoloVision.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4441 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      607 2023-07-03 07:22:50.000000 PJYoloVision-0.0.5/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-03 13:22:52.277925 PJYoloVision-0.0.5/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-07-03 13:22:50.000000 PJYoloVision-0.0.5/setup.py
```

### Comparing `PJYoloVision-0.0.4/LICENCE.md` & `PJYoloVision-0.0.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/__init__.py` & `PJYoloVision-0.0.5/PJYoloVision/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.0'
+__version__ = '0.0.5'
 
 from PJYoloVision.yolo.core.model import YOLO
 from PJYoloVision.yolo.utils.checks import check_yolo as checks
 
 
 def prepare_segmentation(model: YOLO):
     model.task = 'segmentation'
```

### Comparing `PJYoloVision-0.0.4/PJYoloVision/nn/autobackend.py` & `PJYoloVision-0.0.5/PJYoloVision/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/nn/autoshape.py` & `PJYoloVision-0.0.5/PJYoloVision/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/nn/modules.py` & `PJYoloVision-0.0.5/PJYoloVision/nn/modules.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/nn/tasks.py` & `PJYoloVision-0.0.5/PJYoloVision/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/tracker/track.py` & `PJYoloVision-0.0.5/PJYoloVision/tracker/track.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/basetrack.py` & `PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/bot_sort.py` & `PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/tracker/trackers/byte_tracker.py` & `PJYoloVision-0.0.5/PJYoloVision/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/tracker/utils/gmc.py` & `PJYoloVision-0.0.5/PJYoloVision/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/tracker/utils/kalman_filter.py` & `PJYoloVision-0.0.5/PJYoloVision/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/tracker/utils/matching.py` & `PJYoloVision-0.0.5/PJYoloVision/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/cfg/__init__.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/core/exporter.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/core/exporter.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/core/model.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,24 @@
         self.model.args = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}
         self.model.task = self.task
 
     def _load_model(self, weights: str, task=None):
         suffix = Path(weights).suffix
         if suffix == '.pt':
             self.model, self.ckpt = attempt_load_one_weight(weights)
-            self.task = self.model.args['task']
+            try:
+                self.task = task or self.model.args['task']
+            except KeyError:
+                try:
+                    self.task = task or self.model.args['train_args']['task']
+
+                except KeyError:
+                    raise ValueError(
+                        'No Task Found pass task manually !'
+                    )
             self.overrides = self.model.args = self._reset_ckpt_args(self.model.args)
             self.ckpt_path = self.model.pt_path
         else:
             weights = check_file(weights)
             self.model, self.ckpt = weights, None
             self.task = task or get_model_task_from_cfg(weights)
             self.ckpt_path = weights
```

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/core/predictor.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/core/predictor.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/core/results.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/core/results.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/core/trainer.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/core/trainer.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/core/validator.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/core/validator.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/augment.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/base.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/build.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/stream_loaders.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/v5augmentations.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataloaders/v5loader.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataset.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/dataset_wrappers.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/data/utils.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/__init__.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/autobatch.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/benchmarks.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/base.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/clearml.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/comet.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/hub.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/callbacks/tensorboard.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/checks.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/dist.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/downloads.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/files.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/instance.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/loss.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/metrics.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/ops.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/plotting.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/tal.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/utils/torch_utils.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/predict.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/train.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/train.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/classify/val.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/classify/val.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/predict.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/train.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/train.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/detection/val.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/detection/val.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/predict.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/train.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/train.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision/yolo/vision/segmentation/val.py` & `PJYoloVision-0.0.5/PJYoloVision/yolo/vision/segmentation/val.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PJYoloVision.egg-info/PKG-INFO` & `PJYoloVision-0.0.5/PJYoloVision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYoloVision
-Version: 0.0.4
+Version: 0.0.5
 Summary: The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
 Home-page: https://github.com/erfanzar/PJYoloVision
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `PJYoloVision-0.0.4/PJYoloVision.egg-info/SOURCES.txt` & `PJYoloVision-0.0.5/PJYoloVision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/PKG-INFO` & `PJYoloVision-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYoloVision
-Version: 0.0.4
+Version: 0.0.5
 Summary: The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
 Home-page: https://github.com/erfanzar/PJYoloVision
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `PJYoloVision-0.0.4/README.md` & `PJYoloVision-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/pyproject.toml` & `PJYoloVision-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.4/setup.py` & `PJYoloVision-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PJYoloVision',
-    version='0.0.4',
+    version='0.0.5',
     author='Erfan Zare Chavoshi',
     author_email='erfanzare82@eyahoo.com',
     description="""
     The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
     These models can be trained to detect specific types of objects, such as cars, people, animals,
      or any other object of interest. The YOLO models are known for being fast and accurate, 
      making them a good choice for real-time applications.
```

