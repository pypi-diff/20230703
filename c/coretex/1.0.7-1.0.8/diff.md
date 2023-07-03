# Comparing `tmp/coretex-1.0.7.tar.gz` & `tmp/coretex-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-1.0.7.tar", last modified: Fri Jun 23 09:30:00 2023, max compression
+gzip compressed data, was "coretex-1.0.8.tar", last modified: Mon Jul  3 08:16:20 2023, max compression
```

## Comparing `coretex-1.0.7.tar` & `coretex-1.0.8.tar`

### file list

```diff
@@ -1,181 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-06-23 09:29:47.000000 coretex-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-23 09:30:00.421241 coretex-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-23 09:29:47.000000 coretex-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.401240 coretex-1.0.7/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.401240 coretex-1.0.7/coretex/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/cache/cache_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/codable/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/codable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/codable/codable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/codable/descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/annotation/image/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/classes_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/annotation/image/coretex_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converter_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/conversion/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/city_scape_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/create_ml_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/pascal/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/voc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.405240 coretex-1.0.7/coretex/coretex/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/image_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/network_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/experiment_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.409240 coretex-1.0.7/coretex/coretex/experiment/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/metric_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/experiment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/model/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/any_local_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/custom_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/custom_sample/local_custom_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.413241 coretex-1.0.7/coretex/coretex/sample/image_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/image_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_sample/local_image_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/local_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/network_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/sample/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/coretex/space/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/coretex/space/space_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/folder_management/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/folder_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/folder_management/folder_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/log_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.417241 coretex-1.0.7/coretex/networking/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/chunk_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/network_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/requests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/networking/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/project/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/qiime2/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/qiime2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/qiime2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.421241 coretex-1.0.7/coretex/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/console_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-23 09:29:47.000000 coretex-1.0.7/coretex/utils/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:30:00.401240 coretex-1.0.7/coretex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 09:30:00.000000 coretex-1.0.7/coretex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-23 09:29:47.000000 coretex-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:30:00.421241 coretex-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.575549 coretex-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-07-03 08:16:09.000000 coretex-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 08:16:20.571549 coretex-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-03 08:16:09.000000 coretex-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/cache/cache_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/codable/descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.547548 coretex-1.0.8/coretex/coretex/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.547548 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/network_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.547548 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/local_sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.551548 coretex-1.0.8/coretex/coretex/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/experiment_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.551548 coretex-1.0.8/coretex/coretex/experiment/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.555548 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.555548 coretex-1.0.8/coretex/coretex/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.555548 coretex-1.0.8/coretex/coretex/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/coretex/sample/sequence_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sequence_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sequence_sample/local_sequence_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sequence_sample/sequence_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/coretex/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/space_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/folder_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/folder_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/folder_management/folder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.567549 coretex-1.0.8/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/requests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.567549 coretex-1.0.8/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/console_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-03 08:16:09.000000 coretex-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:16:20.575549 coretex-1.0.8/setup.cfg
```

### Comparing `coretex-1.0.7/LICENSE` & `coretex-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/PKG-INFO` & `coretex-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
@@ -57,15 +57,15 @@
     pass
 
 
 if __name__ == "__main__":
     initializeProject(main)
 ```
 
-(Read the documentation and learn how you can migrate your project to the Coretex platform -> [Migrate your project to Coretex](https://app.gitbook.com/o/6QxmEiF5ygi67vFH3kV1/s/YoN0XCeop3vrJ0hyRKxx/getting-started/demo-experiments/migrate-your-project-to-coretex))
+Read the documentation and learn how you can migrate your project to the Coretex platform -> [Migrate your project to Coretex](https://app.gitbook.com/o/6QxmEiF5ygi67vFH3kV1/s/YoN0XCeop3vrJ0hyRKxx/getting-started/demo-experiments/migrate-your-project-to-coretex)
 
 ## Key Features
 
 Coretex.ai offers a range of features to support users in their AI experimentation, including:
 
 * **Project Templates:** Battle-tested templates that make training ML models and processing data simple,
```

### Comparing `coretex-1.0.7/README.md` & `coretex-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     pass
 
 
 if __name__ == "__main__":
     initializeProject(main)
 ```
 
-(Read the documentation and learn how you can migrate your project to the Coretex platform -> [Migrate your project to Coretex](https://app.gitbook.com/o/6QxmEiF5ygi67vFH3kV1/s/YoN0XCeop3vrJ0hyRKxx/getting-started/demo-experiments/migrate-your-project-to-coretex))
+Read the documentation and learn how you can migrate your project to the Coretex platform -> [Migrate your project to Coretex](https://app.gitbook.com/o/6QxmEiF5ygi67vFH3kV1/s/YoN0XCeop3vrJ0hyRKxx/getting-started/demo-experiments/migrate-your-project-to-coretex)
 
 ## Key Features
 
 Coretex.ai offers a range of features to support users in their AI experimentation, including:
 
 * **Project Templates:** Battle-tested templates that make training ML models and processing data simple,
```

