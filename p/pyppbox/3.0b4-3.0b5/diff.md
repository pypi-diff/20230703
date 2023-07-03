# Comparing `tmp/pyppbox-3.0b4.tar.gz` & `tmp/pyppbox-3.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.0b4.tar", last modified: Fri Jun 30 23:11:23 2023, max compression
+gzip compressed data, was "pyppbox-3.0b5.tar", last modified: Mon Jul  3 01:49:29 2023, max compression
```

## Comparing `pyppbox-3.0b4.tar` & `pyppbox-3.0b5.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.082860 pyppbox-3.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-30 23:11:06.000000 pyppbox-3.0b4/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 23:11:06.000000 pyppbox-3.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 23:11:06.000000 pyppbox-3.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-30 23:11:23.082860 pyppbox-3.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-30 23:11:06.000000 pyppbox-3.0b4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-30 23:11:06.000000 pyppbox-3.0b4/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/cfg/cfg.7z
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.070860 pyppbox-3.0b4/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.078860 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.082860 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.082860 pyppbox-3.0b4/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.082860 pyppbox-3.0b4/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.082860 pyppbox-3.0b4/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (123)    45150 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/standalone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.082860 pyppbox-3.0b4/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    26550 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.074860 pyppbox-3.0b4/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-30 23:11:23.000000 pyppbox-3.0b4/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-30 23:11:23.000000 pyppbox-3.0b4/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:11:23.000000 pyppbox-3.0b4/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 23:11:23.000000 pyppbox-3.0b4/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 23:11:23.000000 pyppbox-3.0b4/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 23:11:06.000000 pyppbox-3.0b4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:23.082860 pyppbox-3.0b4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 23:11:06.000000 pyppbox-3.0b4/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 23:11:06.000000 pyppbox-3.0b4/requirements/pippackages_cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-30 23:11:06.000000 pyppbox-3.0b4/requirements/pippackages_cuda.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-30 23:11:06.000000 pyppbox-3.0b4/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 23:11:23.082860 pyppbox-3.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-30 23:11:06.000000 pyppbox-3.0b4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-30 23:11:06.000000 pyppbox-3.0b4/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.471331 pyppbox-3.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-03 01:49:13.000000 pyppbox-3.0b5/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 01:49:13.000000 pyppbox-3.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 01:49:13.000000 pyppbox-3.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 01:49:29.471331 pyppbox-3.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-03 01:49:13.000000 pyppbox-3.0b5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-03 01:49:13.000000 pyppbox-3.0b5/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/cfg.7z
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.447331 pyppbox-3.0b5/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.459331 pyppbox-3.0b5/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.459331 pyppbox-3.0b5/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)    45150 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/standalone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.471331 pyppbox-3.0b5/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26550 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.471331 pyppbox-3.0b5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/pippackages_cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/pippackages_cuda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:49:29.471331 pyppbox-3.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-03 01:49:13.000000 pyppbox-3.0b5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 01:49:13.000000 pyppbox-3.0b5/setup_extra.yaml
```

### Comparing `pyppbox-3.0b4/GETSTARTED.md` & `pyppbox-3.0b5/GETSTARTED.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🚀 Getting Started
 
