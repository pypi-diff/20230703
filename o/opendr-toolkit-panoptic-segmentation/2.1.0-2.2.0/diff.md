# Comparing `tmp/opendr-toolkit-panoptic-segmentation-2.1.0.tar.gz` & `tmp/opendr-toolkit-panoptic-segmentation-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-panoptic-segmentation-2.1.0.tar", last modified: Wed Feb 22 08:10:31 2023, max compression
+gzip compressed data, was "opendr-toolkit-panoptic-segmentation-2.2.0.tar", last modified: Mon Jul  3 13:34:53 2023, max compression
```

## Comparing `opendr-toolkit-panoptic-segmentation-2.1.0.tar` & `opendr-toolkit-panoptic-segmentation-2.2.0.tar`

### file list

```diff
@@ -1,749 +1,749 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.455864 opendr-toolkit-panoptic-segmentation-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-02-22 08:10:31.000000 opendr-toolkit-panoptic-segmentation-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-02-22 08:10:31.455864 opendr-toolkit-panoptic-segmentation-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-panoptic-segmentation-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:31.455864 opendr-toolkit-panoptic-segmentation-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-22 08:10:31.000000 opendr-toolkit-panoptic-segmentation-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.347864 opendr-toolkit-panoptic-segmentation-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.355864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.355864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/
--rw-r--r--   0 runner    (1001) docker     (122)     7956 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15849 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (122)    18030 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/kitti.py
--rw-r--r--   0 runner    (1001) docker     (122)    17196 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/semantic_kitti.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/.git
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/
--rw-r--r--   0 runner    (1001) docker     (122)     6642 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/efficientLPS_multigpu_sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/semantic-kitti.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/
--rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)     3338 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_jit.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     7127 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_me.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_jit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_me.py
--rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/conv2d_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    26792 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/efficientnet_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    63212 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/gen_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    15009 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.359864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.363864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/
--rw-r--r--   0 runner    (1001) docker     (122)  2131183 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/intro.png
--rw-r--r--   0 runner    (1001) docker     (122)    11232 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/opendr_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/
--rw-r--r--   0 runner    (1001) docker     (122)      483 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7226 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (122)     5413 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7740 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3590 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7369 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_target.py
--rw-r--r--   0 runner    (1001) docker     (122)    11809 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/guided_anchor_target.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assign_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.379864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/approx_max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/assign_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     6818 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/atss_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/base_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8572 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/point_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/bbox_target.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/demodata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.383864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/combined_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/instance_balanced_pos_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5956 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/iou_balanced_neg_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/ohem_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/pseudo_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     7768 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.383864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/bbox_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (122)     2829 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)    18577 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/panoptic.py
--rw-r--r--   0 runner    (1001) docker     (122)     6426 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/recall.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.383864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     4564 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.383864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/mask_target.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.383864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/copy_of_sgd.py
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.383864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2812 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/bbox_nms.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/merge_augs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.383864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1856 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.391864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    15064 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (122)    16323 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     7842 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    10932 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/eval_np.py
--rw-r--r--   0 runner    (1001) docker     (122)    10789 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/laserscan_unfolding.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.391864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/build_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.395864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (122)     7390 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (122)     3240 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/instaboost.py
--rw-r--r--   0 runner    (1001) docker     (122)    11409 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/test_aug.py
--rw-r--r--   0 runner    (1001) docker     (122)    33582 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)    12556 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/semantic_kitti.py
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/voc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/wider_face.py
--rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/xml_style.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.395864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.399864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13896 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/anchor_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    19766 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/atss_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    18727 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fcos_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    16362 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fovea_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/free_anchor_retina_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_retina_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     4983 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    25253 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/guided_anchor_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/reppoints_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_sepbn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     4052 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/sep_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     8032 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ssd_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.403864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.403864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11435 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7083 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/convfc_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     5331 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/double_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.403864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/
--rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/KNN.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7399 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    24138 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/efficientLPS.py
--rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/rpn.py
--rw-r--r--   0 runner    (1001) docker     (122)    12963 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    14233 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/two_stage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.403864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/balanced_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2785 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/ghm_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/smooth_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.407864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13279 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientlps_semantic_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7589 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientps_semantic_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     8312 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     8355 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_sep_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fused_semantic_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    15435 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/grid_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/htc_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7454 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/maskiou_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.407864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16442 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/two_way_fpn.py
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.407864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/single_level.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.407864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/res_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.407864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.407864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/activation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/affine_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.363864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/src/
--rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/src/affine_grid_cuda.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8809 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/carafe.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/grad_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.363864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/
--rw-r--r--   0 runner    (1001) docker     (122)     4812 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    20360 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7366 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/context_block.py
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     3383 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17554 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)    10494 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.363864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/
--rw-r--r--   0 runner    (1001) docker     (122)    29535 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    42528 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16116 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    15004 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/generalized_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.363864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.363864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/
--rw-r--r--   0 runner    (1001) docker     (122)    35639 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.363864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/
--rw-r--r--   0 runner    (1001) docker     (122)    32761 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (122)     8283 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cudnn/
--rw-r--r--   0 runner    (1001) docker     (122)     4487 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/grid_sampler.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/masked_conv.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_kernel.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/nms_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/
--rw-r--r--   0 runner    (1001) docker     (122)     6659 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/non_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/gradcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/roi_align.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/
--rw-r--r--   0 runner    (1001) docker     (122)     5194 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10958 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)    13114 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel_v2.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/gradcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/roi_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/
--rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_kernel.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.411864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4051 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2852 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9941 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.h
--rw-r--r--   0 runner    (1001) docker     (122)     4852 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7714 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cuda.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/checks.h
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.415864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/sigmoid_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6412 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.415864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/src/compiling_info.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.415864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14304 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10779 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.415864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3115 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/async_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     8608 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (122)    11300 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12264 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_forward.py
--rw-r--r--   0 runner    (1001) docker     (122)    10906 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_heads.py
--rw-r--r--   0 runner    (1001) docker     (122)     2299 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_nms.py
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_roi_sampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     7324 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_soft_nms.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.419864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_inference.py
--rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_save_predictions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6151 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/convert_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/dist_test.sh
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/dist_train.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4823 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5769 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     5769 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)    34996 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/efficient_lps_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.367864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.419864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/.git
--rw-r--r--   0 runner    (1001) docker     (122)     1883 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.419864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/
--rw-r--r--   0 runner    (1001) docker     (122)     7037 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_multigpu_sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     7015 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_singlegpu_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.419864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.419864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.419864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/
--rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_jit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_me.py
--rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/conv2d_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    26792 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/efficientnet_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    60541 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/gen_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    15009 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/
--rw-r--r--   0 runner    (1001) docker     (122)   169819 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/intro.png
--rw-r--r--   0 runner    (1001) docker     (122)    11232 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/opendr_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.419864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.423864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/
--rw-r--r--   0 runner    (1001) docker     (122)      483 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (122)     5469 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.423864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.423864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3589 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7369 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_target.py
--rw-r--r--   0 runner    (1001) docker     (122)    11809 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/guided_anchor_target.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.423864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assign_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.423864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/approx_max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7027 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/assign_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     6818 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/atss_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/base_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8572 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/point_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/bbox_target.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/demodata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.427864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/combined_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/instance_balanced_pos_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5956 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/iou_balanced_neg_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/ohem_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/pseudo_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     7762 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.427864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/bbox_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)    18574 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/panoptic.py
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/recall.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.427864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     4564 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.427864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/mask_target.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.427864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4565 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/copy_of_sgd.py
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.427864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/bbox_nms.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/merge_augs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.427864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1856 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.431864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (122)    15063 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (122)    16321 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (122)     7841 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/dataset_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.431864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3063 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/build_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6142 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.431864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (122)     7193 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (122)     3240 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/instaboost.py
--rw-r--r--   0 runner    (1001) docker     (122)     6497 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/test_aug.py
--rw-r--r--   0 runner    (1001) docker     (122)    32976 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/voc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/wider_face.py
--rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/xml_style.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.431864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/
--rw-r--r--   0 runner    (1001) docker     (122)      916 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.435864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13895 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/anchor_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/atss_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    18725 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fcos_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    16360 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fovea_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7396 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/free_anchor_retina_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3760 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_retina_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    25251 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/guided_anchor_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    27173 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/reppoints_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3623 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_sepbn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     4297 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/sep_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ssd_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.435864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21496 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.435864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11433 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/convfc_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/double_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.435864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7469 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    18687 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/efficientPS.py
--rw-r--r--   0 runner    (1001) docker     (122)     3523 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/rpn.py
--rw-r--r--   0 runner    (1001) docker     (122)    12961 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/two_stage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.439864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/balanced_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/ghm_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     6653 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/smooth_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.439864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7587 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/efficientps_semantic_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     8309 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     8352 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_sep_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fused_semantic_head.py
--rw-r--r--   0 runner    (1001) docker     (122)    15434 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/grid_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/htc_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/maskiou_head.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.439864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7662 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/two_way_fpn.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.439864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/single_level.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.439864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/res_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.439864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.443864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/activation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.443864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/affine_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/src/
--rw-r--r--   0 runner    (1001) docker     (122)     4868 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/src/affine_grid_cuda.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.443864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8809 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/carafe.py
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/grad_check.py
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/
--rw-r--r--   0 runner    (1001) docker     (122)     4812 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    20360 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7366 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/context_block.py
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     3383 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.443864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17553 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)    10494 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/
--rw-r--r--   0 runner    (1001) docker     (122)    29533 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    42526 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     4021 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16114 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    15004 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/generalized_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.443864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/
--rw-r--r--   0 runner    (1001) docker     (122)    35635 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8358 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/
--rw-r--r--   0 runner    (1001) docker     (122)    32757 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (122)     8281 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cudnn/
--rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3547 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/grid_sampler.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.447864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/masked_conv.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_kernel.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.447864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/nms_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/
--rw-r--r--   0 runner    (1001) docker     (122)     6659 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/non_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.447864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/gradcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/roi_align.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/
--rw-r--r--   0 runner    (1001) docker     (122)     5194 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10958 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (122)    13114 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel_v2.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.447864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/gradcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/roi_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.371864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/
--rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_kernel.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.447864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4051 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2852 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9941 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.h
--rw-r--r--   0 runner    (1001) docker     (122)     4852 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7714 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cuda.cu
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/checks.h
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.447864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/sigmoid_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6412 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.447864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/src/compiling_info.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.451864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14304 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)    10761 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.451864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/async_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     8605 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (122)    11296 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12250 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_forward.py
--rw-r--r--   0 runner    (1001) docker     (122)    10899 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_heads.py
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_nms.py
--rw-r--r--   0 runner    (1001) docker     (122)     2227 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_roi_sampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_soft_nms.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.455864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_demo.py
--rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_inference.py
--rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_save_predictions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6151 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8646 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_kitti.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      257 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/dist_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      232 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/dist_train.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/kitti_demo.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-02-22 08:10:04.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5975 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5926 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_kitti.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)    25846 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/efficient_ps_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:31.375864 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-02-22 08:10:31.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    78875 2023-02-22 08:10:31.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:31.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-02-22 08:10:31.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:31.000000 opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.634913 opendr-toolkit-panoptic-segmentation-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-07-03 13:34:53.000000 opendr-toolkit-panoptic-segmentation-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-07-03 13:34:53.634913 opendr-toolkit-panoptic-segmentation-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-panoptic-segmentation-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:53.634913 opendr-toolkit-panoptic-segmentation-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-03 13:34:53.000000 opendr-toolkit-panoptic-segmentation-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.554912 opendr-toolkit-panoptic-segmentation-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)     7956 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15849 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18030 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/kitti.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17196 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/semantic_kitti.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.562912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-07-03 13:34:27.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/.git
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)     6642 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/efficientLPS_multigpu_sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/semantic-kitti.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.582912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.582912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/
+-rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.566912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)     3338 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_jit.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     7127 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_me.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_jit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_me.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/conv2d_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26792 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/efficientnet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63212 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/gen_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15009 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.566912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.566912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/
+-rw-r--r--   0 runner    (1001) docker     (122)  2131183 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/intro.png
+-rw-r--r--   0 runner    (1001) docker     (122)    11232 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/opendr_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.582912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.582912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      483 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7226 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5413 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7740 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.582912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.582912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3590 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7369 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11809 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/guided_anchor_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.582912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assign_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.586912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/approx_max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7030 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/assign_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6818 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/atss_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/base_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8572 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/point_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/bbox_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/demodata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.586912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/combined_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/instance_balanced_pos_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5956 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/iou_balanced_neg_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/ohem_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/pseudo_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7768 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.586912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/bbox_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2829 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18577 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/panoptic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6426 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/recall.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.586912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4564 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.586912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/mask_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.586912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/copy_of_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.590912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2812 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/bbox_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/merge_augs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.590912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1856 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.590912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15064 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16323 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7842 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10932 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/eval_np.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10789 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/laserscan_unfolding.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.590912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/build_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.590912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7390 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3240 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/instaboost.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11409 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/test_aug.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33582 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12556 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/semantic_kitti.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/voc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/wider_face.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/xml_style.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.590912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.594913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13896 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/anchor_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19766 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/atss_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18727 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fcos_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16362 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fovea_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/free_anchor_retina_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_retina_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4983 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25253 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/guided_anchor_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/reppoints_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_sepbn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4052 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/sep_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8032 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ssd_head.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.594913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.594913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11435 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7083 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/convfc_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5331 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/double_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.594913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/
+-rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/KNN.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7399 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24138 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/efficientLPS.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/rpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12963 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14233 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/two_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.594913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/balanced_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2785 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/ghm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/smooth_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.598913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13279 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientlps_semantic_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7589 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientps_semantic_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8312 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8355 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_sep_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fused_semantic_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15435 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/grid_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/htc_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7454 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/maskiou_head.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.598913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16442 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/two_way_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.598913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/single_level.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.598913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/res_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.598913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.598913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/activation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.598913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/affine_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.566912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/src/affine_grid_cuda.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8809 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/grad_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.566912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     4812 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20360 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7366 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3383 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17554 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10494 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    29535 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    42528 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16116 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15004 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/generalized_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)    35639 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/
+-rw-r--r--   0 runner    (1001) docker     (122)    32761 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     8283 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cudnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     4487 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/grid_sampler.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/masked_conv.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_kernel.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/nms_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6659 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/gradcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/roi_align.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     5194 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10958 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    13114 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel_v2.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/gradcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/roi_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_kernel.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4051 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2852 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9941 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4852 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7714 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cuda.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/checks.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/sigmoid_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6412 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.602913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/src/compiling_info.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.606913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14304 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    10779 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.606913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3115 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/async_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8608 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11300 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12264 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10906 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_heads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2299 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_roi_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7324 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_soft_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.606913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_save_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6151 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/convert_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/dist_test.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/dist_train.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4823 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.570912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5769 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5769 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    34996 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/efficient_lps_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.606913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-03 13:34:27.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/.git
+-rw-r--r--   0 runner    (1001) docker     (122)     1883 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.606913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7037 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_multigpu_sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7015 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_singlegpu_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.606913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/
+-rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_jit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_me.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/conv2d_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26792 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/efficientnet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60541 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/gen_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15009 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/
+-rw-r--r--   0 runner    (1001) docker     (122)   169819 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/intro.png
+-rw-r--r--   0 runner    (1001) docker     (122)    11232 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/opendr_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      483 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5469 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3589 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7369 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11809 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/guided_anchor_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assign_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.610913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/approx_max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7027 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/assign_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6818 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/atss_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/base_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8572 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/point_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/bbox_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/demodata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3077 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.614913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/combined_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/instance_balanced_pos_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5956 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/iou_balanced_neg_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/ohem_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/pseudo_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7762 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.614913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/bbox_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18574 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/panoptic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/recall.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.614913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4564 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.614913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/mask_target.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.614913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4565 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/copy_of_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.614913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/bbox_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/merge_augs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.614913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1856 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.618913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15063 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16321 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7841 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/dataset_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.618913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3063 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/build_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6142 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.618913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7193 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3240 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/instaboost.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6497 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/test_aug.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32976 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/voc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/wider_face.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/xml_style.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.618913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      916 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.618913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13895 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/anchor_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/atss_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18725 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fcos_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16360 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fovea_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7396 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/free_anchor_retina_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3760 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_retina_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25251 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/guided_anchor_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27173 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/reppoints_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3623 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_sepbn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4297 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/sep_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ssd_head.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.622913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21496 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.622913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11433 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/convfc_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/double_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.622913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7469 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18687 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/efficientPS.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3523 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/rpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12961 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/two_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.622913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/balanced_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/ghm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6653 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/smooth_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.622913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7587 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/efficientps_semantic_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8309 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8352 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_sep_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fused_semantic_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15434 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/grid_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/htc_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/maskiou_head.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.622913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7662 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/two_way_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.622913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/single_level.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/res_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/activation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/affine_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     4868 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/src/affine_grid_cuda.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8809 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/grad_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     4812 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20360 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7366 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3383 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17553 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10494 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    29533 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    42526 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4021 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16114 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15004 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/generalized_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)    35635 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8358 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/
+-rw-r--r--   0 runner    (1001) docker     (122)    32757 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     8281 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cudnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3547 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/grid_sampler.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.626913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/masked_conv.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_kernel.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.630913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/nms_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.574912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6659 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.630913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/gradcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/roi_align.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     5194 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10958 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    13114 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel_v2.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.630913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/gradcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/roi_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_kernel.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.630913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4051 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2852 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9941 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4852 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7714 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cuda.cu
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/checks.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.630913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/sigmoid_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6412 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.630913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/src/compiling_info.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.630913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14304 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10761 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.634913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/async_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8605 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11296 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12250 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10899 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_heads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2227 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_roi_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_soft_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.634913 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_demo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_save_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6151 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8646 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_kitti.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      257 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/dist_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      232 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/dist_train.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/kitti_demo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-07-03 13:34:28.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5975 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5926 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_kitti.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    25846 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/efficient_ps_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:53.578912 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-07-03 13:34:53.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    78875 2023-07-03 13:34:53.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:53.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-03 13:34:53.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:53.000000 opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/.clang-format` & `opendr-toolkit-panoptic-segmentation-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/.gitignore` & `opendr-toolkit-panoptic-segmentation-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/CHANGELOG.md` & `opendr-toolkit-panoptic-segmentation-2.2.0/CHANGELOG.md`

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

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-panoptic-segmentation-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/Dockerfile` & `opendr-toolkit-panoptic-segmentation-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/Dockerfile-cuda` & `opendr-toolkit-panoptic-segmentation-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/Dockerfile-embedded` & `opendr-toolkit-panoptic-segmentation-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/LICENSE` & `opendr-toolkit-panoptic-segmentation-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/Makefile` & `opendr-toolkit-panoptic-segmentation-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/PKG-INFO` & `opendr-toolkit-panoptic-segmentation-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-panoptic-segmentation
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/panoptic_segmentation)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/README.md` & `opendr-toolkit-panoptic-segmentation-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/description.txt` & `opendr-toolkit-panoptic-segmentation-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/packages.txt` & `opendr-toolkit-panoptic-segmentation-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/_version.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/constants.py`

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

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/_version.py`

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

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/README.md` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/README.md` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/cityscapes.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/kitti.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/kitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/datasets/semantic_kitti.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/datasets/semantic_kitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/.gitignore` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/LICENSE` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/README.md` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/efficientLPS_multigpu_sample.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/efficientLPS_multigpu_sample.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/semantic-kitti.yaml` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/configs/semantic-kitti.yaml`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/__init__.cpython-37.pyc` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations.cpython-37.pyc` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_jit.cpython-37.pyc` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_jit.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_me.cpython-37.pyc` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/__pycache__/activations_me.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_jit.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_me.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/config.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/conv2d_layers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/efficientnet_builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/gen_efficientnet.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/helpers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/mobilenetv3.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/model_factory.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/PKG-INFO` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/SOURCES.txt` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/geffnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/setup.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/efficientNet/setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/environment.yml` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/environment.yml`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/intro.png` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/intro.png`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/opendr_logo.png` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/images/opendr_logo.png`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/inference.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/inference.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/test.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/test.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/train.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/apis/train.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_generator.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/anchor_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/guided_anchor_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/guided_anchor_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_generator.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_generator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/anchor/point_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assign_sampling.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assign_sampling.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/approx_max_iou_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/approx_max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/assign_result.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/assign_result.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/atss_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/atss_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/max_iou_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/point_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/assigners/point_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/bbox_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/bbox_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/demodata.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/demodata.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/geometry.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/geometry.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/base_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/instance_balanced_pos_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/instance_balanced_pos_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/iou_balanced_neg_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/iou_balanced_neg_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/ohem_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/ohem_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/pseudo_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/pseudo_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/random_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/sampling_result.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/samplers/sampling_result.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/transforms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/bbox/transforms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/bbox_overlaps.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/bbox_overlaps.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/class_names.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/eval_hooks.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/mean_ap.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/mean_ap.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/panoptic.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/panoptic.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/recall.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/evaluation/recall.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/decorators.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/decorators.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/hooks.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/hooks.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/fp16/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/mask_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/mask_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/mask/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/registry.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/optimizer/registry.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/bbox_nms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/bbox_nms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/merge_augs.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/post_processing/merge_augs.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/dist_utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/misc.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/cityscapes.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/coco.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/custom.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/dataset_wrappers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/eval_np.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/eval_np.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/laserscan_unfolding.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/laserscan_unfolding.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/build_loader.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/build_loader.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/loader/sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/auto_augment.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/auto_augment.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/compose.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/formating.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/instaboost.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/instaboost.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/loading.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/test_aug.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/test_aug.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/transforms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/semantic_kitti.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/semantic_kitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/voc.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/wider_face.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/wider_face.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/xml_style.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/datasets/xml_style.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/anchor_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/anchor_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/atss_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/atss_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fcos_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fcos_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fovea_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/fovea_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/free_anchor_retina_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/free_anchor_retina_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_retina_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_retina_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_rpn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ga_rpn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/guided_anchor_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/guided_anchor_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/reppoints_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/reppoints_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_sepbn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/retina_sepbn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/rpn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/rpn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/sep_rpn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/sep_rpn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ssd_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/anchor_heads/ssd_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/resnet.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/bbox_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/bbox_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/convfc_bbox_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/convfc_bbox_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/double_bbox_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/bbox_heads/double_bbox_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/KNN.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/KNN.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/base.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/base.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/efficientLPS.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/efficientLPS.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/rpn.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/rpn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/test_mixins.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/test_mixins.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/two_stage.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/efficientlps/two_stage.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/accuracy.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/balanced_l1_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/balanced_l1_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/cross_entropy_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/focal_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/ghm_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/ghm_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/iou_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/iou_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/mse_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/mse_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/smooth_l1_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientlps_semantic_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientlps_semantic_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientps_semantic_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/efficientps_semantic_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_mask_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_mask_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_sep_mask_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fcn_sep_mask_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fused_semantic_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/fused_semantic_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/grid_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/grid_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/htc_mask_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/htc_mask_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/maskiou_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/mask_heads/maskiou_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/two_way_fpn.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/necks/two_way_fpn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/single_level.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/roi_extractors/single_level.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/res_layer.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/models/shared_heads/res_layer.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/activation.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/activation.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/affine_grid.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/affine_grid.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/src/affine_grid_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/affine_grid/src/affine_grid_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/carafe.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/carafe.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/grad_check.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/grad_check.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/setup.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/carafe/src/carafe_naive_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/context_block.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/context_block.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_module.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_module.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_ws.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/conv_ws.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_conv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_pool.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/deform_pool.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_conv_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/dcn/src/deform_pool_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/depthwise_separable_conv_module.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/generalized_attention.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/grid_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cpu/grid_sampler_cpu.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/grid_sampler.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/grid_sampler/src/grid_sampler.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/masked_conv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/masked_conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/masked_conv/src/masked_conv2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/nms_wrapper.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/nms_wrapper.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cpu.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cpu.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/nms/src/nms_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/non_local.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/non_local.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/norm.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/norm.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/gradcheck.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/gradcheck.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/roi_align.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/roi_align.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel_v2.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_align/src/roi_align_kernel_v2.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/gradcheck.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/gradcheck.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/roi_pool.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/roi_pool.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_pool/src/roi_pool_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/functions.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/functions.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cpu.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cpu.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cuda.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/roi_sampling_cuda.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/checks.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/checks.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/common.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/roi_sampling/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/saconv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/sigmoid_focal_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/sigmoid_focal_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/upsample.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/upsample.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/src/compiling_info.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/ops/utils/src/compiling_info.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/collect_env.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/contextmanagers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/flops_counter.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/logger.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/profiling.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/registry.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/util_mixins.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/mmdet2/utils/util_mixins.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/setup.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/async_benchmark.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/async_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_async.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_config.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_forward.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_forward.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_heads.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_heads.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_nms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_nms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_roi_sampling.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_roi_sampling.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_soft_nms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tests/test_soft_nms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_inference.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_inference.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_save_predictions.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/cityscapes_save_predictions.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/convert_cityscapes.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/convert_cityscapes.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/fuse_conv_bn.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/test.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/test.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/train.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/algorithm/EfficientLPS/tools/train.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_sample.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_sample.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_semantickitti.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/configs/singlegpu_semantickitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/dependencies.ini` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/dependencies.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [runtime]
 python=
-       torch==1.9.0
-       torchvision==0.10.0
+       torch==1.13.1
+       torchvision==0.14.1
        tqdm
        mmcv==0.5.9
        future
        tensorboard
        cityscapesscripts>=2.2.0
        pycocotools
        terminaltables
```

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_lps/efficient_lps_learner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_lps/efficient_lps_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/.gitignore` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/LICENSE` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/README.md` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_multigpu_sample.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_multigpu_sample.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_singlegpu_sample.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/configs/efficientPS_singlegpu_sample.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_jit.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_me.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/config.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/conv2d_layers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/efficientnet_builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/gen_efficientnet.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/helpers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/mobilenetv3.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/model_factory.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/setup.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/efficientNet/setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/environment.yml` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/environment.yml`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/intro.png` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/intro.png`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/opendr_logo.png` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/images/opendr_logo.png`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/inference.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/inference.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/test.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/test.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/train.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/apis/train.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_generator.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/anchor_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/guided_anchor_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/guided_anchor_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_generator.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_generator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/anchor/point_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assign_sampling.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assign_sampling.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/approx_max_iou_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/approx_max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/assign_result.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/assign_result.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/atss_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/atss_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/max_iou_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/point_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/assigners/point_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/bbox_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/bbox_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/demodata.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/demodata.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/geometry.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/geometry.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/base_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/instance_balanced_pos_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/instance_balanced_pos_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/iou_balanced_neg_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/iou_balanced_neg_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/ohem_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/ohem_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/pseudo_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/pseudo_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/random_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/sampling_result.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/samplers/sampling_result.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/transforms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/bbox/transforms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/bbox_overlaps.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/bbox_overlaps.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/class_names.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/eval_hooks.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/mean_ap.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/mean_ap.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/panoptic.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/panoptic.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/recall.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/evaluation/recall.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/decorators.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/decorators.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/hooks.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/hooks.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/fp16/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/mask_target.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/mask_target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/mask/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/registry.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/optimizer/registry.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/bbox_nms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/bbox_nms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/merge_augs.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/post_processing/merge_augs.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/dist_utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/misc.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/cityscapes.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/coco.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/custom.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/dataset_wrappers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/build_loader.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/build_loader.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/loader/sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/auto_augment.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/auto_augment.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/compose.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/formating.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/instaboost.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/instaboost.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/loading.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/test_aug.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/test_aug.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/transforms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/voc.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/wider_face.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/wider_face.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/xml_style.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/datasets/xml_style.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/anchor_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/anchor_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/atss_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/atss_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fcos_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fcos_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fovea_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/fovea_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/free_anchor_retina_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/free_anchor_retina_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_retina_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_retina_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_rpn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ga_rpn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/guided_anchor_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/guided_anchor_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/reppoints_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/reppoints_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_sepbn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/retina_sepbn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/rpn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/rpn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/sep_rpn_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/sep_rpn_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ssd_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/anchor_heads/ssd_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/resnet.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/bbox_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/bbox_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/convfc_bbox_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/convfc_bbox_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/double_bbox_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/bbox_heads/double_bbox_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/builder.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/base.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/base.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/efficientPS.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/efficientPS.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/rpn.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/rpn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/test_mixins.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/test_mixins.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/two_stage.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/efficientps/two_stage.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/accuracy.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/balanced_l1_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/balanced_l1_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/cross_entropy_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/focal_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/ghm_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/ghm_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/iou_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/iou_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/mse_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/mse_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/smooth_l1_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/utils.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/efficientps_semantic_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/efficientps_semantic_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_mask_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_mask_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_sep_mask_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fcn_sep_mask_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fused_semantic_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/fused_semantic_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/grid_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/grid_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/htc_mask_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/htc_mask_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/maskiou_head.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/mask_heads/maskiou_head.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/two_way_fpn.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/necks/two_way_fpn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/single_level.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/roi_extractors/single_level.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/res_layer.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/models/shared_heads/res_layer.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/activation.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/activation.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/affine_grid.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/affine_grid.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/src/affine_grid_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/affine_grid/src/affine_grid_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/carafe.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/carafe.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/grad_check.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/grad_check.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/setup.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/carafe/src/carafe_naive_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/context_block.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/context_block.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_module.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_module.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_ws.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/conv_ws.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/__init__.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_conv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_pool.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/deform_pool.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_conv_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/dcn/src/deform_pool_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/depthwise_separable_conv_module.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/generalized_attention.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/grid_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cpu/grid_sampler_cpu.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cuda/grid_sampler_cuda.cuh`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/cudnn/grid_sampler_cudnn.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/grid_sampler.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/grid_sampler/src/grid_sampler.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/masked_conv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/masked_conv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/masked_conv/src/masked_conv2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/nms_wrapper.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/nms_wrapper.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cpu.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cpu.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/nms/src/nms_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/non_local.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/non_local.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/norm.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/norm.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/gradcheck.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/gradcheck.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/roi_align.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/roi_align.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel_v2.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_align/src/roi_align_kernel_v2.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/gradcheck.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/gradcheck.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/roi_pool.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/roi_pool.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_cuda.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_cuda.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_kernel.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_pool/src/roi_pool_kernel.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/functions.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/functions.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cpu.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cpu.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cuda.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/roi_sampling_cuda.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/checks.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/checks.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/common.h` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/roi_sampling/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/saconv.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/sigmoid_focal_loss.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/sigmoid_focal_loss.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/sigmoid_focal_loss/src/sigmoid_focal_loss_cuda.cu`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/upsample.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/upsample.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/src/compiling_info.cpp` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/ops/utils/src/compiling_info.cpp`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/collect_env.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/contextmanagers.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/flops_counter.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/logger.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/logger.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/profiling.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/registry.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/registry.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/util_mixins.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/mmdet/utils/util_mixins.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/setup.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/async_benchmark.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/async_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_assigner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_async.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_config.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_forward.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_forward.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_heads.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_heads.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_nms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_nms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_roi_sampling.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_roi_sampling.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_sampler.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_soft_nms.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tests/test_soft_nms.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_demo.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_demo.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_inference.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_inference.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_save_predictions.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/cityscapes_save_predictions.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_cityscapes.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_cityscapes.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_kitti.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/convert_kitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/fuse_conv_bn.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/kitti_demo.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/kitti_demo.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/test.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/test.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/train.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/algorithm/EfficientPS/tools/train.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_cityscapes.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_cityscapes.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_kitti.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/configs/singlegpu_kitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/dependencies.ini` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/dependencies.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [runtime]
 python=
-       torch==1.9.0
-       torchvision==0.10.0
+       torch==1.13.1
+       torchvision==0.14.1
        protobuf<=3.20.0
        tqdm
        mmcv==0.5.9
        future
        tensorboard
        cityscapesscripts>=2.2.0
        pycocotools
```

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr/perception/panoptic_segmentation/efficient_ps/efficient_ps_learner.py` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr/perception/panoptic_segmentation/efficient_ps/efficient_ps_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/PKG-INFO` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-panoptic-segmentation
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/panoptic_segmentation)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-panoptic-segmentation-2.1.0/src/opendr_toolkit_panoptic_segmentation.egg-info/SOURCES.txt` & `opendr-toolkit-panoptic-segmentation-2.2.0/src/opendr_toolkit_panoptic_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