### Comparing `coretex-1.0.7/coretex/__init__.py` & `coretex-1.0.8/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/_configuration.py` & `coretex-1.0.8/coretex/_configuration.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/_logger.py` & `coretex-1.0.8/coretex/_logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/cache/__init__.py` & `coretex-1.0.8/coretex/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/cache/cache_module.py` & `coretex-1.0.8/coretex/cache/cache_module.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/codable/__init__.py` & `coretex-1.0.8/coretex/codable/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/codable/codable.py` & `coretex-1.0.8/coretex/codable/codable.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/codable/descriptor.py` & `coretex-1.0.8/coretex/codable/descriptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/__init__.py` & `coretex-1.0.8/coretex/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/annotation/__init__.py` & `coretex-1.0.8/coretex/coretex/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/annotation/image/__init__.py` & `coretex-1.0.8/coretex/coretex/annotation/image/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/annotation/image/bbox.py` & `coretex-1.0.8/coretex/coretex/annotation/image/bbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,57 +24,57 @@
 class BBox(Codable):
 
     """
         Bounding Box as a python class with utility methods
 
         Properties
         ----------
-        minX : float
+        minX : int
             top left x coordinate
-        minY : float
+        minY : int
             top left y coordinate
-        width : float
+        width : int
             width of the bounding box
-        height : float
+        height : int
             height of the bounding box
     """
 
-    def __init__(self, minX: float = 0, minY: float = 0, width: float = 0, height: float = 0) -> None:
+    def __init__(self, minX: int = 0, minY: int = 0, width: int = 0, height: int = 0) -> None:
         self.minX: Final = minX
         self.minY: Final = minY
 
         self.width: Final = width
         self.height: Final = height
 
     @property
-    def maxX(self) -> float:
+    def maxX(self) -> int:
         """
             Returns
             -------
-            float -> bottom right x coordinate
+            int -> bottom right x coordinate
         """
 
         return self.minX + self.width
 
     @property
-    def maxY(self) -> float:
+    def maxY(self) -> int:
         """
             Returns
             -------
-            float -> bottom right y coordinate
+            int -> bottom right y coordinate
         """
 
         return self.minY + self.height
 
     @property