-Installing `pyppbox` is very easy and straightforward. You can install it from [PyPI](https://pypi.org/project/pyppbox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/rathaumons/pyppbox/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependcies or requirements for the modules you needs.
+Installing `pyppbox` is very easy and straightforward. You can install it from [PyPI](https://pypi.org/project/pyppbox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/rathaumons/pyppbox/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependencies or requirements for the modules you needs.
 
-🆕 `pyppbox` `v3.0b2+` supports all Windows, Linux and macOS.
+🆕 `pyppbox` `v3.0b2+` supports all Windows, Linux and macOS. ***Use the most recent version of `pyppbox` for smoother experience!***
 
 ## ⚙️ Requirements
 
 All requirements are not strictly limited. However, some specific modules might need some special dependencies. For example, `YOLO_Classic` (With `.weights` model) relies on [OpenCV DNN](https://docs.opencv.org/4.x/d2/d58/tutorial_table_of_content_dnn.html) in order to make use of GPU power. In this case, you might need to build OpenCV from source by yourself or use our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) instead of the official `opencv-contrib-python` which does not include GPU support.
 
 * Prerequisite: 
   - (Optional) For NVIDIA GPU: [CUDA Toolkit 11.x.x](https://developer.nvidia.com/cuda-downloads) with default installation path
@@ -48,32 +48,32 @@
       pip uninstall -y ultralytics # Remove the official ultralytics
       pip install "setuptools>=67.2.0"
       pip install -r pippackages_cpu.txt
       pip install torch torchvision torchaudio
       ```
 
 * (Optional) For GPU-Only -> Verify the installed dependencies:
-  - Execute the `test_gup.py`
+  - Execute the `test_gpu.py`
     - On Windows -> `test_gpu.cmd`
-    - On Linux -> `python test_gup.py`
+    - On Linux -> `python test_gpu.py`
   - If there is no error, then you are all good and ready to go.
   - For OpenCV, the official `opencv-contrib-python` (No GPU support) is set in the `pippackages_cuda.txt` file. If you need GPU support, check our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) or build one from source by yourself.
 
 * ⚠️ ***Notes:***
   - For CPU-Only, Torchreid does not work on CPU -> `pyppbox-torchreid` is excluded from `pippackages_cpu.txt`.
   - For CPU-Only, YOLO Ultralytics uses GPU by default, you must set `cpu` as string for the parameter `device` in its configuration.
   - For GPU on Windows, [Tensorflow 2.11+ no long provides native GPU support](https://www.tensorflow.org/install/pip#windows-native). 
 
 
 ## 💽 Setup
 
 You need to install the main package which is `pyppbox` and the data for the modules you need `pyppbox-data-xxx`. If you want to have some fun for the demo on our [GTA_V_DATASET](https://github.com/rathaumons/PoseTReID_DATASET), you also need to install `pyppbox-data-gta5`.
 
 * Install `pyppbox`
-  - Use the latest `.whl` from [releases](https://github.com/rathaumons/pyppbox/releases) or install from PyPI:
+  - Use the latest `.whl` from [releases](https://github.com/rathaumons/pyppbox/releases) or install from [PyPI](https://pypi.org/project/pyppbox/):
     ```
     pip install pyppbox
     ``` 
   - Or install directly from GitHub:
     ```
     pip install git+https://github.com/rathaumons/pyppbox.git
     ```
@@ -126,8 +126,8 @@
 
 ### 2️⃣ Customized Torchreid
 
 Similar to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox), our custom `torchreid` is changed to [`pyppbox-torchreid`](https://github.com/rathaumons/torchreid-for-pyppbox). More than the normal package rename, the module name is also changed from `torchreid` to `pyppbox_torchreid` which means the `import` in the code must be also changed. Find out more why `pyppbox` needs the customized `pyppbox-torchreid` -> [[Repo]](https://github.com/rathaumons/torchreid-for-pyppbox) [[PyPI]](https://pypi.org/project/pyppbox-torchreid/)
 
 ### 3️⃣ Customized Ultralytics
 
-Also, similar to `pyppbox_torchreid`, our custom `ultralytics` is changed to [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox), but this time, the module name is still the same `ultralytics` and it is the main reason why the official `ultralytics` must be removed. Find out more why `pyppbox` needs the customized `pyppbox-ultralytics` -> [[Repo]](https://github.com/rathaumons/torchreid-for-pyppbox) [[PyPI]](https://pypi.org/project/pyppbox-torchreid/)
+Also, similar to `pyppbox_torchreid`, our custom `ultralytics` is changed to [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox), but this time, the module name is still the same `ultralytics` and it is the main reason why the official `ultralytics` must be removed. Find out more why `pyppbox` needs the customized `pyppbox-ultralytics` -> [[Repo]](https://github.com/rathaumons/ultralytics-for-pyppbox) [[PyPI]](https://pypi.org/project/pyppbox-ultralytics/)
```

### Comparing `pyppbox-3.0b4/LICENSE` & `pyppbox-3.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/PKG-INFO` & `pyppbox-3.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.0b4
+Version: 3.0b5
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyppbox-3.0b4/README.md` & `pyppbox-3.0b5/README.md`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/RELEASENOTES.md` & `pyppbox-3.0b5/RELEASENOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Release Notes 
 
 ## **pyppbox V3 - Make Simpler and Faster**
 
+* `pyppbox` [v3.0b5](https://github.com/rathaumons/pyppbox/tree/v3.0b5)
+
+  - Fix a critical bug in GUI of FaceNet which can cause missing `train_data` configuration
+  - Fix and improve documentation
+  - **Known issue/limitation**: 
+    - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
+
 * `pyppbox` [v3.0b4](https://github.com/rathaumons/pyppbox/tree/v3.0b4)
 
   - Add hotfix for command `python` in `subprocess` when running on Linux
   - Update and improve dependencies/requirements for macOS and Linux
   - Update and improve `GETSTARTED.md` for macOS and Linux
   - Add core stability test for macOS
   - **Known issue/limitation**:
```

### Comparing `pyppbox-3.0b4/pyppbox/__init__.py` & `pyppbox-3.0b5/pyppbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.0b4'
+__version__ = '3.0b5'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.0b4/pyppbox/config/__init__.py` & `pyppbox-3.0b5/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/config/cfg/cfg.7z` & `pyppbox-3.0b5/pyppbox/config/cfg/cfg.7z`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.0b5/pyppbox/config/cfg/detectors.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.0b5/pyppbox/config/cfg/reiders.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.0b5/pyppbox/config/cfg/trackers.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/config/configtools.py` & `pyppbox-3.0b5/pyppbox/config/configtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/config/myconfig.py` & `pyppbox-3.0b5/pyppbox/config/myconfig.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/config/unifiedstrings.py` & `pyppbox-3.0b5/pyppbox/config/unifiedstrings.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/__init__.py` & `pyppbox-3.0b5/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/assets/TReID.png` & `pyppbox-3.0b5/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/assets/icon.ico` & `pyppbox-3.0b5/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/assets/settings.ico` & `pyppbox-3.0b5/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/guidemo.py` & `pyppbox-3.0b5/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/guihub.py` & `pyppbox-3.0b5/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/guitools.py` & `pyppbox-3.0b5/pyppbox/gui/guitools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_centroid.py` & `pyppbox-3.0b5/pyppbox/gui/ui_centroid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.0b5/pyppbox/gui/ui_deepsort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_facenet.py` & `pyppbox-3.0b5/pyppbox/gui/ui_facenet.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,107 +35,120 @@
         if cfg_mode == 0:
             self.mycfg = MyCFG()
         else:
             self.mycfg = MyCFG(self.cfg_dir)
 
     def setupUi(self, facenet_ui):
         facenet_ui.setObjectName("facenet_ui")
-        facenet_ui.resize(390, 300)
+        facenet_ui.resize(390, 330)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, 
                                            QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(facenet_ui.sizePolicy().hasHeightForWidth())
         facenet_ui.setSizePolicy(sizePolicy)
-        facenet_ui.setMinimumSize(QtCore.QSize(390, 300))
-        facenet_ui.setMaximumSize(QtCore.QSize(390, 300))
+        facenet_ui.setMinimumSize(QtCore.QSize(390, 330))
+        facenet_ui.setMaximumSize(QtCore.QSize(390, 330))
         self.save_pushButton = QtWidgets.QPushButton(facenet_ui)
-        self.save_pushButton.setGeometry(QtCore.QRect(150, 260, 91, 31))
+        self.save_pushButton.setGeometry(QtCore.QRect(150, 290, 91, 31))
         self.save_pushButton.setObjectName("save_pushButton")
         self.fn_min_confidence_label = QtWidgets.QLabel(facenet_ui)
-        self.fn_min_confidence_label.setGeometry(QtCore.QRect(10, 160, 91, 16))
+        self.fn_min_confidence_label.setGeometry(QtCore.QRect(10, 190, 91, 16))
         self.fn_min_confidence_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                                   QtCore.Qt.AlignmentFlag.AlignTrailing|
                                                   QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_min_confidence_label.setObjectName("fn_min_confidence_label")
         self.fn_model_file_lineEdit = QtWidgets.QLineEdit(facenet_ui)
         self.fn_model_file_lineEdit.setGeometry(QtCore.QRect(110, 70, 241, 21))
         self.fn_model_file_lineEdit.setReadOnly(True)
         self.fn_model_file_lineEdit.setObjectName("fn_model_file_lineEdit")
         self.fn_classifier_pkl_label = QtWidgets.QLabel(facenet_ui)
         self.fn_classifier_pkl_label.setGeometry(QtCore.QRect(10, 100, 91, 16))
         self.fn_classifier_pkl_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                                   QtCore.Qt.AlignmentFlag.AlignTrailing|
                                                   QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_classifier_pkl_label.setObjectName("fn_classifier_pkl_label")
+        self.fn_train_data_label = QtWidgets.QLabel(facenet_ui)
+        self.fn_train_data_label.setGeometry(QtCore.QRect(10, 130, 91, 16))
+        self.fn_train_data_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
+                                              QtCore.Qt.AlignmentFlag.AlignTrailing|
+                                              QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.fn_train_data_label.setObjectName("dr_train_data_label")
         self.fn_yl_h_calib_label = QtWidgets.QLabel(facenet_ui)
-        self.fn_yl_h_calib_label.setGeometry(QtCore.QRect(10, 190, 91, 16))
+        self.fn_yl_h_calib_label.setGeometry(QtCore.QRect(10, 220, 91, 16))
         self.fn_yl_h_calib_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                               QtCore.Qt.AlignmentFlag.AlignTrailing|
                                               QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_yl_h_calib_label.setObjectName("fn_yl_h_calib_label")
         self.fn_gpu_mem_label = QtWidgets.QLabel(facenet_ui)
         self.fn_gpu_mem_label.setGeometry(QtCore.QRect(10, 10, 91, 16))
         self.fn_gpu_mem_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                            QtCore.Qt.AlignmentFlag.AlignTrailing|
                                            QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_gpu_mem_label.setObjectName("fn_gpu_mem_label")
         self.fn_model_file_pushButton = QtWidgets.QPushButton(facenet_ui)
         self.fn_model_file_pushButton.setGeometry(QtCore.QRect(360, 70, 21, 24))
         self.fn_model_file_pushButton.setObjectName("fn_model_file_pushButton")
         self.fn_yl_w_calib_label = QtWidgets.QLabel(facenet_ui)
-        self.fn_yl_w_calib_label.setGeometry(QtCore.QRect(10, 220, 91, 16))
+        self.fn_yl_w_calib_label.setGeometry(QtCore.QRect(10, 250, 91, 16))
         self.fn_yl_w_calib_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                               QtCore.Qt.AlignmentFlag.AlignTrailing|
                                               QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_yl_w_calib_label.setObjectName("fn_yl_w_calib_label")
         self.fn_model_det_pushButton = QtWidgets.QPushButton(facenet_ui)
         self.fn_model_det_pushButton.setGeometry(QtCore.QRect(360, 40, 21, 24))
         self.fn_model_det_pushButton.setObjectName("fn_model_det_pushButton")
         self.fn_model_det_label = QtWidgets.QLabel(facenet_ui)
         self.fn_model_det_label.setGeometry(QtCore.QRect(10, 40, 91, 16))
         self.fn_model_det_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                              QtCore.Qt.AlignmentFlag.AlignTrailing|
                                              QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_model_det_label.setObjectName("fn_model_det_label")
         self.fn_yl_w_calib_lineEdit = QtWidgets.QLineEdit(facenet_ui)
-        self.fn_yl_w_calib_lineEdit.setGeometry(QtCore.QRect(110, 220, 241, 21))
+        self.fn_yl_w_calib_lineEdit.setGeometry(QtCore.QRect(110, 250, 241, 21))
         self.fn_yl_w_calib_lineEdit.setReadOnly(False)
         self.fn_yl_w_calib_lineEdit.setObjectName("fn_yl_w_calib_lineEdit")
         self.fn_batch_size_lineEdit = QtWidgets.QLineEdit(facenet_ui)
-        self.fn_batch_size_lineEdit.setGeometry(QtCore.QRect(110, 130, 241, 21))
+        self.fn_batch_size_lineEdit.setGeometry(QtCore.QRect(110, 160, 241, 21))
         self.fn_batch_size_lineEdit.setObjectName("fn_batch_size_lineEdit")
         self.fn_batch_size_label = QtWidgets.QLabel(facenet_ui)
-        self.fn_batch_size_label.setGeometry(QtCore.QRect(10, 130, 91, 16))
+        self.fn_batch_size_label.setGeometry(QtCore.QRect(10, 160, 91, 16))
         self.fn_batch_size_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                               QtCore.Qt.AlignmentFlag.AlignTrailing|
                                               QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_batch_size_label.setObjectName("fn_batch_size_label")
         self.fn_classifier_pkl_lineEdit = QtWidgets.QLineEdit(facenet_ui)
         self.fn_classifier_pkl_lineEdit.setGeometry(QtCore.QRect(110, 100, 241, 21))
         self.fn_classifier_pkl_lineEdit.setReadOnly(True)
         self.fn_classifier_pkl_lineEdit.setObjectName("fn_classifier_pkl_lineEdit")
+        self.fn_train_data_lineEdit = QtWidgets.QLineEdit(facenet_ui)
+        self.fn_train_data_lineEdit.setGeometry(QtCore.QRect(110, 130, 241, 21))
+        self.fn_train_data_lineEdit.setReadOnly(True)
+        self.fn_train_data_lineEdit.setObjectName("dr_train_data_lineEdit")
         self.fn_model_file_label = QtWidgets.QLabel(facenet_ui)
         self.fn_model_file_label.setGeometry(QtCore.QRect(10, 70, 91, 16))
         self.fn_model_file_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                               QtCore.Qt.AlignmentFlag.AlignTrailing|
                                               QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.fn_model_file_label.setObjectName("fn_model_file_label")
         self.fn_gpu_mem_lineEdit = QtWidgets.QLineEdit(facenet_ui)
         self.fn_gpu_mem_lineEdit.setGeometry(QtCore.QRect(110, 10, 241, 21))
         self.fn_gpu_mem_lineEdit.setObjectName("fn_gpu_mem_lineEdit")
         self.fn_min_confidence_lineEdit = QtWidgets.QLineEdit(facenet_ui)
-        self.fn_min_confidence_lineEdit.setGeometry(QtCore.QRect(110, 160, 241, 21))
+        self.fn_min_confidence_lineEdit.setGeometry(QtCore.QRect(110, 190, 241, 21))
         self.fn_min_confidence_lineEdit.setReadOnly(False)
         self.fn_min_confidence_lineEdit.setObjectName("fn_min_confidence_lineEdit")
         self.fn_classifier_pkl_pushButton = QtWidgets.QPushButton(facenet_ui)
         self.fn_classifier_pkl_pushButton.setGeometry(QtCore.QRect(360, 100, 21, 24))
         self.fn_classifier_pkl_pushButton.setObjectName("fn_classifier_pkl_pushButton")
+        self.fn_train_data_pushButton = QtWidgets.QPushButton(facenet_ui)
+        self.fn_train_data_pushButton.setGeometry(QtCore.QRect(360, 130, 21, 24))
+        self.fn_train_data_pushButton.setObjectName("dr_train_data_pushButton")
         self.fn_yl_h_calib_lineEdit = QtWidgets.QLineEdit(facenet_ui)
-        self.fn_yl_h_calib_lineEdit.setGeometry(QtCore.QRect(110, 190, 241, 21))
+        self.fn_yl_h_calib_lineEdit.setGeometry(QtCore.QRect(110, 220, 241, 21))
         self.fn_yl_h_calib_lineEdit.setObjectName("fn_yl_h_calib_lineEdit")
         self.fn_model_det_lineEdit = QtWidgets.QLineEdit(facenet_ui)
         self.fn_model_det_lineEdit.setGeometry(QtCore.QRect(110, 40, 241, 21))
         self.fn_model_det_lineEdit.setReadOnly(True)
         self.fn_model_det_lineEdit.setObjectName("fn_model_det_lineEdit")
         font = QtGui.QFont()
         font.setPointSize(12)
@@ -143,51 +156,56 @@
         self.save_pushButton.setDefault(True)
         self.retranslateUi(facenet_ui)
         # custom
         self.loadFN()
         self.fn_model_det_pushButton.clicked.connect(self.browseModelDet)
         self.fn_model_file_pushButton.clicked.connect(self.browseModelFile)
         self.fn_classifier_pkl_pushButton.clicked.connect(self.browseClassifierFile)
+        self.fn_train_data_pushButton.clicked.connect(self.browseTrainData)
         self.save_pushButton.clicked.connect(lambda: self.updateCFG(facenet_ui))
         QtCore.QMetaObject.connectSlotsByName(facenet_ui)
 
     def retranslateUi(self, facenet_ui):
         _translate = QtCore.QCoreApplication.translate
         facenet_ui.setWindowTitle(_translate("facenet_ui", "FaceNet"))
         self.save_pushButton.setText(_translate("facenet_ui", "Save"))
         self.fn_min_confidence_label.setText(_translate("facenet_ui", "min_confidence"))
         self.fn_classifier_pkl_label.setText(_translate("facenet_ui", "classifier_pkl"))
+        self.fn_train_data_label.setText(_translate("facenet_ui", "train_data"))
         self.fn_yl_h_calib_label.setText(_translate("facenet_ui", "yl_h_calib"))
         self.fn_gpu_mem_label.setText(_translate("facenet_ui", "gpu_mem"))
         self.fn_model_file_pushButton.setText(_translate("facenet_ui", "..."))
         self.fn_yl_w_calib_label.setText(_translate("facenet_ui", "yl_w_calib"))
         self.fn_model_det_pushButton.setText(_translate("facenet_ui", "..."))
         self.fn_model_det_label.setText(_translate("facenet_ui", "model_det"))
         self.fn_batch_size_label.setText(_translate("facenet_ui", "batch_size"))
         self.fn_model_file_label.setText(_translate("facenet_ui", "model_file"))
         self.fn_classifier_pkl_pushButton.setText(_translate("facenet_ui", "..."))
+        self.fn_train_data_pushButton.setText(_translate("facenet_ui", "..."))
 
     def loadFN(self):
         self.mycfg.setAllRCFG()
         self.fn_batch_size_lineEdit.setText(str(self.mycfg.rcfg_facenet.batch_size))
         self.fn_gpu_mem_lineEdit.setText(str(self.mycfg.rcfg_facenet.gpu_mem))
         self.fn_min_confidence_lineEdit.setText(str(self.mycfg.rcfg_facenet.min_confidence))
         self.fn_classifier_pkl_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_facenet.classifier_pkl))
+        self.fn_train_data_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_facenet.train_data))
         self.fn_model_file_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_facenet.model_file))
         self.fn_model_det_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_facenet.model_det))
         self.fn_yl_h_calib_lineEdit.setText(str(self.mycfg.rcfg_facenet.yl_h_calibration))
         self.fn_yl_w_calib_lineEdit.setText(str(self.mycfg.rcfg_facenet.yl_w_calibration))
 
     def updateCFG(self, facenet_ui):
         facenet_doc = {
             "ri_name": "FaceNet",
             "gpu_mem": getFloat(self.fn_gpu_mem_lineEdit.text(), default_val=0.585),
             "model_det": normalizePathFDS(root_dir, self.fn_model_det_lineEdit.text()), 
             "model_file": normalizePathFDS(root_dir, self.fn_model_file_lineEdit.text()),
             "classifier_pkl": normalizePathFDS(root_dir, self.fn_classifier_pkl_lineEdit.text()),
+            "train_data": normalizePathFDS(root_dir, self.fn_train_data_lineEdit.text()),
             "batch_size": getInt(self.fn_batch_size_lineEdit.text(), default_val=0.5),
             "min_confidence": getFloat(self.fn_min_confidence_lineEdit.text(), default_val=0.75),
             "yl_h_calibration": get2Dlist(self.fn_yl_h_calib_lineEdit.text()),
             "yl_w_calibration": get2Dlist(self.fn_yl_w_calib_lineEdit.text())
         }
         deepreid_doc = self.mycfg.rcfg_torchreid.getDocument()
         self.mycfg.dumpAllRCFG([facenet_doc, deepreid_doc])
@@ -214,7 +232,13 @@
     def browseClassifierFile(self):
         default_path = getAncestorDir(self.mycfg.rcfg_facenet.classifier_pkl)
         pkl_filter = "Pickle (*.pkl)"
         source_file, _ = QtWidgets.QFileDialog.getOpenFileName(None, "Classifier file", 
                                                                default_path, pkl_filter)
         if source_file:
             self.fn_classifier_pkl_lineEdit.setText(source_file)
+
+    def browseTrainData(self):
+        default_path = getAncestorDir(self.mycfg.rcfg_facenet.train_data)
+        train_data = QtWidgets.QFileDialog.getExistingDirectory(None, "Train data folder", default_path)
+        if train_data:
+            self.fn_train_data_lineEdit.setText(train_data)
```

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_gt.py` & `pyppbox-3.0b5/pyppbox/gui/ui_gt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_launcher.py` & `pyppbox-3.0b5/pyppbox/gui/ui_launcher.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_sort.py` & `pyppbox-3.0b5/pyppbox/gui/ui_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.0b5/pyppbox/gui/ui_torchreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.0b5/pyppbox/gui/ui_yolocls.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.0b5/pyppbox/gui/ui_yoloult.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
             A :class:`RCFGTorchreid` object which manages the configurations of reidier Torchreid.
         auto_load : bool, optional
             An indication of whether to automatically call :meth:`load_classifier()`.
         """
         self.unk = cfg.unified_strings.unk_did
         self.err = cfg.unified_strings.err_did
         self.mdir = cfg.base_model_path
-        # self.classes_txt = cfg.classes_txt
         self.classifier_pkl = cfg.classifier_pkl
         self.train_data = cfg.train_data
         self.model_name = cfg.model_name
         self.model_path = cfg.model_path
         self.min_confidence = int(100 * cfg.min_confidence)
         # add_info_log("--------RI : Initializing ReID model ...")
         self.extractor = deepreid_extractor(self.model_name, self.mdir, self.model_path)
```

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.0b5/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/standalone/__init__.py` & `pyppbox-3.0b5/pyppbox/standalone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/__init__.py` & `pyppbox-3.0b5/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/commontools.py` & `pyppbox-3.0b5/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/evatools.py` & `pyppbox-3.0b5/pyppbox/utils/evatools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/gttools.py` & `pyppbox-3.0b5/pyppbox/utils/gttools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/logtools.py` & `pyppbox-3.0b5/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/persontools.py` & `pyppbox-3.0b5/pyppbox/utils/persontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/restools.py` & `pyppbox-3.0b5/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox/utils/visualizetools.py` & `pyppbox-3.0b5/pyppbox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.0b5/pyppbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.0b4
+Version: 3.0b5
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyppbox-3.0b4/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.0b5/pyppbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/requirements/test_gpu.py` & `pyppbox-3.0b5/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/setup.py` & `pyppbox-3.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b4/setup_extra.yaml` & `pyppbox-3.0b5/setup_extra.yaml`

 * *Files identical despite different names*

