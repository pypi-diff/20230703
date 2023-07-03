# Comparing `tmp/opendr-toolkit-object-detection-3d-2.1.0.tar.gz` & `tmp/opendr-toolkit-object-detection-3d-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-object-detection-3d-2.1.0.tar", last modified: Wed Feb 22 08:10:30 2023, max compression
+gzip compressed data, was "opendr-toolkit-object-detection-3d-2.2.0.tar", last modified: Mon Jul  3 13:34:52 2023, max compression
```

## Comparing `opendr-toolkit-object-detection-3d-2.1.0.tar` & `opendr-toolkit-object-detection-3d-2.2.0.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.575862 opendr-toolkit-object-detection-3d-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-02-22 08:10:30.000000 opendr-toolkit-object-detection-3d-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-02-22 08:10:30.575862 opendr-toolkit-object-detection-3d-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-object-detection-3d-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:30.575862 opendr-toolkit-object-detection-3d-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-02-22 08:10:30.000000 opendr-toolkit-object-detection-3d-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.535862 opendr-toolkit-object-detection-3d-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.539862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.539862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.539862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.539862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.539862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.539862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11430 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/create_data_kitti.py
--rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.543861 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/
--rw-r--r--   0 runner    (1001) docker     (122)    52625 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)    25983 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/train.txt
--rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/val.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.543861 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/train.txt
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/val.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.543861 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/train.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/val.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.543861 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.543861 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.547862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/anchor_generator_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dbsampler_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/preprocess_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/similarity_calculator_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/target_assigner_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/voxel_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.547862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/
--rw-r--r--   0 runner    (1001) docker     (122)     5871 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.config
--rw-r--r--   0 runner    (1001) docker     (122)     5350 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.tiny.config
--rw-r--r--   0 runner    (1001) docker     (122)     5893 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/people.config
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.547862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.547862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/test_short.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_16.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4377 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_20.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_24.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_28.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.547862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/
--rw-r--r--   0 runner    (1001) docker     (122)     4832 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/test_short.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_16.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_20.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4832 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_24.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_28.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.551862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.551862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/
--rw-r--r--   0 runner    (1001) docker     (122)     4401 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/test_short.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4410 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_16.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4380 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_20.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_24.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_28.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.551862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/test_short.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4862 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_16.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_20.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4835 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_24.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_28.proto
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/tanet.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.555862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_coders.py
--rw-r--r--   0 runner    (1001) docker     (122)    33460 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_np_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.555862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/box_ops.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/box_ops.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.555862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.h
--rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu.h
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu_only.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5248 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_kernel.cu.cc
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.h
--rw-r--r--   0 runner    (1001) docker     (122)     7409 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.555862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5929 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_cpu.py
--rw-r--r--   0 runner    (1001) docker     (122)    25269 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.555862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/bev_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     6982 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/point_cloud_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    36317 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     4203 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/region_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)    15076 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/sample_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_assigner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8739 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/voxel_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.559862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24964 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/kitti_common.py
--rw-r--r--   0 runner    (1001) docker     (122)    16872 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     4288 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/load.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.563862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/activations.proto
--rw-r--r--   0 runner    (1001) docker     (122)    17330 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/activations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors.proto
--rw-r--r--   0 runner    (1001) docker     (122)    28358 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/box_coder.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9082 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/box_coder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader.proto
--rw-r--r--   0 runner    (1001) docker     (122)    20133 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/layers.proto
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/layers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     4742 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses.proto
--rw-r--r--   0 runner    (1001) docker     (122)    38504 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/model.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2538 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer.proto
--rw-r--r--   0 runner    (1001) docker     (122)    33725 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/pipeline.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5733 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/pipeline_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess.proto
--rw-r--r--   0 runner    (1001) docker     (122)    23581 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/sampler.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8977 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/sampler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second.proto
--rw-r--r--   0 runner    (1001) docker     (122)    34390 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10059 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/target.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/target_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14382 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/voxel_generator.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5450 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/voxel_generator_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.563862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.563862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/box_coder_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/input_reader_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5980 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/losses_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5996 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/lr_scheduler_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4690 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/optimizer_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/second_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.563862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_coders.py
--rw-r--r--   0 runner    (1001) docker     (122)    17990 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    19347 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18597 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/loss_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/pointpillars.py
--rw-r--r--   0 runner    (1001) docker     (122)    23561 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/tanet.py
--rw-r--r--   0 runner    (1001) docker     (122)    58499 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/voxelnet.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    27911 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9205 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/array_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6526 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     6635 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/learning_schedules.py
--rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/optim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15702 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/bbox_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.567862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8501 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/pybind11_build.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (122)    36928 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/eval.py
--rw-r--r--   0 runner    (1001) docker     (122)     6655 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/find.py
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5997 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (122)    30153 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/voxel_object_detection_3d_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.571862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.571862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.571862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:30.571862 opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-02-22 08:10:30.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    35912 2023-02-22 08:10:30.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:30.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-02-22 08:10:30.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:30.000000 opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.742896 opendr-toolkit-object-detection-3d-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-03 13:34:52.000000 opendr-toolkit-object-detection-3d-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-07-03 13:34:52.738896 opendr-toolkit-object-detection-3d-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-object-detection-3d-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:52.742896 opendr-toolkit-object-detection-3d-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-03 13:34:52.000000 opendr-toolkit-object-detection-3d-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.714895 opendr-toolkit-object-detection-3d-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11430 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/create_data_kitti.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/
+-rw-r--r--   0 runner    (1001) docker     (122)    52625 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    25983 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/train.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/val.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/train.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/val.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/train.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/nano_kitti_subsets/val.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.718895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/anchor_generator_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1091 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dbsampler_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/preprocess_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/similarity_calculator_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/target_assigner_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/voxel_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5871 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.config
+-rw-r--r--   0 runner    (1001) docker     (122)     5350 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.tiny.config
+-rw-r--r--   0 runner    (1001) docker     (122)     5893 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/people.config
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/test_short.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_16.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4377 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_20.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_24.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4397 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_28.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)     4832 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/test_short.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_16.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_20.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4832 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_24.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_28.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/
+-rw-r--r--   0 runner    (1001) docker     (122)     4401 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/test_short.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4410 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_16.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4380 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_20.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_24.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_28.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.722895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/test_short.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4862 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_16.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_20.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4835 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_24.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_28.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/tanet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.726895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_coders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33460 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_np_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.726895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/box_ops.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/box_ops.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.726895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu.h
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu_only.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5248 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_kernel.cu.cc
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7409 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.726895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5929 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25269 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.726895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/bev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6982 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/point_cloud_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36317 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4203 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/region_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15076 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/sample_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8739 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/voxel_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.726895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24964 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/kitti_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16872 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4288 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/load.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.730895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/activations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    17330 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/activations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    28358 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/box_coder.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9082 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/box_coder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    20133 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/layers.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/layers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4742 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    38504 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/model.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2538 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    33725 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/pipeline.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5733 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/pipeline_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    23581 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/sampler.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8977 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/sampler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    34390 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10059 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/target.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/target_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14382 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/voxel_generator.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5450 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/voxel_generator_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.730895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.730895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/box_coder_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/input_reader_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5980 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/losses_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5996 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/lr_scheduler_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4690 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/optimizer_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/second_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.730895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_coders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17990 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19347 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.730895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18597 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/loss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/pointpillars.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23561 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/tanet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58499 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/voxelnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27911 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.730895 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9205 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/array_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6526 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6635 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/learning_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/optim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15702 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/bbox_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8501 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/pybind11_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36928 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6655 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/find.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5997 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/voxel_object_detection_3d_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:52.734896 opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-07-03 13:34:52.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    35912 2023-07-03 13:34:52.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:52.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-03 13:34:52.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:52.000000 opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/.clang-format` & `opendr-toolkit-object-detection-3d-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/.gitignore` & `opendr-toolkit-object-detection-3d-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/CHANGELOG.md` & `opendr-toolkit-object-detection-3d-2.2.0/CHANGELOG.md`

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

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-object-detection-3d-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/Dockerfile` & `opendr-toolkit-object-detection-3d-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/Dockerfile-cuda` & `opendr-toolkit-object-detection-3d-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/Dockerfile-embedded` & `opendr-toolkit-object-detection-3d-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/LICENSE` & `opendr-toolkit-object-detection-3d-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/Makefile` & `opendr-toolkit-object-detection-3d-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/PKG-INFO` & `opendr-toolkit-object-detection-3d-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-object-detection-3d
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/object_detection_3d)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/README.md` & `opendr-toolkit-object-detection-3d-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/description.txt` & `opendr-toolkit-object-detection-3d-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/packages.txt` & `opendr-toolkit-object-detection-3d-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/_version.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/constants.py`

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

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/_version.py`

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

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/create_data_kitti.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/create_data_kitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/test.txt` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/test.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/train.txt` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/train.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/val.txt` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/kitti_subsets/val.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/train.txt` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/train.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/val.txt` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/datasets/mini_kitti_subsets/val.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/dependencies.ini` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/dependencies.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [runtime]
 # 'python' key expects a value using the Python requirements file format
 #  https://pip.pypa.io/en/stable/reference/pip_install/#requirements-file-format
 
-python=torch==1.9.0
-       torchvision==0.10.0
+python=torch==1.13.1
+       torchvision==0.14.1
        protobuf<=3.20.0
        tensorboardX>=2.0
        opencv-python==4.5.1.48
        matplotlib>=2.2.2
        tqdm
        onnx==1.8.0
        onnxruntime==1.3.0
```

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/logger.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/logger.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/anchor_generator_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/anchor_generator_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dataset_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dbsampler_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/dbsampler_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/preprocess_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/preprocess_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/similarity_calculator_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/similarity_calculator_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/target_assigner_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/target_assigner_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/voxel_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/builder/voxel_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.config` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.config`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.tiny.config` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/car.tiny.config`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/people.config` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/people.config`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/test_short.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/test_short.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_16.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_16.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_20.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_20.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_24.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_24.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_28.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/car/xyres_28.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/test_short.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/test_short.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_16.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_16.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_20.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_20.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_24.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_24.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_28.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/pointpillars/ped_cycle/xyres_28.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/test_short.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/test_short.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_16.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_16.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_20.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_20.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_24.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_24.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_28.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/car/xyres_28.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/test_short.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/test_short.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_16.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_16.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_20.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_20.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_24.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_24.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_28.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/configs/tanet/ped_cycle/xyres_28.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/anchor_generator.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_coders.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_coders.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_np_ops.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/box_np_ops.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/box_ops.h` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/box_ops.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.cc` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.cc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.h` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu.h` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu_only.cc` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_cpu_only.cc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_kernel.cu.cc` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/nms/nms_kernel.cu.cc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.cc` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.cc`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.h` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/cc/point_cloud_ops.h`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/geometry.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/geometry.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_cpu.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_cpu.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_gpu.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/non_max_suppression/nms_gpu.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/bev_ops.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/bev_ops.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/point_cloud_ops.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/point_cloud/point_cloud_ops.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/preprocess.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/preprocess.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/region_similarity.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/region_similarity.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/sample_ops.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/sample_ops.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_assigner.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_assigner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_ops.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/target_ops.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/voxel_generator.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/core/voxel_generator.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/dataset.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/dataset.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/kitti_common.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/kitti_common.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/preprocess.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/load.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/load.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/activations_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/activations_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/anchors_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/box_coder_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/box_coder_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/input_reader_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/layers_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/layers_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/losses_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/model_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/model_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/optimizer_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/pipeline_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/preprocess_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/sampler_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/sampler_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/second_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/similarity_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/target_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/target_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train.proto` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train.proto`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/train_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/voxel_generator_pb2.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/protos/voxel_generator_pb2.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/box_coder_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/box_coder_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/input_reader_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/input_reader_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/losses_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/losses_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/lr_scheduler_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/lr_scheduler_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/optimizer_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/optimizer_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/second_builder.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/builder/second_builder.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_coders.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_coders.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_torch_ops.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/box_torch_ops.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/losses.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/core/losses.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/loss_utils.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/loss_utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/pointpillars.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/pointpillars.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/tanet.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/tanet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/voxelnet.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/models/voxelnet.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/utils.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/run.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/run.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/metrics.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/metrics.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/__init__.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/common.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/nn/modules/common.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/array_ops.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/ops/array_ops.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/tools.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/tools.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/__init__.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/__init__.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/checkpoint.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/common.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/common.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/learning_schedules.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/learning_schedules.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/optim.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/torchplus_tanet/train/optim.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/bbox_plot.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/bbox_plot.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/command.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/command.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/pybind11_build.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/buildtools/pybind11_build.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/eval.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/eval.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/find.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/find.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/loader.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/loader.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/progress_bar.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/second_detector/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/voxel_object_detection_3d_learner.py` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr/perception/object_detection_3d/voxel_object_detection_3d/voxel_object_detection_3d_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,15 +589,15 @@
             output_names.append("Refine_dir_preds")
 
         torch.onnx.export(
             self.model.rpn,
             inp,
             output_name,
             verbose=verbose,
-            enable_onnx_checker=True,
+            opset_version=11,
             do_constant_folding=do_constant_folding,
             input_names=input_names,
             output_names=output_names,
         )
 
     def __load_rpn_from_onnx(self, path):
         """
```

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/PKG-INFO` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-object-detection-3d
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: perception/object_detection_3d)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-object-detection-3d-2.1.0/src/opendr_toolkit_object_detection_3d.egg-info/SOURCES.txt` & `opendr-toolkit-object-detection-3d-2.2.0/src/opendr_toolkit_object_detection_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