-    def polygon(self) -> List[float]:
+    def polygon(self) -> List[int]:
         """
             Returns
             -------
-            List[float] -> Bounding box represented as a polygon (x, y) values
+            List[int] -> Bounding box represented as a polygon (x, y) values
         """
 
         return [
             self.minX, self.minY,  # top left
             self.maxX, self.minY,  # top right
             self.maxX, self.maxY,  # bottom right
             self.minX, self.maxY,  # bottom left
@@ -87,47 +87,47 @@
 
         descriptors["minX"] = KeyDescriptor("top_left_x")
         descriptors["minY"] = KeyDescriptor("top_left_y")
 
         return descriptors
 
     @classmethod
-    def create(cls, minX: float, minY: float, maxX: float, maxY: float) -> Self:
+    def create(cls, minX: int, minY: int, maxX: int, maxY: int) -> Self:
         """
             Utility constructor which has maxX and maxY as parameters instead
             of width and height
 
             Parameters
             ----------
-            minX : float
+            minX : int
                 top left x coordinate
-            minY : float
+            minY : int
                 top left y coordinate
-            maxX : float
+            maxX : int
                 bottom right x coordinate
-            maxY : float
+            maxY : int
                 bottom right y coordinate
 
             Returns
             -------
             Self -> bounding box
         """
 
         return cls(minX, minY, maxX - minX, maxY - minY)
 
     @classmethod
-    def fromPoly(cls, polygon: List[float]) -> Self:
+    def fromPoly(cls, polygon: List[int]) -> Self:
         """
             Creates bounding box from a polygon, by finding
             the minimum x and y coordinates and calculating
             width and height of the polygon
 
             Parameters
             ----------
-            polygon : List[float]
+            polygon : List[int]
                 list of x, y points - length must be even
 
             Returns
             -------
             Self -> bounding box
 
             Example
@@ -136,16 +136,16 @@
             \b
             >>> polygon = [0, 0, 0, 3, 4, 3, 4, 0]
             >>> bbox = Bbox.fromPoly(polygon)
             >>> print(f"minX: {bbox.minX}, minY: {bbox.minY}, width: {bbox.width}, height: {bbox.height}")
             "minX: 0, minY: 0, width: 4, height: 3"
         """
 
-        x: List[float] = []
-        y: List[float] = []
+        x: List[int] = []
+        y: List[int] = []
 
         for index, value in enumerate(polygon):
             if index % 2 == 0:
                 x.append(value)
             else:
                 y.append(value)
```

### Comparing `coretex-1.0.7/coretex/coretex/annotation/image/classes_format.py` & `coretex-1.0.8/coretex/coretex/annotation/image/classes_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/annotation/image/coretex_format.py` & `coretex-1.0.8/coretex/coretex/annotation/image/coretex_format.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 import numpy as np
 
 from .bbox import BBox
 from .classes_format import ImageDatasetClasses
 from ....codable import Codable, KeyDescriptor
 
 
-SegmentationType = List[float]
+SegmentationType = List[int]
 
 
-def toPoly(segmentation: List[float]) -> List[Tuple[float, float]]:
-    points: List[Tuple[float, float]] = []
+def toPoly(segmentation: List[int]) -> List[Tuple[int, int]]:
+    points: List[Tuple[int, int]] = []
 
     for index in range(0, len(segmentation) - 1, 2):
         points.append((segmentation[index], segmentation[index + 1]))
 
     return points
 
 
@@ -141,50 +141,50 @@
         """
 
         binaryMask = self.extractSegmentationMask(width, height)
         binaryMask[binaryMask > 0] = 1
 
         return binaryMask
 
-    def centroid(self) -> Tuple[float, float]:
+    def centroid(self) -> Tuple[int, int]:
         """
             Calculates centroid of segmentations
 
             Returns
             -------
-            Tuple[float, float] -> x, y coordinates of centroid
+            Tuple[int, int] -> x, y coordinates of centroid
         """
 
         flattenedSegmentations = [element for sublist in self.segmentations for element in sublist]
 
         listCX = [value for index, value in enumerate(flattenedSegmentations) if index % 2 == 0]
-        centerX = fsum(listCX) / len(listCX)
+        centerX = sum(listCX) // len(listCX)
 
         listCY = [value for index, value in enumerate(flattenedSegmentations) if index % 2 != 0]
-        centerY = fsum(listCY) / len(listCY)
+        centerY = sum(listCY) // len(listCY)
 
         return centerX, centerY
 
-    def centerSegmentations(self, newCentroid: Tuple[float, float]) -> None:
+    def centerSegmentations(self, newCentroid: Tuple[int, int]) -> None:
         """
             Centers segmentations to the specified center point
 
             Parameters
             ----------
-            newCentroid : Tuple[float, float]
+            newCentroid : Tuple[int, int]
                 x, y coordinates of centroid
             """
 
         newCenterX, newCenterY = newCentroid
         oldCenterX, oldCenterY = self.centroid()
 
-        modifiedSegmentations: List[List[float]] = []
+        modifiedSegmentations: List[List[int]] = []
 
         for segmentation in self.segmentations:
-            modifiedSegmentation: List[float] = []
+            modifiedSegmentation: List[int] = []
 
             for i in range(0, len(segmentation), 2):
                 x = segmentation[i] + (newCenterX - oldCenterX)
                 y = segmentation[i+1] + (newCenterY - oldCenterY)
 
                 modifiedSegmentation.append(x)
                 modifiedSegmentation.append(y)
@@ -199,31 +199,31 @@
 
             Parameters
             ----------
             degrees : int
                 degree of rotation
         """
 
-        rotatedSegmentations: List[List[float]] = []
+        rotatedSegmentations: List[List[int]] = []
         centerX, centerY = self.centroid()
 
         # because rotations with image and segmentations doesn't go in same direction
         # one of the rotations has to be inverted so they go in same direction
         theta = radians(-degrees)
         cosang, sinang = cos(theta), sin(theta)
 
         for segmentation in self.segmentations:
-            rotatedSegmentation: List[float] = []
+            rotatedSegmentation: List[int] = []
 
             for i in range(0, len(segmentation), 2):
                 x = segmentation[i] - centerX
                 y = segmentation[i + 1] - centerY
 
-                newX = (x * cosang - y * sinang) + centerX
-                newY = (x * sinang + y * cosang) + centerY
+                newX = int(x * cosang - y * sinang) + centerX
+                newY = int(x * sinang + y * cosang) + centerY
 
                 rotatedSegmentation.append(newX)
                 rotatedSegmentation.append(newY)
 
             rotatedSegmentations.append(rotatedSegmentation)
 
         self.segmentations = rotatedSegmentations
@@ -234,52 +234,52 @@
     """
         Image Annotation class
 
         Properties
         ----------
         name : str
             name of annotation class
-        width : float
+        width : int
             width of annotation
-        height : float
+        height : int
             height of annotation
         instances : List[CoretexSegmentationInstance]
             list of SegmentationInstance objects
     """
 
     name: str
-    width: float
-    height: float
+    width: int
+    height: int
     instances: List[CoretexSegmentationInstance]
 
     @classmethod
     def _keyDescriptors(cls) -> Dict[str, KeyDescriptor]:
         descriptors = super()._keyDescriptors()
         descriptors["instances"] = KeyDescriptor("instances", CoretexSegmentationInstance, list)
 
         return descriptors
 
     @classmethod
     def create(
         cls,
         name: str,
-        width: float,
-        height: float,
+        width: int,
+        height: int,
         instances: List[CoretexSegmentationInstance]
     ) -> Self:
         """
             Creates CoretexImageAnnotation object with provided parameters
 
             Parameters
             ----------
             name : str
                 name of annotation class
-            width : float
+            width : int
                 width of annotation
-            height : float
+            height : int
                 height of annotation
             instances : List[CoretexSegmentationInstance]
                 list of SegmentationInstance objects
 
             Returns
             -------
             The created CoretexImageAnnotation object
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/__init__.py` & `coretex-1.0.8/coretex/coretex/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/base_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converter_processor_factory.py` & `coretex-1.0.8/coretex/coretex/conversion/converter_processor_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/__init__.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/city_scape_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/city_scape_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/coco_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/create_ml_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/create_ml_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,18 @@
                 data = json.load(jsonFile)[0]
 
                 for annotation in data["annotations"]:
                     labels.add(annotation["label"])
 
         return labels
 
-    def __extractBBox(self, bbox: Dict[str, float]) -> BBox:
+    def __extractBBox(self, bbox: Dict[str, int]) -> BBox:
         return BBox(
-            bbox["x"] - bbox["width"] / 2,
-            bbox["y"] - bbox["height"] / 2,
+            bbox["x"] - bbox["width"] // 2,
+            bbox["y"] - bbox["height"] // 2,
             bbox["width"],
             bbox["height"]
         )
 
     def __extractInstance(self, annotation: Dict[str, Any]) -> Optional[CoretexSegmentationInstance]:
         label = annotation["label"]
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/human_segmentation_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def _dataSource(self) -> List[str]:
         return self.__imageNames
 
     def _extractLabels(self) -> Set[str]:
         return set(["background", "human"])
 
-    def __extractPolygons(self, annotationPath: str, imageWidth: int, imageHeight: int) -> List[List[float]]:
+    def __extractPolygons(self, annotationPath: str, imageWidth: int, imageHeight: int) -> List[List[int]]:
         maskImage = Image.open(annotationPath)
         if maskImage is None:
             return []
 
         maskImage = maskImage.resize((imageWidth, imageHeight), Image.ANTIALIAS)
         subMaskArray = np.asarray(maskImage, dtype = np.uint8)
 
@@ -77,15 +77,15 @@
         subMaskArray[:, 0] = 0
         subMaskArray[0, :] = 0
         subMaskArray[:, -1] = 0
         subMaskArray[-1, :] = 0
 
         contours = skimage.measure.find_contours(subMaskArray, 0.5)
 
-        segmentations: List[List[float]] = []
+        segmentations: List[List[int]] = []
         for contour in contours:
             for i in range(len(contour)):
                 row, col = contour[i]
                 contour[i] = (col - 1, row - 1)
 
             # Make a polygon and simplify it
             poly = Polygon(contour)
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/label_me_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/label_me_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         label = shape["label"]
 
         coretexClass = self._dataset.classByName(label)
         if coretexClass is None:
             logging.getLogger("coretexpylib").info(f">> [Coretex] Class: ({label}) is not a part of dataset")
             return None
 
-        points: List[float] = np.array(shape["points"]).flatten().tolist()
+        points: List[int] = np.array(shape["points"]).flatten().tolist()
         bbox = BBox.fromPoly(points)
 
         return CoretexSegmentationInstance.create(coretexClass.classIds[0], bbox, [points])
 
     def __extractImageAnnotation(self, imageAnnotation: Dict[str, Any]) -> None:
         imageName = Path(imageAnnotation["imagePath"]).stem
         imageName = f"{imageName}.jpg"
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/__init__.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/instance_extractor.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/instance_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import numpy as np
 
 from .shared import getTag, getBoxes
 from ....annotation import CoretexSegmentationInstance, BBox
 from ....dataset import ImageDataset
 
 
-ContourPoints = List[List[float]]
+ContourPoints = List[List[int]]
 SegmentationPolygon = List[ContourPoints]
 
 
 class ObjectCandidate:
 
     """
         Represents the groundtruth object for contour matching
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from typing import List, Set
 
 import os
 import glob
 import xml.etree.ElementTree as ET
 
-from .shared import getTag, toFloat
+from .shared import getTag, toInt
 from .instance_extractor import InstanceExtractor
 from ...base_converter import BaseConverter
 from .....coretex import CoretexImageAnnotation
 
 
 class PascalSegConverter(BaseConverter):
 
@@ -80,15 +80,15 @@
         instanceExtractor = InstanceExtractor(self._dataset)
         instances = instanceExtractor.extractInstances(root, filenamePNG, self.__segmentationPath)
 
         size = root.find('size')
         if size is None:
             return
 
-        width, height = toFloat(size, "width", "height")
+        width, height = toInt(size, "width", "height")
         if width is None or height is None:
             return
 
         coretexAnnotation = CoretexImageAnnotation.create(fileName, width, height, instances)
         self._saveImageAnnotationPair(os.path.join(self.__imagesPath, fileName), coretexAnnotation)
 
     def _extractSingleAnnotation(self, fileName: str) -> None:
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/pascal/shared.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,24 @@
 
     if firstVal is None or secondVal is None:
         return (None, None)
 
     return (float(firstVal), float(secondVal))
 
 
+def toInt(rootEl: ET.Element, firstEl: str, secondEl: str) -> Tuple[Optional[int], Optional[int]]:
+    firstVal = getTag(rootEl, firstEl)
+    secondVal = getTag(rootEl, secondEl)
+
+    if firstVal is None or secondVal is None:
+        return (None, None)
+
+    return (int(firstVal), int(secondVal))
+
+
 def getBoxes(bndbox: ET.Element) -> Optional[Dict[str, float]]:
     xmin, ymin = toFloat(bndbox, "xmin", "ymin")
     xmax, ymax = toFloat(bndbox, "xmax", "ymax")
 
     if xmax is None: return None
     if xmin is None: return None
     if ymax is None: return None
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/voc_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/voc_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Optional, List, Set
 
 import os
 import logging
 import glob
 import xml.etree.ElementTree as ET
 
-from .pascal.shared import getTag, getBoxes, toFloat
+from .pascal.shared import getTag, getBoxes, toInt
 from ..base_converter import BaseConverter
 from ...annotation import CoretexImageAnnotation, CoretexSegmentationInstance, BBox
 
 
 class VOCConverter(BaseConverter):
 
     def __init__(self, datasetName: str, spaceId: int, datasetPath: str) -> None:
@@ -87,15 +87,15 @@
         if fileName is None:
             return
 
         size = root.find('size')
         if size is None:
             return
 
-        width, height = toFloat(size, "width", "height")
+        width, height = toInt(size, "width", "height")
         if width is None or height is None:
             return
 
         coretexAnnotation = CoretexImageAnnotation.create(fileName, width, height, [])
 
         for obj in root.findall("object"):
             instance = self.__extractInstance(obj)
```

### Comparing `coretex-1.0.7/coretex/coretex/conversion/converters/yolo_converter.py` & `coretex-1.0.8/coretex/coretex/conversion/converters/yolo_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,18 @@
 
     def __extractBBox(self, rawInstance: List[str], width: int, height: int) -> BBox:
         xYolo = float(rawInstance[1])
         yYolo = float(rawInstance[2])
         wYolo = float(rawInstance[3])
         hYolo = float(rawInstance[4])
 
-        boxWidth = wYolo * width
-        boxHeight = hYolo * height
-        xMin = float(xYolo * width - (boxWidth / 2))
-        yMin = float(yYolo * height - (boxHeight / 2))
+        boxWidth = int(wYolo * width)
+        boxHeight = int(hYolo * height)
+        xMin = int(xYolo * width - (boxWidth / 2))
+        yMin = int(yYolo * height - (boxHeight / 2))
 
         return BBox(xMin, yMin, boxWidth, boxHeight)
 
     def __extractInstance(self, rawInstance: List[str], width: int, height: int) -> Optional[CoretexSegmentationInstance]:
         # Get class name
         labelId = int(rawInstance[0])
         label = self.__rawLabels[labelId]
```

### Comparing `coretex-1.0.7/coretex/coretex/dataset/__init__.py` & `coretex-1.0.8/coretex/coretex/dataset/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 from .image_dataset import ImageDataset, LocalImageDataset, augmentDataset
 from .image_segmentation_dataset import ImageSegmentationDataset, LocalImageSegmentationDataset
 from .computer_vision_dataset import ComputerVisionDataset, LocalComputerVisionDataset
 from .dataset import Dataset
 from .local_dataset import LocalDataset
 from .network_dataset import NetworkDataset
 from .utils import downloadDataset
+from .sequence_dataset import SequenceDataset, LocalSequenceDataset
```

### Comparing `coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/__init__.py` & `coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/__init__.py` & `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/base.py` & `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/custom_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_dataset/__init__.py` & `coretex-1.0.8/coretex/coretex/dataset/image_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_dataset/base.py` & `coretex-1.0.8/coretex/coretex/dataset/image_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_dataset/image_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/image_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_dataset/local_image_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/image_dataset/local_image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py` & `coretex-1.0.8/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 
 
 def composeImage(
     segmentedImages: List[PILImage],
     backgroundImage: np.ndarray,
     angle: int,
     scale: float
-) -> Tuple[PILImage, List[Tuple[float, float]]]:
+) -> Tuple[PILImage, List[Tuple[int, int]]]:
 
-    centroids: List[Tuple[float, float]] = []
+    centroids: List[Tuple[int, int]] = []
     locations: List[Tuple[int, int, int, int]] = []
 
     background = Image.fromarray(backgroundImage)
 
     for segmentedImage in segmentedImages:
         image = segmentedImage
 
@@ -132,16 +132,16 @@
 
             # Check if the image overlaps with any previously pasted images
             if not isOverlapping(x, y, resizedImage, locations):
                 break
 
         background.paste(resizedImage, (x, y), resizedImage)
 
-        centerX = x + resizedImage.width / 2
-        centerY = y + resizedImage.height / 2
+        centerX = x + resizedImage.width // 2
+        centerY = y + resizedImage.height // 2
 
         centroids.append((centerX, centerY))
 
         # Add the location to the list
         locations.append((x, y, resizedImage.width, resizedImage.height))
 
     return background, centroids
```

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/__init__.py` & `coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/local_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/network_dataset.py` & `coretex-1.0.8/coretex/coretex/dataset/network_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/dataset/utils.py` & `coretex-1.0.8/coretex/coretex/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/__init__.py` & `coretex-1.0.8/coretex/coretex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/artifact.py` & `coretex-1.0.8/coretex/coretex/experiment/artifact.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/experiment.py` & `coretex-1.0.8/coretex/coretex/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/experiment_builder.py` & `coretex-1.0.8/coretex/coretex/experiment/experiment_builder.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/__init__.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/metric.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/metric_factory.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/metric_type.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/metrics/utils.py` & `coretex-1.0.8/coretex/coretex/experiment/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/parameters.py` & `coretex-1.0.8/coretex/coretex/experiment/parameters.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/status.py` & `coretex-1.0.8/coretex/coretex/experiment/status.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/experiment/utils.py` & `coretex-1.0.8/coretex/coretex/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/model/__init__.py` & `coretex-1.0.8/coretex/coretex/model/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/model/model.py` & `coretex-1.0.8/coretex/coretex/model/model.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/__init__.py` & `coretex-1.0.8/coretex/coretex/sample/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,7 +19,9 @@
 from .image_sample import AnnotatedImageSampleData, LocalImageSample, ImageSample
 from .image_segmentation_sample import LocalImageSegmentationSample, ImageSegmentationSample
 from .computer_vision_sample import LocalComputerVisionSample, ComputerVisionSample
 from .any_local_sample import AnyLocalSample
 from .sample import Sample
 from .local_sample import LocalSample
 from .network_sample import NetworkSample
+from .sequence_sample import LocalSequenceSample, SequenceSample
+from .utils import chunkSampleImport
```

### Comparing `coretex-1.0.7/coretex/coretex/sample/any_local_sample.py` & `coretex-1.0.8/coretex/coretex/sample/any_local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/__init__.py` & `coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py` & `coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py` & `coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/custom_sample/__init__.py` & `coretex-1.0.8/coretex/coretex/sample/custom_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample.py` & `coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 
 from typing import Optional, Union
 from typing_extensions import Self
 from pathlib import Path
 
 from .custom_sample_data import CustomSampleData
 from .local_custom_sample import LocalCustomSample
+from ..utils import chunkSampleImport
 from ..network_sample import NetworkSample
-from ....networking import networkManager, ChunkUploadSession, MAX_CHUNK_SIZE
-from ....utils.file import isArchive
 
 
 class CustomSample(NetworkSample[CustomSampleData], LocalCustomSample):
 
     """
         Represents the custom Sample object from Coretex.ai\n
         Custom samples are used when working with Other Task\n
@@ -71,27 +70,9 @@
             >>> from coretex import CustomSample
             \b
             >>> sample = CustomSample.createCustomSample("name", 1023, "path/to/file")
             >>> if sample is None:
                     print("Failed to create custom sample")
         """
 
-        if isinstance(filePath, str):
-            filePath = Path(filePath)
-
-        if not isArchive(filePath):
-            raise ValueError(">> [Coretex] File must be an archive [.zip, .tar, .tar.gz]")
-
-        uploadSession = ChunkUploadSession(MAX_CHUNK_SIZE, filePath)
-        uploadId = uploadSession.run()
-
-        parameters = {
-            "name": name,
-            "dataset_id": datasetId,
-            "file_id": uploadId
-        }
-
-        response = networkManager.genericFormData("session/import", parameters)
-        if response.hasFailed():
-            return None
-
+        response = chunkSampleImport(name, datasetId, filePath)
         return cls.decode(response.json)
```

### Comparing `coretex-1.0.7/coretex/coretex/sample/custom_sample/custom_sample_data.py` & `coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/custom_sample/local_custom_sample.py` & `coretex-1.0.8/coretex/coretex/sample/custom_sample/local_custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_sample/__init__.py` & `coretex-1.0.8/coretex/coretex/sample/image_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_sample/image_format.py` & `coretex-1.0.8/coretex/coretex/sample/image_sample/image_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample.py` & `coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_sample/image_sample_data.py` & `coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_sample/local_image_sample.py` & `coretex-1.0.8/coretex/coretex/sample/image_sample/local_image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/__init__.py` & `coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py` & `coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py` & `coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/local_sample.py` & `coretex-1.0.8/coretex/coretex/sample/local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/network_sample.py` & `coretex-1.0.8/coretex/coretex/sample/network_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/sample/sample.py` & `coretex-1.0.8/coretex/coretex/sample/sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/space/__init__.py` & `coretex-1.0.8/coretex/coretex/space/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/space/base.py` & `coretex-1.0.8/coretex/coretex/space/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/space/project.py` & `coretex-1.0.8/coretex/coretex/space/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/space/space.py` & `coretex-1.0.8/coretex/coretex/space/space.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/coretex/space/space_task.py` & `coretex-1.0.8/coretex/coretex/space/space_task.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/folder_management/__init__.py` & `coretex-1.0.8/coretex/folder_management/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/folder_management/folder_manager.py` & `coretex-1.0.8/coretex/folder_management/folder_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/logging/__init__.py` & `coretex-1.0.8/coretex/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/logging/log.py` & `coretex-1.0.8/coretex/logging/log.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/logging/log_severity.py` & `coretex-1.0.8/coretex/logging/log_severity.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/logging/logger.py` & `coretex-1.0.8/coretex/logging/logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/__init__.py` & `coretex-1.0.8/coretex/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/chunk_upload_session.py` & `coretex-1.0.8/coretex/networking/chunk_upload_session.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/file_data.py` & `coretex-1.0.8/coretex/networking/file_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/network_manager.py` & `coretex-1.0.8/coretex/networking/network_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/network_manager_base.py` & `coretex-1.0.8/coretex/networking/network_manager_base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/network_object.py` & `coretex-1.0.8/coretex/networking/network_object.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/network_response.py` & `coretex-1.0.8/coretex/networking/network_response.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/request_type.py` & `coretex-1.0.8/coretex/networking/request_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/requests_manager.py` & `coretex-1.0.8/coretex/networking/requests_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/networking/user_data.py` & `coretex-1.0.8/coretex/networking/user_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/nlp/__init__.py` & `coretex-1.0.8/coretex/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/nlp/text.py` & `coretex-1.0.8/coretex/nlp/text.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/nlp/token.py` & `coretex-1.0.8/coretex/nlp/token.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/nlp/transcriber.py` & `coretex-1.0.8/coretex/nlp/transcriber.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/nlp/transcription.py` & `coretex-1.0.8/coretex/nlp/transcription.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/nlp/utils.py` & `coretex-1.0.8/coretex/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/project/__init__.py` & `coretex-1.0.8/coretex/project/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/project/base.py` & `coretex-1.0.8/coretex/project/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     def __init__(self, experiment: Experiment, refreshToken: str) -> None:
         self._experiment: Final = experiment
 
         self.__outputStream, self.__inputStream = multiprocessing.Pipe()
 
         self.process = multiprocessing.Process(
             target = uploadMetricsWorker,
-            args = (self.__outputStream, refreshToken, self._experiment.id)
+            args = (self.__outputStream, refreshToken, self._experiment.id),
+            daemon = True
         )
 
     @classmethod
     def create(cls, experimentId: int, refreshToken: str) -> Self:
         return cls(Experiment.fetchById(experimentId), refreshToken)
 
     def onStart(self) -> None:
@@ -67,15 +68,17 @@
     def onNetworkConnectionLost(self) -> None:
         FolderManager.instance().clearTempFiles()
 
         sys.exit(1)
 
     def onCleanUp(self) -> None:
         logging.getLogger("coretexpylib").info("Experiment execution finished")
+
         self.process.kill()
+        self.process.join()
 
         try:
             from py3nvml import py3nvml
             py3nvml.nvmlShutdown()
         except:
             pass
```

### Comparing `coretex-1.0.7/coretex/project/calculate_metrics.py` & `coretex-1.0.8/coretex/project/calculate_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,15 +86,25 @@
     try:
         experiment.createMetrics(METRICS)
     except NetworkRequestError:
         sendFailure(outputStream, "Failed to create metrics")
 
     sendSuccess(outputStream, "Metrics worker succcessfully started")
 
-    while True:
+    while outputStream.writable and not outputStream.closed:
+        try:
+            # If parent process gets killed with SIGKILL there
+            # is no guarantee that the child process will get
+            # closed so we ping the parent process to check if
+            # the pipe is available or not
+            outputStream.send(None)
+        except BrokenPipeError:
+            outputStream.close()
+            break
+
         startTime = time.time()
         metricValues: Dict[str, Tuple[float, float]] = {}
 
         for metric in experiment.metrics:
             metricValue = metric.extract()
 
             if metricValue is not None:
```

### Comparing `coretex-1.0.7/coretex/project/heartbeat.py` & `coretex-1.0.8/coretex/project/heartbeat.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/project/local.py` & `coretex-1.0.8/coretex/project/local.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/project/remote.py` & `coretex-1.0.8/coretex/project/remote.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/qiime2/__init__.py` & `coretex-1.0.8/coretex/qiime2/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/qiime2/utils.py` & `coretex-1.0.8/coretex/qiime2/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/threading/__init__.py` & `coretex-1.0.8/coretex/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/threading/threaded_data_processor.py` & `coretex-1.0.8/coretex/threading/threaded_data_processor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/utils/__init__.py` & `coretex-1.0.8/coretex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/utils/console_progress_bar.py` & `coretex-1.0.8/coretex/utils/console_progress_bar.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/utils/date.py` & `coretex-1.0.8/coretex/utils/date.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex/utils/file.py` & `coretex-1.0.8/coretex/utils/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,14 +130,38 @@
     if not isGzip(source):
         raise ValueError(">> [Coretex] Not a .gz file")
 
     with gzip.open(source, "r") as gzipFile, open(destination, "wb") as destinationFile:
         shutil.copyfileobj(gzipFile, destinationFile)
 
 
+def archive(source: Path, destination: Path) -> None:
+    """
+        Archives and compresses the provided file or directory
+        using ZipFile module
+
+        Parameters
+        ----------
+        source : Path
+            file to be archived and compressed
+        destination : Path
+            location to which the zip file will be stored
+    """
+
+    with ZipFile(destination, "w", zipfile.ZIP_DEFLATED) as destinationFile:
+        if source.is_file():
+            destinationFile.write(source, source.name)
+        else:
+            for path in source.rglob("*"):
+                if not path.is_file():
+                    continue
+
+                destinationFile.write(path, path.relative_to(source))
+
+
 def walk(path: Path) -> Generator[Path, None, None]:
     """
         os.walk implementation for pathlib.Path
 
         Parameters
         ----------
         path : Path
```

### Comparing `coretex-1.0.7/coretex/utils/number.py` & `coretex-1.0.8/coretex/utils/number.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.7/coretex.egg-info/PKG-INFO` & `coretex-1.0.8/coretex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
@@ -57,15 +57,15 @@
     pass
 
 
 if __name__ == "__main__":
     initializeProject(main)
 ```
 
-(Read the documentation and learn how you can migrate your project to the Coretex platform -> [Migrate your project to Coretex](https://app.gitbook.com/o/6QxmEiF5ygi67vFH3kV1/s/YoN0XCeop3vrJ0hyRKxx/getting-started/demo-experiments/migrate-your-project-to-coretex))
+Read the documentation and learn how you can migrate your project to the Coretex platform -> [Migrate your project to Coretex](https://app.gitbook.com/o/6QxmEiF5ygi67vFH3kV1/s/YoN0XCeop3vrJ0hyRKxx/getting-started/demo-experiments/migrate-your-project-to-coretex)
 
 ## Key Features
 
 Coretex.ai offers a range of features to support users in their AI experimentation, including:
 
 * **Project Templates:** Battle-tested templates that make training ML models and processing data simple,
```

### Comparing `coretex-1.0.7/coretex.egg-info/SOURCES.txt` & `coretex-1.0.8/coretex.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,18 @@
 coretex/coretex/dataset/image_dataset/base.py
 coretex/coretex/dataset/image_dataset/image_dataset.py
 coretex/coretex/dataset/image_dataset/local_image_dataset.py
 coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
 coretex/coretex/dataset/image_segmentation_dataset/__init__.py
 coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
 coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+coretex/coretex/dataset/sequence_dataset/__init__.py
+coretex/coretex/dataset/sequence_dataset/base.py
+coretex/coretex/dataset/sequence_dataset/local_sequence_dataset.py
+coretex/coretex/dataset/sequence_dataset/sequence_dataset.py
 coretex/coretex/experiment/__init__.py
 coretex/coretex/experiment/artifact.py
 coretex/coretex/experiment/experiment.py
 coretex/coretex/experiment/experiment_builder.py
 coretex/coretex/experiment/parameters.py
 coretex/coretex/experiment/status.py
 coretex/coretex/experiment/utils.py
@@ -82,14 +86,15 @@
 coretex/coretex/model/__init__.py
 coretex/coretex/model/model.py
 coretex/coretex/sample/__init__.py
 coretex/coretex/sample/any_local_sample.py
 coretex/coretex/sample/local_sample.py
 coretex/coretex/sample/network_sample.py
 coretex/coretex/sample/sample.py
+coretex/coretex/sample/utils.py
 coretex/coretex/sample/computer_vision_sample/__init__.py
 coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
 coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
 coretex/coretex/sample/custom_sample/__init__.py
 coretex/coretex/sample/custom_sample/custom_sample.py
 coretex/coretex/sample/custom_sample/custom_sample_data.py
 coretex/coretex/sample/custom_sample/local_custom_sample.py
@@ -97,14 +102,17 @@
 coretex/coretex/sample/image_sample/image_format.py
 coretex/coretex/sample/image_sample/image_sample.py
 coretex/coretex/sample/image_sample/image_sample_data.py
 coretex/coretex/sample/image_sample/local_image_sample.py
 coretex/coretex/sample/image_segmentation_sample/__init__.py
 coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
 coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+coretex/coretex/sample/sequence_sample/__init__.py
+coretex/coretex/sample/sequence_sample/local_sequence_sample.py
+coretex/coretex/sample/sequence_sample/sequence_sample.py
 coretex/coretex/space/__init__.py
 coretex/coretex/space/base.py
 coretex/coretex/space/project.py
 coretex/coretex/space/space.py
 coretex/coretex/space/space_task.py
 coretex/folder_management/__init__.py
 coretex/folder_management/folder_manager.py
```

### Comparing `coretex-1.0.7/pyproject.toml` & `coretex-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "coretex"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" }
 ]
 maintainers = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
   { name="Igor Perić", email="igor@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
```

