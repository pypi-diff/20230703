# Comparing `tmp/mmengine-0.7.4.tar.gz` & `tmp/mmengine-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.7.4.tar", last modified: Sat Jun  3 15:55:57 2023, max compression
+gzip compressed data, was "dist/mmengine-0.8.0.tar", last modified: Mon Jul  3 12:32:28 2023, max compression
```

## Comparing `mmengine-0.7.4.tar` & `mmengine-0.8.0.tar`

### file list

```diff
@@ -1,183 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-03 15:54:29.000000 mmengine-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-06-03 15:55:57.000000 mmengine-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-03 15:54:29.000000 mmengine-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29215 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    63464 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    25968 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)   100622 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36462 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-06-03 15:54:29.000000 mmengine-0.7.4/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-03 15:55:57.000000 mmengine-0.7.4/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 15:55:56.000000 mmengine-0.7.4/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-03 15:55:57.000000 mmengine-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-03 15:54:29.000000 mmengine-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-03 12:30:58.000000 mmengine-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-07-03 12:32:28.000000 mmengine-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-07-03 12:30:58.000000 mmengine-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70813 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/_flexible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101587 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 12:32:28.000000 mmengine-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-03 12:30:59.000000 mmengine-0.8.0/setup.py
```

### Comparing `mmengine-0.7.4/PKG-INFO` & `mmengine-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6d 656e  : 2.1.Name: mmen
 00000020: 6769 6e65 0a56 6572 7369 6f6e 3a20 302e  gine.Version: 0.
-00000030: 372e 340a 5375 6d6d 6172 793a 2045 6e67  7.4.Summary: Eng
+00000030: 382e 300a 5375 6d6d 6172 793a 2045 6e67  8.0.Summary: Eng
 00000040: 696e 6520 6f66 204f 7065 6e4d 4d4c 6162  ine of OpenMMLab
 00000050: 2070 726f 6a65 6374 730a 486f 6d65 2d70   projects.Home-p
 00000060: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000070: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
 00000080: 6162 2f6d 6d65 6e67 696e 650a 4175 7468  ab/mmengine.Auth
 00000090: 6f72 3a20 4d4d 456e 6769 6e65 2041 7574  or: MMEngine Aut
 000000a0: 686f 7273 0a41 7574 686f 722d 656d 6169  hors.Author-emai
@@ -261,1018 +261,1067 @@
 00001040: 2f32 3139 3032 3631 3230 2d62 6137 3165  /219026120-ba71e
 00001050: 3438 622d 3665 3934 2d34 6264 342d 6234  48b-6e94-4bd4-b4
 00001060: 6539 2d62 3764 3137 3562 3565 3336 322e  e9-b7d175b5e362.
 00001070: 706e 6722 2077 6964 7468 3d22 3325 2220  png" width="3%" 
 00001080: 616c 743d 2222 202f 3e3c 2f61 3e0a 2020  alt="" /></a>.  
 00001090: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
 000010a0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-000010b0: 2049 6e74 726f 6475 6374 696f 6e0a 2020   Introduction.  
-000010c0: 2020 2020 2020 0a20 2020 2020 2020 204d        .        M
-000010d0: 4d45 6e67 696e 6520 6973 2061 2066 6f75  MEngine is a fou
-000010e0: 6e64 6174 696f 6e61 6c20 6c69 6272 6172  ndational librar
-000010f0: 7920 666f 7220 7472 6169 6e69 6e67 2064  y for training d
-00001100: 6565 7020 6c65 6172 6e69 6e67 206d 6f64  eep learning mod
-00001110: 656c 7320 6261 7365 6420 6f6e 2050 7954  els based on PyT
-00001120: 6f72 6368 2e20 4974 2070 726f 7669 6465  orch. It provide
-00001130: 7320 6120 736f 6c69 6420 656e 6769 6e65  s a solid engine
-00001140: 6572 696e 6720 666f 756e 6461 7469 6f6e  ering foundation
-00001150: 2061 6e64 2066 7265 6573 2064 6576 656c   and frees devel
-00001160: 6f70 6572 7320 6672 6f6d 2077 7269 7469  opers from writi
-00001170: 6e67 2072 6564 756e 6461 6e74 2063 6f64  ng redundant cod
-00001180: 6573 206f 6e20 776f 726b 666c 6f77 732e  es on workflows.
-00001190: 2049 7420 7365 7276 6573 2061 7320 7468   It serves as th
-000011a0: 6520 7472 6169 6e69 6e67 2065 6e67 696e  e training engin
-000011b0: 6520 6f66 2061 6c6c 204f 7065 6e4d 4d4c  e of all OpenMML
-000011c0: 6162 2063 6f64 6562 6173 6573 2c20 7768  ab codebases, wh
-000011d0: 6963 6820 7375 7070 6f72 7420 6875 6e64  ich support hund
-000011e0: 7265 6473 206f 6620 616c 676f 7269 7468  reds of algorith
-000011f0: 6d73 2069 6e20 7661 7269 6f75 7320 7265  ms in various re
-00001200: 7365 6172 6368 2061 7265 6173 2e20 4d6f  search areas. Mo
-00001210: 7265 6f76 6572 2c20 4d4d 456e 6769 6e65  reover, MMEngine
-00001220: 2069 7320 616c 736f 2067 656e 6572 6963   is also generic
-00001230: 2074 6f20 6265 2061 7070 6c69 6564 2074   to be applied t
-00001240: 6f20 6e6f 6e2d 4f70 656e 4d4d 4c61 6220  o non-OpenMMLab 
-00001250: 7072 6f6a 6563 7473 2e0a 2020 2020 2020  projects..      
-00001260: 2020 0a20 2020 2020 2020 204d 616a 6f72    .        Major
-00001270: 2066 6561 7475 7265 733a 0a20 2020 2020   features:.     
-00001280: 2020 200a 2020 2020 2020 2020 312e 202a     .        1. *
-00001290: 2a41 2075 6e69 7665 7273 616c 2061 6e64  *A universal and
-000012a0: 2070 6f77 6572 6675 6c20 7275 6e6e 6572   powerful runner
-000012b0: 2a2a 3a0a 2020 2020 2020 2020 0a20 2020  **:.        .   
-000012c0: 2020 2020 2020 2020 2d20 5375 7070 6f72          - Suppor
-000012d0: 7473 2074 7261 696e 696e 6720 6469 6666  ts training diff
-000012e0: 6572 656e 7420 7461 736b 7320 7769 7468  erent tasks with
-000012f0: 2061 2073 6d61 6c6c 2061 6d6f 756e 7420   a small amount 
-00001300: 6f66 2063 6f64 652c 2065 2e67 2e2c 2049  of code, e.g., I
-00001310: 6d61 6765 4e65 7420 6361 6e20 6265 2074  mageNet can be t
-00001320: 7261 696e 6564 2077 6974 6820 6f6e 6c79  rained with only
-00001330: 2038 3020 6c69 6e65 7320 6f66 2063 6f64   80 lines of cod
-00001340: 6520 2834 3030 206c 696e 6573 206f 6620  e (400 lines of 
-00001350: 7468 6520 6f72 6967 696e 616c 2050 7954  the original PyT
-00001360: 6f72 6368 2065 7861 6d70 6c65 292e 0a20  orch example).. 
-00001370: 2020 2020 2020 2020 2020 2d20 4561 7369            - Easi
-00001380: 6c79 2063 6f6d 7061 7469 626c 6520 7769  ly compatible wi
-00001390: 7468 206d 6f64 656c 7320 6672 6f6d 2070  th models from p
-000013a0: 6f70 756c 6172 2061 6c67 6f72 6974 686d  opular algorithm
-000013b0: 206c 6962 7261 7269 6573 2073 7563 6820   libraries such 
-000013c0: 6173 2054 494d 4d2c 2054 6f72 6368 5669  as TIMM, TorchVi
-000013d0: 7369 6f6e 2c20 616e 6420 4465 7465 6374  sion, and Detect
-000013e0: 726f 6e32 2e0a 2020 2020 2020 2020 0a20  ron2..        . 
-000013f0: 2020 2020 2020 2032 2e20 2a2a 4f70 656e         2. **Open
-00001400: 2061 7263 6869 7465 6374 7572 6520 7769   architecture wi
-00001410: 7468 2075 6e69 6669 6564 2069 6e74 6572  th unified inter
-00001420: 6661 6365 732a 2a3a 0a20 2020 2020 2020  faces**:.       
-00001430: 200a 2020 2020 2020 2020 2020 202d 2048   .           - H
-00001440: 616e 646c 6573 2064 6966 6665 7265 6e74  andles different
-00001450: 2061 6c67 6f72 6974 686d 2074 6173 6b73   algorithm tasks
-00001460: 2077 6974 6820 756e 6966 6965 6420 4150   with unified AP
-00001470: 4973 2c20 652e 672e 2c20 696d 706c 656d  Is, e.g., implem
-00001480: 656e 7420 6120 6d65 7468 6f64 2061 6e64  ent a method and
-00001490: 2061 7070 6c79 2069 7420 746f 2061 6c6c   apply it to all
-000014a0: 2063 6f6d 7061 7469 626c 6520 6d6f 6465   compatible mode
-000014b0: 6c73 2e0a 2020 2020 2020 2020 2020 202d  ls..           -
-000014c0: 2050 726f 7669 6465 7320 6120 756e 6966   Provides a unif
-000014d0: 6965 6420 6162 7374 7261 6374 696f 6e20  ied abstraction 
-000014e0: 666f 7220 7570 7065 722d 6c65 7665 6c20  for upper-level 
-000014f0: 616c 676f 7269 7468 6d20 6c69 6272 6172  algorithm librar
-00001500: 6965 732c 2077 6869 6368 2073 7570 706f  ies, which suppo
-00001510: 7274 7320 7661 7269 6f75 7320 6261 636b  rts various back
-00001520: 2d65 6e64 2064 6576 6963 6573 2073 7563  -end devices suc
-00001530: 6820 6173 204e 7669 6469 6120 4355 4441  h as Nvidia CUDA
-00001540: 2c20 4d61 6320 4d50 532c 2041 4d44 2c20  , Mac MPS, AMD, 
-00001550: 4d4c 552c 2061 6e64 206d 6f72 6520 666f  MLU, and more fo
-00001560: 7220 6d6f 6465 6c20 7472 6169 6e69 6e67  r model training
-00001570: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00001580: 2020 2033 2e20 2a2a 4375 7374 6f6d 697a     3. **Customiz
-00001590: 6162 6c65 2074 7261 696e 696e 6720 7072  able training pr
-000015a0: 6f63 6573 732a 2a3a 0a20 2020 2020 2020  ocess**:.       
-000015b0: 200a 2020 2020 2020 2020 2020 202d 2044   .           - D
-000015c0: 6566 696e 6573 2074 6865 2074 7261 696e  efines the train
-000015d0: 696e 6720 7072 6f63 6573 7320 6a75 7374  ing process just
-000015e0: 206c 696b 6520 706c 6179 696e 6720 7769   like playing wi
-000015f0: 7468 204c 6567 6f73 2e0a 2020 2020 2020  th Legos..      
-00001600: 2020 2020 202d 2050 726f 7669 6465 7320       - Provides 
-00001610: 7269 6368 2063 6f6d 706f 6e65 6e74 7320  rich components 
-00001620: 616e 6420 7374 7261 7465 6769 6573 2e0a  and strategies..
-00001630: 2020 2020 2020 2020 2020 202d 2043 6f6d             - Com
-00001640: 706c 6574 6520 636f 6e74 726f 6c73 206f  plete controls o
-00001650: 6e20 7468 6520 7472 6169 6e69 6e67 2070  n the training p
-00001660: 726f 6365 7373 2077 6974 6820 6469 6666  rocess with diff
-00001670: 6572 656e 7420 6c65 7665 6c73 206f 6620  erent levels of 
-00001680: 4150 4973 2e0a 2020 2020 2020 2020 0a20  APIs..        . 
-00001690: 2020 2020 2020 2023 2320 5768 6174 2773         ## What's
-000016a0: 204e 6577 0a20 2020 2020 2020 200a 2020   New.        .  
-000016b0: 2020 2020 2020 7630 2e37 2e34 2077 6173        v0.7.4 was
-000016c0: 2072 656c 6561 7365 6420 6f6e 2032 3032   released on 202
-000016d0: 332d 3036 2d30 332e 0a20 2020 2020 2020  3-06-03..       
-000016e0: 200a 2020 2020 2020 2020 2323 2320 4869   .        ### Hi
-000016f0: 6768 6c69 6768 7473 0a20 2020 2020 2020  ghlights.       
-00001700: 200a 2020 2020 2020 2020 2d20 5375 7070   .        - Supp
-00001710: 6f72 7420 7573 696e 6720 5b60 436c 6561  ort using [`Clea
-00001720: 724d 4c60 5d28 6874 7470 733a 2f2f 6d6d  rML`](https://mm
-00001730: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
-00001740: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001750: 636f 6d6d 6f6e 5f75 7361 6765 2f76 6973  common_usage/vis
-00001760: 7561 6c69 7a65 5f74 7261 696e 696e 675f  ualize_training_
-00001770: 6c6f 672e 6874 6d6c 2363 6c65 6172 6d6c  log.html#clearml
-00001780: 2920 746f 2072 6563 6f72 6420 6578 7065  ) to record expe
-00001790: 7269 6d65 6e74 2064 6174 610a 2020 2020  riment data.    
-000017a0: 2020 2020 2d20 4164 6420 5b60 536f 7068      - Add [`Soph
-000017b0: 6961 605d 2868 7474 7073 3a2f 2f6d 6d65  ia`](https://mme
-000017c0: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
-000017d0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f63  s.io/en/latest/c
-000017e0: 6f6d 6d6f 6e5f 7573 6167 652f 6265 7474  ommon_usage/bett
-000017f0: 6572 5f6f 7074 696d 697a 6572 732e 6874  er_optimizers.ht
-00001800: 6d6c 2373 6f70 6869 6129 206f 7074 696d  ml#sophia) optim
-00001810: 697a 6572 730a 2020 2020 2020 2020 0a20  izers.        . 
-00001820: 2020 2020 2020 2052 6561 6420 5b43 6861         Read [Cha
-00001830: 6e67 656c 6f67 5d28 2e2f 646f 6373 2f65  ngelog](./docs/e
-00001840: 6e2f 6e6f 7465 732f 6368 616e 6765 6c6f  n/notes/changelo
-00001850: 672e 6d64 2376 3037 342d 3036 3033 3230  g.md#v074-060320
-00001860: 3233 2920 666f 7220 6d6f 7265 2064 6574  23) for more det
-00001870: 6169 6c73 2e0a 2020 2020 2020 2020 0a20  ails..        . 
-00001880: 2020 2020 2020 2023 2320 496e 7374 616c         ## Instal
-00001890: 6c61 7469 6f6e 0a20 2020 2020 2020 200a  lation.        .
-000018a0: 2020 2020 2020 2020 4265 666f 7265 2069          Before i
-000018b0: 6e73 7461 6c6c 696e 6720 4d4d 456e 6769  nstalling MMEngi
-000018c0: 6e65 2c20 706c 6561 7365 2065 6e73 7572  ne, please ensur
-000018d0: 6520 7468 6174 2050 7954 6f72 6368 2068  e that PyTorch h
-000018e0: 6173 2062 6565 6e20 7375 6363 6573 7366  as been successf
-000018f0: 756c 6c79 2069 6e73 7461 6c6c 6564 2066  ully installed f
-00001900: 6f6c 6c6f 7769 6e67 2074 6865 205b 6f66  ollowing the [of
-00001910: 6669 6369 616c 2067 7569 6465 5d28 6874  ficial guide](ht
-00001920: 7470 733a 2f2f 7079 746f 7263 682e 6f72  tps://pytorch.or
-00001930: 672f 6765 742d 7374 6172 7465 642f 6c6f  g/get-started/lo
-00001940: 6361 6c6c 792f 292e 0a20 2020 2020 2020  cally/)..       
-00001950: 200a 2020 2020 2020 2020 496e 7374 616c   .        Instal
-00001960: 6c20 4d4d 456e 6769 6e65 0a20 2020 2020  l MMEngine.     
-00001970: 2020 200a 2020 2020 2020 2020 6060 6062     .        ```b
-00001980: 6173 680a 2020 2020 2020 2020 7069 7020  ash.        pip 
-00001990: 696e 7374 616c 6c20 2d55 206f 7065 6e6d  install -U openm
-000019a0: 696d 0a20 2020 2020 2020 206d 696d 2069  im.        mim i
-000019b0: 6e73 7461 6c6c 206d 6d65 6e67 696e 650a  nstall mmengine.
-000019c0: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
-000019d0: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-000019e0: 6966 7920 7468 6520 696e 7374 616c 6c61  ify the installa
-000019f0: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
-00001a00: 2020 2020 2020 6060 6062 6173 680a 2020        ```bash.  
-00001a10: 2020 2020 2020 7079 7468 6f6e 202d 6320        python -c 
-00001a20: 2766 726f 6d20 6d6d 656e 6769 6e65 2e75  'from mmengine.u
-00001a30: 7469 6c73 2e64 6c5f 7574 696c 7320 696d  tils.dl_utils im
-00001a40: 706f 7274 2063 6f6c 6c65 6374 5f65 6e76  port collect_env
-00001a50: 3b70 7269 6e74 2863 6f6c 6c65 6374 5f65  ;print(collect_e
-00001a60: 6e76 2829 2927 0a20 2020 2020 2020 2060  nv())'.        `
-00001a70: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00001a80: 2020 2020 2323 2047 6574 2053 7461 7274      ## Get Start
-00001a90: 6564 0a20 2020 2020 2020 200a 2020 2020  ed.        .    
-00001aa0: 2020 2020 5461 6b69 6e67 2074 6865 2074      Taking the t
-00001ab0: 7261 696e 696e 6720 6f66 2061 2052 6573  raining of a Res
-00001ac0: 4e65 742d 3530 206d 6f64 656c 206f 6e20  Net-50 model on 
-00001ad0: 7468 6520 4349 4641 522d 3130 2064 6174  the CIFAR-10 dat
-00001ae0: 6173 6574 2061 7320 616e 2065 7861 6d70  aset as an examp
-00001af0: 6c65 2c20 7765 2077 696c 6c20 7573 6520  le, we will use 
-00001b00: 4d4d 456e 6769 6e65 2074 6f20 6275 696c  MMEngine to buil
-00001b10: 6420 6120 636f 6d70 6c65 7465 2c20 636f  d a complete, co
-00001b20: 6e66 6967 7572 6162 6c65 2074 7261 696e  nfigurable train
-00001b30: 696e 6720 616e 6420 7661 6c69 6461 7469  ing and validati
-00001b40: 6f6e 2070 726f 6365 7373 2069 6e20 6c65  on process in le
-00001b50: 7373 2074 6861 6e20 3830 206c 696e 6573  ss than 80 lines
-00001b60: 206f 6620 636f 6465 2e0a 2020 2020 2020   of code..      
-00001b70: 2020 0a20 2020 2020 2020 203c 6465 7461    .        <deta
-00001b80: 696c 733e 0a20 2020 2020 2020 203c 7375  ils>.        <su
-00001b90: 6d6d 6172 793e 4275 696c 6420 4d6f 6465  mmary>Build Mode
-00001ba0: 6c73 3c2f 7375 6d6d 6172 793e 0a20 2020  ls</summary>.   
-00001bb0: 2020 2020 200a 2020 2020 2020 2020 4669       .        Fi
-00001bc0: 7273 742c 2077 6520 6e65 6564 2074 6f20  rst, we need to 
-00001bd0: 6465 6669 6e65 2061 202a 2a6d 6f64 656c  define a **model
-00001be0: 2a2a 2077 6869 6368 2031 2920 696e 6865  ** which 1) inhe
-00001bf0: 7269 7473 2066 726f 6d20 6042 6173 654d  rits from `BaseM
-00001c00: 6f64 656c 6020 616e 6420 3229 2061 6363  odel` and 2) acc
-00001c10: 6570 7473 2061 6e20 6164 6469 7469 6f6e  epts an addition
-00001c20: 616c 2061 7267 756d 656e 7420 606d 6f64  al argument `mod
-00001c30: 6560 2069 6e20 7468 6520 6066 6f72 7761  e` in the `forwa
-00001c40: 7264 6020 6d65 7468 6f64 2c20 696e 2061  rd` method, in a
-00001c50: 6464 6974 696f 6e20 746f 2074 686f 7365  ddition to those
-00001c60: 2061 7267 756d 656e 7473 2072 656c 6174   arguments relat
-00001c70: 6564 2074 6f20 7468 6520 6461 7461 7365  ed to the datase
-00001c80: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-00001c90: 2020 2020 2d20 4475 7269 6e67 2074 7261      - During tra
-00001ca0: 696e 696e 672c 2074 6865 2076 616c 7565  ining, the value
-00001cb0: 206f 6620 606d 6f64 6560 2069 7320 226c   of `mode` is "l
-00001cc0: 6f73 7322 2c20 616e 6420 7468 6520 6066  oss", and the `f
-00001cd0: 6f72 7761 7264 6020 6d65 7468 6f64 2073  orward` method s
-00001ce0: 686f 756c 6420 7265 7475 726e 2061 2060  hould return a `
-00001cf0: 6469 6374 6020 636f 6e74 6169 6e69 6e67  dict` containing
-00001d00: 2074 6865 206b 6579 2022 6c6f 7373 222e   the key "loss".
-00001d10: 0a20 2020 2020 2020 202d 2044 7572 696e  .        - Durin
-00001d20: 6720 7661 6c69 6461 7469 6f6e 2c20 7468  g validation, th
-00001d30: 6520 7661 6c75 6520 6f66 2060 6d6f 6465  e value of `mode
-00001d40: 6020 6973 2022 7072 6564 6963 7422 2c20  ` is "predict", 
-00001d50: 616e 6420 7468 6520 666f 7277 6172 6420  and the forward 
-00001d60: 6d65 7468 6f64 2073 686f 756c 6420 7265  method should re
-00001d70: 7475 726e 2072 6573 756c 7473 2063 6f6e  turn results con
-00001d80: 7461 696e 696e 6720 626f 7468 2070 7265  taining both pre
-00001d90: 6469 6374 696f 6e73 2061 6e64 206c 6162  dictions and lab
-00001da0: 656c 732e 0a20 2020 2020 2020 200a 2020  els..        .  
-00001db0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00001dc0: 2020 2020 2020 2020 696d 706f 7274 2074          import t
-00001dd0: 6f72 6368 2e6e 6e2e 6675 6e63 7469 6f6e  orch.nn.function
-00001de0: 616c 2061 7320 460a 2020 2020 2020 2020  al as F.        
-00001df0: 696d 706f 7274 2074 6f72 6368 7669 7369  import torchvisi
-00001e00: 6f6e 0a20 2020 2020 2020 2066 726f 6d20  on.        from 
-00001e10: 6d6d 656e 6769 6e65 2e6d 6f64 656c 2069  mmengine.model i
-00001e20: 6d70 6f72 7420 4261 7365 4d6f 6465 6c0a  mport BaseModel.
-00001e30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001e40: 2063 6c61 7373 204d 4d52 6573 4e65 7435   class MMResNet5
-00001e50: 3028 4261 7365 4d6f 6465 6c29 3a0a 2020  0(BaseModel):.  
-00001e60: 2020 2020 2020 2020 2020 6465 6620 5f5f            def __
-00001e70: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-00001e80: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00001e90: 7065 7228 292e 5f5f 696e 6974 5f5f 2829  per().__init__()
-00001ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001eb0: 2073 656c 662e 7265 736e 6574 203d 2074   self.resnet = t
-00001ec0: 6f72 6368 7669 7369 6f6e 2e6d 6f64 656c  orchvision.model
-00001ed0: 732e 7265 736e 6574 3530 2829 0a20 2020  s.resnet50().   
-00001ee0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00001ef0: 2020 6465 6620 666f 7277 6172 6428 7365    def forward(se
-00001f00: 6c66 2c20 696d 6773 2c20 6c61 6265 6c73  lf, imgs, labels
-00001f10: 2c20 6d6f 6465 293a 0a20 2020 2020 2020  , mode):.       
-00001f20: 2020 2020 2020 2020 2078 203d 2073 656c           x = sel
-00001f30: 662e 7265 736e 6574 2869 6d67 7329 0a20  f.resnet(imgs). 
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001f50: 6620 6d6f 6465 203d 3d20 276c 6f73 7327  f mode == 'loss'
-00001f60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001f70: 2020 2020 2020 7265 7475 726e 207b 276c        return {'l
-00001f80: 6f73 7327 3a20 462e 6372 6f73 735f 656e  oss': F.cross_en
-00001f90: 7472 6f70 7928 782c 206c 6162 656c 7329  tropy(x, labels)
-00001fa0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00001fb0: 2020 656c 6966 206d 6f64 6520 3d3d 2027    elif mode == '
-00001fc0: 7072 6564 6963 7427 3a0a 2020 2020 2020  predict':.      
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001fe0: 7475 726e 2078 2c20 6c61 6265 6c73 0a20  turn x, labels. 
-00001ff0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00002000: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
-00002010: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
-00002020: 2020 2020 2020 2020 3c64 6574 6169 6c73          <details
-00002030: 3e0a 2020 2020 2020 2020 3c73 756d 6d61  >.        <summa
-00002040: 7279 3e42 7569 6c64 2044 6174 6173 6574  ry>Build Dataset
-00002050: 733c 2f73 756d 6d61 7279 3e0a 2020 2020  s</summary>.    
-00002060: 2020 2020 0a20 2020 2020 2020 204e 6578      .        Nex
-00002070: 742c 2077 6520 6e65 6564 2074 6f20 6372  t, we need to cr
-00002080: 6561 7465 202a 2a44 6174 6173 6574 2a2a  eate **Dataset**
-00002090: 7320 616e 6420 2a2a 4461 7461 4c6f 6164  s and **DataLoad
-000020a0: 6572 2a2a 7320 666f 7220 7472 6169 6e69  er**s for traini
-000020b0: 6e67 2061 6e64 2076 616c 6964 6174 696f  ng and validatio
-000020c0: 6e2e 0a20 2020 2020 2020 2049 6e20 7468  n..        In th
-000020d0: 6973 2063 6173 652c 2077 6520 7369 6d70  is case, we simp
-000020e0: 6c79 2075 7365 2062 7569 6c74 2d69 6e20  ly use built-in 
-000020f0: 6461 7461 7365 7473 2073 7570 706f 7274  datasets support
-00002100: 6564 2069 6e20 546f 7263 6856 6973 696f  ed in TorchVisio
-00002110: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00002120: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
-00002130: 2020 2020 2020 696d 706f 7274 2074 6f72        import tor
-00002140: 6368 7669 7369 6f6e 2e74 7261 6e73 666f  chvision.transfo
-00002150: 726d 7320 6173 2074 7261 6e73 666f 726d  rms as transform
-00002160: 730a 2020 2020 2020 2020 6672 6f6d 2074  s.        from t
-00002170: 6f72 6368 2e75 7469 6c73 2e64 6174 6120  orch.utils.data 
-00002180: 696d 706f 7274 2044 6174 614c 6f61 6465  import DataLoade
-00002190: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-000021a0: 2020 206e 6f72 6d5f 6366 6720 3d20 6469     norm_cfg = di
-000021b0: 6374 286d 6561 6e3d 5b30 2e34 3931 2c20  ct(mean=[0.491, 
-000021c0: 302e 3438 322c 2030 2e34 3437 5d2c 2073  0.482, 0.447], s
-000021d0: 7464 3d5b 302e 3230 322c 2030 2e31 3939  td=[0.202, 0.199
-000021e0: 2c20 302e 3230 315d 290a 2020 2020 2020  , 0.201]).      
-000021f0: 2020 7472 6169 6e5f 6461 7461 6c6f 6164    train_dataload
-00002200: 6572 203d 2044 6174 614c 6f61 6465 7228  er = DataLoader(
-00002210: 6261 7463 685f 7369 7a65 3d33 322c 0a20  batch_size=32,. 
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002240: 2020 2020 2073 6875 6666 6c65 3d54 7275       shuffle=Tru
-00002250: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
-00002280: 3d74 6f72 6368 7669 7369 6f6e 2e64 6174  =torchvision.dat
-00002290: 6173 6574 732e 4349 4641 5231 3028 0a20  asets.CIFAR10(. 
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2057 6861 7427 7320 4e65 770a 2020 2020   What's New.    
+000010c0: 2020 2020 0a20 2020 2020 2020 2076 302e      .        v0.
+000010d0: 382e 3020 7761 7320 7265 6c65 6173 6564  8.0 was released
+000010e0: 206f 6e20 3230 3233 2d30 362d 3330 2e0a   on 2023-06-30..
+000010f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001100: 2048 6967 686c 6967 6874 733a 0a20 2020   Highlights:.   
+00001110: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001120: 5375 7070 6f72 7420 7472 6169 6e69 6e67  Support training
+00001130: 2077 6974 6820 5b46 5344 505d 2868 7474   with [FSDP](htt
+00001140: 7073 3a2f 2f70 7974 6f72 6368 2e6f 7267  ps://pytorch.org
+00001150: 2f74 7574 6f72 6961 6c73 2f69 6e74 6572  /tutorials/inter
+00001160: 6d65 6469 6174 652f 4653 4450 5f61 6461  mediate/FSDP_ada
+00001170: 766e 6365 645f 7475 746f 7269 616c 2e68  vnced_tutorial.h
+00001180: 746d 6c3f 6869 6768 6c69 6768 743d 6673  tml?highlight=fs
+00001190: 6470 2920 616e 6420 5b44 6565 7053 7065  dp) and [DeepSpe
+000011a0: 6564 5d28 6874 7470 733a 2f2f 7777 772e  ed](https://www.
+000011b0: 6465 6570 7370 6565 642e 6169 2f29 2e20  deepspeed.ai/). 
+000011c0: 5265 6665 7220 746f 2074 6865 205b 6578  Refer to the [ex
+000011d0: 616d 706c 655d 2868 7474 7073 3a2f 2f67  ample](https://g
+000011e0: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+000011f0: 6d6c 6162 2f6d 6d65 6e67 696e 652f 626c  mlab/mmengine/bl
+00001200: 6f62 2f6d 6169 6e2f 6578 616d 706c 6573  ob/main/examples
+00001210: 2f64 6973 7472 6962 7574 6564 5f74 7261  /distributed_tra
+00001220: 696e 696e 675f 7769 7468 5f66 6c65 7869  ining_with_flexi
+00001230: 626c 655f 7275 6e6e 6572 2e70 7929 2066  ble_runner.py) f
+00001240: 6f72 206d 6f72 6520 6465 7461 696c 6564  or more detailed
+00001250: 2075 7361 6765 732e 0a20 2020 2020 2020   usages..       
+00001260: 200a 2020 2020 2020 2020 2d20 496e 7472   .        - Intr
+00001270: 6f64 7563 6520 7468 6520 7075 7265 2050  oduce the pure P
+00001280: 7974 686f 6e20 7374 796c 6520 636f 6e66  ython style conf
+00001290: 6967 7572 6174 696f 6e20 6669 6c65 3a0a  iguration file:.
+000012a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000012b0: 2020 202d 2053 7570 706f 7274 206e 6176     - Support nav
+000012c0: 6967 6174 696e 6720 746f 2062 6173 6520  igating to base 
+000012d0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+000012e0: 6c65 2069 6e20 4944 450a 2020 2020 2020  le in IDE.      
+000012f0: 2020 2020 2d20 5375 7070 6f72 7420 6e61      - Support na
+00001300: 7669 6761 7469 6e67 2074 6f20 6261 7365  vigating to base
+00001310: 2076 6172 6961 626c 6520 696e 2049 4445   variable in IDE
+00001320: 0a20 2020 2020 2020 2020 202d 2053 7570  .          - Sup
+00001330: 706f 7274 206e 6176 6967 6174 696e 6720  port navigating 
+00001340: 746f 2073 6f75 7263 6520 636f 6465 206f  to source code o
+00001350: 6620 636c 6173 7320 696e 2049 4445 0a20  f class in IDE. 
+00001360: 2020 2020 2020 2020 202d 2053 7570 706f           - Suppo
+00001370: 7274 2069 6e68 6572 6974 696e 6720 7477  rt inheriting tw
+00001380: 6f20 636f 6e66 6967 7572 6174 696f 6e20  o configuration 
+00001390: 6669 6c65 7320 636f 6e74 6169 6e69 6e67  files containing
+000013a0: 2074 6865 2073 616d 6520 6669 656c 640a   the same field.
+000013b0: 2020 2020 2020 2020 2020 2d20 4c6f 6164            - Load
+000013c0: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+000013d0: 6f6e 2066 696c 6520 7769 7468 6f75 7420  on file without 
+000013e0: 6f74 6865 7220 7468 6972 642d 7061 7274  other third-part
+000013f0: 7920 7265 7175 6972 656d 656e 7473 0a20  y requirements. 
+00001400: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001410: 2020 5265 6665 7220 746f 2074 6865 205b    Refer to the [
+00001420: 7475 746f 7269 616c 5d28 6874 7470 733a  tutorial](https:
+00001430: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+00001440: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001450: 6573 742f 6164 7661 6e63 6564 5f74 7574  est/advanced_tut
+00001460: 6f72 6961 6c73 2f63 6f6e 6669 672e 6874  orials/config.ht
+00001470: 6d6c 2361 2d70 7572 652d 7079 7468 6f6e  ml#a-pure-python
+00001480: 2d73 7479 6c65 2d63 6f6e 6669 6775 7261  -style-configura
+00001490: 7469 6f6e 2d66 696c 652d 6265 7461 2920  tion-file-beta) 
+000014a0: 666f 7220 6d6f 7265 2064 6574 6169 6c65  for more detaile
+000014b0: 6420 7573 6167 6573 2e0a 2020 2020 2020  d usages..      
+000014c0: 2020 0a20 2020 2020 2020 2020 2021 5b6e    .          ![n
+000014d0: 6577 2d63 6f6e 6669 672d 656e 5d28 6874  ew-config-en](ht
+000014e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000014f0: 2f6f 7065 6e2d 6d6d 6c61 622f 6d6d 656e  /open-mmlab/mmen
+00001500: 6769 6e65 2f61 7373 6574 732f 3537 3536  gine/assets/5756
+00001510: 3636 3330 2f37 6562 3431 3734 382d 3933  6630/7eb41748-93
+00001520: 3734 2d34 3838 662d 3930 3165 2d66 6364  74-488f-901e-fcd
+00001530: 3766 3064 3363 3861 3129 0a20 2020 2020  7f0d3c8a1).     
+00001540: 2020 200a 2020 2020 2020 2020 5265 6164     .        Read
+00001550: 205b 4368 616e 6765 6c6f 675d 282e 2f64   [Changelog](./d
+00001560: 6f63 732f 656e 2f6e 6f74 6573 2f63 6861  ocs/en/notes/cha
+00001570: 6e67 656c 6f67 2e6d 6423 7630 3830 2d30  ngelog.md#v080-0
+00001580: 3633 3032 3032 3329 2066 6f72 206d 6f72  6302023) for mor
+00001590: 6520 6465 7461 696c 732e 0a20 2020 2020  e details..     
+000015a0: 2020 200a 2020 2020 2020 2020 2323 2049     .        ## I
+000015b0: 6e74 726f 6475 6374 696f 6e0a 2020 2020  ntroduction.    
+000015c0: 2020 2020 0a20 2020 2020 2020 204d 4d45      .        MME
+000015d0: 6e67 696e 6520 6973 2061 2066 6f75 6e64  ngine is a found
+000015e0: 6174 696f 6e61 6c20 6c69 6272 6172 7920  ational library 
+000015f0: 666f 7220 7472 6169 6e69 6e67 2064 6565  for training dee
+00001600: 7020 6c65 6172 6e69 6e67 206d 6f64 656c  p learning model
+00001610: 7320 6261 7365 6420 6f6e 2050 7954 6f72  s based on PyTor
+00001620: 6368 2e20 4974 2070 726f 7669 6465 7320  ch. It provides 
+00001630: 6120 736f 6c69 6420 656e 6769 6e65 6572  a solid engineer
+00001640: 696e 6720 666f 756e 6461 7469 6f6e 2061  ing foundation a
+00001650: 6e64 2066 7265 6573 2064 6576 656c 6f70  nd frees develop
+00001660: 6572 7320 6672 6f6d 2077 7269 7469 6e67  ers from writing
+00001670: 2072 6564 756e 6461 6e74 2063 6f64 6573   redundant codes
+00001680: 206f 6e20 776f 726b 666c 6f77 732e 2049   on workflows. I
+00001690: 7420 7365 7276 6573 2061 7320 7468 6520  t serves as the 
+000016a0: 7472 6169 6e69 6e67 2065 6e67 696e 6520  training engine 
+000016b0: 6f66 2061 6c6c 204f 7065 6e4d 4d4c 6162  of all OpenMMLab
+000016c0: 2063 6f64 6562 6173 6573 2c20 7768 6963   codebases, whic
+000016d0: 6820 7375 7070 6f72 7420 6875 6e64 7265  h support hundre
+000016e0: 6473 206f 6620 616c 676f 7269 7468 6d73  ds of algorithms
+000016f0: 2069 6e20 7661 7269 6f75 7320 7265 7365   in various rese
+00001700: 6172 6368 2061 7265 6173 2e20 4d6f 7265  arch areas. More
+00001710: 6f76 6572 2c20 4d4d 456e 6769 6e65 2069  over, MMEngine i
+00001720: 7320 616c 736f 2067 656e 6572 6963 2074  s also generic t
+00001730: 6f20 6265 2061 7070 6c69 6564 2074 6f20  o be applied to 
+00001740: 6e6f 6e2d 4f70 656e 4d4d 4c61 6220 7072  non-OpenMMLab pr
+00001750: 6f6a 6563 7473 2e0a 2020 2020 2020 2020  ojects..        
+00001760: 0a20 2020 2020 2020 204d 616a 6f72 2066  .        Major f
+00001770: 6561 7475 7265 733a 0a20 2020 2020 2020  eatures:.       
+00001780: 200a 2020 2020 2020 2020 312e 202a 2a41   .        1. **A
+00001790: 2075 6e69 7665 7273 616c 2061 6e64 2070   universal and p
+000017a0: 6f77 6572 6675 6c20 7275 6e6e 6572 2a2a  owerful runner**
+000017b0: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+000017c0: 2020 2020 2020 2d20 5375 7070 6f72 7473        - Supports
+000017d0: 2074 7261 696e 696e 6720 6469 6666 6572   training differ
+000017e0: 656e 7420 7461 736b 7320 7769 7468 2061  ent tasks with a
+000017f0: 2073 6d61 6c6c 2061 6d6f 756e 7420 6f66   small amount of
+00001800: 2063 6f64 652c 2065 2e67 2e2c 2049 6d61   code, e.g., Ima
+00001810: 6765 4e65 7420 6361 6e20 6265 2074 7261  geNet can be tra
+00001820: 696e 6564 2077 6974 6820 6f6e 6c79 2038  ined with only 8
+00001830: 3020 6c69 6e65 7320 6f66 2063 6f64 6520  0 lines of code 
+00001840: 2834 3030 206c 696e 6573 206f 6620 7468  (400 lines of th
+00001850: 6520 6f72 6967 696e 616c 2050 7954 6f72  e original PyTor
+00001860: 6368 2065 7861 6d70 6c65 292e 0a20 2020  ch example)..   
+00001870: 2020 2020 2020 2020 2d20 4561 7369 6c79          - Easily
+00001880: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
+00001890: 206d 6f64 656c 7320 6672 6f6d 2070 6f70   models from pop
+000018a0: 756c 6172 2061 6c67 6f72 6974 686d 206c  ular algorithm l
+000018b0: 6962 7261 7269 6573 2073 7563 6820 6173  ibraries such as
+000018c0: 2054 494d 4d2c 2054 6f72 6368 5669 7369   TIMM, TorchVisi
+000018d0: 6f6e 2c20 616e 6420 4465 7465 6374 726f  on, and Detectro
+000018e0: 6e32 2e0a 2020 2020 2020 2020 0a20 2020  n2..        .   
+000018f0: 2020 2020 2032 2e20 2a2a 4f70 656e 2061       2. **Open a
+00001900: 7263 6869 7465 6374 7572 6520 7769 7468  rchitecture with
+00001910: 2075 6e69 6669 6564 2069 6e74 6572 6661   unified interfa
+00001920: 6365 732a 2a3a 0a20 2020 2020 2020 200a  ces**:.        .
+00001930: 2020 2020 2020 2020 2020 202d 2048 616e             - Han
+00001940: 646c 6573 2064 6966 6665 7265 6e74 2061  dles different a
+00001950: 6c67 6f72 6974 686d 2074 6173 6b73 2077  lgorithm tasks w
+00001960: 6974 6820 756e 6966 6965 6420 4150 4973  ith unified APIs
+00001970: 2c20 652e 672e 2c20 696d 706c 656d 656e  , e.g., implemen
+00001980: 7420 6120 6d65 7468 6f64 2061 6e64 2061  t a method and a
+00001990: 7070 6c79 2069 7420 746f 2061 6c6c 2063  pply it to all c
+000019a0: 6f6d 7061 7469 626c 6520 6d6f 6465 6c73  ompatible models
+000019b0: 2e0a 2020 2020 2020 2020 2020 202d 2050  ..           - P
+000019c0: 726f 7669 6465 7320 6120 756e 6966 6965  rovides a unifie
+000019d0: 6420 6162 7374 7261 6374 696f 6e20 666f  d abstraction fo
+000019e0: 7220 7570 7065 722d 6c65 7665 6c20 616c  r upper-level al
+000019f0: 676f 7269 7468 6d20 6c69 6272 6172 6965  gorithm librarie
+00001a00: 732c 2077 6869 6368 2073 7570 706f 7274  s, which support
+00001a10: 7320 7661 7269 6f75 7320 6261 636b 2d65  s various back-e
+00001a20: 6e64 2064 6576 6963 6573 2073 7563 6820  nd devices such 
+00001a30: 6173 204e 7669 6469 6120 4355 4441 2c20  as Nvidia CUDA, 
+00001a40: 4d61 6320 4d50 532c 2041 4d44 2c20 4d4c  Mac MPS, AMD, ML
+00001a50: 552c 2061 6e64 206d 6f72 6520 666f 7220  U, and more for 
+00001a60: 6d6f 6465 6c20 7472 6169 6e69 6e67 2e0a  model training..
+00001a70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001a80: 2033 2e20 2a2a 4375 7374 6f6d 697a 6162   3. **Customizab
+00001a90: 6c65 2074 7261 696e 696e 6720 7072 6f63  le training proc
+00001aa0: 6573 732a 2a3a 0a20 2020 2020 2020 200a  ess**:.        .
+00001ab0: 2020 2020 2020 2020 2020 202d 2044 6566             - Def
+00001ac0: 696e 6573 2074 6865 2074 7261 696e 696e  ines the trainin
+00001ad0: 6720 7072 6f63 6573 7320 6a75 7374 206c  g process just l
+00001ae0: 696b 6520 706c 6179 696e 6720 7769 7468  ike playing with
+00001af0: 204c 6567 6f73 2e0a 2020 2020 2020 2020   Legos..        
+00001b00: 2020 202d 2050 726f 7669 6465 7320 7269     - Provides ri
+00001b10: 6368 2063 6f6d 706f 6e65 6e74 7320 616e  ch components an
+00001b20: 6420 7374 7261 7465 6769 6573 2e0a 2020  d strategies..  
+00001b30: 2020 2020 2020 2020 202d 2043 6f6d 706c           - Compl
+00001b40: 6574 6520 636f 6e74 726f 6c73 206f 6e20  ete controls on 
+00001b50: 7468 6520 7472 6169 6e69 6e67 2070 726f  the training pro
+00001b60: 6365 7373 2077 6974 6820 6469 6666 6572  cess with differ
+00001b70: 656e 7420 6c65 7665 6c73 206f 6620 4150  ent levels of AP
+00001b80: 4973 2e0a 2020 2020 2020 2020 0a20 2020  Is..        .   
+00001b90: 2020 2020 2023 2320 496e 7374 616c 6c61       ## Installa
+00001ba0: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
+00001bb0: 2020 2020 2020 4265 666f 7265 2069 6e73        Before ins
+00001bc0: 7461 6c6c 696e 6720 4d4d 456e 6769 6e65  talling MMEngine
+00001bd0: 2c20 706c 6561 7365 2065 6e73 7572 6520  , please ensure 
+00001be0: 7468 6174 2050 7954 6f72 6368 2068 6173  that PyTorch has
+00001bf0: 2062 6565 6e20 7375 6363 6573 7366 756c   been successful
+00001c00: 6c79 2069 6e73 7461 6c6c 6564 2066 6f6c  ly installed fol
+00001c10: 6c6f 7769 6e67 2074 6865 205b 6f66 6669  lowing the [offi
+00001c20: 6369 616c 2067 7569 6465 5d28 6874 7470  cial guide](http
+00001c30: 733a 2f2f 7079 746f 7263 682e 6f72 672f  s://pytorch.org/
+00001c40: 6765 742d 7374 6172 7465 642f 6c6f 6361  get-started/loca
+00001c50: 6c6c 792f 292e 0a20 2020 2020 2020 200a  lly/)..        .
+00001c60: 2020 2020 2020 2020 496e 7374 616c 6c20          Install 
+00001c70: 4d4d 456e 6769 6e65 0a20 2020 2020 2020  MMEngine.       
+00001c80: 200a 2020 2020 2020 2020 6060 6062 6173   .        ```bas
+00001c90: 680a 2020 2020 2020 2020 7069 7020 696e  h.        pip in
+00001ca0: 7374 616c 6c20 2d55 206f 7065 6e6d 696d  stall -U openmim
+00001cb0: 0a20 2020 2020 2020 206d 696d 2069 6e73  .        mim ins
+00001cc0: 7461 6c6c 206d 6d65 6e67 696e 650a 2020  tall mmengine.  
+00001cd0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001ce0: 2020 0a20 2020 2020 2020 2056 6572 6966    .        Verif
+00001cf0: 7920 7468 6520 696e 7374 616c 6c61 7469  y the installati
+00001d00: 6f6e 0a20 2020 2020 2020 200a 2020 2020  on.        .    
+00001d10: 2020 2020 6060 6062 6173 680a 2020 2020      ```bash.    
+00001d20: 2020 2020 7079 7468 6f6e 202d 6320 2766      python -c 'f
+00001d30: 726f 6d20 6d6d 656e 6769 6e65 2e75 7469  rom mmengine.uti
+00001d40: 6c73 2e64 6c5f 7574 696c 7320 696d 706f  ls.dl_utils impo
+00001d50: 7274 2063 6f6c 6c65 6374 5f65 6e76 3b70  rt collect_env;p
+00001d60: 7269 6e74 2863 6f6c 6c65 6374 5f65 6e76  rint(collect_env
+00001d70: 2829 2927 0a20 2020 2020 2020 2060 6060  ())'.        ```
+00001d80: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001d90: 2020 2323 2047 6574 2053 7461 7274 6564    ## Get Started
+00001da0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001db0: 2020 5461 6b69 6e67 2074 6865 2074 7261    Taking the tra
+00001dc0: 696e 696e 6720 6f66 2061 2052 6573 4e65  ining of a ResNe
+00001dd0: 742d 3530 206d 6f64 656c 206f 6e20 7468  t-50 model on th
+00001de0: 6520 4349 4641 522d 3130 2064 6174 6173  e CIFAR-10 datas
+00001df0: 6574 2061 7320 616e 2065 7861 6d70 6c65  et as an example
+00001e00: 2c20 7765 2077 696c 6c20 7573 6520 4d4d  , we will use MM
+00001e10: 456e 6769 6e65 2074 6f20 6275 696c 6420  Engine to build 
+00001e20: 6120 636f 6d70 6c65 7465 2c20 636f 6e66  a complete, conf
+00001e30: 6967 7572 6162 6c65 2074 7261 696e 696e  igurable trainin
+00001e40: 6720 616e 6420 7661 6c69 6461 7469 6f6e  g and validation
+00001e50: 2070 726f 6365 7373 2069 6e20 6c65 7373   process in less
+00001e60: 2074 6861 6e20 3830 206c 696e 6573 206f   than 80 lines o
+00001e70: 6620 636f 6465 2e0a 2020 2020 2020 2020  f code..        
+00001e80: 0a20 2020 2020 2020 203c 6465 7461 696c  .        <detail
+00001e90: 733e 0a20 2020 2020 2020 203c 7375 6d6d  s>.        <summ
+00001ea0: 6172 793e 4275 696c 6420 4d6f 6465 6c73  ary>Build Models
+00001eb0: 3c2f 7375 6d6d 6172 793e 0a20 2020 2020  </summary>.     
+00001ec0: 2020 200a 2020 2020 2020 2020 4669 7273     .        Firs
+00001ed0: 742c 2077 6520 6e65 6564 2074 6f20 6465  t, we need to de
+00001ee0: 6669 6e65 2061 202a 2a6d 6f64 656c 2a2a  fine a **model**
+00001ef0: 2077 6869 6368 2031 2920 696e 6865 7269   which 1) inheri
+00001f00: 7473 2066 726f 6d20 6042 6173 654d 6f64  ts from `BaseMod
+00001f10: 656c 6020 616e 6420 3229 2061 6363 6570  el` and 2) accep
+00001f20: 7473 2061 6e20 6164 6469 7469 6f6e 616c  ts an additional
+00001f30: 2061 7267 756d 656e 7420 606d 6f64 6560   argument `mode`
+00001f40: 2069 6e20 7468 6520 6066 6f72 7761 7264   in the `forward
+00001f50: 6020 6d65 7468 6f64 2c20 696e 2061 6464  ` method, in add
+00001f60: 6974 696f 6e20 746f 2074 686f 7365 2061  ition to those a
+00001f70: 7267 756d 656e 7473 2072 656c 6174 6564  rguments related
+00001f80: 2074 6f20 7468 6520 6461 7461 7365 742e   to the dataset.
+00001f90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001fa0: 2020 2d20 4475 7269 6e67 2074 7261 696e    - During train
+00001fb0: 696e 672c 2074 6865 2076 616c 7565 206f  ing, the value o
+00001fc0: 6620 606d 6f64 6560 2069 7320 226c 6f73  f `mode` is "los
+00001fd0: 7322 2c20 616e 6420 7468 6520 6066 6f72  s", and the `for
+00001fe0: 7761 7264 6020 6d65 7468 6f64 2073 686f  ward` method sho
+00001ff0: 756c 6420 7265 7475 726e 2061 2060 6469  uld return a `di
+00002000: 6374 6020 636f 6e74 6169 6e69 6e67 2074  ct` containing t
+00002010: 6865 206b 6579 2022 6c6f 7373 222e 0a20  he key "loss".. 
+00002020: 2020 2020 2020 202d 2044 7572 696e 6720         - During 
+00002030: 7661 6c69 6461 7469 6f6e 2c20 7468 6520  validation, the 
+00002040: 7661 6c75 6520 6f66 2060 6d6f 6465 6020  value of `mode` 
+00002050: 6973 2022 7072 6564 6963 7422 2c20 616e  is "predict", an
+00002060: 6420 7468 6520 666f 7277 6172 6420 6d65  d the forward me
+00002070: 7468 6f64 2073 686f 756c 6420 7265 7475  thod should retu
+00002080: 726e 2072 6573 756c 7473 2063 6f6e 7461  rn results conta
+00002090: 696e 696e 6720 626f 7468 2070 7265 6469  ining both predi
+000020a0: 6374 696f 6e73 2061 6e64 206c 6162 656c  ctions and label
+000020b0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+000020c0: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
+000020d0: 2020 2020 2020 696d 706f 7274 2074 6f72        import tor
+000020e0: 6368 2e6e 6e2e 6675 6e63 7469 6f6e 616c  ch.nn.functional
+000020f0: 2061 7320 460a 2020 2020 2020 2020 696d   as F.        im
+00002100: 706f 7274 2074 6f72 6368 7669 7369 6f6e  port torchvision
+00002110: 0a20 2020 2020 2020 2066 726f 6d20 6d6d  .        from mm
+00002120: 656e 6769 6e65 2e6d 6f64 656c 2069 6d70  engine.model imp
+00002130: 6f72 7420 4261 7365 4d6f 6465 6c0a 2020  ort BaseModel.  
+00002140: 2020 2020 2020 0a20 2020 2020 2020 2063        .        c
+00002150: 6c61 7373 204d 4d52 6573 4e65 7435 3028  lass MMResNet50(
+00002160: 4261 7365 4d6f 6465 6c29 3a0a 2020 2020  BaseModel):.    
+00002170: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
+00002180: 6974 5f5f 2873 656c 6629 3a0a 2020 2020  it__(self):.    
+00002190: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+000021a0: 7228 292e 5f5f 696e 6974 5f5f 2829 0a20  r().__init__(). 
+000021b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000021c0: 656c 662e 7265 736e 6574 203d 2074 6f72  elf.resnet = tor
+000021d0: 6368 7669 7369 6f6e 2e6d 6f64 656c 732e  chvision.models.
+000021e0: 7265 736e 6574 3530 2829 0a20 2020 2020  resnet50().     
+000021f0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+00002200: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
+00002210: 2c20 696d 6773 2c20 6c61 6265 6c73 2c20  , imgs, labels, 
+00002220: 6d6f 6465 293a 0a20 2020 2020 2020 2020  mode):.         
+00002230: 2020 2020 2020 2078 203d 2073 656c 662e         x = self.
+00002240: 7265 736e 6574 2869 6d67 7329 0a20 2020  resnet(imgs).   
+00002250: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002260: 6d6f 6465 203d 3d20 276c 6f73 7327 3a0a  mode == 'loss':.
+00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002280: 2020 2020 7265 7475 726e 207b 276c 6f73      return {'los
+00002290: 7327 3a20 462e 6372 6f73 735f 656e 7472  s': F.cross_entr
+000022a0: 6f70 7928 782c 206c 6162 656c 7329 7d0a  opy(x, labels)}.
 000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2020 2020 2020 2027 6461 7461 2f63           'data/c
-000022d0: 6966 6172 3130 272c 0a20 2020 2020 2020  ifar10',.       
-000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2074 7261 696e 3d54 7275 652c 0a20     train=True,. 
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 2020 2020 2020 2064 6f77 6e6c 6f61           downloa
-00002340: 643d 5472 7565 2c0a 2020 2020 2020 2020  d=True,.        
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 7472 616e 7366 6f72 6d3d 7472 616e    transform=tran
-00002380: 7366 6f72 6d73 2e43 6f6d 706f 7365 285b  sforms.Compose([
-00002390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000023c0: 7261 6e73 666f 726d 732e 5261 6e64 6f6d  ransforms.Random
-000023d0: 4372 6f70 2833 322c 2070 6164 6469 6e67  Crop(32, padding
-000023e0: 3d34 292c 0a20 2020 2020 2020 2020 2020  =4),.           
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2074 7261 6e73 666f 726d 732e 5261     transforms.Ra
-00002420: 6e64 6f6d 486f 7269 7a6f 6e74 616c 466c  ndomHorizontalFl
-00002430: 6970 2829 2c0a 2020 2020 2020 2020 2020  ip(),.          
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 2020 2020 7472 616e 7366 6f72 6d73 2e54      transforms.T
-00002470: 6f54 656e 736f 7228 292c 0a20 2020 2020  oTensor(),.     
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-000024b0: 726d 732e 4e6f 726d 616c 697a 6528 2a2a  rms.Normalize(**
-000024c0: 6e6f 726d 5f63 6667 290a 2020 2020 2020  norm_cfg).      
-000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: 2020 2020 5d29 2929 0a20 2020 2020 2020      ]))).       
-00002500: 2076 616c 5f64 6174 616c 6f61 6465 7220   val_dataloader 
-00002510: 3d20 4461 7461 4c6f 6164 6572 2862 6174  = DataLoader(bat
-00002520: 6368 5f73 697a 653d 3332 2c0a 2020 2020  ch_size=32,.    
+000022c0: 656c 6966 206d 6f64 6520 3d3d 2027 7072  elif mode == 'pr
+000022d0: 6564 6963 7427 3a0a 2020 2020 2020 2020  edict':.        
+000022e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000022f0: 726e 2078 2c20 6c61 6265 6c73 0a20 2020  rn x, labels.   
+00002300: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+00002310: 200a 2020 2020 2020 2020 3c2f 6465 7461   .        </deta
+00002320: 696c 733e 0a20 2020 2020 2020 200a 2020  ils>.        .  
+00002330: 2020 2020 2020 3c64 6574 6169 6c73 3e0a        <details>.
+00002340: 2020 2020 2020 2020 3c73 756d 6d61 7279          <summary
+00002350: 3e42 7569 6c64 2044 6174 6173 6574 733c  >Build Datasets<
+00002360: 2f73 756d 6d61 7279 3e0a 2020 2020 2020  /summary>.      
+00002370: 2020 0a20 2020 2020 2020 204e 6578 742c    .        Next,
+00002380: 2077 6520 6e65 6564 2074 6f20 6372 6561   we need to crea
+00002390: 7465 202a 2a44 6174 6173 6574 2a2a 7320  te **Dataset**s 
+000023a0: 616e 6420 2a2a 4461 7461 4c6f 6164 6572  and **DataLoader
+000023b0: 2a2a 7320 666f 7220 7472 6169 6e69 6e67  **s for training
+000023c0: 2061 6e64 2076 616c 6964 6174 696f 6e2e   and validation.
+000023d0: 0a20 2020 2020 2020 2049 6e20 7468 6973  .        In this
+000023e0: 2063 6173 652c 2077 6520 7369 6d70 6c79   case, we simply
+000023f0: 2075 7365 2062 7569 6c74 2d69 6e20 6461   use built-in da
+00002400: 7461 7365 7473 2073 7570 706f 7274 6564  tasets supported
+00002410: 2069 6e20 546f 7263 6856 6973 696f 6e2e   in TorchVision.
+00002420: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002430: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+00002440: 2020 2020 696d 706f 7274 2074 6f72 6368      import torch
+00002450: 7669 7369 6f6e 2e74 7261 6e73 666f 726d  vision.transform
+00002460: 7320 6173 2074 7261 6e73 666f 726d 730a  s as transforms.
+00002470: 2020 2020 2020 2020 6672 6f6d 2074 6f72          from tor
+00002480: 6368 2e75 7469 6c73 2e64 6174 6120 696d  ch.utils.data im
+00002490: 706f 7274 2044 6174 614c 6f61 6465 720a  port DataLoader.
+000024a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000024b0: 206e 6f72 6d5f 6366 6720 3d20 6469 6374   norm_cfg = dict
+000024c0: 286d 6561 6e3d 5b30 2e34 3931 2c20 302e  (mean=[0.491, 0.
+000024d0: 3438 322c 2030 2e34 3437 5d2c 2073 7464  482, 0.447], std
+000024e0: 3d5b 302e 3230 322c 2030 2e31 3939 2c20  =[0.202, 0.199, 
+000024f0: 302e 3230 315d 290a 2020 2020 2020 2020  0.201]).        
+00002500: 7472 6169 6e5f 6461 7461 6c6f 6164 6572  train_dataloader
+00002510: 203d 2044 6174 614c 6f61 6465 7228 6261   = DataLoader(ba
+00002520: 7463 685f 7369 7a65 3d33 322c 0a20 2020  tch_size=32,.   
 00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 7368 7566 666c 653d 4661 6c73 652c 0a20  shuffle=False,. 
-00002560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 2020 2073 6875 6666 6c65 3d54 7275 652c     shuffle=True,
+00002560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002580: 2020 2064 6174 6173 6574 3d74 6f72 6368     dataset=torch
-00002590: 7669 7369 6f6e 2e64 6174 6173 6574 732e  vision.datasets.
-000025a0: 4349 4641 5231 3028 0a20 2020 2020 2020  CIFAR10(.       
+00002580: 2020 2020 2020 2064 6174 6173 6574 3d74         dataset=t
+00002590: 6f72 6368 7669 7369 6f6e 2e64 6174 6173  orchvision.datas
+000025a0: 6574 732e 4349 4641 5231 3028 0a20 2020  ets.CIFAR10(.   
 000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2027 6461 7461 2f63 6966 6172 3130 272c   'data/cifar10',
-000025e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000025d0: 2020 2020 2020 2027 6461 7461 2f63 6966         'data/cif
+000025e0: 6172 3130 272c 0a20 2020 2020 2020 2020  ar10',.         
 000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 2020 2020 2020 2074 7261 696e 3d46           train=F
-00002610: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2074 7261 696e 3d54 7275 652c 0a20 2020   train=True,.   
 00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2020 2020 2020 646f                do
-00002640: 776e 6c6f 6164 3d54 7275 652c 0a20 2020  wnload=True,.   
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 2064 6f77 6e6c 6f61 643d         download=
+00002650: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
 00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 2020 2074 7261 6e73 666f 726d 3d74       transform=t
-00002680: 7261 6e73 666f 726d 732e 436f 6d70 6f73  ransforms.Compos
-00002690: 6528 5b0a 2020 2020 2020 2020 2020 2020  e([.            
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 7472 616e 7366 6f72 6d3d 7472 616e 7366  transform=transf
+00002690: 6f72 6d73 2e43 6f6d 706f 7365 285b 0a20  orms.Compose([. 
 000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 7472 616e 7366 6f72 6d73 2e54 6f54 656e  transforms.ToTen
-000026d0: 736f 7228 292c 0a20 2020 2020 2020 2020  sor(),.         
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 2074 7261 6e73 666f 726d 732e 4e6f     transforms.No
-00002710: 726d 616c 697a 6528 2a2a 6e6f 726d 5f63  rmalize(**norm_c
-00002720: 6667 290a 2020 2020 2020 2020 2020 2020  fg).            
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2020 2020 2020 2020 2020 2020 5d29 2929              ])))
-00002750: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00002760: 2020 2020 200a 2020 2020 2020 2020 3c2f       .        </
-00002770: 6465 7461 696c 733e 0a20 2020 2020 2020  details>.       
-00002780: 200a 2020 2020 2020 2020 3c64 6574 6169   .        <detai
-00002790: 6c73 3e0a 2020 2020 2020 2020 3c73 756d  ls>.        <sum
-000027a0: 6d61 7279 3e42 7569 6c64 204d 6574 7269  mary>Build Metri
-000027b0: 6373 3c2f 7375 6d6d 6172 793e 0a20 2020  cs</summary>.   
-000027c0: 2020 2020 200a 2020 2020 2020 2020 546f       .        To
-000027d0: 2076 616c 6964 6174 6520 616e 6420 7465   validate and te
-000027e0: 7374 2074 6865 206d 6f64 656c 2c20 7765  st the model, we
-000027f0: 206e 6565 6420 746f 2064 6566 696e 6520   need to define 
-00002800: 6120 2a2a 4d65 7472 6963 2a2a 2063 616c  a **Metric** cal
-00002810: 6c65 6420 6163 6375 7261 6379 2074 6f20  led accuracy to 
-00002820: 6576 616c 7561 7465 2074 6865 206d 6f64  evaluate the mod
-00002830: 656c 2e20 5468 6973 206d 6574 7269 6320  el. This metric 
-00002840: 6e65 6564 7320 746f 2069 6e68 6572 6974  needs to inherit
-00002850: 2066 726f 6d20 6042 6173 654d 6574 7269   from `BaseMetri
-00002860: 6360 2061 6e64 2069 6d70 6c65 6d65 6e74  c` and implement
-00002870: 7320 7468 6520 6070 726f 6365 7373 6020  s the `process` 
-00002880: 616e 6420 6063 6f6d 7075 7465 5f6d 6574  and `compute_met
-00002890: 7269 6373 6020 6d65 7468 6f64 732e 0a20  rics` methods.. 
-000028a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000028b0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-000028c0: 2020 6672 6f6d 206d 6d65 6e67 696e 652e    from mmengine.
-000028d0: 6576 616c 7561 746f 7220 696d 706f 7274  evaluator import
-000028e0: 2042 6173 654d 6574 7269 630a 2020 2020   BaseMetric.    
-000028f0: 2020 2020 0a20 2020 2020 2020 2063 6c61      .        cla
-00002900: 7373 2041 6363 7572 6163 7928 4261 7365  ss Accuracy(Base
-00002910: 4d65 7472 6963 293a 0a20 2020 2020 2020  Metric):.       
-00002920: 2020 2020 2064 6566 2070 726f 6365 7373       def process
-00002930: 2873 656c 662c 2064 6174 615f 6261 7463  (self, data_batc
-00002940: 682c 2064 6174 615f 7361 6d70 6c65 7329  h, data_samples)
-00002950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002960: 2020 7363 6f72 652c 2067 7420 3d20 6461    score, gt = da
-00002970: 7461 5f73 616d 706c 6573 0a20 2020 2020  ta_samples.     
-00002980: 2020 2020 2020 2020 2020 2023 2053 6176             # Sav
-00002990: 6520 7468 6520 7265 7375 6c74 7320 6f66  e the results of
-000029a0: 2061 2062 6174 6368 2074 6f20 6073 656c   a batch to `sel
-000029b0: 662e 7265 7375 6c74 7360 0a20 2020 2020  f.results`.     
-000029c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000029d0: 7265 7375 6c74 732e 6170 7065 6e64 287b  results.append({
-000029e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029f0: 2020 2020 2027 6261 7463 685f 7369 7a65       'batch_size
-00002a00: 273a 206c 656e 2867 7429 2c0a 2020 2020  ': len(gt),.    
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2763 6f72 7265 6374 273a 2028 7363 6f72  'correct': (scor
-00002a30: 652e 6172 676d 6178 2864 696d 3d31 2920  e.argmax(dim=1) 
-00002a40: 3d3d 2067 7429 2e73 756d 2829 2e63 7075  == gt).sum().cpu
-00002a50: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00002a60: 2020 2020 7d29 0a20 2020 2020 2020 2020      }).         
-00002a70: 2020 2064 6566 2063 6f6d 7075 7465 5f6d     def compute_m
-00002a80: 6574 7269 6373 2873 656c 662c 2072 6573  etrics(self, res
-00002a90: 756c 7473 293a 0a20 2020 2020 2020 2020  ults):.         
-00002aa0: 2020 2020 2020 2074 6f74 616c 5f63 6f72         total_cor
-00002ab0: 7265 6374 203d 2073 756d 2869 7465 6d5b  rect = sum(item[
-00002ac0: 2763 6f72 7265 6374 275d 2066 6f72 2069  'correct'] for i
-00002ad0: 7465 6d20 696e 2072 6573 756c 7473 290a  tem in results).
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 746f 7461 6c5f 7369 7a65 203d 2073 756d  total_size = sum
-00002b00: 2869 7465 6d5b 2762 6174 6368 5f73 697a  (item['batch_siz
-00002b10: 6527 5d20 666f 7220 6974 656d 2069 6e20  e'] for item in 
-00002b20: 7265 7375 6c74 7329 0a20 2020 2020 2020  results).       
-00002b30: 2020 2020 2020 2020 2023 2052 6574 7572           # Retur
-00002b40: 6e73 2061 2064 6963 7469 6f6e 6172 7920  ns a dictionary 
-00002b50: 7769 7468 2074 6865 2072 6573 756c 7473  with the results
-00002b60: 206f 6620 7468 6520 6576 616c 7561 7465   of the evaluate
-00002b70: 6420 6d65 7472 6963 732c 0a20 2020 2020  d metrics,.     
-00002b80: 2020 2020 2020 2020 2020 2023 2077 6865             # whe
-00002b90: 7265 2074 6865 206b 6579 2069 7320 7468  re the key is th
-00002ba0: 6520 6e61 6d65 206f 6620 7468 6520 6d65  e name of the me
-00002bb0: 7472 6963 0a20 2020 2020 2020 2020 2020  tric.           
-00002bc0: 2020 2020 2072 6574 7572 6e20 6469 6374       return dict
-00002bd0: 2861 6363 7572 6163 793d 3130 3020 2a20  (accuracy=100 * 
-00002be0: 746f 7461 6c5f 636f 7272 6563 7420 2f20  total_correct / 
-00002bf0: 746f 7461 6c5f 7369 7a65 290a 2020 2020  total_size).    
-00002c00: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00002c10: 0a20 2020 2020 2020 203c 2f64 6574 6169  .        </detai
-00002c20: 6c73 3e0a 2020 2020 2020 2020 0a20 2020  ls>.        .   
-00002c30: 2020 2020 203c 6465 7461 696c 733e 0a20       <details>. 
-00002c40: 2020 2020 2020 203c 7375 6d6d 6172 793e         <summary>
-00002c50: 4275 696c 6420 6120 5275 6e6e 6572 3c2f  Build a Runner</
-00002c60: 7375 6d6d 6172 793e 0a20 2020 2020 2020  summary>.       
-00002c70: 200a 2020 2020 2020 2020 4669 6e61 6c6c   .        Finall
-00002c80: 792c 2077 6520 6361 6e20 636f 6e73 7472  y, we can constr
-00002c90: 7563 7420 6120 2a2a 5275 6e6e 6572 2a2a  uct a **Runner**
-00002ca0: 2077 6974 6820 7072 6576 696f 7573 6c79   with previously
-00002cb0: 2064 6566 696e 6564 2060 4d6f 6465 6c60   defined `Model`
-00002cc0: 2c20 6044 6174 614c 6f61 6465 7260 2c20  , `DataLoader`, 
-00002cd0: 616e 6420 604d 6574 7269 6373 602c 2077  and `Metrics`, w
-00002ce0: 6974 6820 736f 6d65 206f 7468 6572 2063  ith some other c
-00002cf0: 6f6e 6669 6773 2c20 6173 2073 686f 776e  onfigs, as shown
-00002d00: 2062 656c 6f77 2e0a 2020 2020 2020 2020   below..        
-00002d10: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
-00002d20: 6f6e 0a20 2020 2020 2020 2066 726f 6d20  on.        from 
-00002d30: 746f 7263 682e 6f70 7469 6d20 696d 706f  torch.optim impo
-00002d40: 7274 2053 4744 0a20 2020 2020 2020 2066  rt SGD.        f
-00002d50: 726f 6d20 6d6d 656e 6769 6e65 2e72 756e  rom mmengine.run
-00002d60: 6e65 7220 696d 706f 7274 2052 756e 6e65  ner import Runne
-00002d70: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-00002d80: 2020 2072 756e 6e65 7220 3d20 5275 6e6e     runner = Runn
-00002d90: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00002da0: 6d6f 6465 6c3d 4d4d 5265 734e 6574 3530  model=MMResNet50
-00002db0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00002dc0: 776f 726b 5f64 6972 3d27 2e2f 776f 726b  work_dir='./work
-00002dd0: 5f64 6972 272c 0a20 2020 2020 2020 2020  _dir',.         
-00002de0: 2020 2074 7261 696e 5f64 6174 616c 6f61     train_dataloa
-00002df0: 6465 723d 7472 6169 6e5f 6461 7461 6c6f  der=train_datalo
-00002e00: 6164 6572 2c0a 2020 2020 2020 2020 2020  ader,.          
-00002e10: 2020 2320 6120 7772 6170 7065 7220 746f    # a wrapper to
-00002e20: 2065 7865 6375 7465 2062 6163 6b20 7072   execute back pr
-00002e30: 6f70 6167 6174 696f 6e20 616e 6420 6772  opagation and gr
-00002e40: 6164 6965 6e74 2075 7064 6174 652c 2065  adient update, e
-00002e50: 7463 2e0a 2020 2020 2020 2020 2020 2020  tc..            
-00002e60: 6f70 7469 6d5f 7772 6170 7065 723d 6469  optim_wrapper=di
-00002e70: 6374 286f 7074 696d 697a 6572 3d64 6963  ct(optimizer=dic
-00002e80: 7428 7479 7065 3d53 4744 2c20 6c72 3d30  t(type=SGD, lr=0
-00002e90: 2e30 3031 2c20 6d6f 6d65 6e74 756d 3d30  .001, momentum=0
-00002ea0: 2e39 2929 2c0a 2020 2020 2020 2020 2020  .9)),.          
-00002eb0: 2020 2320 7365 7420 736f 6d65 2074 7261    # set some tra
-00002ec0: 696e 696e 6720 636f 6e66 6967 7320 6c69  ining configs li
-00002ed0: 6b65 2065 706f 6368 730a 2020 2020 2020  ke epochs.      
-00002ee0: 2020 2020 2020 7472 6169 6e5f 6366 673d        train_cfg=
-00002ef0: 6469 6374 2862 795f 6570 6f63 683d 5472  dict(by_epoch=Tr
-00002f00: 7565 2c20 6d61 785f 6570 6f63 6873 3d35  ue, max_epochs=5
-00002f10: 2c20 7661 6c5f 696e 7465 7276 616c 3d31  , val_interval=1
-00002f20: 292c 0a20 2020 2020 2020 2020 2020 2076  ),.            v
-00002f30: 616c 5f64 6174 616c 6f61 6465 723d 7661  al_dataloader=va
-00002f40: 6c5f 6461 7461 6c6f 6164 6572 2c0a 2020  l_dataloader,.  
-00002f50: 2020 2020 2020 2020 2020 7661 6c5f 6366            val_cf
-00002f60: 673d 6469 6374 2829 2c0a 2020 2020 2020  g=dict(),.      
-00002f70: 2020 2020 2020 7661 6c5f 6576 616c 7561        val_evalua
-00002f80: 746f 723d 6469 6374 2874 7970 653d 4163  tor=dict(type=Ac
-00002f90: 6375 7261 6379 292c 0a20 2020 2020 2020  curacy),.       
-00002fa0: 2029 0a20 2020 2020 2020 2060 6060 0a20   ).        ```. 
-00002fb0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002fc0: 3c2f 6465 7461 696c 733e 0a20 2020 2020  </details>.     
-00002fd0: 2020 200a 2020 2020 2020 2020 3c64 6574     .        <det
-00002fe0: 6169 6c73 3e0a 2020 2020 2020 2020 3c73  ails>.        <s
-00002ff0: 756d 6d61 7279 3e4c 6175 6e63 6820 5472  ummary>Launch Tr
-00003000: 6169 6e69 6e67 3c2f 7375 6d6d 6172 793e  aining</summary>
-00003010: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003020: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00003030: 2020 2020 7275 6e6e 6572 2e74 7261 696e      runner.train
-00003040: 2829 0a20 2020 2020 2020 2060 6060 0a20  ().        ```. 
-00003050: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003060: 3c2f 6465 7461 696c 733e 0a20 2020 2020  </details>.     
-00003070: 2020 200a 2020 2020 2020 2020 2323 204c     .        ## L
-00003080: 6561 726e 204d 6f72 650a 2020 2020 2020  earn More.      
-00003090: 2020 0a20 2020 2020 2020 203c 6465 7461    .        <deta
-000030a0: 696c 733e 0a20 2020 2020 2020 203c 7375  ils>.        <su
-000030b0: 6d6d 6172 793e 5475 746f 7269 616c 733c  mmary>Tutorials<
-000030c0: 2f73 756d 6d61 7279 3e0a 2020 2020 2020  /summary>.      
-000030d0: 2020 0a20 2020 2020 2020 202d 205b 5275    .        - [Ru
-000030e0: 6e6e 6572 5d28 6874 7470 733a 2f2f 6d6d  nner](https://mm
-000030f0: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
-00003100: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00003110: 7475 746f 7269 616c 732f 7275 6e6e 6572  tutorials/runner
-00003120: 2e68 746d 6c29 0a20 2020 2020 2020 202d  .html).        -
-00003130: 205b 4461 7461 7365 7420 616e 6420 4461   [Dataset and Da
-00003140: 7461 4c6f 6164 6572 5d28 6874 7470 733a  taLoader](https:
-00003150: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
-00003160: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00003170: 6573 742f 7475 746f 7269 616c 732f 6461  est/tutorials/da
-00003180: 7461 7365 742e 6874 6d6c 290a 2020 2020  taset.html).    
-00003190: 2020 2020 2d20 5b4d 6f64 656c 5d28 6874      - [Model](ht
-000031a0: 7470 733a 2f2f 6d6d 656e 6769 6e65 2e72  tps://mmengine.r
-000031b0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000031c0: 2f6c 6174 6573 742f 7475 746f 7269 616c  /latest/tutorial
-000031d0: 732f 6d6f 6465 6c2e 6874 6d6c 290a 2020  s/model.html).  
-000031e0: 2020 2020 2020 2d20 5b45 7661 6c75 6174        - [Evaluat
-000031f0: 696f 6e5d 2868 7474 7073 3a2f 2f6d 6d65  ion](https://mme
-00003200: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
-00003210: 732e 696f 2f65 6e2f 6c61 7465 7374 2f74  s.io/en/latest/t
-00003220: 7574 6f72 6961 6c73 2f65 7661 6c75 6174  utorials/evaluat
-00003230: 696f 6e2e 6874 6d6c 290a 2020 2020 2020  ion.html).      
-00003240: 2020 2d20 5b4f 7074 696d 5772 6170 7065    - [OptimWrappe
-00003250: 725d 2868 7474 7073 3a2f 2f6d 6d65 6e67  r](https://mmeng
-00003260: 696e 652e 7265 6164 7468 6564 6f63 732e  ine.readthedocs.
-00003270: 696f 2f65 6e2f 6c61 7465 7374 2f74 7574  io/en/latest/tut
-00003280: 6f72 6961 6c73 2f6f 7074 696d 5f77 7261  orials/optim_wra
-00003290: 7070 6572 2e68 746d 6c29 0a20 2020 2020  pper.html).     
-000032a0: 2020 202d 205b 5061 7261 6d65 7465 7220     - [Parameter 
-000032b0: 5363 6865 6475 6c65 725d 2868 7474 7073  Scheduler](https
-000032c0: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-000032d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000032e0: 7465 7374 2f74 7574 6f72 6961 6c73 2f70  test/tutorials/p
-000032f0: 6172 616d 5f73 6368 6564 756c 6572 2e68  aram_scheduler.h
-00003300: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-00003310: 486f 6f6b 5d28 6874 7470 733a 2f2f 6d6d  Hook](https://mm
-00003320: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
-00003330: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00003340: 7475 746f 7269 616c 732f 686f 6f6b 2e68  tutorials/hook.h
-00003350: 746d 6c29 0a20 2020 2020 2020 200a 2020  tml).        .  
-00003360: 2020 2020 2020 3c2f 6465 7461 696c 733e        </details>
-00003370: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003380: 2020 3c64 6574 6169 6c73 3e0a 2020 2020    <details>.    
-00003390: 2020 2020 3c73 756d 6d61 7279 3e41 6476      <summary>Adv
-000033a0: 616e 6365 6420 7475 746f 7269 616c 733c  anced tutorials<
-000033b0: 2f73 756d 6d61 7279 3e0a 2020 2020 2020  /summary>.      
-000033c0: 2020 0a20 2020 2020 2020 202d 205b 5265    .        - [Re
-000033d0: 6769 7374 7279 5d28 6874 7470 733a 2f2f  gistry](https://
-000033e0: 6d6d 656e 6769 6e65 2e72 6561 6474 6865  mmengine.readthe
-000033f0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00003400: 742f 6164 7661 6e63 6564 5f74 7574 6f72  t/advanced_tutor
-00003410: 6961 6c73 2f72 6567 6973 7472 792e 6874  ials/registry.ht
-00003420: 6d6c 290a 2020 2020 2020 2020 2d20 5b43  ml).        - [C
-00003430: 6f6e 6669 675d 2868 7474 7073 3a2f 2f6d  onfig](https://m
-00003440: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-00003450: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00003460: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
-00003470: 616c 732f 636f 6e66 6967 2e68 746d 6c29  als/config.html)
-00003480: 0a20 2020 2020 2020 202d 205b 4261 7365  .        - [Base
-00003490: 4461 7461 7365 745d 2868 7474 7073 3a2f  Dataset](https:/
-000034a0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-000034b0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-000034c0: 7374 2f61 6476 616e 6365 645f 7475 746f  st/advanced_tuto
-000034d0: 7269 616c 732f 6261 7365 6461 7461 7365  rials/basedatase
-000034e0: 742e 6874 6d6c 290a 2020 2020 2020 2020  t.html).        
-000034f0: 2d20 5b44 6174 6120 5472 616e 7366 6f72  - [Data Transfor
-00003500: 6d5d 2868 7474 7073 3a2f 2f6d 6d65 6e67  m](https://mmeng
+000026c0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000026d0: 6e73 666f 726d 732e 5261 6e64 6f6d 4372  nsforms.RandomCr
+000026e0: 6f70 2833 322c 2070 6164 6469 6e67 3d34  op(32, padding=4
+000026f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002720: 2074 7261 6e73 666f 726d 732e 5261 6e64   transforms.Rand
+00002730: 6f6d 486f 7269 7a6f 6e74 616c 466c 6970  omHorizontalFlip
+00002740: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 7472 616e 7366 6f72 6d73 2e54 6f54    transforms.ToT
+00002780: 656e 736f 7228 292c 0a20 2020 2020 2020  ensor(),.       
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000027c0: 732e 4e6f 726d 616c 697a 6528 2a2a 6e6f  s.Normalize(**no
+000027d0: 726d 5f63 6667 290a 2020 2020 2020 2020  rm_cfg).        
+000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002800: 2020 5d29 2929 0a20 2020 2020 2020 2076    ]))).        v
+00002810: 616c 5f64 6174 616c 6f61 6465 7220 3d20  al_dataloader = 
+00002820: 4461 7461 4c6f 6164 6572 2862 6174 6368  DataLoader(batch
+00002830: 5f73 697a 653d 3332 2c0a 2020 2020 2020  _size=32,.      
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+00002860: 7566 666c 653d 4661 6c73 652c 0a20 2020  uffle=False,.   
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2064 6174 6173 6574 3d74 6f72 6368 7669   dataset=torchvi
+000028a0: 7369 6f6e 2e64 6174 6173 6574 732e 4349  sion.datasets.CI
+000028b0: 4641 5231 3028 0a20 2020 2020 2020 2020  FAR10(.         
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000028e0: 6461 7461 2f63 6966 6172 3130 272c 0a20  data/cifar10',. 
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 2020 2074 7261 696e 3d46 616c         train=Fal
+00002920: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 2020 2020 2020 646f 776e              down
+00002950: 6c6f 6164 3d54 7275 652c 0a20 2020 2020  load=True,.     
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2074 7261 6e73 666f 726d 3d74 7261     transform=tra
+00002990: 6e73 666f 726d 732e 436f 6d70 6f73 6528  nsforms.Compose(
+000029a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029c0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000029d0: 616e 7366 6f72 6d73 2e54 6f54 656e 736f  ansforms.ToTenso
+000029e0: 7228 292c 0a20 2020 2020 2020 2020 2020  r(),.           
+000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 2074 7261 6e73 666f 726d 732e 4e6f 726d   transforms.Norm
+00002a20: 616c 697a 6528 2a2a 6e6f 726d 5f63 6667  alize(**norm_cfg
+00002a30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 2020 2020 2020 2020 2020 5d29 2929 0a20            ]))). 
+00002a60: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00002a70: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
+00002a80: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
+00002a90: 2020 2020 2020 2020 3c64 6574 6169 6c73          <details
+00002aa0: 3e0a 2020 2020 2020 2020 3c73 756d 6d61  >.        <summa
+00002ab0: 7279 3e42 7569 6c64 204d 6574 7269 6373  ry>Build Metrics
+00002ac0: 3c2f 7375 6d6d 6172 793e 0a20 2020 2020  </summary>.     
+00002ad0: 2020 200a 2020 2020 2020 2020 546f 2076     .        To v
+00002ae0: 616c 6964 6174 6520 616e 6420 7465 7374  alidate and test
+00002af0: 2074 6865 206d 6f64 656c 2c20 7765 206e   the model, we n
+00002b00: 6565 6420 746f 2064 6566 696e 6520 6120  eed to define a 
+00002b10: 2a2a 4d65 7472 6963 2a2a 2063 616c 6c65  **Metric** calle
+00002b20: 6420 6163 6375 7261 6379 2074 6f20 6576  d accuracy to ev
+00002b30: 616c 7561 7465 2074 6865 206d 6f64 656c  aluate the model
+00002b40: 2e20 5468 6973 206d 6574 7269 6320 6e65  . This metric ne
+00002b50: 6564 7320 746f 2069 6e68 6572 6974 2066  eds to inherit f
+00002b60: 726f 6d20 6042 6173 654d 6574 7269 6360  rom `BaseMetric`
+00002b70: 2061 6e64 2069 6d70 6c65 6d65 6e74 7320   and implements 
+00002b80: 7468 6520 6070 726f 6365 7373 6020 616e  the `process` an
+00002b90: 6420 6063 6f6d 7075 7465 5f6d 6574 7269  d `compute_metri
+00002ba0: 6373 6020 6d65 7468 6f64 732e 0a20 2020  cs` methods..   
+00002bb0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
+00002bc0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00002bd0: 6672 6f6d 206d 6d65 6e67 696e 652e 6576  from mmengine.ev
+00002be0: 616c 7561 746f 7220 696d 706f 7274 2042  aluator import B
+00002bf0: 6173 654d 6574 7269 630a 2020 2020 2020  aseMetric.      
+00002c00: 2020 0a20 2020 2020 2020 2063 6c61 7373    .        class
+00002c10: 2041 6363 7572 6163 7928 4261 7365 4d65   Accuracy(BaseMe
+00002c20: 7472 6963 293a 0a20 2020 2020 2020 2020  tric):.         
+00002c30: 2020 2064 6566 2070 726f 6365 7373 2873     def process(s
+00002c40: 656c 662c 2064 6174 615f 6261 7463 682c  elf, data_batch,
+00002c50: 2064 6174 615f 7361 6d70 6c65 7329 3a0a   data_samples):.
+00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c70: 7363 6f72 652c 2067 7420 3d20 6461 7461  score, gt = data
+00002c80: 5f73 616d 706c 6573 0a20 2020 2020 2020  _samples.       
+00002c90: 2020 2020 2020 2020 2023 2053 6176 6520           # Save 
+00002ca0: 7468 6520 7265 7375 6c74 7320 6f66 2061  the results of a
+00002cb0: 2062 6174 6368 2074 6f20 6073 656c 662e   batch to `self.
+00002cc0: 7265 7375 6c74 7360 0a20 2020 2020 2020  results`.       
+00002cd0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00002ce0: 7375 6c74 732e 6170 7065 6e64 287b 0a20  sults.append({. 
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2027 6261 7463 685f 7369 7a65 273a     'batch_size':
+00002d10: 206c 656e 2867 7429 2c0a 2020 2020 2020   len(gt),.      
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+00002d30: 6f72 7265 6374 273a 2028 7363 6f72 652e  orrect': (score.
+00002d40: 6172 676d 6178 2864 696d 3d31 2920 3d3d  argmax(dim=1) ==
+00002d50: 2067 7429 2e73 756d 2829 2e63 7075 2829   gt).sum().cpu()
+00002d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002d70: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
+00002d80: 2064 6566 2063 6f6d 7075 7465 5f6d 6574   def compute_met
+00002d90: 7269 6373 2873 656c 662c 2072 6573 756c  rics(self, resul
+00002da0: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+00002db0: 2020 2020 2074 6f74 616c 5f63 6f72 7265       total_corre
+00002dc0: 6374 203d 2073 756d 2869 7465 6d5b 2763  ct = sum(item['c
+00002dd0: 6f72 7265 6374 275d 2066 6f72 2069 7465  orrect'] for ite
+00002de0: 6d20 696e 2072 6573 756c 7473 290a 2020  m in results).  
+00002df0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00002e00: 7461 6c5f 7369 7a65 203d 2073 756d 2869  tal_size = sum(i
+00002e10: 7465 6d5b 2762 6174 6368 5f73 697a 6527  tem['batch_size'
+00002e20: 5d20 666f 7220 6974 656d 2069 6e20 7265  ] for item in re
+00002e30: 7375 6c74 7329 0a20 2020 2020 2020 2020  sults).         
+00002e40: 2020 2020 2020 2023 2052 6574 7572 6e73         # Returns
+00002e50: 2061 2064 6963 7469 6f6e 6172 7920 7769   a dictionary wi
+00002e60: 7468 2074 6865 2072 6573 756c 7473 206f  th the results o
+00002e70: 6620 7468 6520 6576 616c 7561 7465 6420  f the evaluated 
+00002e80: 6d65 7472 6963 732c 0a20 2020 2020 2020  metrics,.       
+00002e90: 2020 2020 2020 2020 2023 2077 6865 7265           # where
+00002ea0: 2074 6865 206b 6579 2069 7320 7468 6520   the key is the 
+00002eb0: 6e61 6d65 206f 6620 7468 6520 6d65 7472  name of the metr
+00002ec0: 6963 0a20 2020 2020 2020 2020 2020 2020  ic.             
+00002ed0: 2020 2072 6574 7572 6e20 6469 6374 2861     return dict(a
+00002ee0: 6363 7572 6163 793d 3130 3020 2a20 746f  ccuracy=100 * to
+00002ef0: 7461 6c5f 636f 7272 6563 7420 2f20 746f  tal_correct / to
+00002f00: 7461 6c5f 7369 7a65 290a 2020 2020 2020  tal_size).      
+00002f10: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00002f20: 2020 2020 2020 203c 2f64 6574 6169 6c73         </details
+00002f30: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
+00002f40: 2020 203c 6465 7461 696c 733e 0a20 2020     <details>.   
+00002f50: 2020 2020 203c 7375 6d6d 6172 793e 4275       <summary>Bu
+00002f60: 696c 6420 6120 5275 6e6e 6572 3c2f 7375  ild a Runner</su
+00002f70: 6d6d 6172 793e 0a20 2020 2020 2020 200a  mmary>.        .
+00002f80: 2020 2020 2020 2020 4669 6e61 6c6c 792c          Finally,
+00002f90: 2077 6520 6361 6e20 636f 6e73 7472 7563   we can construc
+00002fa0: 7420 6120 2a2a 5275 6e6e 6572 2a2a 2077  t a **Runner** w
+00002fb0: 6974 6820 7072 6576 696f 7573 6c79 2064  ith previously d
+00002fc0: 6566 696e 6564 2060 4d6f 6465 6c60 2c20  efined `Model`, 
+00002fd0: 6044 6174 614c 6f61 6465 7260 2c20 616e  `DataLoader`, an
+00002fe0: 6420 604d 6574 7269 6373 602c 2077 6974  d `Metrics`, wit
+00002ff0: 6820 736f 6d65 206f 7468 6572 2063 6f6e  h some other con
+00003000: 6669 6773 2c20 6173 2073 686f 776e 2062  figs, as shown b
+00003010: 656c 6f77 2e0a 2020 2020 2020 2020 0a20  elow..        . 
+00003020: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00003030: 0a20 2020 2020 2020 2066 726f 6d20 746f  .        from to
+00003040: 7263 682e 6f70 7469 6d20 696d 706f 7274  rch.optim import
+00003050: 2053 4744 0a20 2020 2020 2020 2066 726f   SGD.        fro
+00003060: 6d20 6d6d 656e 6769 6e65 2e72 756e 6e65  m mmengine.runne
+00003070: 7220 696d 706f 7274 2052 756e 6e65 720a  r import Runner.
+00003080: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003090: 2072 756e 6e65 7220 3d20 5275 6e6e 6572   runner = Runner
+000030a0: 280a 2020 2020 2020 2020 2020 2020 6d6f  (.            mo
+000030b0: 6465 6c3d 4d4d 5265 734e 6574 3530 2829  del=MMResNet50()
+000030c0: 2c0a 2020 2020 2020 2020 2020 2020 776f  ,.            wo
+000030d0: 726b 5f64 6972 3d27 2e2f 776f 726b 5f64  rk_dir='./work_d
+000030e0: 6972 272c 0a20 2020 2020 2020 2020 2020  ir',.           
+000030f0: 2074 7261 696e 5f64 6174 616c 6f61 6465   train_dataloade
+00003100: 723d 7472 6169 6e5f 6461 7461 6c6f 6164  r=train_dataload
+00003110: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00003120: 2320 6120 7772 6170 7065 7220 746f 2065  # a wrapper to e
+00003130: 7865 6375 7465 2062 6163 6b20 7072 6f70  xecute back prop
+00003140: 6167 6174 696f 6e20 616e 6420 6772 6164  agation and grad
+00003150: 6965 6e74 2075 7064 6174 652c 2065 7463  ient update, etc
+00003160: 2e0a 2020 2020 2020 2020 2020 2020 6f70  ..            op
+00003170: 7469 6d5f 7772 6170 7065 723d 6469 6374  tim_wrapper=dict
+00003180: 286f 7074 696d 697a 6572 3d64 6963 7428  (optimizer=dict(
+00003190: 7479 7065 3d53 4744 2c20 6c72 3d30 2e30  type=SGD, lr=0.0
+000031a0: 3031 2c20 6d6f 6d65 6e74 756d 3d30 2e39  01, momentum=0.9
+000031b0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+000031c0: 2320 7365 7420 736f 6d65 2074 7261 696e  # set some train
+000031d0: 696e 6720 636f 6e66 6967 7320 6c69 6b65  ing configs like
+000031e0: 2065 706f 6368 730a 2020 2020 2020 2020   epochs.        
+000031f0: 2020 2020 7472 6169 6e5f 6366 673d 6469      train_cfg=di
+00003200: 6374 2862 795f 6570 6f63 683d 5472 7565  ct(by_epoch=True
+00003210: 2c20 6d61 785f 6570 6f63 6873 3d35 2c20  , max_epochs=5, 
+00003220: 7661 6c5f 696e 7465 7276 616c 3d31 292c  val_interval=1),
+00003230: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00003240: 5f64 6174 616c 6f61 6465 723d 7661 6c5f  _dataloader=val_
+00003250: 6461 7461 6c6f 6164 6572 2c0a 2020 2020  dataloader,.    
+00003260: 2020 2020 2020 2020 7661 6c5f 6366 673d          val_cfg=
+00003270: 6469 6374 2829 2c0a 2020 2020 2020 2020  dict(),.        
+00003280: 2020 2020 7661 6c5f 6576 616c 7561 746f      val_evaluato
+00003290: 723d 6469 6374 2874 7970 653d 4163 6375  r=dict(type=Accu
+000032a0: 7261 6379 292c 0a20 2020 2020 2020 2029  racy),.        )
+000032b0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+000032c0: 2020 2020 200a 2020 2020 2020 2020 3c2f       .        </
+000032d0: 6465 7461 696c 733e 0a20 2020 2020 2020  details>.       
+000032e0: 200a 2020 2020 2020 2020 3c64 6574 6169   .        <detai
+000032f0: 6c73 3e0a 2020 2020 2020 2020 3c73 756d  ls>.        <sum
+00003300: 6d61 7279 3e4c 6175 6e63 6820 5472 6169  mary>Launch Trai
+00003310: 6e69 6e67 3c2f 7375 6d6d 6172 793e 0a20  ning</summary>. 
+00003320: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003330: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00003340: 2020 7275 6e6e 6572 2e74 7261 696e 2829    runner.train()
+00003350: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00003360: 2020 2020 200a 2020 2020 2020 2020 3c2f       .        </
+00003370: 6465 7461 696c 733e 0a20 2020 2020 2020  details>.       
+00003380: 200a 2020 2020 2020 2020 2323 204c 6561   .        ## Lea
+00003390: 726e 204d 6f72 650a 2020 2020 2020 2020  rn More.        
+000033a0: 0a20 2020 2020 2020 203c 6465 7461 696c  .        <detail
+000033b0: 733e 0a20 2020 2020 2020 203c 7375 6d6d  s>.        <summ
+000033c0: 6172 793e 5475 746f 7269 616c 733c 2f73  ary>Tutorials</s
+000033d0: 756d 6d61 7279 3e0a 2020 2020 2020 2020  ummary>.        
+000033e0: 0a20 2020 2020 2020 202d 205b 5275 6e6e  .        - [Runn
+000033f0: 6572 5d28 6874 7470 733a 2f2f 6d6d 656e  er](https://mmen
+00003400: 6769 6e65 2e72 6561 6474 6865 646f 6373  gine.readthedocs
+00003410: 2e69 6f2f 656e 2f6c 6174 6573 742f 7475  .io/en/latest/tu
+00003420: 746f 7269 616c 732f 7275 6e6e 6572 2e68  torials/runner.h
+00003430: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
+00003440: 4461 7461 7365 7420 616e 6420 4461 7461  Dataset and Data
+00003450: 4c6f 6164 6572 5d28 6874 7470 733a 2f2f  Loader](https://
+00003460: 6d6d 656e 6769 6e65 2e72 6561 6474 6865  mmengine.readthe
+00003470: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00003480: 742f 7475 746f 7269 616c 732f 6461 7461  t/tutorials/data
+00003490: 7365 742e 6874 6d6c 290a 2020 2020 2020  set.html).      
+000034a0: 2020 2d20 5b4d 6f64 656c 5d28 6874 7470    - [Model](http
+000034b0: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
+000034c0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000034d0: 6174 6573 742f 7475 746f 7269 616c 732f  atest/tutorials/
+000034e0: 6d6f 6465 6c2e 6874 6d6c 290a 2020 2020  model.html).    
+000034f0: 2020 2020 2d20 5b45 7661 6c75 6174 696f      - [Evaluatio
+00003500: 6e5d 2868 7474 7073 3a2f 2f6d 6d65 6e67  n](https://mmeng
 00003510: 696e 652e 7265 6164 7468 6564 6f63 732e  ine.readthedocs.
-00003520: 696f 2f65 6e2f 6c61 7465 7374 2f61 6476  io/en/latest/adv
-00003530: 616e 6365 645f 7475 746f 7269 616c 732f  anced_tutorials/
-00003540: 6461 7461 5f74 7261 6e73 666f 726d 2e68  data_transform.h
-00003550: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-00003560: 5765 6967 6874 2049 6e69 7469 616c 697a  Weight Initializ
-00003570: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6d  ation](https://m
-00003580: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-00003590: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000035a0: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
-000035b0: 616c 732f 696e 6974 6961 6c69 7a65 2e68  als/initialize.h
-000035c0: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-000035d0: 5669 7375 616c 697a 6174 696f 6e5d 2868  Visualization](h
-000035e0: 7474 7073 3a2f 2f6d 6d65 6e67 696e 652e  ttps://mmengine.
-000035f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00003600: 6e2f 6c61 7465 7374 2f61 6476 616e 6365  n/latest/advance
-00003610: 645f 7475 746f 7269 616c 732f 7669 7375  d_tutorials/visu
-00003620: 616c 697a 6174 696f 6e2e 6874 6d6c 290a  alization.html).
-00003630: 2020 2020 2020 2020 2d20 5b41 6273 7472          - [Abstr
-00003640: 6163 7420 4461 7461 2045 6c65 6d65 6e74  act Data Element
-00003650: 5d28 6874 7470 733a 2f2f 6d6d 656e 6769  ](https://mmengi
-00003660: 6e65 2e72 6561 6474 6865 646f 6373 2e69  ne.readthedocs.i
-00003670: 6f2f 656e 2f6c 6174 6573 742f 6164 7661  o/en/latest/adva
-00003680: 6e63 6564 5f74 7574 6f72 6961 6c73 2f64  nced_tutorials/d
-00003690: 6174 615f 656c 656d 656e 742e 6874 6d6c  ata_element.html
-000036a0: 290a 2020 2020 2020 2020 2d20 5b44 6973  ).        - [Dis
-000036b0: 7472 6962 7574 696f 6e20 436f 6d6d 756e  tribution Commun
-000036c0: 6963 6174 696f 6e5d 2868 7474 7073 3a2f  ication](https:/
-000036d0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-000036e0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-000036f0: 7374 2f61 6476 616e 6365 645f 7475 746f  st/advanced_tuto
-00003700: 7269 616c 732f 6469 7374 7269 6275 7465  rials/distribute
-00003710: 642e 6874 6d6c 290a 2020 2020 2020 2020  d.html).        
-00003720: 2d20 5b4c 6f67 6769 6e67 5d28 6874 7470  - [Logging](http
-00003730: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
-00003740: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00003750: 6174 6573 742f 6164 7661 6e63 6564 5f74  atest/advanced_t
-00003760: 7574 6f72 6961 6c73 2f6c 6f67 6769 6e67  utorials/logging
-00003770: 2e68 746d 6c29 0a20 2020 2020 2020 202d  .html).        -
-00003780: 205b 4669 6c65 2049 4f5d 2868 7474 7073   [File IO](https
-00003790: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-000037a0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000037b0: 7465 7374 2f61 6476 616e 6365 645f 7475  test/advanced_tu
-000037c0: 746f 7269 616c 732f 6669 6c65 696f 2e68  torials/fileio.h
-000037d0: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-000037e0: 476c 6f62 616c 206d 616e 6167 6572 2028  Global manager (
-000037f0: 4d61 6e61 6765 724d 6978 696e 295d 2868  ManagerMixin)](h
-00003800: 7474 7073 3a2f 2f6d 6d65 6e67 696e 652e  ttps://mmengine.
-00003810: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00003820: 6e2f 6c61 7465 7374 2f61 6476 616e 6365  n/latest/advance
-00003830: 645f 7475 746f 7269 616c 732f 6d61 6e61  d_tutorials/mana
-00003840: 6765 725f 6d69 7869 6e2e 6874 6d6c 290a  ger_mixin.html).
-00003850: 2020 2020 2020 2020 2d20 5b55 7365 206d          - [Use m
-00003860: 6f64 756c 6573 2066 726f 6d20 6f74 6865  odules from othe
-00003870: 7220 6c69 6272 6172 6965 735d 2868 7474  r libraries](htt
-00003880: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
-00003890: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-000038a0: 6c61 7465 7374 2f61 6476 616e 6365 645f  latest/advanced_
-000038b0: 7475 746f 7269 616c 732f 6372 6f73 735f  tutorials/cross_
-000038c0: 6c69 6272 6172 792e 6874 6d6c 290a 2020  library.html).  
-000038d0: 2020 2020 2020 2d20 5b54 6573 7420 5469        - [Test Ti
-000038e0: 6d65 2041 6775 6d65 6e74 6174 696f 6e5d  me Agumentation]
-000038f0: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
-00003900: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00003910: 2f65 6e2f 6c61 7465 7374 2f61 6476 616e  /en/latest/advan
-00003920: 6365 645f 7475 746f 7269 616c 732f 7465  ced_tutorials/te
-00003930: 7374 5f74 696d 655f 6175 676d 656e 7461  st_time_augmenta
-00003940: 7469 6f6e 2e68 746d 6c29 0a20 2020 2020  tion.html).     
-00003950: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
-00003960: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
-00003970: 2020 2020 2020 2020 3c64 6574 6169 6c73          <details
-00003980: 3e0a 2020 2020 2020 2020 3c73 756d 6d61  >.        <summa
-00003990: 7279 3e45 7861 6d70 6c65 733c 2f73 756d  ry>Examples</sum
-000039a0: 6d61 7279 3e0a 2020 2020 2020 2020 0a20  mary>.        . 
-000039b0: 2020 2020 2020 202d 205b 5472 6169 6e20         - [Train 
-000039c0: 6120 4741 4e5d 2868 7474 7073 3a2f 2f6d  a GAN](https://m
-000039d0: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-000039e0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000039f0: 2f65 7861 6d70 6c65 732f 7472 6169 6e5f  /examples/train_
-00003a00: 615f 6761 6e2e 6874 6d6c 290a 2020 2020  a_gan.html).    
-00003a10: 2020 2020 0a20 2020 2020 2020 203c 2f64      .        </d
-00003a20: 6574 6169 6c73 3e0a 2020 2020 2020 2020  etails>.        
-00003a30: 0a20 2020 2020 2020 203c 6465 7461 696c  .        <detail
-00003a40: 733e 0a20 2020 2020 2020 203c 7375 6d6d  s>.        <summ
-00003a50: 6172 793e 436f 6d6d 6f6e 2055 7361 6765  ary>Common Usage
-00003a60: 3c2f 7375 6d6d 6172 793e 0a20 2020 2020  </summary>.     
-00003a70: 2020 200a 2020 2020 2020 2020 2d20 5b52     .        - [R
-00003a80: 6573 756d 6520 5472 6169 6e69 6e67 5d28  esume Training](
-00003a90: 6874 7470 733a 2f2f 6d6d 656e 6769 6e65  https://mmengine
-00003aa0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00003ab0: 656e 2f6c 6174 6573 742f 636f 6d6d 6f6e  en/latest/common
-00003ac0: 5f75 7361 6765 2f72 6573 756d 655f 7472  _usage/resume_tr
-00003ad0: 6169 6e69 6e67 2e68 746d 6c29 0a20 2020  aining.html).   
-00003ae0: 2020 2020 202d 205b 5370 6565 6420 7570       - [Speed up
-00003af0: 2054 7261 696e 696e 675d 2868 7474 7073   Training](https
-00003b00: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-00003b10: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00003b20: 7465 7374 2f63 6f6d 6d6f 6e5f 7573 6167  test/common_usag
-00003b30: 652f 7370 6565 645f 7570 5f74 7261 696e  e/speed_up_train
-00003b40: 696e 672e 6874 6d6c 290a 2020 2020 2020  ing.html).      
-00003b50: 2020 2d20 5b53 6176 6520 4d65 6d6f 7279    - [Save Memory
-00003b60: 206f 6e20 4750 555d 2868 7474 7073 3a2f   on GPU](https:/
-00003b70: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00003b80: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003b90: 7374 2f63 6f6d 6d6f 6e5f 7573 6167 652f  st/common_usage/
-00003ba0: 7361 7665 5f67 7075 5f6d 656d 6f72 792e  save_gpu_memory.
-00003bb0: 6874 6d6c 290a 2020 2020 2020 2020 0a20  html).        . 
-00003bc0: 2020 2020 2020 203c 2f64 6574 6169 6c73         </details
-00003bd0: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
-00003be0: 2020 203c 6465 7461 696c 733e 0a20 2020     <details>.   
-00003bf0: 2020 2020 203c 7375 6d6d 6172 793e 4465       <summary>De
-00003c00: 7369 676e 3c2f 7375 6d6d 6172 793e 0a20  sign</summary>. 
-00003c10: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003c20: 2d20 5b48 6f6f 6b5d 2868 7474 7073 3a2f  - [Hook](https:/
-00003c30: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00003c40: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003c50: 7374 2f64 6573 6967 6e2f 686f 6f6b 2e68  st/design/hook.h
-00003c60: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-00003c70: 5275 6e6e 6572 5d28 6874 7470 733a 2f2f  Runner](https://
-00003c80: 6d6d 656e 6769 6e65 2e72 6561 6474 6865  mmengine.readthe
-00003c90: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00003ca0: 742f 6465 7369 676e 2f72 756e 6e65 722e  t/design/runner.
-00003cb0: 6874 6d6c 290a 2020 2020 2020 2020 2d20  html).        - 
-00003cc0: 5b45 7661 6c75 6174 696f 6e5d 2868 7474  [Evaluation](htt
-00003cd0: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
-00003ce0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00003cf0: 6c61 7465 7374 2f64 6573 6967 6e2f 6576  latest/design/ev
-00003d00: 616c 7561 7469 6f6e 2e68 746d 6c29 0a20  aluation.html). 
-00003d10: 2020 2020 2020 202d 205b 5669 7375 616c         - [Visual
-00003d20: 697a 6174 696f 6e5d 2868 7474 7073 3a2f  ization](https:/
-00003d30: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00003d40: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003d50: 7374 2f64 6573 6967 6e2f 7669 7375 616c  st/design/visual
-00003d60: 697a 6174 696f 6e2e 6874 6d6c 290a 2020  ization.html).  
-00003d70: 2020 2020 2020 2d20 5b4c 6f67 6769 6e67        - [Logging
-00003d80: 5d28 6874 7470 733a 2f2f 6d6d 656e 6769  ](https://mmengi
-00003d90: 6e65 2e72 6561 6474 6865 646f 6373 2e69  ne.readthedocs.i
-00003da0: 6f2f 656e 2f6c 6174 6573 742f 6465 7369  o/en/latest/desi
-00003db0: 676e 2f6c 6f67 6769 6e67 2e68 746d 6c29  gn/logging.html)
-00003dc0: 0a20 2020 2020 2020 202d 205b 496e 6665  .        - [Infe
-00003dd0: 725d 2868 7474 7073 3a2f 2f6d 6d65 6e67  r](https://mmeng
-00003de0: 696e 652e 7265 6164 7468 6564 6f63 732e  ine.readthedocs.
-00003df0: 696f 2f65 6e2f 6c61 7465 7374 2f64 6573  io/en/latest/des
-00003e00: 6967 6e2f 696e 6665 722e 6874 6d6c 290a  ign/infer.html).
-00003e10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003e20: 203c 2f64 6574 6169 6c73 3e0a 2020 2020   </details>.    
-00003e30: 2020 2020 0a20 2020 2020 2020 203c 6465      .        <de
-00003e40: 7461 696c 733e 0a20 2020 2020 2020 203c  tails>.        <
-00003e50: 7375 6d6d 6172 793e 4d69 6772 6174 696f  summary>Migratio
-00003e60: 6e20 6775 6964 653c 2f73 756d 6d61 7279  n guide</summary
-00003e70: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
-00003e80: 2020 202d 205b 4d69 6772 6174 6520 5275     - [Migrate Ru
-00003e90: 6e6e 6572 2066 726f 6d20 4d4d 4356 2074  nner from MMCV t
-00003ea0: 6f20 4d4d 456e 6769 6e65 5d28 6874 7470  o MMEngine](http
-00003eb0: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
-00003ec0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00003ed0: 6174 6573 742f 6d69 6772 6174 696f 6e2f  atest/migration/
-00003ee0: 7275 6e6e 6572 2e68 746d 6c29 0a20 2020  runner.html).   
-00003ef0: 2020 2020 202d 205b 4d69 6772 6174 6520       - [Migrate 
-00003f00: 486f 6f6b 2066 726f 6d20 4d4d 4356 2074  Hook from MMCV t
-00003f10: 6f20 4d4d 456e 6769 6e65 5d28 6874 7470  o MMEngine](http
-00003f20: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
-00003f30: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00003f40: 6174 6573 742f 6d69 6772 6174 696f 6e2f  atest/migration/
-00003f50: 686f 6f6b 2e68 746d 6c29 0a20 2020 2020  hook.html).     
-00003f60: 2020 202d 205b 4d69 6772 6174 6520 4d6f     - [Migrate Mo
-00003f70: 6465 6c20 6672 6f6d 204d 4d43 5620 746f  del from MMCV to
-00003f80: 204d 4d45 6e67 696e 655d 2868 7474 7073   MMEngine](https
-00003f90: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-00003fa0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00003fb0: 7465 7374 2f6d 6967 7261 7469 6f6e 2f6d  test/migration/m
-00003fc0: 6f64 656c 2e68 746d 6c29 0a20 2020 2020  odel.html).     
-00003fd0: 2020 202d 205b 4d69 6772 6174 6520 5061     - [Migrate Pa
-00003fe0: 7261 6d65 7465 7220 5363 6865 6475 6c65  rameter Schedule
-00003ff0: 7220 6672 6f6d 204d 4d43 5620 746f 204d  r from MMCV to M
-00004000: 4d45 6e67 696e 655d 2868 7474 7073 3a2f  MEngine](https:/
-00004010: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00004020: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00004030: 7374 2f6d 6967 7261 7469 6f6e 2f70 6172  st/migration/par
-00004040: 616d 5f73 6368 6564 756c 6572 2e68 746d  am_scheduler.htm
-00004050: 6c29 0a20 2020 2020 2020 202d 205b 4d69  l).        - [Mi
-00004060: 6772 6174 6520 4461 7461 2054 7261 6e73  grate Data Trans
-00004070: 666f 726d 2074 6f20 4f70 656e 4d4d 4c61  form to OpenMMLa
-00004080: 6220 322e 305d 2868 7474 7073 3a2f 2f6d  b 2.0](https://m
-00004090: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-000040a0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000040b0: 2f6d 6967 7261 7469 6f6e 2f74 7261 6e73  /migration/trans
-000040c0: 666f 726d 2e68 746d 6c29 0a20 2020 2020  form.html).     
-000040d0: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
-000040e0: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
-000040f0: 2020 2020 2020 2020 2323 2043 6f6e 7472          ## Contr
-00004100: 6962 7574 696e 670a 2020 2020 2020 2020  ibuting.        
-00004110: 0a20 2020 2020 2020 2057 6520 6170 7072  .        We appr
-00004120: 6563 6961 7465 2061 6c6c 2063 6f6e 7472  eciate all contr
-00004130: 6962 7574 696f 6e73 2074 6f20 696d 7072  ibutions to impr
-00004140: 6f76 6520 4d4d 456e 6769 6e65 2e20 506c  ove MMEngine. Pl
-00004150: 6561 7365 2072 6566 6572 2074 6f20 5b43  ease refer to [C
-00004160: 4f4e 5452 4942 5554 494e 472e 6d64 5d28  ONTRIBUTING.md](
-00004170: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
-00004180: 2066 6f72 2074 6865 2063 6f6e 7472 6962   for the contrib
-00004190: 7574 696e 6720 6775 6964 656c 696e 652e  uting guideline.
-000041a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000041b0: 2020 2323 2043 6974 6174 696f 6e0a 2020    ## Citation.  
-000041c0: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
-000041d0: 6620 796f 7520 6669 6e64 2074 6869 7320  f you find this 
-000041e0: 7072 6f6a 6563 7420 7573 6566 756c 2069  project useful i
-000041f0: 6e20 796f 7572 2072 6573 6561 7263 682c  n your research,
-00004200: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
-00004210: 2063 6974 653a 0a20 2020 2020 2020 200a   cite:.        .
-00004220: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
-00004230: 2020 2020 4061 7274 6963 6c65 7b6d 6d65      @article{mme
-00004240: 6e67 696e 6532 3032 322c 0a20 2020 2020  ngine2022,.     
-00004250: 2020 2020 2074 6974 6c65 2020 203d 207b       title   = {
-00004260: 7b4d 4d45 6e67 696e 657d 3a20 4f70 656e  {MMEngine}: Open
-00004270: 4d4d 4c61 6220 466f 756e 6461 7469 6f6e  MMLab Foundation
-00004280: 616c 204c 6962 7261 7279 2066 6f72 2054  al Library for T
-00004290: 7261 696e 696e 6720 4465 6570 204c 6561  raining Deep Lea
-000042a0: 726e 696e 6720 4d6f 6465 6c73 7d2c 0a20  rning Models},. 
-000042b0: 2020 2020 2020 2020 2061 7574 686f 7220           author 
-000042c0: 203d 207b 4d4d 456e 6769 6e65 2043 6f6e   = {MMEngine Con
-000042d0: 7472 6962 7574 6f72 737d 2c0a 2020 2020  tributors},.    
-000042e0: 2020 2020 2020 686f 7770 7562 6c69 7368        howpublish
-000042f0: 6564 203d 207b 5c75 726c 7b68 7474 7073  ed = {\url{https
-00004300: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f70  ://github.com/op
-00004310: 656e 2d6d 6d6c 6162 2f6d 6d65 6e67 696e  en-mmlab/mmengin
-00004320: 657d 7d2c 0a20 2020 2020 2020 2020 2079  e}},.          y
-00004330: 6561 723d 7b32 3032 327d 0a20 2020 2020  ear={2022}.     
-00004340: 2020 207d 0a20 2020 2020 2020 2060 6060     }.        ```
-00004350: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004360: 2020 2323 204c 6963 656e 7365 0a20 2020    ## License.   
-00004370: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-00004380: 6973 2070 726f 6a65 6374 2069 7320 7265  is project is re
-00004390: 6c65 6173 6564 2075 6e64 6572 2074 6865  leased under the
-000043a0: 205b 4170 6163 6865 2032 2e30 206c 6963   [Apache 2.0 lic
-000043b0: 656e 7365 5d28 4c49 4345 4e53 4529 2e0a  ense](LICENSE)..
-000043c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000043d0: 2023 2320 5072 6f6a 6563 7473 2069 6e20   ## Projects in 
-000043e0: 4f70 656e 4d4d 4c61 620a 2020 2020 2020  OpenMMLab.      
-000043f0: 2020 0a20 2020 2020 2020 202d 205b 4d49    .        - [MI
-00004400: 4d5d 2868 7474 7073 3a2f 2f67 6974 6875  M](https://githu
-00004410: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
-00004420: 2f6d 696d 293a 204d 494d 2069 6e73 7461  /mim): MIM insta
-00004430: 6c6c 7320 4f70 656e 4d4d 4c61 6220 7061  lls OpenMMLab pa
-00004440: 636b 6167 6573 2e0a 2020 2020 2020 2020  ckages..        
-00004450: 2d20 5b4d 4d43 565d 2868 7474 7073 3a2f  - [MMCV](https:/
-00004460: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004470: 2d6d 6d6c 6162 2f6d 6d63 7629 3a20 4f70  -mmlab/mmcv): Op
-00004480: 656e 4d4d 4c61 6220 666f 756e 6461 7469  enMMLab foundati
-00004490: 6f6e 616c 206c 6962 7261 7279 2066 6f72  onal library for
-000044a0: 2063 6f6d 7075 7465 7220 7669 7369 6f6e   computer vision
-000044b0: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d45  ..        - [MME
-000044c0: 7661 6c5d 2868 7474 7073 3a2f 2f67 6974  val](https://git
-000044d0: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
-000044e0: 6162 2f6d 6d65 7661 6c29 3a20 4120 756e  ab/mmeval): A un
-000044f0: 6966 6965 6420 6576 616c 7561 7469 6f6e  ified evaluation
-00004500: 206c 6962 7261 7279 2066 6f72 206d 756c   library for mul
-00004510: 7469 706c 6520 6d61 6368 696e 6520 6c65  tiple machine le
-00004520: 6172 6e69 6e67 206c 6962 7261 7269 6573  arning libraries
-00004530: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d50  ..        - [MMP
-00004540: 7265 5472 6169 6e5d 2868 7474 7073 3a2f  reTrain](https:/
-00004550: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004560: 2d6d 6d6c 6162 2f6d 6d70 7265 7472 6169  -mmlab/mmpretrai
-00004570: 6e29 3a20 4f70 656e 4d4d 4c61 6220 7072  n): OpenMMLab pr
-00004580: 652d 7472 6169 6e69 6e67 2074 6f6f 6c62  e-training toolb
-00004590: 6f78 2061 6e64 2062 656e 6368 6d61 726b  ox and benchmark
-000045a0: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d61  ..        - [MMa
-000045b0: 6769 635d 2868 7474 7073 3a2f 2f67 6974  gic](https://git
-000045c0: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
-000045d0: 6162 2f6d 6d61 6769 6329 3a20 4f70 656e  ab/mmagic): Open
-000045e0: 2a2a 4d4d 2a2a 4c61 6220 2a2a 412a 2a64  **MM**Lab **A**d
-000045f0: 7661 6e63 6564 2c20 2a2a 472a 2a65 6e65  vanced, **G**ene
-00004600: 7261 7469 7665 2061 6e64 202a 2a49 2a2a  rative and **I**
-00004610: 6e74 656c 6c69 6765 6e74 202a 2a43 2a2a  ntelligent **C**
-00004620: 7265 6174 696f 6e20 746f 6f6c 626f 782e  reation toolbox.
-00004630: 0a20 2020 2020 2020 202d 205b 4d4d 4465  .        - [MMDe
-00004640: 7465 6374 696f 6e5d 2868 7474 7073 3a2f  tection](https:/
-00004650: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004660: 2d6d 6d6c 6162 2f6d 6d64 6574 6563 7469  -mmlab/mmdetecti
-00004670: 6f6e 293a 204f 7065 6e4d 4d4c 6162 2064  on): OpenMMLab d
-00004680: 6574 6563 7469 6f6e 2074 6f6f 6c62 6f78  etection toolbox
-00004690: 2061 6e64 2062 656e 6368 6d61 726b 2e0a   and benchmark..
-000046a0: 2020 2020 2020 2020 2d20 5b4d 4d59 4f4c          - [MMYOL
-000046b0: 4f5d 2868 7474 7073 3a2f 2f67 6974 6875  O](https://githu
-000046c0: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
-000046d0: 2f6d 6d79 6f6c 6f29 3a20 4f70 656e 4d4d  /mmyolo): OpenMM
-000046e0: 4c61 6220 594f 4c4f 2073 6572 6965 7320  Lab YOLO series 
-000046f0: 746f 6f6c 626f 7820 616e 6420 6265 6e63  toolbox and benc
-00004700: 686d 6172 6b2e 0a20 2020 2020 2020 202d  hmark..        -
-00004710: 205b 4d4d 4465 7465 6374 696f 6e33 445d   [MMDetection3D]
-00004720: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00004730: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
-00004740: 6d64 6574 6563 7469 6f6e 3364 293a 204f  mdetection3d): O
-00004750: 7065 6e4d 4d4c 6162 2773 206e 6578 742d  penMMLab's next-
-00004760: 6765 6e65 7261 7469 6f6e 2070 6c61 7466  generation platf
-00004770: 6f72 6d20 666f 7220 6765 6e65 7261 6c20  orm for general 
-00004780: 3344 206f 626a 6563 7420 6465 7465 6374  3D object detect
-00004790: 696f 6e2e 0a20 2020 2020 2020 202d 205b  ion..        - [
-000047a0: 4d4d 526f 7461 7465 5d28 6874 7470 733a  MMRotate](https:
-000047b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7065  //github.com/ope
-000047c0: 6e2d 6d6d 6c61 622f 6d6d 726f 7461 7465  n-mmlab/mmrotate
-000047d0: 293a 204f 7065 6e4d 4d4c 6162 2072 6f74  ): OpenMMLab rot
-000047e0: 6174 6564 206f 626a 6563 7420 6465 7465  ated object dete
-000047f0: 6374 696f 6e20 746f 6f6c 626f 7820 616e  ction toolbox an
-00004800: 6420 6265 6e63 686d 6172 6b2e 0a20 2020  d benchmark..   
-00004810: 2020 2020 202d 205b 4d4d 5472 6163 6b69       - [MMTracki
-00004820: 6e67 5d28 6874 7470 733a 2f2f 6769 7468  ng](https://gith
-00004830: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
-00004840: 622f 6d6d 7472 6163 6b69 6e67 293a 204f  b/mmtracking): O
-00004850: 7065 6e4d 4d4c 6162 2076 6964 656f 2070  penMMLab video p
-00004860: 6572 6365 7074 696f 6e20 746f 6f6c 626f  erception toolbo
-00004870: 7820 616e 6420 6265 6e63 686d 6172 6b2e  x and benchmark.
-00004880: 0a20 2020 2020 2020 202d 205b 4d4d 506f  .        - [MMPo
-00004890: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-000048a0: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
-000048b0: 622f 6d6d 706f 7365 293a 204f 7065 6e4d  b/mmpose): OpenM
-000048c0: 4d4c 6162 2070 6f73 6520 6573 7469 6d61  MLab pose estima
-000048d0: 7469 6f6e 2074 6f6f 6c62 6f78 2061 6e64  tion toolbox and
-000048e0: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
-000048f0: 2020 2020 2d20 5b4d 4d53 6567 6d65 6e74      - [MMSegment
-00004900: 6174 696f 6e5d 2868 7474 7073 3a2f 2f67  ation](https://g
-00004910: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
-00004920: 6d6c 6162 2f6d 6d73 6567 6d65 6e74 6174  mlab/mmsegmentat
-00004930: 696f 6e29 3a20 4f70 656e 4d4d 4c61 6220  ion): OpenMMLab 
-00004940: 7365 6d61 6e74 6963 2073 6567 6d65 6e74  semantic segment
-00004950: 6174 696f 6e20 746f 6f6c 626f 7820 616e  ation toolbox an
-00004960: 6420 6265 6e63 686d 6172 6b2e 0a20 2020  d benchmark..   
-00004970: 2020 2020 202d 205b 4d4d 4f43 525d 2868       - [MMOCR](h
-00004980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004990: 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d 6d6f  m/open-mmlab/mmo
-000049a0: 6372 293a 204f 7065 6e4d 4d4c 6162 2074  cr): OpenMMLab t
-000049b0: 6578 7420 6465 7465 6374 696f 6e2c 2072  ext detection, r
-000049c0: 6563 6f67 6e69 7469 6f6e 2c20 616e 6420  ecognition, and 
-000049d0: 756e 6465 7273 7461 6e64 696e 6720 746f  understanding to
-000049e0: 6f6c 626f 782e 0a20 2020 2020 2020 202d  olbox..        -
-000049f0: 205b 4d4d 4875 6d61 6e33 445d 2868 7474   [MMHuman3D](htt
-00004a00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004a10: 6f70 656e 2d6d 6d6c 6162 2f6d 6d68 756d  open-mmlab/mmhum
-00004a20: 616e 3364 293a 204f 7065 6e4d 4d4c 6162  an3d): OpenMMLab
-00004a30: 2033 4420 6875 6d61 6e20 7061 7261 6d65   3D human parame
-00004a40: 7472 6963 206d 6f64 656c 2074 6f6f 6c62  tric model toolb
-00004a50: 6f78 2061 6e64 2062 656e 6368 6d61 726b  ox and benchmark
-00004a60: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d53  ..        - [MMS
-00004a70: 656c 6653 7570 5d28 6874 7470 733a 2f2f  elfSup](https://
-00004a80: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e2d  github.com/open-
-00004a90: 6d6d 6c61 622f 6d6d 7365 6c66 7375 7029  mmlab/mmselfsup)
-00004aa0: 3a20 4f70 656e 4d4d 4c61 6220 7365 6c66  : OpenMMLab self
-00004ab0: 2d73 7570 6572 7669 7365 6420 6c65 6172  -supervised lear
-00004ac0: 6e69 6e67 2074 6f6f 6c62 6f78 2061 6e64  ning toolbox and
-00004ad0: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
-00004ae0: 2020 2020 2d20 5b4d 4d46 6577 5368 6f74      - [MMFewShot
-00004af0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004b00: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
-00004b10: 6d6d 6665 7773 686f 7429 3a20 4f70 656e  mmfewshot): Open
-00004b20: 4d4d 4c61 6220 6665 7773 686f 7420 6c65  MMLab fewshot le
-00004b30: 6172 6e69 6e67 2074 6f6f 6c62 6f78 2061  arning toolbox a
-00004b40: 6e64 2062 656e 6368 6d61 726b 2e0a 2020  nd benchmark..  
-00004b50: 2020 2020 2020 2d20 5b4d 4d41 6374 696f        - [MMActio
-00004b60: 6e32 5d28 6874 7470 733a 2f2f 6769 7468  n2](https://gith
-00004b70: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
-00004b80: 622f 6d6d 6163 7469 6f6e 3229 3a20 4f70  b/mmaction2): Op
-00004b90: 656e 4d4d 4c61 6227 7320 6e65 7874 2d67  enMMLab's next-g
-00004ba0: 656e 6572 6174 696f 6e20 6163 7469 6f6e  eneration action
-00004bb0: 2075 6e64 6572 7374 616e 6469 6e67 2074   understanding t
-00004bc0: 6f6f 6c62 6f78 2061 6e64 2062 656e 6368  oolbox and bench
-00004bd0: 6d61 726b 2e0a 2020 2020 2020 2020 2d20  mark..        - 
-00004be0: 5b4d 4d46 6c6f 775d 2868 7474 7073 3a2f  [MMFlow](https:/
-00004bf0: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004c00: 2d6d 6d6c 6162 2f6d 6d66 6c6f 7729 3a20  -mmlab/mmflow): 
-00004c10: 4f70 656e 4d4d 4c61 6220 6f70 7469 6361  OpenMMLab optica
-00004c20: 6c20 666c 6f77 2074 6f6f 6c62 6f78 2061  l flow toolbox a
-00004c30: 6e64 2062 656e 6368 6d61 726b 2e0a 2020  nd benchmark..  
-00004c40: 2020 2020 2020 2d20 5b4d 4d44 6570 6c6f        - [MMDeplo
-00004c50: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00004c60: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
-00004c70: 2f6d 6d64 6570 6c6f 7929 3a20 4f70 656e  /mmdeploy): Open
-00004c80: 4d4d 4c61 6220 6d6f 6465 6c20 6465 706c  MMLab model depl
-00004c90: 6f79 6d65 6e74 2066 7261 6d65 776f 726b  oyment framework
-00004ca0: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d52  ..        - [MMR
-00004cb0: 617a 6f72 5d28 6874 7470 733a 2f2f 6769  azor](https://gi
-00004cc0: 7468 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d  thub.com/open-mm
-00004cd0: 6c61 622f 6d6d 7261 7a6f 7229 3a20 4f70  lab/mmrazor): Op
-00004ce0: 656e 4d4d 4c61 6220 6d6f 6465 6c20 636f  enMMLab model co
-00004cf0: 6d70 7265 7373 696f 6e20 746f 6f6c 626f  mpression toolbo
-00004d00: 7820 616e 6420 6265 6e63 686d 6172 6b2e  x and benchmark.
-00004d10: 0a20 2020 2020 2020 202d 205b 506c 6179  .        - [Play
-00004d20: 6772 6f75 6e64 5d28 6874 7470 733a 2f2f  ground](https://
-00004d30: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e2d  github.com/open-
-00004d40: 6d6d 6c61 622f 706c 6179 6772 6f75 6e64  mmlab/playground
-00004d50: 293a 2041 2063 656e 7472 616c 2068 7562  ): A central hub
-00004d60: 2066 6f72 2067 6174 6865 7269 6e67 2061   for gathering a
-00004d70: 6e64 2073 686f 7763 6173 696e 6720 616d  nd showcasing am
-00004d80: 617a 696e 6720 7072 6f6a 6563 7473 2062  azing projects b
-00004d90: 7569 6c74 2075 706f 6e20 4f70 656e 4d4d  uilt upon OpenMM
-00004da0: 4c61 622e 0a20 2020 2020 2020 200a 506c  Lab..        .Pl
-00004db0: 6174 666f 726d 3a20 554e 4b4e 4f57 4e0a  atform: UNKNOWN.
-00004dc0: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
-00004dd0: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00004de0: 3a20 3420 2d20 4265 7461 0a43 6c61 7373  : 4 - Beta.Class
-00004df0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00004e00: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00004e10: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
-00004e20: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
-00004e30: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00004e40: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00004e50: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
-00004e60: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00004e70: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00004e80: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
-00004e90: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00004ea0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00004eb0: 686f 6e20 3a3a 2033 2e37 0a43 6c61 7373  hon :: 3.7.Class
-00004ec0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00004ed0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00004ee0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
-00004ef0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00004f00: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00004f10: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-00004f20: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00004f30: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00004f40: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00004f50: 300a 436c 6173 7369 6669 6572 3a20 546f  0.Classifier: To
-00004f60: 7069 6320 3a3a 2055 7469 6c69 7469 6573  pic :: Utilities
-00004f70: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-00004f80: 3a20 3e3d 332e 370a 4465 7363 7269 7074  : >=3.7.Descript
-00004f90: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00004fa0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00004fb0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00004fc0: 616c 6c0a 5072 6f76 6964 6573 2d45 7874  all.Provides-Ext
-00004fd0: 7261 3a20 7465 7374 730a                 ra: tests.
+00003520: 696f 2f65 6e2f 6c61 7465 7374 2f74 7574  io/en/latest/tut
+00003530: 6f72 6961 6c73 2f65 7661 6c75 6174 696f  orials/evaluatio
+00003540: 6e2e 6874 6d6c 290a 2020 2020 2020 2020  n.html).        
+00003550: 2d20 5b4f 7074 696d 5772 6170 7065 725d  - [OptimWrapper]
+00003560: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
+00003570: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00003580: 2f65 6e2f 6c61 7465 7374 2f74 7574 6f72  /en/latest/tutor
+00003590: 6961 6c73 2f6f 7074 696d 5f77 7261 7070  ials/optim_wrapp
+000035a0: 6572 2e68 746d 6c29 0a20 2020 2020 2020  er.html).       
+000035b0: 202d 205b 5061 7261 6d65 7465 7220 5363   - [Parameter Sc
+000035c0: 6865 6475 6c65 725d 2868 7474 7073 3a2f  heduler](https:/
+000035d0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+000035e0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000035f0: 7374 2f74 7574 6f72 6961 6c73 2f70 6172  st/tutorials/par
+00003600: 616d 5f73 6368 6564 756c 6572 2e68 746d  am_scheduler.htm
+00003610: 6c29 0a20 2020 2020 2020 202d 205b 486f  l).        - [Ho
+00003620: 6f6b 5d28 6874 7470 733a 2f2f 6d6d 656e  ok](https://mmen
+00003630: 6769 6e65 2e72 6561 6474 6865 646f 6373  gine.readthedocs
+00003640: 2e69 6f2f 656e 2f6c 6174 6573 742f 7475  .io/en/latest/tu
+00003650: 746f 7269 616c 732f 686f 6f6b 2e68 746d  torials/hook.htm
+00003660: 6c29 0a20 2020 2020 2020 200a 2020 2020  l).        .    
+00003670: 2020 2020 3c2f 6465 7461 696c 733e 0a20      </details>. 
+00003680: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003690: 3c64 6574 6169 6c73 3e0a 2020 2020 2020  <details>.      
+000036a0: 2020 3c73 756d 6d61 7279 3e41 6476 616e    <summary>Advan
+000036b0: 6365 6420 7475 746f 7269 616c 733c 2f73  ced tutorials</s
+000036c0: 756d 6d61 7279 3e0a 2020 2020 2020 2020  ummary>.        
+000036d0: 0a20 2020 2020 2020 202d 205b 5265 6769  .        - [Regi
+000036e0: 7374 7279 5d28 6874 7470 733a 2f2f 6d6d  stry](https://mm
+000036f0: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
+00003700: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00003710: 6164 7661 6e63 6564 5f74 7574 6f72 6961  advanced_tutoria
+00003720: 6c73 2f72 6567 6973 7472 792e 6874 6d6c  ls/registry.html
+00003730: 290a 2020 2020 2020 2020 2d20 5b43 6f6e  ).        - [Con
+00003740: 6669 675d 2868 7474 7073 3a2f 2f6d 6d65  fig](https://mme
+00003750: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+00003760: 732e 696f 2f65 6e2f 6c61 7465 7374 2f61  s.io/en/latest/a
+00003770: 6476 616e 6365 645f 7475 746f 7269 616c  dvanced_tutorial
+00003780: 732f 636f 6e66 6967 2e68 746d 6c29 0a20  s/config.html). 
+00003790: 2020 2020 2020 202d 205b 4261 7365 4461         - [BaseDa
+000037a0: 7461 7365 745d 2868 7474 7073 3a2f 2f6d  taset](https://m
+000037b0: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+000037c0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000037d0: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
+000037e0: 616c 732f 6261 7365 6461 7461 7365 742e  als/basedataset.
+000037f0: 6874 6d6c 290a 2020 2020 2020 2020 2d20  html).        - 
+00003800: 5b44 6174 6120 5472 616e 7366 6f72 6d5d  [Data Transform]
+00003810: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
+00003820: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00003830: 2f65 6e2f 6c61 7465 7374 2f61 6476 616e  /en/latest/advan
+00003840: 6365 645f 7475 746f 7269 616c 732f 6461  ced_tutorials/da
+00003850: 7461 5f74 7261 6e73 666f 726d 2e68 746d  ta_transform.htm
+00003860: 6c29 0a20 2020 2020 2020 202d 205b 5765  l).        - [We
+00003870: 6967 6874 2049 6e69 7469 616c 697a 6174  ight Initializat
+00003880: 696f 6e5d 2868 7474 7073 3a2f 2f6d 6d65  ion](https://mme
+00003890: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+000038a0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f61  s.io/en/latest/a
+000038b0: 6476 616e 6365 645f 7475 746f 7269 616c  dvanced_tutorial
+000038c0: 732f 696e 6974 6961 6c69 7a65 2e68 746d  s/initialize.htm
+000038d0: 6c29 0a20 2020 2020 2020 202d 205b 5669  l).        - [Vi
+000038e0: 7375 616c 697a 6174 696f 6e5d 2868 7474  sualization](htt
+000038f0: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
+00003900: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00003910: 6c61 7465 7374 2f61 6476 616e 6365 645f  latest/advanced_
+00003920: 7475 746f 7269 616c 732f 7669 7375 616c  tutorials/visual
+00003930: 697a 6174 696f 6e2e 6874 6d6c 290a 2020  ization.html).  
+00003940: 2020 2020 2020 2d20 5b41 6273 7472 6163        - [Abstrac
+00003950: 7420 4461 7461 2045 6c65 6d65 6e74 5d28  t Data Element](
+00003960: 6874 7470 733a 2f2f 6d6d 656e 6769 6e65  https://mmengine
+00003970: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00003980: 656e 2f6c 6174 6573 742f 6164 7661 6e63  en/latest/advanc
+00003990: 6564 5f74 7574 6f72 6961 6c73 2f64 6174  ed_tutorials/dat
+000039a0: 615f 656c 656d 656e 742e 6874 6d6c 290a  a_element.html).
+000039b0: 2020 2020 2020 2020 2d20 5b44 6973 7472          - [Distr
+000039c0: 6962 7574 696f 6e20 436f 6d6d 756e 6963  ibution Communic
+000039d0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6d  ation](https://m
+000039e0: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+000039f0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003a00: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
+00003a10: 616c 732f 6469 7374 7269 6275 7465 642e  als/distributed.
+00003a20: 6874 6d6c 290a 2020 2020 2020 2020 2d20  html).        - 
+00003a30: 5b4c 6f67 6769 6e67 5d28 6874 7470 733a  [Logging](https:
+00003a40: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+00003a50: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00003a60: 6573 742f 6164 7661 6e63 6564 5f74 7574  est/advanced_tut
+00003a70: 6f72 6961 6c73 2f6c 6f67 6769 6e67 2e68  orials/logging.h
+00003a80: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
+00003a90: 4669 6c65 2049 4f5d 2868 7474 7073 3a2f  File IO](https:/
+00003aa0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+00003ab0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00003ac0: 7374 2f61 6476 616e 6365 645f 7475 746f  st/advanced_tuto
+00003ad0: 7269 616c 732f 6669 6c65 696f 2e68 746d  rials/fileio.htm
+00003ae0: 6c29 0a20 2020 2020 2020 202d 205b 476c  l).        - [Gl
+00003af0: 6f62 616c 206d 616e 6167 6572 2028 4d61  obal manager (Ma
+00003b00: 6e61 6765 724d 6978 696e 295d 2868 7474  nagerMixin)](htt
+00003b10: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
+00003b20: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00003b30: 6c61 7465 7374 2f61 6476 616e 6365 645f  latest/advanced_
+00003b40: 7475 746f 7269 616c 732f 6d61 6e61 6765  tutorials/manage
+00003b50: 725f 6d69 7869 6e2e 6874 6d6c 290a 2020  r_mixin.html).  
+00003b60: 2020 2020 2020 2d20 5b55 7365 206d 6f64        - [Use mod
+00003b70: 756c 6573 2066 726f 6d20 6f74 6865 7220  ules from other 
+00003b80: 6c69 6272 6172 6965 735d 2868 7474 7073  libraries](https
+00003b90: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
+00003ba0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00003bb0: 7465 7374 2f61 6476 616e 6365 645f 7475  test/advanced_tu
+00003bc0: 746f 7269 616c 732f 6372 6f73 735f 6c69  torials/cross_li
+00003bd0: 6272 6172 792e 6874 6d6c 290a 2020 2020  brary.html).    
+00003be0: 2020 2020 2d20 5b54 6573 7420 5469 6d65      - [Test Time
+00003bf0: 2041 6775 6d65 6e74 6174 696f 6e5d 2868   Agumentation](h
+00003c00: 7474 7073 3a2f 2f6d 6d65 6e67 696e 652e  ttps://mmengine.
+00003c10: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00003c20: 6e2f 6c61 7465 7374 2f61 6476 616e 6365  n/latest/advance
+00003c30: 645f 7475 746f 7269 616c 732f 7465 7374  d_tutorials/test
+00003c40: 5f74 696d 655f 6175 676d 656e 7461 7469  _time_augmentati
+00003c50: 6f6e 2e68 746d 6c29 0a20 2020 2020 2020  on.html).       
+00003c60: 200a 2020 2020 2020 2020 3c2f 6465 7461   .        </deta
+00003c70: 696c 733e 0a20 2020 2020 2020 200a 2020  ils>.        .  
+00003c80: 2020 2020 2020 3c64 6574 6169 6c73 3e0a        <details>.
+00003c90: 2020 2020 2020 2020 3c73 756d 6d61 7279          <summary
+00003ca0: 3e45 7861 6d70 6c65 733c 2f73 756d 6d61  >Examples</summa
+00003cb0: 7279 3e0a 2020 2020 2020 2020 0a20 2020  ry>.        .   
+00003cc0: 2020 2020 202d 205b 5472 6169 6e20 6120       - [Train a 
+00003cd0: 4741 4e5d 2868 7474 7073 3a2f 2f6d 6d65  GAN](https://mme
+00003ce0: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+00003cf0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f65  s.io/en/latest/e
+00003d00: 7861 6d70 6c65 732f 7472 6169 6e5f 615f  xamples/train_a_
+00003d10: 6761 6e2e 6874 6d6c 290a 2020 2020 2020  gan.html).      
+00003d20: 2020 0a20 2020 2020 2020 203c 2f64 6574    .        </det
+00003d30: 6169 6c73 3e0a 2020 2020 2020 2020 0a20  ails>.        . 
+00003d40: 2020 2020 2020 203c 6465 7461 696c 733e         <details>
+00003d50: 0a20 2020 2020 2020 203c 7375 6d6d 6172  .        <summar
+00003d60: 793e 436f 6d6d 6f6e 2055 7361 6765 3c2f  y>Common Usage</
+00003d70: 7375 6d6d 6172 793e 0a20 2020 2020 2020  summary>.       
+00003d80: 200a 2020 2020 2020 2020 2d20 5b52 6573   .        - [Res
+00003d90: 756d 6520 5472 6169 6e69 6e67 5d28 6874  ume Training](ht
+00003da0: 7470 733a 2f2f 6d6d 656e 6769 6e65 2e72  tps://mmengine.r
+00003db0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00003dc0: 2f6c 6174 6573 742f 636f 6d6d 6f6e 5f75  /latest/common_u
+00003dd0: 7361 6765 2f72 6573 756d 655f 7472 6169  sage/resume_trai
+00003de0: 6e69 6e67 2e68 746d 6c29 0a20 2020 2020  ning.html).     
+00003df0: 2020 202d 205b 5370 6565 6420 7570 2054     - [Speed up T
+00003e00: 7261 696e 696e 675d 2868 7474 7073 3a2f  raining](https:/
+00003e10: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+00003e20: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00003e30: 7374 2f63 6f6d 6d6f 6e5f 7573 6167 652f  st/common_usage/
+00003e40: 7370 6565 645f 7570 5f74 7261 696e 696e  speed_up_trainin
+00003e50: 672e 6874 6d6c 290a 2020 2020 2020 2020  g.html).        
+00003e60: 2d20 5b53 6176 6520 4d65 6d6f 7279 206f  - [Save Memory o
+00003e70: 6e20 4750 555d 2868 7474 7073 3a2f 2f6d  n GPU](https://m
+00003e80: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00003e90: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003ea0: 2f63 6f6d 6d6f 6e5f 7573 6167 652f 7361  /common_usage/sa
+00003eb0: 7665 5f67 7075 5f6d 656d 6f72 792e 6874  ve_gpu_memory.ht
+00003ec0: 6d6c 290a 2020 2020 2020 2020 0a20 2020  ml).        .   
+00003ed0: 2020 2020 203c 2f64 6574 6169 6c73 3e0a       </details>.
+00003ee0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003ef0: 203c 6465 7461 696c 733e 0a20 2020 2020   <details>.     
+00003f00: 2020 203c 7375 6d6d 6172 793e 4465 7369     <summary>Desi
+00003f10: 676e 3c2f 7375 6d6d 6172 793e 0a20 2020  gn</summary>.   
+00003f20: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00003f30: 5b48 6f6f 6b5d 2868 7474 7073 3a2f 2f6d  [Hook](https://m
+00003f40: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00003f50: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003f60: 2f64 6573 6967 6e2f 686f 6f6b 2e68 746d  /design/hook.htm
+00003f70: 6c29 0a20 2020 2020 2020 202d 205b 5275  l).        - [Ru
+00003f80: 6e6e 6572 5d28 6874 7470 733a 2f2f 6d6d  nner](https://mm
+00003f90: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
+00003fa0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00003fb0: 6465 7369 676e 2f72 756e 6e65 722e 6874  design/runner.ht
+00003fc0: 6d6c 290a 2020 2020 2020 2020 2d20 5b45  ml).        - [E
+00003fd0: 7661 6c75 6174 696f 6e5d 2868 7474 7073  valuation](https
+00003fe0: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
+00003ff0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00004000: 7465 7374 2f64 6573 6967 6e2f 6576 616c  test/design/eval
+00004010: 7561 7469 6f6e 2e68 746d 6c29 0a20 2020  uation.html).   
+00004020: 2020 2020 202d 205b 5669 7375 616c 697a       - [Visualiz
+00004030: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6d  ation](https://m
+00004040: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00004050: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00004060: 2f64 6573 6967 6e2f 7669 7375 616c 697a  /design/visualiz
+00004070: 6174 696f 6e2e 6874 6d6c 290a 2020 2020  ation.html).    
+00004080: 2020 2020 2d20 5b4c 6f67 6769 6e67 5d28      - [Logging](
+00004090: 6874 7470 733a 2f2f 6d6d 656e 6769 6e65  https://mmengine
+000040a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+000040b0: 656e 2f6c 6174 6573 742f 6465 7369 676e  en/latest/design
+000040c0: 2f6c 6f67 6769 6e67 2e68 746d 6c29 0a20  /logging.html). 
+000040d0: 2020 2020 2020 202d 205b 496e 6665 725d         - [Infer]
+000040e0: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
+000040f0: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00004100: 2f65 6e2f 6c61 7465 7374 2f64 6573 6967  /en/latest/desig
+00004110: 6e2f 696e 6665 722e 6874 6d6c 290a 2020  n/infer.html).  
+00004120: 2020 2020 2020 0a20 2020 2020 2020 203c        .        <
+00004130: 2f64 6574 6169 6c73 3e0a 2020 2020 2020  /details>.      
+00004140: 2020 0a20 2020 2020 2020 203c 6465 7461    .        <deta
+00004150: 696c 733e 0a20 2020 2020 2020 203c 7375  ils>.        <su
+00004160: 6d6d 6172 793e 4d69 6772 6174 696f 6e20  mmary>Migration 
+00004170: 6775 6964 653c 2f73 756d 6d61 7279 3e0a  guide</summary>.
+00004180: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004190: 202d 205b 4d69 6772 6174 6520 5275 6e6e   - [Migrate Runn
+000041a0: 6572 2066 726f 6d20 4d4d 4356 2074 6f20  er from MMCV to 
+000041b0: 4d4d 456e 6769 6e65 5d28 6874 7470 733a  MMEngine](https:
+000041c0: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+000041d0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+000041e0: 6573 742f 6d69 6772 6174 696f 6e2f 7275  est/migration/ru
+000041f0: 6e6e 6572 2e68 746d 6c29 0a20 2020 2020  nner.html).     
+00004200: 2020 202d 205b 4d69 6772 6174 6520 486f     - [Migrate Ho
+00004210: 6f6b 2066 726f 6d20 4d4d 4356 2074 6f20  ok from MMCV to 
+00004220: 4d4d 456e 6769 6e65 5d28 6874 7470 733a  MMEngine](https:
+00004230: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+00004240: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00004250: 6573 742f 6d69 6772 6174 696f 6e2f 686f  est/migration/ho
+00004260: 6f6b 2e68 746d 6c29 0a20 2020 2020 2020  ok.html).       
+00004270: 202d 205b 4d69 6772 6174 6520 4d6f 6465   - [Migrate Mode
+00004280: 6c20 6672 6f6d 204d 4d43 5620 746f 204d  l from MMCV to M
+00004290: 4d45 6e67 696e 655d 2868 7474 7073 3a2f  MEngine](https:/
+000042a0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+000042b0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000042c0: 7374 2f6d 6967 7261 7469 6f6e 2f6d 6f64  st/migration/mod
+000042d0: 656c 2e68 746d 6c29 0a20 2020 2020 2020  el.html).       
+000042e0: 202d 205b 4d69 6772 6174 6520 5061 7261   - [Migrate Para
+000042f0: 6d65 7465 7220 5363 6865 6475 6c65 7220  meter Scheduler 
+00004300: 6672 6f6d 204d 4d43 5620 746f 204d 4d45  from MMCV to MME
+00004310: 6e67 696e 655d 2868 7474 7073 3a2f 2f6d  ngine](https://m
+00004320: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00004330: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00004340: 2f6d 6967 7261 7469 6f6e 2f70 6172 616d  /migration/param
+00004350: 5f73 6368 6564 756c 6572 2e68 746d 6c29  _scheduler.html)
+00004360: 0a20 2020 2020 2020 202d 205b 4d69 6772  .        - [Migr
+00004370: 6174 6520 4461 7461 2054 7261 6e73 666f  ate Data Transfo
+00004380: 726d 2074 6f20 4f70 656e 4d4d 4c61 6220  rm to OpenMMLab 
+00004390: 322e 305d 2868 7474 7073 3a2f 2f6d 6d65  2.0](https://mme
+000043a0: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+000043b0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6d  s.io/en/latest/m
+000043c0: 6967 7261 7469 6f6e 2f74 7261 6e73 666f  igration/transfo
+000043d0: 726d 2e68 746d 6c29 0a20 2020 2020 2020  rm.html).       
+000043e0: 200a 2020 2020 2020 2020 3c2f 6465 7461   .        </deta
+000043f0: 696c 733e 0a20 2020 2020 2020 200a 2020  ils>.        .  
+00004400: 2020 2020 2020 2323 2043 6f6e 7472 6962        ## Contrib
+00004410: 7574 696e 670a 2020 2020 2020 2020 0a20  uting.        . 
+00004420: 2020 2020 2020 2057 6520 6170 7072 6563         We apprec
+00004430: 6961 7465 2061 6c6c 2063 6f6e 7472 6962  iate all contrib
+00004440: 7574 696f 6e73 2074 6f20 696d 7072 6f76  utions to improv
+00004450: 6520 4d4d 456e 6769 6e65 2e20 506c 6561  e MMEngine. Plea
+00004460: 7365 2072 6566 6572 2074 6f20 5b43 4f4e  se refer to [CON
+00004470: 5452 4942 5554 494e 472e 6d64 5d28 434f  TRIBUTING.md](CO
+00004480: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
+00004490: 6f72 2074 6865 2063 6f6e 7472 6962 7574  or the contribut
+000044a0: 696e 6720 6775 6964 656c 696e 652e 0a20  ing guideline.. 
+000044b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000044c0: 2323 2043 6974 6174 696f 6e0a 2020 2020  ## Citation.    
+000044d0: 2020 2020 0a20 2020 2020 2020 2049 6620      .        If 
+000044e0: 796f 7520 6669 6e64 2074 6869 7320 7072  you find this pr
+000044f0: 6f6a 6563 7420 7573 6566 756c 2069 6e20  oject useful in 
+00004500: 796f 7572 2072 6573 6561 7263 682c 2070  your research, p
+00004510: 6c65 6173 6520 636f 6e73 6964 6572 2063  lease consider c
+00004520: 6974 653a 0a20 2020 2020 2020 200a 2020  ite:.        .  
+00004530: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00004540: 2020 4061 7274 6963 6c65 7b6d 6d65 6e67    @article{mmeng
+00004550: 696e 6532 3032 322c 0a20 2020 2020 2020  ine2022,.       
+00004560: 2020 2074 6974 6c65 2020 203d 207b 7b4d     title   = {{M
+00004570: 4d45 6e67 696e 657d 3a20 4f70 656e 4d4d  MEngine}: OpenMM
+00004580: 4c61 6220 466f 756e 6461 7469 6f6e 616c  Lab Foundational
+00004590: 204c 6962 7261 7279 2066 6f72 2054 7261   Library for Tra
+000045a0: 696e 696e 6720 4465 6570 204c 6561 726e  ining Deep Learn
+000045b0: 696e 6720 4d6f 6465 6c73 7d2c 0a20 2020  ing Models},.   
+000045c0: 2020 2020 2020 2061 7574 686f 7220 203d         author  =
+000045d0: 207b 4d4d 456e 6769 6e65 2043 6f6e 7472   {MMEngine Contr
+000045e0: 6962 7574 6f72 737d 2c0a 2020 2020 2020  ibutors},.      
+000045f0: 2020 2020 686f 7770 7562 6c69 7368 6564      howpublished
+00004600: 203d 207b 5c75 726c 7b68 7474 7073 3a2f   = {\url{https:/
+00004610: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
+00004620: 2d6d 6d6c 6162 2f6d 6d65 6e67 696e 657d  -mmlab/mmengine}
+00004630: 7d2c 0a20 2020 2020 2020 2020 2079 6561  },.          yea
+00004640: 723d 7b32 3032 327d 0a20 2020 2020 2020  r={2022}.       
+00004650: 207d 0a20 2020 2020 2020 2060 6060 0a20   }.        ```. 
+00004660: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00004670: 2323 204c 6963 656e 7365 0a20 2020 2020  ## License.     
+00004680: 2020 200a 2020 2020 2020 2020 5468 6973     .        This
+00004690: 2070 726f 6a65 6374 2069 7320 7265 6c65   project is rele
+000046a0: 6173 6564 2075 6e64 6572 2074 6865 205b  ased under the [
+000046b0: 4170 6163 6865 2032 2e30 206c 6963 656e  Apache 2.0 licen
+000046c0: 7365 5d28 4c49 4345 4e53 4529 2e0a 2020  se](LICENSE)..  
+000046d0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000046e0: 2320 5072 6f6a 6563 7473 2069 6e20 4f70  # Projects in Op
+000046f0: 656e 4d4d 4c61 620a 2020 2020 2020 2020  enMMLab.        
+00004700: 0a20 2020 2020 2020 202d 205b 4d49 4d5d  .        - [MIM]
+00004710: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004720: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
+00004730: 696d 293a 204d 494d 2069 6e73 7461 6c6c  im): MIM install
+00004740: 7320 4f70 656e 4d4d 4c61 6220 7061 636b  s OpenMMLab pack
+00004750: 6167 6573 2e0a 2020 2020 2020 2020 2d20  ages..        - 
+00004760: 5b4d 4d43 565d 2868 7474 7073 3a2f 2f67  [MMCV](https://g
+00004770: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004780: 6d6c 6162 2f6d 6d63 7629 3a20 4f70 656e  mlab/mmcv): Open
+00004790: 4d4d 4c61 6220 666f 756e 6461 7469 6f6e  MMLab foundation
+000047a0: 616c 206c 6962 7261 7279 2066 6f72 2063  al library for c
+000047b0: 6f6d 7075 7465 7220 7669 7369 6f6e 2e0a  omputer vision..
+000047c0: 2020 2020 2020 2020 2d20 5b4d 4d45 7661          - [MMEva
+000047d0: 6c5d 2868 7474 7073 3a2f 2f67 6974 6875  l](https://githu
+000047e0: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
+000047f0: 2f6d 6d65 7661 6c29 3a20 4120 756e 6966  /mmeval): A unif
+00004800: 6965 6420 6576 616c 7561 7469 6f6e 206c  ied evaluation l
+00004810: 6962 7261 7279 2066 6f72 206d 756c 7469  ibrary for multi
+00004820: 706c 6520 6d61 6368 696e 6520 6c65 6172  ple machine lear
+00004830: 6e69 6e67 206c 6962 7261 7269 6573 2e0a  ning libraries..
+00004840: 2020 2020 2020 2020 2d20 5b4d 4d50 7265          - [MMPre
+00004850: 5472 6169 6e5d 2868 7474 7073 3a2f 2f67  Train](https://g
+00004860: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004870: 6d6c 6162 2f6d 6d70 7265 7472 6169 6e29  mlab/mmpretrain)
+00004880: 3a20 4f70 656e 4d4d 4c61 6220 7072 652d  : OpenMMLab pre-
+00004890: 7472 6169 6e69 6e67 2074 6f6f 6c62 6f78  training toolbox
+000048a0: 2061 6e64 2062 656e 6368 6d61 726b 2e0a   and benchmark..
+000048b0: 2020 2020 2020 2020 2d20 5b4d 4d61 6769          - [MMagi
+000048c0: 635d 2868 7474 7073 3a2f 2f67 6974 6875  c](https://githu
+000048d0: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
+000048e0: 2f6d 6d61 6769 6329 3a20 4f70 656e 2a2a  /mmagic): Open**
+000048f0: 4d4d 2a2a 4c61 6220 2a2a 412a 2a64 7661  MM**Lab **A**dva
+00004900: 6e63 6564 2c20 2a2a 472a 2a65 6e65 7261  nced, **G**enera
+00004910: 7469 7665 2061 6e64 202a 2a49 2a2a 6e74  tive and **I**nt
+00004920: 656c 6c69 6765 6e74 202a 2a43 2a2a 7265  elligent **C**re
+00004930: 6174 696f 6e20 746f 6f6c 626f 782e 0a20  ation toolbox.. 
+00004940: 2020 2020 2020 202d 205b 4d4d 4465 7465         - [MMDete
+00004950: 6374 696f 6e5d 2868 7474 7073 3a2f 2f67  ction](https://g
+00004960: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004970: 6d6c 6162 2f6d 6d64 6574 6563 7469 6f6e  mlab/mmdetection
+00004980: 293a 204f 7065 6e4d 4d4c 6162 2064 6574  ): OpenMMLab det
+00004990: 6563 7469 6f6e 2074 6f6f 6c62 6f78 2061  ection toolbox a
+000049a0: 6e64 2062 656e 6368 6d61 726b 2e0a 2020  nd benchmark..  
+000049b0: 2020 2020 2020 2d20 5b4d 4d59 4f4c 4f5d        - [MMYOLO]
+000049c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000049d0: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
+000049e0: 6d79 6f6c 6f29 3a20 4f70 656e 4d4d 4c61  myolo): OpenMMLa
+000049f0: 6220 594f 4c4f 2073 6572 6965 7320 746f  b YOLO series to
+00004a00: 6f6c 626f 7820 616e 6420 6265 6e63 686d  olbox and benchm
+00004a10: 6172 6b2e 0a20 2020 2020 2020 202d 205b  ark..        - [
+00004a20: 4d4d 4465 7465 6374 696f 6e33 445d 2868  MMDetection3D](h
+00004a30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004a40: 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d 6d64  m/open-mmlab/mmd
+00004a50: 6574 6563 7469 6f6e 3364 293a 204f 7065  etection3d): Ope
+00004a60: 6e4d 4d4c 6162 2773 206e 6578 742d 6765  nMMLab's next-ge
+00004a70: 6e65 7261 7469 6f6e 2070 6c61 7466 6f72  neration platfor
+00004a80: 6d20 666f 7220 6765 6e65 7261 6c20 3344  m for general 3D
+00004a90: 206f 626a 6563 7420 6465 7465 6374 696f   object detectio
+00004aa0: 6e2e 0a20 2020 2020 2020 202d 205b 4d4d  n..        - [MM
+00004ab0: 526f 7461 7465 5d28 6874 7470 733a 2f2f  Rotate](https://
+00004ac0: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e2d  github.com/open-
+00004ad0: 6d6d 6c61 622f 6d6d 726f 7461 7465 293a  mmlab/mmrotate):
+00004ae0: 204f 7065 6e4d 4d4c 6162 2072 6f74 6174   OpenMMLab rotat
+00004af0: 6564 206f 626a 6563 7420 6465 7465 6374  ed object detect
+00004b00: 696f 6e20 746f 6f6c 626f 7820 616e 6420  ion toolbox and 
+00004b10: 6265 6e63 686d 6172 6b2e 0a20 2020 2020  benchmark..     
+00004b20: 2020 202d 205b 4d4d 5472 6163 6b69 6e67     - [MMTracking
+00004b30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004b40: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
+00004b50: 6d6d 7472 6163 6b69 6e67 293a 204f 7065  mmtracking): Ope
+00004b60: 6e4d 4d4c 6162 2076 6964 656f 2070 6572  nMMLab video per
+00004b70: 6365 7074 696f 6e20 746f 6f6c 626f 7820  ception toolbox 
+00004b80: 616e 6420 6265 6e63 686d 6172 6b2e 0a20  and benchmark.. 
+00004b90: 2020 2020 2020 202d 205b 4d4d 506f 7365         - [MMPose
+00004ba0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004bb0: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
+00004bc0: 6d6d 706f 7365 293a 204f 7065 6e4d 4d4c  mmpose): OpenMML
+00004bd0: 6162 2070 6f73 6520 6573 7469 6d61 7469  ab pose estimati
+00004be0: 6f6e 2074 6f6f 6c62 6f78 2061 6e64 2062  on toolbox and b
+00004bf0: 656e 6368 6d61 726b 2e0a 2020 2020 2020  enchmark..      
+00004c00: 2020 2d20 5b4d 4d53 6567 6d65 6e74 6174    - [MMSegmentat
+00004c10: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
+00004c20: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
+00004c30: 6162 2f6d 6d73 6567 6d65 6e74 6174 696f  ab/mmsegmentatio
+00004c40: 6e29 3a20 4f70 656e 4d4d 4c61 6220 7365  n): OpenMMLab se
+00004c50: 6d61 6e74 6963 2073 6567 6d65 6e74 6174  mantic segmentat
+00004c60: 696f 6e20 746f 6f6c 626f 7820 616e 6420  ion toolbox and 
+00004c70: 6265 6e63 686d 6172 6b2e 0a20 2020 2020  benchmark..     
+00004c80: 2020 202d 205b 4d4d 4f43 525d 2868 7474     - [MMOCR](htt
+00004c90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004ca0: 6f70 656e 2d6d 6d6c 6162 2f6d 6d6f 6372  open-mmlab/mmocr
+00004cb0: 293a 204f 7065 6e4d 4d4c 6162 2074 6578  ): OpenMMLab tex
+00004cc0: 7420 6465 7465 6374 696f 6e2c 2072 6563  t detection, rec
+00004cd0: 6f67 6e69 7469 6f6e 2c20 616e 6420 756e  ognition, and un
+00004ce0: 6465 7273 7461 6e64 696e 6720 746f 6f6c  derstanding tool
+00004cf0: 626f 782e 0a20 2020 2020 2020 202d 205b  box..        - [
+00004d00: 4d4d 4875 6d61 6e33 445d 2868 7474 7073  MMHuman3D](https
+00004d10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f70  ://github.com/op
+00004d20: 656e 2d6d 6d6c 6162 2f6d 6d68 756d 616e  en-mmlab/mmhuman
+00004d30: 3364 293a 204f 7065 6e4d 4d4c 6162 2033  3d): OpenMMLab 3
+00004d40: 4420 6875 6d61 6e20 7061 7261 6d65 7472  D human parametr
+00004d50: 6963 206d 6f64 656c 2074 6f6f 6c62 6f78  ic model toolbox
+00004d60: 2061 6e64 2062 656e 6368 6d61 726b 2e0a   and benchmark..
+00004d70: 2020 2020 2020 2020 2d20 5b4d 4d53 656c          - [MMSel
+00004d80: 6653 7570 5d28 6874 7470 733a 2f2f 6769  fSup](https://gi
+00004d90: 7468 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d  thub.com/open-mm
+00004da0: 6c61 622f 6d6d 7365 6c66 7375 7029 3a20  lab/mmselfsup): 
+00004db0: 4f70 656e 4d4d 4c61 6220 7365 6c66 2d73  OpenMMLab self-s
+00004dc0: 7570 6572 7669 7365 6420 6c65 6172 6e69  upervised learni
+00004dd0: 6e67 2074 6f6f 6c62 6f78 2061 6e64 2062  ng toolbox and b
+00004de0: 656e 6368 6d61 726b 2e0a 2020 2020 2020  enchmark..      
+00004df0: 2020 2d20 5b4d 4d46 6577 5368 6f74 5d28    - [MMFewShot](
+00004e00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004e10: 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f 6d6d  om/open-mmlab/mm
+00004e20: 6665 7773 686f 7429 3a20 4f70 656e 4d4d  fewshot): OpenMM
+00004e30: 4c61 6220 6665 7773 686f 7420 6c65 6172  Lab fewshot lear
+00004e40: 6e69 6e67 2074 6f6f 6c62 6f78 2061 6e64  ning toolbox and
+00004e50: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
+00004e60: 2020 2020 2d20 5b4d 4d41 6374 696f 6e32      - [MMAction2
+00004e70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004e80: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
+00004e90: 6d6d 6163 7469 6f6e 3229 3a20 4f70 656e  mmaction2): Open
+00004ea0: 4d4d 4c61 6227 7320 6e65 7874 2d67 656e  MMLab's next-gen
+00004eb0: 6572 6174 696f 6e20 6163 7469 6f6e 2075  eration action u
+00004ec0: 6e64 6572 7374 616e 6469 6e67 2074 6f6f  nderstanding too
+00004ed0: 6c62 6f78 2061 6e64 2062 656e 6368 6d61  lbox and benchma
+00004ee0: 726b 2e0a 2020 2020 2020 2020 2d20 5b4d  rk..        - [M
+00004ef0: 4d46 6c6f 775d 2868 7474 7073 3a2f 2f67  MFlow](https://g
+00004f00: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004f10: 6d6c 6162 2f6d 6d66 6c6f 7729 3a20 4f70  mlab/mmflow): Op
+00004f20: 656e 4d4d 4c61 6220 6f70 7469 6361 6c20  enMMLab optical 
+00004f30: 666c 6f77 2074 6f6f 6c62 6f78 2061 6e64  flow toolbox and
+00004f40: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
+00004f50: 2020 2020 2d20 5b4d 4d44 6570 6c6f 795d      - [MMDeploy]
+00004f60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004f70: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
+00004f80: 6d64 6570 6c6f 7929 3a20 4f70 656e 4d4d  mdeploy): OpenMM
+00004f90: 4c61 6220 6d6f 6465 6c20 6465 706c 6f79  Lab model deploy
+00004fa0: 6d65 6e74 2066 7261 6d65 776f 726b 2e0a  ment framework..
+00004fb0: 2020 2020 2020 2020 2d20 5b4d 4d52 617a          - [MMRaz
+00004fc0: 6f72 5d28 6874 7470 733a 2f2f 6769 7468  or](https://gith
+00004fd0: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
+00004fe0: 622f 6d6d 7261 7a6f 7229 3a20 4f70 656e  b/mmrazor): Open
+00004ff0: 4d4d 4c61 6220 6d6f 6465 6c20 636f 6d70  MMLab model comp
+00005000: 7265 7373 696f 6e20 746f 6f6c 626f 7820  ression toolbox 
+00005010: 616e 6420 6265 6e63 686d 6172 6b2e 0a20  and benchmark.. 
+00005020: 2020 2020 2020 202d 205b 506c 6179 6772         - [Playgr
+00005030: 6f75 6e64 5d28 6874 7470 733a 2f2f 6769  ound](https://gi
+00005040: 7468 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d  thub.com/open-mm
+00005050: 6c61 622f 706c 6179 6772 6f75 6e64 293a  lab/playground):
+00005060: 2041 2063 656e 7472 616c 2068 7562 2066   A central hub f
+00005070: 6f72 2067 6174 6865 7269 6e67 2061 6e64  or gathering and
+00005080: 2073 686f 7763 6173 696e 6720 616d 617a   showcasing amaz
+00005090: 696e 6720 7072 6f6a 6563 7473 2062 7569  ing projects bui
+000050a0: 6c74 2075 706f 6e20 4f70 656e 4d4d 4c61  lt upon OpenMMLa
+000050b0: 622e 0a20 2020 2020 2020 200a 506c 6174  b..        .Plat
+000050c0: 666f 726d 3a20 554e 4b4e 4f57 4e0a 436c  form: UNKNOWN.Cl
+000050d0: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
+000050e0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000050f0: 3420 2d20 4265 7461 0a43 6c61 7373 6966  4 - Beta.Classif
+00005100: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
+00005110: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00005120: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
+00005130: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+00005140: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00005150: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00005160: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
+00005170: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00005180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00005190: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+000051a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000051b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000051c0: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
+000051d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000051e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000051f0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00005200: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00005210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00005220: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00005230: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00005240: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00005250: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00005260: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00005270: 6320 3a3a 2055 7469 6c69 7469 6573 0a52  c :: Utilities.R
+00005280: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+00005290: 3e3d 332e 370a 4465 7363 7269 7074 696f  >=3.7.Descriptio
+000052a0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+000052b0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
+000052c0: 6f76 6964 6573 2d45 7874 7261 3a20 616c  ovides-Extra: al
+000052d0: 6c0a 5072 6f76 6964 6573 2d45 7874 7261  l.Provides-Extra
+000052e0: 3a20 7465 7374 730a                      : tests.
```

### Comparing `mmengine-0.7.4/README.md` & `mmengine-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,36 @@
   <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
 </div>
 
+## What's New
+
+v0.8.0 was released on 2023-06-30.
+
+Highlights:
+
+- Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [example](https://github.com/open-mmlab/mmengine/blob/main/examples/distributed_training_with_flexible_runner.py) for more detailed usages.
+
+- Introduce the pure Python style configuration file:
+
+  - Support navigating to base configuration file in IDE
+  - Support navigating to base variable in IDE
+  - Support navigating to source code of class in IDE
+  - Support inheriting two configuration files containing the same field
+  - Load the configuration file without other third-party requirements
+
+  Refer to the [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) for more detailed usages.
+
+  ![new-config-en](https://github.com/open-mmlab/mmengine/assets/57566630/7eb41748-9374-488f-901e-fcd7f0d3c8a1)
+
+Read [Changelog](./docs/en/notes/changelog.md#v080-06302023) for more details.
+
 ## Introduction
 
 MMEngine is a foundational library for training deep learning models based on PyTorch. It provides a solid engineering foundation and frees developers from writing redundant codes on workflows. It serves as the training engine of all OpenMMLab codebases, which support hundreds of algorithms in various research areas. Moreover, MMEngine is also generic to be applied to non-OpenMMLab projects.
 
 Major features:
 
 1. **A universal and powerful runner**:
@@ -74,25 +96,14 @@
 
 3. **Customizable training process**:
 
    - Defines the training process just like playing with Legos.
    - Provides rich components and strategies.
    - Complete controls on the training process with different levels of APIs.
 
-## What's New
-
-v0.7.4 was released on 2023-06-03.
-
-### Highlights
-
-- Support using [`ClearML`](https://mmengine.readthedocs.io/en/latest/common_usage/visualize_training_log.html#clearml) to record experiment data
-- Add [`Sophia`](https://mmengine.readthedocs.io/en/latest/common_usage/better_optimizers.html#sophia) optimizers
-
-Read [Changelog](./docs/en/notes/changelog.md#v074-06032023) for more details.
-
 ## Installation
 
 Before installing MMEngine, please ensure that PyTorch has been successfully installed following the [official guide](https://pytorch.org/get-started/locally/).
 
 Install MMEngine
 
 ```bash
```

### Comparing `mmengine-0.7.4/mmengine/analysis/complexity_analysis.py` & `mmengine-0.8.0/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/analysis/jit_analysis.py` & `mmengine-0.8.0/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/analysis/jit_handles.py` & `mmengine-0.8.0/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/analysis/print_helper.py` & `mmengine-0.8.0/mmengine/analysis/print_helper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/config/config.py` & `mmengine-0.8.0/mmengine/config/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,27 +7,31 @@
 import shutil
 import sys
 import tempfile
 import types
 import uuid
 import warnings
 from argparse import Action, ArgumentParser, Namespace
-from collections import abc
+from collections import OrderedDict, abc
+from contextlib import contextmanager
 from pathlib import Path
 from typing import Any, Optional, Sequence, Tuple, Union
 
 from addict import Dict
 from yapf.yapflib.yapf_api import FormatCode
 
 from mmengine.fileio import dump, load
 from mmengine.logging import print_log
 from mmengine.utils import (check_file_exist, get_installed_path,
                             import_modules_from_strings, is_installed)
-from .utils import (RemoveAssignFromAST, _get_external_cfg_base_path,
-                    _get_external_cfg_path, _get_package_and_cfg_path)
+from .lazy import LazyAttr, LazyObject
+from .utils import (ConfigParsingError, ImportTransformer, RemoveAssignFromAST,
+                    _gather_abs_import_lazyobj, _get_external_cfg_base_path,
+                    _get_external_cfg_path, _get_package_and_cfg_path,
+                    _is_builtin_module)
 
 BASE_KEY = '_base_'
 DELETE_KEY = '_delete_'
 DEPRECATION_KEY = '_deprecation_'
 RESERVED_KEYS = ['filename', 'text', 'pretty_text', 'env_variables']
 
 if platform.system() == 'Windows':
@@ -38,30 +42,236 @@
 
 class ConfigDict(Dict):
     """A dictionary for config which has the same interface as python's built-
     in dictionary and can be used as a normal dictionary.
 
     The Config class would transform the nested fields (dictionary-like fields)
     in config file into ``ConfigDict``.
+
+    If the class attribute ``lazy``  is ``False``, users will get the
+    object built by ``LazyObject`` or ``LazyAttr``, otherwise users will get
+    the ``LazyObject`` or ``LazyAttr`` itself.
+
+    The ``lazy`` should be set to ``True`` to avoid building the imported
+    object during configuration parsing, and it should be set to False outside
+    the Config to ensure that users do not experience the ``LazyObject``.
     """
+    lazy = False
+
+    def __init__(__self, *args, **kwargs):
+        object.__setattr__(__self, '__parent', kwargs.pop('__parent', None))
+        object.__setattr__(__self, '__key', kwargs.pop('__key', None))
+        object.__setattr__(__self, '__frozen', False)
+        for arg in args:
+            if not arg:
+                continue
+            # Since ConfigDict.items will convert LazyObject to real object
+            # automatically, we need to call super().items() to make sure
+            # the LazyObject will not be converted.
+            if isinstance(arg, ConfigDict):
+                for key, val in dict.items(arg):
+                    __self[key] = __self._hook(val)
+            elif isinstance(arg, dict):
+                for key, val in arg.items():
+                    __self[key] = __self._hook(val)
+            elif isinstance(arg, tuple) and (not isinstance(arg[0], tuple)):
+                __self[arg[0]] = __self._hook(arg[1])
+            else:
+                for key, val in iter(arg):
+                    __self[key] = __self._hook(val)
+
+        for key, val in dict.items(kwargs):
+            __self[key] = __self._hook(val)
 
     def __missing__(self, name):
         raise KeyError(name)
 
     def __getattr__(self, name):
         try:
             value = super().__getattr__(name)
+            if isinstance(value, (LazyAttr, LazyObject)) and not self.lazy:
+                value = value.build()
         except KeyError:
             raise AttributeError(f"'{self.__class__.__name__}' object has no "
                                  f"attribute '{name}'")
         except Exception as e:
             raise e
         else:
             return value
 
+    @classmethod
+    def _hook(cls, item):
+        # avoid to convert user defined dict to ConfigDict.
+        if type(item) in (dict, OrderedDict):
+            return cls(item)
+        elif isinstance(item, (list, tuple)):
+            return type(item)(cls._hook(elem) for elem in item)
+        return item
+
+    def __setattr__(self, name, value):
+        value = self._hook(value)
+        return super().__setattr__(name, value)
+
+    def __setitem__(self, name, value):
+        value = self._hook(value)
+        return super().__setitem__(name, value)
+
+    def __getitem__(self, key):
+        return self.build_lazy(super().__getitem__(key))
+
+    def __deepcopy__(self, memo):
+        other = self.__class__()
+        memo[id(self)] = other
+        for key, value in super().items():
+            other[copy.deepcopy(key, memo)] = copy.deepcopy(value, memo)
+        return other
+
+    def __copy__(self):
+        other = self.__class__()
+        for key, value in super().items():
+            other[key] = value
+        return other
+
+    copy = __copy__
+
+    def __iter__(self):
+        # Implement `__iter__` to overwrite the unpacking operator `**cfg_dict`
+        # to get the built lazy object
+        return iter(self.keys())
+
+    def get(self, key: str, default: Optional[Any] = None) -> Any:
+        """Get the value of the key. If class attribute ``lazy`` is True, the
+        LazyObject will be built and returned.
+
+        Args:
+            key (str): The key.
+            default (any, optional): The default value. Defaults to None.
+
+        Returns:
+            Any: The value of the key.
+        """
+        return self.build_lazy(super().get(key, default))
+
+    def pop(self, key, default=None):
+        """Pop the value of the key. If class attribute ``lazy`` is True, the
+        LazyObject will be built and returned.
+
+        Args:
+            key (str): The key.
+            default (any, optional): The default value. Defaults to None.
+
+        Returns:
+            Any: The value of the key.
+        """
+        return self.build_lazy(super().pop(key, default))
+
+    def update(self, *args, **kwargs) -> None:
+        """Override this method to make sure the LazyObject will not be built
+        during updating."""
+        other = {}
+        if args:
+            if len(args) > 1:
+                raise TypeError('update only accept one positional argument')
+            # Avoid to used self.items to build LazyObject
+            for key, value in dict.items(args[0]):
+                other[key] = value
+
+        for key, value in dict(kwargs).items():
+            other[key] = value
+        for k, v in other.items():
+            if ((k not in self) or (not isinstance(self[k], dict))
+                    or (not isinstance(v, dict))):
+                self[k] = self._hook(v)
+            else:
+                self[k].update(v)
+
+    def build_lazy(self, value: Any) -> Any:
+        """If class attribute ``lazy`` is False, the LazyObject will be built
+        and returned.
+
+        Args:
+            value (Any): The value to be built.
+
+        Returns:
+            Any: The built value.
+        """
+        if isinstance(value, (LazyAttr, LazyObject)) and not self.lazy:
+            value = value.build()
+        return value
+
+    def values(self):
+        """Yield the values of the dictionary.
+
+        If class attribute ``lazy`` is False, the value of ``LazyObject`` or
+        ``LazyAttr`` will be built and returned.
+        """
+        values = []
+        for value in super().values():
+            values.append(self.build_lazy(value))
+        return values
+
+    def items(self):
+        """Yield the keys and values of the dictionary.
+
+        If class attribute ``lazy`` is False, the value of ``LazyObject`` or
+        ``LazyAttr`` will be built and returned.
+        """
+        items = []
+        for key, value in super().items():
+            items.append((key, self.build_lazy(value)))
+        return items
+
+    def merge(self, other: dict):
+        """Merge another dictionary into current dictionary.
+
+        Args:
+            other (dict): Another dictionary.
+        """
+        default = object()
+
+        def _merge_a_into_b(a, b):
+            if isinstance(a, dict):
+                if not isinstance(b, dict):
+                    a.pop(DELETE_KEY, None)
+                    return a
+                if a.pop(DELETE_KEY, False):
+                    b.clear()
+                all_keys = list(b.keys()) + list(a.keys())
+                return {
+                    key:
+                    _merge_a_into_b(a.get(key, default), b.get(key, default))
+                    for key in all_keys if key != DELETE_KEY
+                }
+            else:
+                return a if a is not default else b
+
+        merged = _merge_a_into_b(copy.deepcopy(other), copy.deepcopy(self))
+        self.clear()
+        for key, value in merged.items():
+            self[key] = value
+
+    def to_dict(self):
+        """Convert the ConfigDict to a normal dictionary recursively, and keep
+        the ``LazyObject`` or ``LazyAttr`` object not built."""
+
+        def _to_dict(data):
+            if isinstance(data, ConfigDict):
+                return {
+                    key: _to_dict(value)
+                    for key, value in Dict.items(data)
+                }
+            elif isinstance(data, dict):
+                return {key: _to_dict(value) for key, value in data.items()}
+            elif isinstance(data, (list, tuple)):
+                return type(data)(_to_dict(item) for item in data)
+            else:
+                return data
+
+        return _to_dict(self)
+
 
 def add_args(parser: ArgumentParser,
              cfg: dict,
              prefix: str = '') -> ArgumentParser:
     """Add config fields into argument parser.
 
     Args:
@@ -105,14 +315,16 @@
 
     Args:
         cfg_dict (dict, optional): A config dictionary. Defaults to None.
         cfg_text (str, optional): Text of config. Defaults to None.
         filename (str or Path, optional): Name of config file.
             Defaults to None.
 
+    Here is a simple example:
+
     Examples:
         >>> cfg = Config(dict(a=1, b=dict(b1=[0, 1])))
         >>> cfg.a
         1
         >>> cfg.b
         {'b1': [0, 1]}
         >>> cfg.b.b1
@@ -122,15 +334,19 @@
         "/home/username/projects/mmengine/tests/data/config/a.py"
         >>> cfg.item4
         'test'
         >>> cfg
         "Config [path: /home/username/projects/mmengine/tests/data/config/a.py]
         :"
         "{'item1': [1, 2], 'item2': {'a': 0}, 'item3': True, 'item4': 'test'}"
-    """
+
+    You can find more advance usage in the `config tutorial`_.
+
+    .. _config tutorial: https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html
+    """  # noqa: E501
 
     def __init__(self,
                  cfg_dict: dict = None,
                  cfg_text: Optional[str] = None,
                  filename: Optional[Union[str, Path]] = None,
                  env_variables: Optional[dict] = None):
         filename = str(filename) if isinstance(filename, Path) else filename
@@ -139,15 +355,17 @@
         elif not isinstance(cfg_dict, dict):
             raise TypeError('cfg_dict must be a dict, but '
                             f'got {type(cfg_dict)}')
         for key in cfg_dict:
             if key in RESERVED_KEYS:
                 raise KeyError(f'{key} is reserved for config file')
 
-        super().__setattr__('_cfg_dict', ConfigDict(cfg_dict))
+        if not isinstance(cfg_dict, ConfigDict):
+            cfg_dict = ConfigDict(cfg_dict)
+        super().__setattr__('_cfg_dict', cfg_dict)
         super().__setattr__('_filename', filename)
         if cfg_text:
             text = cfg_text
         elif filename:
             with open(filename, encoding='utf-8') as f:
                 text = f.read()
         else:
@@ -157,48 +375,78 @@
             env_variables = dict()
         super().__setattr__('_env_variables', env_variables)
 
     @staticmethod
     def fromfile(filename: Union[str, Path],
                  use_predefined_variables: bool = True,
                  import_custom_modules: bool = True,
-                 use_environment_variables: bool = True) -> 'Config':
+                 use_environment_variables: bool = True,
+                 lazy_import: Optional[bool] = None) -> 'Config':
         """Build a Config instance from config file.
 
         Args:
             filename (str or Path): Name of config file.
             use_predefined_variables (bool, optional): Whether to use
                 predefined variables. Defaults to True.
             import_custom_modules (bool, optional): Whether to support
-                importing custom modules in config. Defaults to True.
+                importing custom modules in config. Defaults to None.
+            lazy_import (bool): Whether to load config in `lazy_import` mode.
+                If it is `None`, it will be deduced by the content of the
+                config file. Defaults to None.
 
         Returns:
             Config: Config instance built from config file.
         """
         filename = str(filename) if isinstance(filename, Path) else filename
-        cfg_dict, cfg_text, env_variables = Config._file2dict(
-            filename, use_predefined_variables, use_environment_variables)
-        if import_custom_modules and cfg_dict.get('custom_imports', None):
+        if lazy_import is None:
+            lazy_import = Config._is_lazy_import(filename)
+        if not lazy_import:
+            cfg_dict, cfg_text, env_variables = Config._file2dict(
+                filename, use_predefined_variables, use_environment_variables)
+            if import_custom_modules and cfg_dict.get('custom_imports', None):
+                try:
+                    import_modules_from_strings(**cfg_dict['custom_imports'])
+                except ImportError as e:
+                    err_msg = (
+                        'Failed to import custom modules from '
+                        f"{cfg_dict['custom_imports']}, the current sys.path "
+                        'is: ')
+                    for p in sys.path:
+                        err_msg += f'\n    {p}'
+                    err_msg += (
+                        '\nYou should set `PYTHONPATH` to make `sys.path` '
+                        'include the directory which contains your custom '
+                        'module')
+                    raise ImportError(err_msg) from e
+            return Config(
+                cfg_dict,
+                cfg_text=cfg_text,
+                filename=filename,
+                env_variables=env_variables)
+        else:
+            # Enable lazy import when parsing the config.
+            # Using try-except to make sure ``ConfigDict.lazy`` will be reset
+            # to False. See more details about lazy in the docstring of
+            # ConfigDict
+            ConfigDict.lazy = True
             try:
-                import_modules_from_strings(**cfg_dict['custom_imports'])
-            except ImportError as e:
-                err_msg = (
-                    'Failed to import custom modules from '
-                    f"{cfg_dict['custom_imports']}, the current sys.path is: ")
-                for p in sys.path:
-                    err_msg += f'\n    {p}'
-                err_msg += (
-                    '\nYou should set `PYTHONPATH` to make `sys.path` include '
-                    'the directory which contains your custom module')
-                raise ImportError(err_msg) from e
-        return Config(
-            cfg_dict,
-            cfg_text=cfg_text,
-            filename=filename,
-            env_variables=env_variables)
+                cfg_dict, imported_names = Config._parse_lazy_import(filename)
+            except Exception as e:
+                raise e
+            finally:
+                ConfigDict.lazy = False
+            for key, value in list(cfg_dict.to_dict().items()):
+                if isinstance(value, (types.FunctionType, types.ModuleType)):
+                    cfg_dict.pop(key)
+
+            # disable lazy import to get the real type. See more details about
+            # lazy in the docstring of ConfigDict
+            cfg = Config(cfg_dict, filename=filename)
+            object.__setattr__(cfg, '_imported_names', imported_names)
+            return cfg
 
     @staticmethod
     def fromstring(cfg_str: str, file_format: str) -> 'Config':
         """Build a Config instance from config text.
 
         Args:
             cfg_str (str): Config text.
@@ -229,14 +477,88 @@
             temp_file.write(cfg_str)
 
         cfg = Config.fromfile(temp_file.name)
         os.remove(temp_file.name)  # manually delete the temporary file
         return cfg
 
     @staticmethod
+    def _get_base_modules(nodes: list) -> list:
+        """Get base module name from parsed code.
+
+        Args:
+            nodes (list): Parsed code of the config file.
+
+        Returns:
+            list: Name of base modules.
+        """
+
+        def _get_base_module_from_with(with_nodes: list) -> list:
+            """Get base module name from if statement in python file.
+
+            Args:
+                with_nodes (list): List of if statement.
+
+            Returns:
+                list: Name of base modules.
+            """
+            base_modules = []
+            for node in with_nodes:
+                assert isinstance(node, ast.ImportFrom), (
+                    'Illegal syntax in config file! Only '
+                    '`from ... import ...` could be implemented` in '
+                    'with read_base()`')
+                assert node.module is not None, (
+                    'Illegal syntax in config file! Syntax like '
+                    '`from . import xxx` is not allowed in `with read_base()`')
+                base_modules.append(node.level * '.' + node.module)
+            return base_modules
+
+        for idx, node in enumerate(nodes):
+            if (isinstance(node, ast.Assign)
+                    and isinstance(node.targets[0], ast.Name)
+                    and node.targets[0].id == BASE_KEY):
+                raise ConfigParsingError(
+                    'The configuration file type in the inheritance chain '
+                    'must match the current configuration file type, either '
+                    '"lazy_import" or non-"lazy_import". You got this error '
+                    f'since you use the syntax like `_base_ = "{node.targets[0].id}"` '  # noqa: E501
+                    'in your config. You should use `with read_base(): ... to` '  # noqa: E501
+                    'mark the inherited config file. See more information '
+                    'in https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html'  # noqa: E501
+                )
+
+            if not isinstance(node, ast.With):
+                continue
+
+            expr = node.items[0].context_expr
+            if (not isinstance(expr, ast.Call)
+                    or not expr.func.id == 'read_base' or  # type: ignore
+                    len(node.items) > 1):
+                raise ConfigParsingError(
+                    'Only `read_base` context manager can be used in the '
+                    'config')
+
+            # The original code:
+            # ```
+            # with read_base():
+            #     from .._base_.default_runtime import *
+            # ```
+            # The processed code:
+            # ```
+            # from .._base_.default_runtime import *
+            # ```
+            # As you can see, the if statement is removed and the
+            # from ... import statement will be unindent
+            for nested_idx, nested_node in enumerate(node.body):
+                nodes.insert(idx + nested_idx + 1, nested_node)
+            nodes.pop(idx)
+            return _get_base_module_from_with(node.body)
+        return []
+
+    @staticmethod
     def _validate_py_syntax(filename: str):
         """Validate syntax of python config.
 
         Args:
             filename (str): Filename of python config file.
         """
         with open(filename, encoding='utf-8') as f:
@@ -450,97 +772,115 @@
             filename (str): Name of config file.
             use_predefined_variables (bool, optional): Whether to use
                 predefined variables. Defaults to True.
 
         Returns:
             Tuple[dict, str]: Variables dictionary and text of Config.
         """
+        if Config._is_lazy_import(filename):
+            raise RuntimeError(
+                'The configuration file type in the inheritance chain '
+                'must match the current configuration file type, either '
+                '"lazy_import" or non-"lazy_import". You got this error '
+                'since you use the syntax like `with read_base(): ...` '
+                f'or import non-builtin module in {filename}. See more '
+                'information in https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html'  # noqa: E501
+            )
+
         filename = osp.abspath(osp.expanduser(filename))
         check_file_exist(filename)
         fileExtname = osp.splitext(filename)[1]
         if fileExtname not in ['.py', '.json', '.yaml', '.yml']:
             raise OSError('Only py/yml/yaml/json type are supported now!')
+        try:
+            with tempfile.TemporaryDirectory() as temp_config_dir:
+                temp_config_file = tempfile.NamedTemporaryFile(
+                    dir=temp_config_dir, suffix=fileExtname, delete=False)
+                if platform.system() == 'Windows':
+                    temp_config_file.close()
+
+                # Substitute predefined variables
+                if use_predefined_variables:
+                    Config._substitute_predefined_vars(filename,
+                                                       temp_config_file.name)
+                else:
+                    shutil.copyfile(filename, temp_config_file.name)
+                # Substitute environment variables
+                env_variables = dict()
+                if use_environment_variables:
+                    env_variables = Config._substitute_env_variables(
+                        temp_config_file.name, temp_config_file.name)
+                # Substitute base variables from placeholders to strings
+                base_var_dict = Config._pre_substitute_base_vars(
+                    temp_config_file.name, temp_config_file.name)
 
-        with tempfile.TemporaryDirectory() as temp_config_dir:
-            temp_config_file = tempfile.NamedTemporaryFile(
-                dir=temp_config_dir, suffix=fileExtname)
-            if platform.system() == 'Windows':
+                # Handle base files
+                base_cfg_dict = ConfigDict()
+                cfg_text_list = list()
+                for base_cfg_path in Config._get_base_files(
+                        temp_config_file.name):
+                    base_cfg_path, scope = Config._get_cfg_path(
+                        base_cfg_path, filename)
+                    _cfg_dict, _cfg_text, _env_variables = Config._file2dict(
+                        filename=base_cfg_path,
+                        use_predefined_variables=use_predefined_variables,
+                        use_environment_variables=use_environment_variables)
+                    cfg_text_list.append(_cfg_text)
+                    env_variables.update(_env_variables)
+                    duplicate_keys = base_cfg_dict.keys() & _cfg_dict.keys()
+                    if len(duplicate_keys) > 0:
+                        raise KeyError(
+                            'Duplicate key is not allowed among bases. '
+                            f'Duplicate keys: {duplicate_keys}')
+
+                    # _dict_to_config_dict will do the following things:
+                    # 1. Recursively converts ``dict`` to :obj:`ConfigDict`.
+                    # 2. Set `_scope_` for the outer dict variable for the base
+                    # config.
+                    # 3. Set `scope` attribute for each base variable.
+                    # Different from `_scope_`， `scope` is not a key of base
+                    # dict, `scope` attribute will be parsed to key `_scope_`
+                    # by function `_parse_scope` only if the base variable is
+                    # accessed by the current config.
+                    _cfg_dict = Config._dict_to_config_dict(_cfg_dict, scope)
+                    base_cfg_dict.update(_cfg_dict)
+
+                if filename.endswith('.py'):
+                    with open(temp_config_file.name, encoding='utf-8') as f:
+                        parsed_codes = ast.parse(f.read())
+                        parsed_codes = RemoveAssignFromAST(BASE_KEY).visit(
+                            parsed_codes)
+                    codeobj = compile(parsed_codes, '', mode='exec')
+                    # Support load global variable in nested function of the
+                    # config.
+                    global_locals_var = {BASE_KEY: base_cfg_dict}
+                    ori_keys = set(global_locals_var.keys())
+                    eval(codeobj, global_locals_var, global_locals_var)
+                    cfg_dict = {
+                        key: value
+                        for key, value in global_locals_var.items()
+                        if (key not in ori_keys and not key.startswith('__'))
+                    }
+                elif filename.endswith(('.yml', '.yaml', '.json')):
+                    cfg_dict = load(temp_config_file.name)
+                # close temp file
+                for key, value in list(cfg_dict.items()):
+                    if isinstance(value,
+                                  (types.FunctionType, types.ModuleType)):
+                        cfg_dict.pop(key)
                 temp_config_file.close()
 
-            # Substitute predefined variables
-            if use_predefined_variables:
-                Config._substitute_predefined_vars(filename,
-                                                   temp_config_file.name)
-            else:
-                shutil.copyfile(filename, temp_config_file.name)
-            # Substitute environment variables
-            env_variables = dict()
-            if use_environment_variables:
-                env_variables = Config._substitute_env_variables(
-                    temp_config_file.name, temp_config_file.name)
-            # Substitute base variables from placeholders to strings
-            base_var_dict = Config._pre_substitute_base_vars(
-                temp_config_file.name, temp_config_file.name)
-
-            # Handle base files
-            base_cfg_dict = ConfigDict()
-            cfg_text_list = list()
-            for base_cfg_path in Config._get_base_files(temp_config_file.name):
-                base_cfg_path, scope = Config._get_cfg_path(
-                    base_cfg_path, filename)
-                _cfg_dict, _cfg_text, _env_variables = Config._file2dict(
-                    filename=base_cfg_path,
-                    use_predefined_variables=use_predefined_variables,
-                    use_environment_variables=use_environment_variables)
-                cfg_text_list.append(_cfg_text)
-                env_variables.update(_env_variables)
-                duplicate_keys = base_cfg_dict.keys() & _cfg_dict.keys()
-                if len(duplicate_keys) > 0:
-                    raise KeyError('Duplicate key is not allowed among bases. '
-                                   f'Duplicate keys: {duplicate_keys}')
-
-                # _dict_to_config_dict will do the following things:
-                # 1. Recursively converts ``dict`` to :obj:`ConfigDict`.
-                # 2. Set `_scope_` for the outer dict variable for the base
-                # config.
-                # 3. Set `scope` attribute for each base variable. Different
-                # from `_scope_`， `scope` is not a key of base dict,
-                # `scope` attribute will be parsed to key `_scope_` by
-                # function `_parse_scope` only if the base variable is
-                # accessed by the current config.
-                _cfg_dict = Config._dict_to_config_dict(_cfg_dict, scope)
-                base_cfg_dict.update(_cfg_dict)
-
-            if filename.endswith('.py'):
-                with open(temp_config_file.name, encoding='utf-8') as f:
-                    codes = ast.parse(f.read())
-                    codes = RemoveAssignFromAST(BASE_KEY).visit(codes)
-                codeobj = compile(codes, '', mode='exec')
-                # Support load global variable in nested function of the
-                # config.
-                global_locals_var = {'_base_': base_cfg_dict}
-                ori_keys = set(global_locals_var.keys())
-                eval(codeobj, global_locals_var, global_locals_var)
-                cfg_dict = {
-                    key: value
-                    for key, value in global_locals_var.items()
-                    if (key not in ori_keys and not key.startswith('__'))
-                }
-            elif filename.endswith(('.yml', '.yaml', '.json')):
-                cfg_dict = load(temp_config_file.name)
-            # close temp file
-            for key, value in list(cfg_dict.items()):
-                if isinstance(value, (types.FunctionType, types.ModuleType)):
-                    cfg_dict.pop(key)
-            temp_config_file.close()
-
-            # If the current config accesses a base variable of base
-            # configs, The ``scope`` attribute of corresponding variable
-            # will be converted to the `_scope_`.
-            Config._parse_scope(cfg_dict)
+                # If the current config accesses a base variable of base
+                # configs, The ``scope`` attribute of corresponding variable
+                # will be converted to the `_scope_`.
+                Config._parse_scope(cfg_dict)
+        except Exception as e:
+            if osp.exists(temp_config_dir):
+                shutil.rmtree(temp_config_dir)
+            raise e
 
         # check deprecation information
         if DEPRECATION_KEY in cfg_dict:
             deprecation_info = cfg_dict.pop(DEPRECATION_KEY)
             warning_msg = f'The config file {filename} will be deprecated ' \
                 'in the future.'
             if 'expected' in deprecation_info:
@@ -570,14 +910,177 @@
         # merge cfg_text
         cfg_text_list.append(cfg_text)
         cfg_text = '\n'.join(cfg_text_list)
 
         return cfg_dict, cfg_text, env_variables
 
     @staticmethod
+    def _parse_lazy_import(filename: str) -> Tuple[ConfigDict, set]:
+        """Transform file to variables dictionary.
+
+        Args:
+            filename (str): Name of config file.
+
+        Returns:
+            Tuple[dict, dict]: ``cfg_dict`` and ``imported_names``.
+
+              - cfg_dict (dict): Variables dictionary of parsed config.
+              - imported_names (set): Used to mark the names of
+                imported object.
+        """
+        # In lazy import mode, users can use the Python syntax `import` to
+        # implement inheritance between configuration files, which is easier
+        # for users to understand the hierarchical relationships between
+        # different configuration files.
+
+        # Besides, users can also using `import` syntax to import corresponding
+        # module which will be filled in the `type` field. It means users
+        # can directly navigate to the source of the module in the
+        # configuration file by clicking the `type` field.
+
+        # To avoid really importing the third party package like `torch`
+        # during import `type` object, we use `_parse_lazy_import` to parse the
+        # configuration file, which will not actually trigger the import
+        # process, but simply parse the imported `type`s as LazyObject objects.
+
+        # The overall pipeline of _parse_lazy_import is:
+        # 1. Parse the base module from the config file.
+        #                       ||
+        #                       \/
+        #       base_module = ['mmdet.configs.default_runtime']
+        #                       ||
+        #                       \/
+        # 2. recursively parse the base module and gather imported objects to
+        #    a dict.
+        #                       ||
+        #                       \/
+        #       The base_dict will be:
+        #       {
+        #           'mmdet.configs.default_runtime': {...}
+        #           'mmdet.configs.retinanet_r50_fpn_1x_coco': {...}
+        #           ...
+        #       }, each item in base_dict is a dict of `LazyObject`
+        # 3. parse the current config file filling the imported variable
+        #    with the base_dict.
+        #
+        # 4. During the parsing process, all imported variable will be
+        #    recorded in the `imported_names` set. These variables can be
+        #    accessed, but will not be dumped by default.
+
+        with open(filename, encoding='utf-8') as f:
+            global_dict = {'LazyObject': LazyObject}
+            base_dict = {}
+
+            parsed_codes = ast.parse(f.read())
+            # get the names of base modules, and remove the
+            # `with read_base():'` statement
+            base_modules = Config._get_base_modules(parsed_codes.body)
+            base_imported_names = set()
+            for base_module in base_modules:
+                # If base_module means a relative import, assuming the level is
+                # 2, which means the module is imported like
+                # "from ..a.b import c". we must ensure that c is an
+                # object `defined` in module b, and module b should not be a
+                # package including `__init__` file but a single python file.
+                level = len(re.match(r'\.*', base_module).group())
+                if level > 0:
+                    # Relative import
+                    base_dir = osp.dirname(filename)
+                    module_path = osp.join(
+                        base_dir, *(['..'] * (level - 1)),
+                        f'{base_module[level:].replace(".", "/")}.py')
+                else:
+                    # Absolute import
+                    module_list = base_module.split('.')
+                    if len(module_list) == 1:
+                        raise ConfigParsingError(
+                            'The imported configuration file should not be '
+                            f'an independent package {module_list[0]}. Here '
+                            'is an example: '
+                            '`with read_base(): from mmdet.configs.retinanet_r50_fpn_1x_coco import *`'  # noqa: E501
+                        )
+                    else:
+                        package = module_list[0]
+                        root_path = get_installed_path(package)
+                        module_path = f'{osp.join(root_path, *module_list[1:])}.py'  # noqa: E501
+                if not osp.isfile(module_path):
+                    raise ConfigParsingError(
+                        f'{module_path} not found! It means that incorrect '
+                        'module is defined in '
+                        f'`with read_base(): = from {base_module} import ...`, please '  # noqa: E501
+                        'make sure the base config module is valid '
+                        'and is consistent with the prior import '
+                        'logic')
+                _base_cfg_dict, _base_imported_names = Config._parse_lazy_import(  # noqa: E501
+                    module_path)
+                base_imported_names |= _base_imported_names
+                # The base_dict will be:
+                # {
+                #     'mmdet.configs.default_runtime': {...}
+                #     'mmdet.configs.retinanet_r50_fpn_1x_coco': {...}
+                #     ...
+                # }
+                base_dict[base_module] = _base_cfg_dict
+
+            # `base_dict` contains all the imported modules from `base_cfg`.
+            # In order to collect the specific imported module from `base_cfg`
+            # before parse the current file, we using AST Transform to
+            # transverse the imported module from base_cfg and merge then into
+            # the global dict. After the ast transformation, most of import
+            # syntax will be removed (except for the builtin import) and
+            # replaced with the `LazyObject`
+            transform = ImportTransformer(
+                global_dict=global_dict,
+                base_dict=base_dict,
+                filename=filename)
+            modified_code = transform.visit(parsed_codes)
+            modified_code, abs_imported = _gather_abs_import_lazyobj(
+                modified_code, filename=filename)
+            imported_names = transform.imported_obj | abs_imported
+            imported_names |= base_imported_names
+            modified_code = ast.fix_missing_locations(modified_code)
+            exec(
+                compile(modified_code, filename, mode='exec'), global_dict,
+                global_dict)
+
+            ret: dict = {}
+            for key, value in global_dict.items():
+                if key.startswith('__') or key in ['LazyObject']:
+                    continue
+                ret[key] = value
+            # convert dict to ConfigDict
+            cfg_dict = Config._dict_to_config_dict_lazy(ret)
+
+            return cfg_dict, imported_names
+
+    @staticmethod
+    def _dict_to_config_dict_lazy(cfg: dict):
+        """Recursively converts ``dict`` to :obj:`ConfigDict`. The only
+        difference between ``_dict_to_config_dict_lazy`` and
+        ``_dict_to_config_dict_lazy`` is that the former one does not consider
+        the scope, and will not trigger the building of ``LazyObject``.
+
+        Args:
+            cfg (dict): Config dict.
+
+        Returns:
+            ConfigDict: Converted dict.
+        """
+        # Only the outer dict with key `type` should have the key `_scope_`.
+        if isinstance(cfg, dict):
+            cfg_dict = ConfigDict()
+            for key, value in cfg.items():
+                cfg_dict[key] = Config._dict_to_config_dict_lazy(value)
+            return cfg_dict
+        if isinstance(cfg, (tuple, list)):
+            return type(cfg)(
+                Config._dict_to_config_dict_lazy(_cfg) for _cfg in cfg)
+        return cfg
+
+    @staticmethod
     def _dict_to_config_dict(cfg: dict,
                              scope: Optional[str] = None,
                              has_scope=True):
         """Recursively converts ``dict`` to :obj:`ConfigDict`.
 
         Args:
             cfg (dict): Config dict.
@@ -640,22 +1143,23 @@
         Returns:
             list: A list of base config.
         """
         file_format = osp.splitext(filename)[1]
         if file_format == '.py':
             Config._validate_py_syntax(filename)
             with open(filename, encoding='utf-8') as f:
-                codes = ast.parse(f.read()).body
+                parsed_codes = ast.parse(f.read()).body
 
                 def is_base_line(c):
                     return (isinstance(c, ast.Assign)
                             and isinstance(c.targets[0], ast.Name)
                             and c.targets[0].id == BASE_KEY)
 
-                base_code = next((c for c in codes if is_base_line(c)), None)
+                base_code = next((c for c in parsed_codes if is_base_line(c)),
+                                 None)
                 if base_code is not None:
                     base_code = ast.Expression(  # type: ignore
                         body=base_code.value)  # type: ignore
                     base_files = eval(compile(base_code, '', mode='eval'))
                 else:
                     base_files = []
         elif file_format in ('.yml', '.yaml', '.json'):
@@ -813,41 +1317,59 @@
             s = '\n'.join(s)
             s = first + '\n' + s
             return s
 
         def _format_basic_types(k, v, use_mapping=False):
             if isinstance(v, str):
                 v_str = repr(v)
+            elif isinstance(v, (LazyObject, LazyAttr)):
+                v_str = f"'{v.module}.{str(v)}'"
             else:
                 v_str = str(v)
 
             if use_mapping:
                 k_str = f"'{k}'" if isinstance(k, str) else str(k)
                 attr_str = f'{k_str}: {v_str}'
             else:
                 attr_str = f'{str(k)}={v_str}'
             attr_str = _indent(attr_str, indent)
 
             return attr_str
 
-        def _format_list(k, v, use_mapping=False):
+        def _format_list_tuple(k, v, use_mapping=False):
+            if isinstance(v, list):
+                left = '['
+                right = ']'
+            else:
+                left = '('
+                right = ')'
+
+            v_str = f'{left}\n'
             # check if all items in the list are dict
-            if all(isinstance(_, dict) for _ in v):
-                v_str = '[\n'
-                v_str += '\n'.join(
-                    f'dict({_indent(_format_dict(v_), indent)}),'
-                    for v_ in v).rstrip(',')
-                if use_mapping:
-                    k_str = f"'{k}'" if isinstance(k, str) else str(k)
-                    attr_str = f'{k_str}: {v_str}'
+            for item in v:
+                if isinstance(item, dict):
+                    v_str += f'dict({_indent(_format_dict(item), indent)}),\n'
+                elif isinstance(item, tuple):
+                    v_str += f'{_indent(_format_list_tuple(None, item), indent)},\n'  # noqa: 501
+                elif isinstance(item, list):
+                    v_str += f'{_indent(_format_list_tuple(None, item), indent)},\n'  # noqa: 501
+                elif isinstance(item, str):
+                    v_str += f'{_indent(repr(item), indent)},\n'
+                elif isinstance(item, (LazyObject, LazyAttr)):
+                    v_str += f"'{str(item)}',\n"
                 else:
-                    attr_str = f'{str(k)}={v_str}'
-                attr_str = _indent(attr_str, indent) + ']'
+                    v_str += str(item) + ',\n'
+            if k is None:
+                return _indent(v_str, indent) + right
+            if use_mapping:
+                k_str = f"'{k}'" if isinstance(k, str) else str(k)
+                attr_str = f'{k_str}: {v_str}'
             else:
-                attr_str = _format_basic_types(k, v, use_mapping)
+                attr_str = f'{str(k)}={v_str}'
+            attr_str = _indent(attr_str, indent) + right
             return attr_str
 
         def _contain_invalid_identifier(dict_str):
             contain_invalid_identifier = False
             for key_name in dict_str:
                 contain_invalid_identifier |= \
                     (not str(key_name).isidentifier())
@@ -859,41 +1381,47 @@
 
             use_mapping = _contain_invalid_identifier(input_dict)
             if use_mapping:
                 r += '{'
             for idx, (k, v) in enumerate(input_dict.items()):
                 is_last = idx >= len(input_dict) - 1
                 end = '' if outest_level or is_last else ','
-                if isinstance(v, dict):
+                if isinstance(v, (LazyObject, LazyAttr)):
+                    attr_str = _format_basic_types(k, v, use_mapping) + end
+                elif isinstance(v, dict):
                     v_str = '\n' + _format_dict(v)
                     if use_mapping:
                         k_str = f"'{k}'" if isinstance(k, str) else str(k)
                         attr_str = f'{k_str}: dict({v_str}'
                     else:
                         attr_str = f'{str(k)}=dict({v_str}'
                     attr_str = _indent(attr_str, indent) + ')' + end
-                elif isinstance(v, list):
-                    attr_str = _format_list(k, v, use_mapping) + end
+                elif isinstance(v, (list, tuple)):
+                    attr_str = _format_list_tuple(k, v, use_mapping) + end
                 else:
                     attr_str = _format_basic_types(k, v, use_mapping) + end
 
                 s.append(attr_str)
             r += '\n'.join(s)
             if use_mapping:
                 r += '}'
             return r
 
-        cfg_dict = self._cfg_dict.to_dict()
+        cfg_dict = self._to_lazy_dict()
         text = _format_dict(cfg_dict, outest_level=True)
         # copied from setup.cfg
         yapf_style = dict(
             based_on_style='pep8',
             blank_line_before_nested_class_or_def=True,
             split_before_expression_after_opening_paren=True)
-        text, _ = FormatCode(text, style_config=yapf_style, verify=True)
+        try:
+            text, _ = FormatCode(text, style_config=yapf_style, verify=True)
+        except:  # noqa: E722
+            raise SyntaxError('Failed to format the config file, please '
+                              f'check the syntax of: \n{text}')
 
         return text
 
     def __repr__(self):
         return f'Config (path: {self.filename}): {self._cfg_dict.__repr__()}'
 
     def __len__(self):
@@ -932,17 +1460,20 @@
 
         return other
 
     def __copy__(self):
         cls = self.__class__
         other = cls.__new__(cls)
         other.__dict__.update(self.__dict__)
+        super(Config, other).__setattr__('_cfg_dict', self._cfg_dict.copy())
 
         return other
 
+    copy = __copy__
+
     def __setstate__(self, state: Tuple[dict, Optional[str], Optional[str],
                                         dict]):
         _cfg_dict, _filename, _text, _env_variables = state
         super().__setattr__('_cfg_dict', _cfg_dict)
         super().__setattr__('_filename', _filename)
         super().__setattr__('_text', _text)
         super().__setattr__('_text', _env_variables)
@@ -1016,14 +1547,92 @@
 
         cfg_dict = super().__getattribute__('_cfg_dict')
         super().__setattr__(
             '_cfg_dict',
             Config._merge_a_into_b(
                 option_cfg_dict, cfg_dict, allow_list_keys=allow_list_keys))
 
+    @staticmethod
+    def _is_lazy_import(filename: str) -> bool:
+        if not filename.endswith('.py'):
+            return False
+        with open(filename, encoding='utf-8') as f:
+            codes_str = f.read()
+            parsed_codes = ast.parse(codes_str)
+        for node in ast.walk(parsed_codes):
+            if (isinstance(node, ast.Assign)
+                    and isinstance(node.targets[0], ast.Name)
+                    and node.targets[0].id == BASE_KEY):
+                return False
+
+            if isinstance(node, ast.With):
+                expr = node.items[0].context_expr
+                if (not isinstance(expr, ast.Call)
+                        or not expr.func.id == 'read_base'):  # type: ignore
+                    raise ConfigParsingError(
+                        'Only `read_base` context manager can be used in the '
+                        'config')
+                return True
+            if isinstance(node, ast.ImportFrom):
+                # relative import -> lazy_import
+                if node.level != 0:
+                    return True
+                # Skip checking when using `mmengine.config` in cfg file
+                if (node.module == 'mmengine' and len(node.names) == 1
+                        and node.names[0].name == 'Config'):
+                    continue
+                if not isinstance(node.module, str):
+                    continue
+                # non-builtin module -> lazy_import
+                if not _is_builtin_module(node.module):
+                    return True
+            if isinstance(node, ast.Import):
+                for alias_node in node.names:
+                    if not _is_builtin_module(alias_node.name):
+                        return True
+        return False
+
+    def _to_lazy_dict(self, keep_imported: bool = False) -> dict:
+        """Convert config object to dictionary and filter the imported
+        object."""
+        res = self._cfg_dict.to_dict()
+        if hasattr(self, '_imported_names') and not keep_imported:
+            res = {
+                key: value
+                for key, value in res.items()
+                if key not in self._imported_names
+            }
+        return res
+
+    def to_dict(self, keep_imported: bool = False):
+        """Convert all data in the config to a builtin ``dict``.
+
+        Args:
+            keep_imported (bool): Whether to keep the imported field.
+                Defaults to False
+
+        If you import third-party objects in the config file, all imported
+        objects will be converted to a string like ``torch.optim.SGD``
+        """
+        _cfg_dict = self._to_lazy_dict(keep_imported)
+
+        def lazy2string(cfg_dict):
+            if isinstance(cfg_dict, dict):
+                return type(cfg_dict)(
+                    {k: lazy2string(v)
+                     for k, v in cfg_dict.items()})
+            elif isinstance(cfg_dict, (tuple, list)):
+                return type(cfg_dict)(lazy2string(v) for v in cfg_dict)
+            elif isinstance(cfg_dict, (LazyAttr, LazyObject)):
+                return f'{cfg_dict.module}.{str(cfg_dict)}'
+            else:
+                return cfg_dict
+
+        return lazy2string(_cfg_dict)
+
 
 class DictAction(Action):
     """
     argparse action to split an argument into KEY=VALUE form
     on the first = and append to a dictionary. List options can
     be passed as comma separated values, i.e 'KEY=V1,V2,V3', or with explicit
     brackets, i.e. 'KEY=[V1,V2,V3]'. It also support nested brackets to build
@@ -1130,7 +1739,23 @@
         # Copied behavior from `argparse._ExtendAction`.
         options = copy.copy(getattr(namespace, self.dest, None) or {})
         if values is not None:
             for kv in values:
                 key, val = kv.split('=', maxsplit=1)
                 options[key] = self._parse_iterable(val)
         setattr(namespace, self.dest, options)
+
+
+@contextmanager
+def read_base():
+    """Context manager to mark the base config.
+
+    The pure Python-style configuration file allows you to use the import
+    syntax. However, it is important to note that you need to import the base
+    configuration file within the context of ``read_base``, and import other
+    dependencies outside of it.
+
+    You can see more usage of Python-style configuration in the `tutorial`_
+
+    .. _tutorial: https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta
+    """  # noqa: E501
+    yield
```

### Comparing `mmengine-0.7.4/mmengine/dataset/__init__.py` & `mmengine-0.8.0/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/dataset/base_dataset.py` & `mmengine-0.8.0/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.8.0/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/dataset/sampler.py` & `mmengine-0.8.0/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/dataset/utils.py` & `mmengine-0.8.0/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/device/utils.py` & `mmengine-0.8.0/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/dist/__init__.py` & `mmengine-0.8.0/mmengine/dist/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
                    collect_results, gather, broadcast, gather_object,
                    sync_random_seed, broadcast_object_list,
                    collect_results_cpu, collect_results_gpu, all_reduce_params)
 from .utils import (get_dist_info, init_dist, init_local_group, get_backend,
                     get_world_size, get_rank, get_local_size, get_local_rank,
                     is_main_process, master_only, barrier, get_local_group,
                     is_distributed, get_default_group, get_data_device,
-                    get_comm_device, cast_data_device)
+                    get_comm_device, cast_data_device, infer_launcher)
 
 __all__ = [
     'all_gather_object', 'all_reduce', 'all_gather', 'all_reduce_dict',
     'collect_results', 'collect_results_cpu', 'collect_results_gpu', 'gather',
     'broadcast', 'gather_object', 'sync_random_seed', 'broadcast_object_list',
     'get_dist_info', 'init_dist', 'init_local_group', 'get_backend',
     'get_world_size', 'get_rank', 'get_local_size', 'get_local_group',
     'get_local_rank', 'is_main_process', 'master_only', 'barrier',
     'is_distributed', 'get_default_group', 'all_reduce_params',
-    'get_data_device', 'get_comm_device', 'cast_data_device'
+    'get_data_device', 'get_comm_device', 'cast_data_device', 'infer_launcher'
 ]
```

### Comparing `mmengine-0.7.4/mmengine/dist/dist.py` & `mmengine-0.8.0/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/dist/utils.py` & `mmengine-0.8.0/mmengine/dist/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,29 @@
 
 def get_default_group() -> Optional[ProcessGroup]:
     """Return default process group."""
 
     return torch_dist.distributed_c10d._get_default_group()
 
 
-def init_dist(launcher, backend='nccl', **kwargs) -> None:
+def infer_launcher():
+    if 'WORLD_SIZE' in os.environ:
+        return 'pytorch'
+    elif 'SLURM_NTASKS' in os.environ:
+        return 'slurm'
+    elif 'OMPI_COMM_WORLD_LOCAL_RANK' in os.environ:
+        return 'mpi'
+    else:
+        return 'none'
+
+
+def init_dist(launcher,
+              backend='nccl',
+              init_backend='torch',
+              **kwargs) -> None:
     """Initialize distributed environment.
 
     Args:
         launcher (str): Way to launcher multi processes. Supported launchers
             are 'pytorch', 'mpi' and 'slurm'.
         backend (str): Communication Backends. Supported backends are 'nccl',
             'gloo' and 'mpi'. Defaults to 'nccl'.
@@ -63,24 +77,24 @@
                 f'Timeout for distributed training must be provided as '
                 f"timeout in seconds, but we've received the type "
                 f'{type(timeout)}. Please specify the timeout like this: '
                 f"dist_cfg=dict(backend='nccl', timeout=1800)") from exception
     if mp.get_start_method(allow_none=True) is None:
         mp.set_start_method('spawn')
     if launcher == 'pytorch':
-        _init_dist_pytorch(backend, **kwargs)
+        _init_dist_pytorch(backend, init_backend=init_backend, **kwargs)
     elif launcher == 'mpi':
         _init_dist_mpi(backend, **kwargs)
     elif launcher == 'slurm':
-        _init_dist_slurm(backend, **kwargs)
+        _init_dist_slurm(backend, init_backend=init_backend, **kwargs)
     else:
         raise ValueError(f'Invalid launcher type: {launcher}')
 
 
-def _init_dist_pytorch(backend, **kwargs) -> None:
+def _init_dist_pytorch(backend, init_backend='torch', **kwargs) -> None:
     """Initialize distributed environment with PyTorch launcher.
 
     Args:
         backend (str): Backend of torch.distributed. Supported backends are
             'nccl', 'gloo' and 'mpi'. Defaults to 'nccl'.
         **kwargs: keyword arguments are passed to ``init_process_group``.
     """
@@ -101,15 +115,24 @@
             rank=rank,
             world_size=int(os.environ['WORLD_SIZE']),
             **kwargs)
     else:
         # LOCAL_RANK is set by `torch.distributed.launch` since PyTorch 1.1
         local_rank = int(os.environ['LOCAL_RANK'])
         torch.cuda.set_device(local_rank)
-        torch_dist.init_process_group(backend=backend, **kwargs)
+
+        if init_backend == 'torch':
+            torch_dist.init_process_group(backend=backend, **kwargs)
+        elif init_backend == 'deepspeed':
+            import deepspeed
+            deepspeed.init_distributed(dist_backend=backend, **kwargs)
+        else:
+            raise ValueError(
+                'supported "init_backend" is "torch" or "deepspeed", '
+                f'but got {init_backend}')
 
 
 def _init_dist_mpi(backend, **kwargs) -> None:
     """Initialize distributed environment with MPI launcher.
 
     Args:
         backend (str): Backend of torch.distributed. Supported backends are
@@ -133,15 +156,18 @@
     if 'MASTER_ADDR' not in os.environ:
         raise KeyError('The environment variable MASTER_ADDR is not set')
     os.environ['WORLD_SIZE'] = os.environ['OMPI_COMM_WORLD_SIZE']
     os.environ['RANK'] = os.environ['OMPI_COMM_WORLD_RANK']
     torch_dist.init_process_group(backend=backend, **kwargs)
 
 
-def _init_dist_slurm(backend, port=None) -> None:
+def _init_dist_slurm(backend,
+                     port=None,
+                     init_backend='torch',
+                     **kwargs) -> None:
     """Initialize slurm distributed training environment.
 
     If argument ``port`` is not specified, then the master port will be system
     environment variable ``MASTER_PORT``. If ``MASTER_PORT`` is not in system
     environment variable, then a default port ``29500`` will be used.
 
     Args:
@@ -171,15 +197,23 @@
         os.environ['MASTER_PORT'] = '29500'
     # use MASTER_ADDR in the environment variable if it already exists
     if 'MASTER_ADDR' not in os.environ:
         os.environ['MASTER_ADDR'] = addr
     os.environ['WORLD_SIZE'] = str(ntasks)
     os.environ['LOCAL_RANK'] = str(local_rank)
     os.environ['RANK'] = str(proc_id)
-    torch_dist.init_process_group(backend=backend)
+
+    if init_backend == 'torch':
+        torch_dist.init_process_group(backend=backend, **kwargs)
+    elif init_backend == 'deepspeed':
+        import deepspeed
+        deepspeed.init_distributed(dist_backend=backend, **kwargs)
+    else:
+        raise ValueError('supported "init_backend" is "torch" or "deepspeed", '
+                         f'but got {init_backend}')
 
 
 def init_local_group(node_rank: int, num_gpus_per_node: int):
     """Setup the local process group.
 
     Setup a process group which only includes processes that on the same
     machine as the current process.
```

### Comparing `mmengine-0.7.4/mmengine/evaluator/evaluator.py` & `mmengine-0.8.0/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/evaluator/metric.py` & `mmengine-0.8.0/mmengine/evaluator/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         if self.collect_device == 'cpu':
             results = collect_results(
                 self.results,
                 size,
                 self.collect_device,
                 tmpdir=self.collect_dir)
         else:
-            collect_results(self.results, size, self.collect_device)
+            results = collect_results(self.results, size, self.collect_device)
 
         if is_main_process():
             # cast all tensors in results list to cpu
             results = _to_cpu(results)
             _metrics = self.compute_metrics(results)  # type: ignore
             # Add prefix to metric names
             if self.prefix:
```

### Comparing `mmengine-0.7.4/mmengine/evaluator/utils.py` & `mmengine-0.8.0/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/__init__.py` & `mmengine-0.8.0/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/__init__.py` & `mmengine-0.8.0/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/base.py` & `mmengine-0.8.0/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/http_backend.py` & `mmengine-0.8.0/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.8.0/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/local_backend.py` & `mmengine-0.8.0/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.8.0/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.8.0/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.8.0/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/file_client.py` & `mmengine-0.8.0/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/handlers/base.py` & `mmengine-0.8.0/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.8.0/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.8.0/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.8.0/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.8.0/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/io.py` & `mmengine-0.8.0/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/fileio/parse.py` & `mmengine-0.8.0/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/__init__.py` & `mmengine-0.8.0/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.8.0/mmengine/hooks/checkpoint_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,23 +514,27 @@
 
             best_ckpt_updated = True
 
             best_score = key_score
             runner.message_hub.update_info(best_score_key, best_score)
 
             if best_ckpt_path and is_main_process():
+                is_removed = False
                 if self.file_backend.isfile(best_ckpt_path):
                     self.file_backend.remove(best_ckpt_path)
-                else:
+                    is_removed = True
+                elif self.file_backend.isdir(best_ckpt_path):
                     # checkpoints saved by deepspeed are directories
                     self.file_backend.rmtree(best_ckpt_path)
+                    is_removed = True
 
-                runner.logger.info(
-                    f'The previous best checkpoint {best_ckpt_path} '
-                    'is removed')
+                if is_removed:
+                    runner.logger.info(
+                        f'The previous best checkpoint {best_ckpt_path} '
+                        'is removed')
 
             best_ckpt_name = f'best_{key_indicator}_{ckpt_filename}'
             # Replace illegal characters for filename with `_`
             best_ckpt_name = best_ckpt_name.replace('/', '_')
             if len(self.key_indicators) == 1:
                 self.best_ckpt_path = self.file_backend.join_path(  # type: ignore # noqa: E501
                     self.out_dir, best_ckpt_name)
```

### Comparing `mmengine-0.7.4/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.8.0/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/ema_hook.py` & `mmengine-0.8.0/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.8.0/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/hook.py` & `mmengine-0.8.0/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.8.0/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/logger_hook.py` & `mmengine-0.8.0/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.8.0/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.8.0/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/profiler_hook.py` & `mmengine-0.8.0/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.8.0/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.8.0/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/sync_buffer_hook.py` & `mmengine-0.8.0/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.8.0/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hub/hub.py` & `mmengine-0.8.0/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hub/mmcls.json` & `mmengine-0.8.0/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hub/openmmlab.json` & `mmengine-0.8.0/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/hub/torchvision_0.12.json` & `mmengine-0.8.0/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/infer/infer.py` & `mmengine-0.8.0/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/logging/history_buffer.py` & `mmengine-0.8.0/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/logging/logger.py` & `mmengine-0.8.0/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/logging/message_hub.py` & `mmengine-0.8.0/mmengine/logging/message_hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/__init__.py` & `mmengine-0.8.0/mmengine/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
     'uniform_init', 'kaiming_init', 'caffe2_xavier_init',
     'bias_init_with_prob', 'BaseInit', 'ConstantInit', 'XavierInit',
     'NormalInit', 'TruncNormalInit', 'UniformInit', 'KaimingInit',
     'Caffe2XavierInit', 'PretrainedInit', 'initialize',
     'convert_sync_batchnorm', 'BaseTTAModel'
 ]
 
-if digit_version(TORCH_VERSION) >= digit_version('1.11.0'):
+if digit_version(TORCH_VERSION) >= digit_version('2.0.0'):
     from .wrappers import MMFullyShardedDataParallel  # noqa:F401
     __all__.append('MMFullyShardedDataParallel')
```

### Comparing `mmengine-0.7.4/mmengine/model/averaged_model.py` & `mmengine-0.8.0/mmengine/model/averaged_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,9 +254,10 @@
 
         Args:
             averaged_param (Tensor): The averaged parameters.
             source_param (Tensor): The source parameters.
             steps (int): The number of times the parameters have been
                 updated.
         """
-        momentum = max(self.momentum, self.gamma / (self.gamma + self.steps))
+        momentum = max(self.momentum,
+                       self.gamma / (self.gamma + self.steps.item()))
         averaged_param.lerp_(source_param, momentum)
```

### Comparing `mmengine-0.7.4/mmengine/model/base_model/base_model.py` & `mmengine-0.8.0/mmengine/model/base_model/base_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.8.0/mmengine/model/base_model/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/base_module.py` & `mmengine-0.8.0/mmengine/model/base_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from logging import FileHandler
 from typing import Iterable, List, Optional, Union
 
 import torch.nn as nn
 
 from mmengine.dist import master_only
 from mmengine.logging import MMLogger, print_log
-from .weight_init import initialize, update_init_info
+from .weight_init import PretrainedInit, initialize, update_init_info
 from .wrappers.utils import is_model_wrapper
 
 
 class BaseModule(nn.Module, metaclass=ABCMeta):
     """Base module for all modules in openmmlab. ``BaseModule`` is a wrapper of
     ``torch.nn.Module`` with additional functionality of parameter
     initialization. Compared with ``torch.nn.Module``, ``BaseModule`` mainly
@@ -112,15 +112,16 @@
                 # Therefore we initialize `pretrained_cfg` last to overwrite
                 # the previous initialized weights.
                 # See details in https://github.com/open-mmlab/mmengine/issues/691 # noqa E501
                 other_cfgs = []
                 pretrained_cfg = []
                 for init_cfg in init_cfgs:
                     assert isinstance(init_cfg, dict)
-                    if init_cfg['type'] == 'Pretrained':
+                    if (init_cfg['type'] == 'Pretrained'
+                            or init_cfg['type'] is PretrainedInit):
                         pretrained_cfg.append(init_cfg)
                     else:
                         other_cfgs.append(init_cfg)
 
                 initialize(self, other_cfgs)
 
             for m in self.children():
```

### Comparing `mmengine-0.7.4/mmengine/model/test_time_aug.py` & `mmengine-0.8.0/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/utils.py` & `mmengine-0.8.0/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/weight_init.py` & `mmengine-0.8.0/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/wrappers/__init__.py` & `mmengine-0.8.0/mmengine/model/wrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 from .utils import is_model_wrapper
 
 __all__ = [
     'MMDistributedDataParallel', 'is_model_wrapper',
     'MMSeparateDistributedDataParallel'
 ]
 
-if digit_version(TORCH_VERSION) >= digit_version('1.11.0'):
+if digit_version(TORCH_VERSION) >= digit_version('2.0.0'):
     from .fully_sharded_distributed import \
         MMFullyShardedDataParallel  # noqa:F401
     __all__.append('MMFullyShardedDataParallel')
```

### Comparing `mmengine-0.7.4/mmengine/model/wrappers/distributed.py` & `mmengine-0.8.0/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.8.0/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/model/wrappers/utils.py` & `mmengine-0.8.0/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/optim/__init__.py` & `mmengine-0.8.0/mmengine/optim/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .optimizer import (OPTIM_WRAPPER_CONSTRUCTORS, OPTIMIZERS,
-                        AmpOptimWrapper, ApexOptimWrapper,
+                        AmpOptimWrapper, ApexOptimWrapper, BaseOptimWrapper,
                         DefaultOptimWrapperConstructor, OptimWrapper,
                         OptimWrapperDict, ZeroRedundancyOptimizer,
                         build_optim_wrapper)
 # yapf: disable
 from .scheduler import (ConstantLR, ConstantMomentum, ConstantParamScheduler,
                         CosineAnnealingLR, CosineAnnealingMomentum,
                         CosineAnnealingParamScheduler, ExponentialLR,
@@ -27,9 +27,9 @@
     'MultiStepMomentum', 'StepMomentum', 'ConstantParamScheduler',
     'CosineAnnealingParamScheduler', 'ExponentialParamScheduler',
     'LinearParamScheduler', 'MultiStepParamScheduler', 'StepParamScheduler',
     '_ParamScheduler', 'OptimWrapper', 'AmpOptimWrapper', 'ApexOptimWrapper',
     'OptimWrapperDict', 'OneCycleParamScheduler', 'OneCycleLR', 'PolyLR',
     'PolyMomentum', 'PolyParamScheduler', 'ReduceOnPlateauLR',
     'ReduceOnPlateauMomentum', 'ReduceOnPlateauParamScheduler',
-    'ZeroRedundancyOptimizer'
+    'ZeroRedundancyOptimizer', 'BaseOptimWrapper'
 ]
```

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/__init__.py` & `mmengine-0.8.0/mmengine/optim/optimizer/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+from mmengine.utils import is_installed
 from .amp_optimizer_wrapper import AmpOptimWrapper
 from .apex_optimizer_wrapper import ApexOptimWrapper
+from .base import BaseOptimWrapper
 from .builder import (OPTIM_WRAPPER_CONSTRUCTORS, OPTIMIZERS,
                       build_optim_wrapper)
 from .default_constructor import DefaultOptimWrapperConstructor
 from .optimizer_wrapper import OptimWrapper
 from .optimizer_wrapper_dict import OptimWrapperDict
 from .zero_optimizer import ZeroRedundancyOptimizer
 
 __all__ = [
     'OPTIM_WRAPPER_CONSTRUCTORS', 'OPTIMIZERS',
     'DefaultOptimWrapperConstructor', 'build_optim_wrapper', 'OptimWrapper',
     'AmpOptimWrapper', 'ApexOptimWrapper', 'OptimWrapperDict',
-    'ZeroRedundancyOptimizer'
+    'ZeroRedundancyOptimizer', 'BaseOptimWrapper'
 ]
+
+if is_installed('deepspeed'):
+    from ._deepspeed import DeepSpeedOptimWrapper  # noqa:F401
+    __all__.append('DeepSpeedOptimWrapper')
```

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.8.0/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 
         dtype (str or torch.dtype, optional): The data type to autocast in amp.
             If a ``str`` is given, it will be converted to ``torch.dtype``.
             Valid ``str`` format are `'float16'`, `'bfloat16'`, `'float32'` and
             `'float64'`. If set to ``None``, the default data type will be used.
             Defaults to None.
             `New in version 0.6.1.`
+        use_fsdp (bool): Using ``ShardedGradScaler`` when it is True. It should
+            be enabled when using ``FullyShardedDataParallel``.
+            Defaults to False.
+            `New in version 0.8.0.`
         **kwargs: Keyword arguments passed to OptimWrapper.
 
     Warnings:
         ``dtype`` argument is only available with PyTorch version >= 1.10.0. If
         you use PyTorch of an older version, it will be ignored.
 
     Note:
@@ -61,33 +65,46 @@
     """
 
     valid_dtypes = ('float16', 'bfloat16', 'float32', 'float64')
 
     def __init__(self,
                  loss_scale: str = 'dynamic',
                  dtype: Union[str, torch.dtype] = None,
+                 use_fsdp: bool = False,
                  **kwargs):
         assert digit_version(TORCH_VERSION) >= digit_version('1.6.0'), (
             '`torch.cuda.amp` is only available when pytorch version >= 1.6')
         assert is_cuda_available() or is_npu_available() or is_mlu_available(
         ), ('``AmpOptimizerWrapper`` is only available training '
             'on gpu, npu or mlu')
         super().__init__(**kwargs)
         self._scale_update_param = None
+
+        if use_fsdp:
+            if digit_version(torch.__version__) >= digit_version('2.0.0'):
+                from torch.distributed.fsdp.sharded_grad_scaler import \
+                    ShardedGradScaler
+                scaler_type = ShardedGradScaler
+            else:
+                raise RuntimeError(
+                    'PyTorch>=2.0.0 is required when sets `use_fsdp=True`')
+        else:
+            scaler_type = GradScaler
+
         if loss_scale == 'dynamic':
             #  If loss_scale is a string, it must be 'dynamic', then dynamic
             #  loss scaling will be used.
-            self.loss_scaler = GradScaler()
+            self.loss_scaler = scaler_type()
         elif isinstance(loss_scale, float):
             # Static loss scaling
             self._scale_update_param = loss_scale
-            self.loss_scaler = GradScaler(init_scale=loss_scale)
+            self.loss_scaler = scaler_type(init_scale=loss_scale)
         elif isinstance(loss_scale, dict):
             # More specific configuration.
-            self.loss_scaler = GradScaler(**loss_scale)
+            self.loss_scaler = scaler_type(**loss_scale)
         else:
             raise TypeError('loss_scale must be of type float, dict, or '
                             f'"dynamic", but got {loss_scale}')
 
         # convert string value to torch.dtype
         if isinstance(dtype, str):
             assert dtype in self.valid_dtypes, (
@@ -129,15 +146,15 @@
         dictionary will add a key named "loss_scaler".
 
         Returns:
             dict: The merged state dict of :attr:`loss_scaler` and
             :attr:`optimizer`.
         """
         # save state_dict of loss_scaler
-        state_dict = self.optimizer.state_dict()
+        state_dict = super().state_dict()
         state_dict['loss_scaler'] = self.loss_scaler.state_dict()
         return state_dict
 
     def load_state_dict(self, state_dict: dict):
         """Load and parse the state dictionary of :attr:`optimizer` and
         :attr:`loss_scaler`.
 
@@ -147,14 +164,19 @@
 
         Args:
             state_dict (dict): The state dict of :attr:`optimizer` and
                 :attr:`loss_scaler`
         """
         if 'loss_scaler' in state_dict:
             self.loss_scaler.load_state_dict(state_dict.pop('loss_scaler'))
+
+        if 'base_param_settings' in state_dict:
+            self.base_param_settings = state_dict.pop('base_param_settings')
+
+        # load state_dict of optimizer
         self.optimizer.load_state_dict(state_dict)
 
     @contextmanager
     def optim_context(self, model: nn.Module):
         """Enables the context for mixed precision training, and enables the
         context for disabling gradient synchronization during gradient
         accumulation context.
```

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.8.0/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/builder.py` & `mmengine-0.8.0/mmengine/optim/optimizer/builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -125,14 +125,50 @@
                 optimizers.append(module_name)
     return optimizers
 
 
 SOPHIA_OPTIMIZERS = register_sophia_optimizers()
 
 
+def register_deepspeed_optimizers() -> List[str]:
+    """Register optimizers in ``deepspeed`` to the ``OPTIMIZERS`` registry.
+
+    Returns:
+        List[str]: A list of registered optimizers' name.
+    """
+    deepspeed_optimizers = []
+    try:
+        import deepspeed  # noqa: F401
+    except ImportError:
+        pass
+    else:
+        from deepspeed.ops.adam import DeepSpeedCPUAdam, FusedAdam
+        from deepspeed.ops.lamb import FusedLamb
+        from deepspeed.runtime.fp16.onebit import (OnebitAdam, OnebitLamb,
+                                                   ZeroOneAdam)
+
+        OPTIMIZERS.register_module(module=DeepSpeedCPUAdam)
+        deepspeed_optimizers.append('DeepSpeedCPUAdam')
+        OPTIMIZERS.register_module(module=FusedAdam)
+        deepspeed_optimizers.append('FusedAdam')
+        OPTIMIZERS.register_module(module=FusedLamb)
+        deepspeed_optimizers.append('FusedLamb')
+        OPTIMIZERS.register_module(module=OnebitAdam)
+        deepspeed_optimizers.append('OnebitAdam')
+        OPTIMIZERS.register_module(module=OnebitLamb)
+        deepspeed_optimizers.append('OnebitLamb')
+        OPTIMIZERS.register_module(module=ZeroOneAdam)
+        deepspeed_optimizers.append('ZeroOneAdam')
+
+    return deepspeed_optimizers
+
+
+DEEPSPEED_OPTIMIZERS = register_deepspeed_optimizers()
+
+
 def build_optim_wrapper(model: nn.Module,
                         cfg: Union[dict, Config, ConfigDict]) -> OptimWrapper:
     """Build function of OptimWrapper.
 
     If ``constructor`` is set in the ``cfg``, this method will build an
     optimizer wrapper constructor, and use optimizer wrapper constructor to
     build the optimizer wrapper. If ``constructor`` is not set, the
```

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.8.0/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 
 from mmengine.logging import MessageHub, print_log
 from mmengine.registry import OPTIM_WRAPPERS
 from mmengine.utils.dl_utils import has_batch_norm
+from .base import BaseOptimWrapper
 
 
 @OPTIM_WRAPPERS.register_module()
-class OptimWrapper:
+class OptimWrapper(BaseOptimWrapper):
     """Optimizer wrapper provides a common interface for updating parameters.
 
     Optimizer wrapper provides a unified interface for single precision
     training and automatic mixed precision training with different hardware.
     OptimWrapper encapsulates optimizer to provide simplified interfaces
     for commonly used training techniques such as gradient accumulative and
     grad clips. ``OptimWrapper`` implements the basic logic of gradient
@@ -157,18 +158,33 @@
         # `accumulative_counts`.
         self._max_counts = -1
         # The `_remainder_iter` is used for calculating loss factor at the
         # last few iterations. If `_max_counts` has not been initialized,
         # the loss factor will always be the same as `_accumulative_counts`.
         self._remainder_counts = -1
 
-    def update_params(self,
-                      loss: torch.Tensor,
-                      step_kwargs: Optional[Dict] = None,
-                      zero_kwargs: Optional[Dict] = None) -> None:
+        # The Following code is used to initialize `base_param_settings`.
+        # `base_param_settings` is used to store the parameters that are not
+        # updated by the optimizer.
+        # The `base_param_settings` used for tracking the base learning in the
+        # optimizer. If the optimizer has multiple parameter groups, this
+        # params will not be scaled by the loss factor.
+        if len(optimizer.param_groups) > 1:
+            self.base_param_settings = {
+                'params': torch.tensor([0.0], dtype=torch.float)
+            }
+            self.base_param_settings.update(**self.optimizer.defaults)
+        else:
+            self.base_param_settings = None  # type: ignore
+
+    def update_params(  # type: ignore
+            self,
+            loss: torch.Tensor,
+            step_kwargs: Optional[Dict] = None,
+            zero_kwargs: Optional[Dict] = None) -> None:
         """Update parameters in :attr:`optimizer`.
 
         Args:
             loss (torch.Tensor): A tensor for back propagation.
             step_kwargs (dict): Arguments for optimizer.step.
                 Defaults to None.
                 New in version v0.4.0.
@@ -236,94 +252,14 @@
             kwargs: Keyword arguments passed to
                 :meth:`torch.optim.Optimizer.step`.
         """
         if self.clip_grad_kwargs:
             self._clip_grad()
         self.optimizer.step(**kwargs)
 
-    def state_dict(self) -> dict:
-        """A wrapper of ``Optimizer.state_dict``.
-
-        Provide unified ``state_dict`` interface compatible with automatic
-        mixed precision training. Subclass can overload this method to
-        implement the required logic. For example, the state dictionary of
-        GradScaler should be saved when training with ``torch.cuda.amp``.
-
-        Returns:
-            dict: The state dictionary of :attr:`optimizer`.
-        """
-        return self.optimizer.state_dict()
-
-    def load_state_dict(self, state_dict: dict) -> None:
-        """A wrapper of ``Optimizer.load_state_dict``. load the state dict of
-        :attr:`optimizer`.
-
-        Provide unified ``load_state_dict`` interface compatible with automatic
-        mixed precision training. Subclass can overload this method to
-        implement the required logic. For example, the state dictionary of
-        GradScaler should be loaded when training with ``torch.cuda.amp``.
-
-        Args:
-            state_dict (dict): The state dictionary of :attr:`optimizer`.
-        """
-        self.optimizer.load_state_dict(state_dict)
-
-    @property
-    def param_groups(self) -> List[dict]:
-        """A wrapper of ``Optimizer.param_groups``.
-
-        Make OptimizeWrapper compatible with :class:`_ParamScheduler`.
-
-        Returns:
-             dict: the ``param_groups`` of :attr:`optimizer`.
-        """
-        return self.optimizer.param_groups
-
-    @property
-    def defaults(self) -> dict:
-        """A wrapper of ``Optimizer.defaults``.
-
-        Make OptimizeWrapper compatible with :class:`_ParamScheduler`.
-
-        Returns:
-             dict: the ``param_groups`` of :attr:`optimizer`.
-        """
-        return self.optimizer.defaults
-
-    def get_lr(self) -> Dict[str, List[float]]:
-        """Get the learning rate of the optimizer.
-
-        Provide unified interface to get learning rate of optimizer.
-
-        Returns:
-            Dict[str, List[float]]: Learning rate of the optimizer.
-        """
-        lr = [group['lr'] for group in self.param_groups]
-        return dict(lr=lr)
-
-    def get_momentum(self) -> Dict[str, List[float]]:
-        """Get the momentum of the optimizer.
-
-        Provide unified interface to get momentum of optimizer.
-
-        Returns:
-            Dict[str, List[float]]: Momentum of the optimizer.
-        """
-        momentum = []
-        for group in self.param_groups:
-            # Get momentum of SGD.
-            if 'momentum' in group.keys():
-                momentum.append(group['momentum'])
-            # Get momentum of Adam.
-            elif 'betas' in group.keys():
-                momentum.append(group['betas'][0])
-            else:
-                momentum.append(0)
-        return dict(momentum=momentum)
-
     @contextmanager
     def optim_context(self, model: nn.Module):
         """A Context for gradient accumulation and automatic mix precision
         training.
 
         If subclasses need to enable the context for mix precision training,
         e.g., ``:class:`AmpOptimWrapper``,  the corresponding context should be
```

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,19 @@
     def __init__(self, **optim_wrapper_dict: OptimWrapper):
         for key, value in optim_wrapper_dict.items():
             assert isinstance(value, OptimWrapper), (
                 '`OptimWrapperDict` only accept OptimWrapper instance, '
                 f'but got {key}: {type(value)}')
         self.optim_wrappers = optim_wrapper_dict
 
-    def update_params(self,
-                      loss: torch.Tensor,
-                      step_kwargs: Optional[Dict] = None,
-                      zero_kwargs: Optional[Dict] = None) -> None:
+    def update_params(  # type: ignore
+            self,
+            loss: torch.Tensor,
+            step_kwargs: Optional[Dict] = None,
+            zero_kwargs: Optional[Dict] = None) -> None:
         """Update all optimizer wrappers would lead to a duplicate backward
         errors, and OptimWrapperDict does not know which optimizer wrapper
         should be updated.
 
         Therefore, this method is not implemented. The optimizer wrapper of
         OptimWrapperDict should be accessed and call its `update_params`.
         """
@@ -111,15 +112,18 @@
         """Get the learning rate of all optimizers.
 
         Returns:
             Dict[str, List[float]]: Learning rate of all optimizers.
         """
         lr_dict = dict()
         for name, optim_wrapper in self.optim_wrappers.items():
-            lr_dict[f'{name}.lr'] = optim_wrapper.get_lr()['lr']
+            inner_lr_dict = optim_wrapper.get_lr()
+            if 'base_lr' in inner_lr_dict:
+                lr_dict[f'{name}.base_lr'] = inner_lr_dict['base_lr']
+            lr_dict[f'{name}.lr'] = inner_lr_dict['lr']
         return lr_dict
 
     def get_momentum(self) -> Dict[str, List[float]]:
         """Get the momentum of all optimizers.
 
         Returns:
             Dict[str, List[float]]: momentum of all optimizers.
```

### Comparing `mmengine-0.7.4/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.8.0/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/optim/scheduler/__init__.py` & `mmengine-0.8.0/mmengine/optim/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.8.0/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.8.0/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.8.0/mmengine/optim/scheduler/param_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 from collections import Counter
 from functools import wraps
 from typing import Callable, List, Optional, Sequence, Union
 
 from torch.optim import Optimizer
 
 from mmengine.logging import print_log
-from mmengine.optim import OptimWrapper
+from mmengine.optim import BaseOptimWrapper
 from mmengine.registry import PARAM_SCHEDULERS
 
 INF = int(1e9)
 
-OptimizerType = Union[OptimWrapper, Optimizer]
+OptimizerType = Union[BaseOptimWrapper, Optimizer]
 
 
 class _ParamScheduler:
     """Base class for parameter schedulers.
 
     It should be inherited by all schedulers that schedule parameters in the
     optimizer's ``param_groups``. All subclasses should overwrite the
     ``_get_value()`` according to their own schedule strategy.
     The implementation is motivated by
     https://github.com/pytorch/pytorch/blob/master/torch/optim/lr_scheduler.py.
 
     Args:
-        optimizer (OptimWrapper or Optimizer): Wrapped optimizer.
+        optimizer (BaseOptimWrapper or Optimizer): Wrapped optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         begin (int): Step at which to start updating the parameters.
             Defaults to 0.
         end (int): Step at which to stop updating the parameters.
             Defaults to INF.
         last_step (int): The index of last step. Used for resuming without
@@ -54,15 +54,15 @@
                  begin: int = 0,
                  end: int = INF,
                  last_step: int = -1,
                  by_epoch: bool = True,
                  verbose: bool = False):
 
         # Attach optimizer
-        if not isinstance(optimizer, (Optimizer, OptimWrapper)):
+        if not isinstance(optimizer, (Optimizer, BaseOptimWrapper)):
             raise TypeError('``optimizer`` should be an Optimizer,'
                             'but got {}'.format(type(optimizer).__name__))
         self.optimizer = optimizer
         self.param_name = param_name
 
         if end <= begin:
             raise ValueError('end should be larger than begin, but got'
@@ -224,15 +224,15 @@
 @PARAM_SCHEDULERS.register_module()
 class StepParamScheduler(_ParamScheduler):
     """Decays the parameter value of each parameter group by gamma every
     step_size epochs. Notice that such decay can happen simultaneously with
     other changes to the parameter value from outside this scheduler.
 
     Args:
-        optimizer (OptimWrapper or Optimizer): Wrapped optimizer.
+        optimizer (BaseOptimWrapper or Optimizer): Wrapped optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         step_size (int): Period of parameter value decay.
         gamma (float): Multiplicative factor of parameter value decay.
             Defaults to 0.1.
         begin (int): Step at which to start updating the parameters.
             Defaults to 0.
@@ -312,15 +312,15 @@
 class MultiStepParamScheduler(_ParamScheduler):
     """Decays the specified parameter in each parameter group by gamma once the
     number of epoch reaches one of the milestones. Notice that such decay can
     happen simultaneously with other changes to the parameter from outside this
     scheduler.
 
     Args:
-        optimizer (OptimWrapper or Optimizer): Wrapped optimizer.
+        optimizer (BaseOptimWrapper or Optimizer): Wrapped optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         milestones (list): List of epoch indices. Must be increasing.
         gamma (float): Multiplicative factor of parameter value decay.
             Defaults to 0.1.
         begin (int): Step at which to start updating the parameters.
             Defaults to 0.
@@ -401,15 +401,15 @@
 class ConstantParamScheduler(_ParamScheduler):
     """Decays the parameter value of each parameter group by a small constant
     factor until the number of epoch reaches a pre-defined milestone: ``end``.
     Notice that such decay can happen simultaneously with other changes to the
     parameter value from outside this scheduler.
 
     Args:
-        optimizer (Optimizer or OptimWrapper): optimizer or Wrapped
+        optimizer (Optimizer or BaseOptimWrapper): optimizer or Wrapped
             optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         factor (float): The number we multiply parameter value until the
             milestone. Defaults to 1./3.
         begin (int): Step at which to start updating the parameters.
             Defaults to 0.
@@ -490,15 +490,15 @@
 
 
 @PARAM_SCHEDULERS.register_module()
 class ExponentialParamScheduler(_ParamScheduler):
     """Decays the parameter value of each parameter group by gamma every epoch.
 
     Args:
-        optimizer (Optimizer or OptimWrapper): optimizer or Wrapped
+        optimizer (Optimizer or BaseOptimWrapper): optimizer or Wrapped
             optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         gamma (float): Multiplicative factor of parameter value decay.
         begin (int): Step at which to start updating the parameters.
             Defaults to 0.
         end (int): Step at which to stop updating the parameters.
@@ -589,15 +589,15 @@
         \cos\left(\frac{T_{cur}}{T_{max}}\pi\right)\right)
 
     It has been proposed in
     `SGDR: Stochastic Gradient Descent with Warm Restarts`_. Note that this
     only implements the cosine annealing part of SGDR, and not the restarts.
 
     Args:
-        optimizer (Optimizer or OptimWrapper): optimizer or Wrapped
+        optimizer (Optimizer or BaseOptimWrapper): optimizer or Wrapped
             optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         T_max (int, optional): Maximum number of iterations. If not specified,
             use ``end - begin``. Defaults to None.
         eta_min (float, optional): Minimum parameter value. Defaults to None.
         begin (int): Step at which to start updating the parameters.
@@ -616,15 +616,15 @@
             New in version 0.3.2.
 
     .. _SGDR\: Stochastic Gradient Descent with Warm Restarts:
         https://arxiv.org/abs/1608.03983
     """
 
     def __init__(self,
-                 optimizer: Union[Optimizer, OptimWrapper],
+                 optimizer: Union[Optimizer, BaseOptimWrapper],
                  param_name: str,
                  T_max: Optional[int] = None,
                  eta_min: Optional[float] = None,
                  begin: int = 0,
                  end: int = INF,
                  last_step: int = -1,
                  by_epoch: bool = True,
@@ -710,15 +710,15 @@
     small multiplicative factor until the number of epoch reaches a pre-defined
     milestone: ``end``.
 
     Notice that such decay can happen simultaneously with other changes to the
     parameter value from outside this scheduler.
 
     Args:
-        optimizer (Optimizer or OptimWrapper): optimizer or Wrapped
+        optimizer (Optimizer or BaseOptimWrapper): optimizer or Wrapped
             optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         start_factor (float): The number we multiply parameter value in the
             first epoch. The multiplication factor changes towards end_factor
             in the following epochs. Defaults to 1./3.
         end_factor (float): The number we multiply parameter value at the end
@@ -732,15 +732,15 @@
         by_epoch (bool): Whether the scheduled parameters are updated by
             epochs. Defaults to True.
         verbose (bool): Whether to print the value for each update.
             Defaults to False.
     """
 
     def __init__(self,
-                 optimizer: Union[Optimizer, OptimWrapper],
+                 optimizer: Union[Optimizer, BaseOptimWrapper],
                  param_name: str,
                  start_factor: float = 1.0 / 3,
                  end_factor: float = 1.0,
                  begin: int = 0,
                  end: int = INF,
                  last_step: int = -1,
                  by_epoch: bool = True,
@@ -808,15 +808,15 @@
     """Decays the parameter value of each parameter group in a polynomial decay
     scheme.
 
     Notice that such decay can happen simultaneously with other changes to the
     parameter value from outside this scheduler.
 
     Args:
-        optimizer (Optimizer or OptimWrapper): optimizer or Wrapped
+        optimizer (Optimizer or BaseOptimWrapper): optimizer or Wrapped
             optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         eta_min (float): Minimum parameter value at the end of scheduling.
             Defaults to 0.
         power (float): The power of the polynomial. Defaults to 1.0.
         begin (int): Step at which to start updating the parameters.
@@ -828,15 +828,15 @@
         by_epoch (bool): Whether the scheduled parameters are updated by
             epochs. Defaults to True.
         verbose (bool): Whether to print the value for each update.
             Defaults to False.
     """
 
     def __init__(self,
-                 optimizer: Union[Optimizer, OptimWrapper],
+                 optimizer: Union[Optimizer, BaseOptimWrapper],
                  param_name: str,
                  eta_min: float = 0,
                  power: float = 1.0,
                  begin: int = 0,
                  end: int = INF,
                  last_step: int = -1,
                  by_epoch: bool = True,
@@ -950,15 +950,15 @@
             Defaults to False.
 
     .. _Super-Convergence\: Very Fast Training of Neural Networks Using Large Learning Rates:
         https://arxiv.org/abs/1708.07120
     """  # noqa E501
 
     def __init__(self,
-                 optimizer: Union[Optimizer, OptimWrapper],
+                 optimizer: Union[Optimizer, BaseOptimWrapper],
                  param_name: str,
                  eta_max: float = 0,
                  total_steps: Optional[int] = None,
                  pct_start: float = 0.3,
                  anneal_strategy: str = 'cos',
                  div_factor: float = 25.,
                  final_div_factor: float = 1e4,
@@ -1139,15 +1139,15 @@
     """Sets the parameters of each parameter group according to the cosine
     annealing with restarts scheme. The cosine restart policy anneals the
     parameter from the initial value to `eta_min` with a cosine annealing
     schedule and then restarts another period from the maximum value multiplied
     with `restart_weight`.
 
     Args:
-        optimizer (Optimizer or OptimWrapper): optimizer or Wrapped
+        optimizer (Optimizer or BaseOptimWrapper): optimizer or Wrapped
             optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         periods (list[int]): Periods for each cosine anneling cycle.
         restart_weights (list[float]): Restart weights at each
             restart iteration. Defaults to [1].
         eta_min (float, optional): Minimum parameter value at the end of
@@ -1164,15 +1164,15 @@
         by_epoch (bool): Whether the scheduled parameters are updated by
             epochs. Defaults to True.
         verbose (bool): Whether to print the value for each update.
             Defaults to False.
     """
 
     def __init__(self,
-                 optimizer: Union[Optimizer, OptimWrapper],
+                 optimizer: Union[Optimizer, BaseOptimWrapper],
                  param_name: str,
                  periods: List[int],
                  restart_weights: Sequence[float] = (1, ),
                  eta_min: Optional[float] = None,
                  eta_min_ratio: Optional[float] = None,
                  begin: int = 0,
                  end: int = INF,
@@ -1292,15 +1292,15 @@
     2-10 once learning stagnates. This scheduler reads a metrics quantity and
     if no improvement is seen for a ``patience`` number of epochs, the
     parameters are reduced.
 
     The implementation is motivated by `PyTorch ReduceLROnPlateau`_.
 
     Args:
-        optimizer (Optimizer or OptimWrapper): optimizer or Wrapped
+        optimizer (Optimizer or BaseOptimWrapper): optimizer or Wrapped
             optimizer.
         param_name (str): Name of the parameter to be adjusted, such as
             ``lr``, ``momentum``.
         monitor (str): The name of the metric to measure whether
             the performance of the model is improved.
         rule (str): One of `less`, `greater`. In `less` rule, parameters will
             be reduced when the quantity monitored has stopped
@@ -1365,15 +1365,15 @@
                  begin: int = 0,
                  end: int = INF,
                  last_step: int = -1,
                  by_epoch: bool = True,
                  verbose: bool = False):
 
         # Attach optimizer
-        if not isinstance(optimizer, (Optimizer, OptimWrapper)):
+        if not isinstance(optimizer, (Optimizer, BaseOptimWrapper)):
             raise TypeError('``optimizer`` should be an Optimizer,'
                             'but got {}'.format(type(optimizer).__name__))
         self.optimizer = optimizer
         self.param_name = param_name
 
         if end <= begin:
             raise ValueError('end should be larger than begin, but got'
@@ -1405,19 +1405,36 @@
         self._global_step = 0
         self.verbose = verbose
 
         if factor >= 1.0:
             raise ValueError('Factor should be < 1.0.')
         self.factor = factor
 
+        # This code snippet handles compatibility with the optimizer wrapper.
+        # The optimizer wrapper includes an additional parameter to record the
+        # base learning rate (lr) which is not affected by the paramwise_cfg.
+        # By retrieving the base lr, we can obtain the actual base lr that
+        # reflects the learning progress.
+        if isinstance(optimizer, BaseOptimWrapper):
+            raw_optimizer = optimizer.optimizer
+        else:
+            raw_optimizer = optimizer
+
         if isinstance(min_value, (list, tuple)):
-            if len(min_value) != len(optimizer.param_groups):
+            if len(min_value) != len(raw_optimizer.param_groups):
                 raise ValueError('expected {} min_lrs, got {}'.format(
-                    len(optimizer.param_groups), len(min_value)))
+                    len(raw_optimizer.param_groups), len(min_value)))
             self.min_values = list(min_value)
+            # Consider the `min_value` of the last param_groups
+            # as the base setting. And we only add this value when
+            # the optimizer is OptimWrapper.
+            if isinstance(optimizer, BaseOptimWrapper) and \
+                    optimizer.base_param_settings is not None:  # type: ignore
+                self.min_values.append(self.min_values[-1])
+
         else:
             self.min_values = [min_value] * len(  # type: ignore
                 optimizer.param_groups)
 
         self.patience = patience
         self.cooldown = cooldown
         self.cooldown_counter = 0
```

### Comparing `mmengine-0.7.4/mmengine/registry/__init__.py` & `mmengine-0.8.0/mmengine/registry/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
                               build_runner_from_cfg, build_scheduler_from_cfg)
 from .default_scope import DefaultScope
 from .registry import Registry
 from .root import (DATA_SAMPLERS, DATASETS, EVALUATOR, FUNCTIONS, HOOKS,
                    INFERENCERS, LOG_PROCESSORS, LOOPS, METRICS, MODEL_WRAPPERS,
                    MODELS, OPTIM_WRAPPER_CONSTRUCTORS, OPTIM_WRAPPERS,
                    OPTIMIZERS, PARAM_SCHEDULERS, RUNNER_CONSTRUCTORS, RUNNERS,
-                   TASK_UTILS, TRANSFORMS, VISBACKENDS, VISUALIZERS,
-                   WEIGHT_INITIALIZERS)
+                   STRATEGIES, TASK_UTILS, TRANSFORMS, VISBACKENDS,
+                   VISUALIZERS, WEIGHT_INITIALIZERS)
 from .utils import (count_registered_modules, init_default_scope,
                     traverse_registry_tree)
 
 __all__ = [
     'Registry', 'RUNNERS', 'RUNNER_CONSTRUCTORS', 'HOOKS', 'DATASETS',
     'DATA_SAMPLERS', 'TRANSFORMS', 'MODELS', 'WEIGHT_INITIALIZERS',
     'OPTIMIZERS', 'OPTIM_WRAPPER_CONSTRUCTORS', 'TASK_UTILS',
     'PARAM_SCHEDULERS', 'METRICS', 'MODEL_WRAPPERS', 'OPTIM_WRAPPERS', 'LOOPS',
     'VISBACKENDS', 'VISUALIZERS', 'LOG_PROCESSORS', 'EVALUATOR', 'INFERENCERS',
     'DefaultScope', 'traverse_registry_tree', 'count_registered_modules',
     'build_model_from_cfg', 'build_runner_from_cfg', 'build_from_cfg',
-    'build_scheduler_from_cfg', 'init_default_scope', 'FUNCTIONS'
+    'build_scheduler_from_cfg', 'init_default_scope', 'FUNCTIONS', 'STRATEGIES'
 ]
```

### Comparing `mmengine-0.7.4/mmengine/registry/build_functions.py` & `mmengine-0.8.0/mmengine/registry/build_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
     args = cfg.copy()
     # Runner should be built under target scope, if `_scope_` is defined
     # in cfg, current default scope should switch to specified scope
     # temporarily.
     scope = args.pop('_scope_', None)
     with registry.switch_scope_and_registry(scope) as registry:
-        obj_type = args.get('runner_type', 'mmengine.Runner')
+        obj_type = args.get('runner_type', 'Runner')
         if isinstance(obj_type, str):
             runner_cls = registry.get(obj_type)
             if runner_cls is None:
                 raise KeyError(
                     f'{obj_type} is not in the {registry.name} registry. '
                     f'Please check whether the value of `{obj_type}` is '
                     'correct or it was registered as expected. More details '
```

### Comparing `mmengine-0.7.4/mmengine/registry/default_scope.py` & `mmengine-0.8.0/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/registry/registry.py` & `mmengine-0.8.0/mmengine/registry/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from importlib import import_module
 from typing import Any, Dict, Generator, List, Optional, Tuple, Type, Union
 
 from rich.console import Console
 from rich.table import Table
 
 from mmengine.config.utils import MODULE2PACKAGE
-from mmengine.utils import is_seq_of
+from mmengine.utils import get_object_from_string, is_seq_of
 from .default_scope import DefaultScope
 
 
 class Registry:
     """A registry to map strings to classes or functions.
 
     Registered object could be built from registry. Meanwhile, registered
@@ -380,16 +380,20 @@
                     logger='current',
                     level=logging.DEBUG)
             self._imported = True
 
     def get(self, key: str) -> Optional[Type]:
         """Get the registry record.
 
-        The method will first parse :attr:`key` and check whether it contains
-        a scope name. The logic to search for :attr:`key`:
+        If `key`` represents the whole object name with its module
+        information, for example, `mmengine.model.BaseModel`, ``get``
+        will directly return the class object :class:`BaseModel`.
+
+        Otherwise, it will first parse ``key`` and check whether it
+        contains a scope name. The logic to search for ``key``:
 
         - ``key`` does not contain a scope name, i.e., it is purely a module
           name like "ResNet": :meth:`get` will search for ``ResNet`` from the
           current registry to its parent or ancestors until finding it.
 
         - ``key`` contains a scope name and it is equal to the scope of the
           current registry (e.g., "mmcls"), e.g., "mmcls.ResNet": :meth:`get`
@@ -429,14 +433,19 @@
             >>>     pass
             >>> # `get` from its sibling registries
             >>> mobilenet_cls = DETECTORS.get('cls.MobileNet')
         """
         # Avoid circular import
         from ..logging import print_log
 
+        if not isinstance(key, str):
+            raise TypeError(
+                'The key argument of `Registry.get` must be a str, '
+                f'got {type(key)}')
+
         scope, real_key = self.split_scope_key(key)
         obj_cls = None
         registry_name = self.name
         scope_name = self.scope
 
         # lazy import the modules to register them into the registry
         self.import_from_location()
@@ -482,23 +491,36 @@
                 if scope != root._scope and scope not in root._children:
                     # If not skip directly, `root.get(key)` will recursively
                     # call itself until RecursionError is thrown.
                     pass
                 else:
                     obj_cls = root.get(key)
 
+        if obj_cls is None:
+            # Actually, it's strange to implement this `try ... except` to
+            # get the object by its name in `Registry.get`. However, If we
+            # want to build the model using a configuration like
+            # `dict(type='mmengine.model.BaseModel')`, which can
+            # be dumped by lazy import config, we need this code snippet
+            # for `Registry.get` to work.
+            try:
+                obj_cls = get_object_from_string(key)
+            except Exception:
+                raise RuntimeError(f'Failed to get {key}')
+
         if obj_cls is not None:
             # For some rare cases (e.g. obj_cls is a partial function), obj_cls
             # doesn't have `__name__`. Use default value to prevent error
             cls_name = getattr(obj_cls, '__name__', str(obj_cls))
             print_log(
                 f'Get class `{cls_name}` from "{registry_name}"'
                 f' registry in "{scope_name}"',
                 logger='current',
                 level=logging.DEBUG)
+
         return obj_cls
 
     def _search_child(self, scope: str) -> Optional['Registry']:
         """Depth-first search for the corresponding registry in its children.
 
         Note that the method only search for the corresponding registry from
         the current registry. Therefore, if we want to search from the root
```

### Comparing `mmengine-0.7.4/mmengine/registry/root.py` & `mmengine-0.8.0/mmengine/registry/root.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 # manage runner constructors that define how to initialize runners
 RUNNER_CONSTRUCTORS = Registry('runner constructor')
 # manage all kinds of loops like `EpochBasedTrainLoop`
 LOOPS = Registry('loop')
 # manage all kinds of hooks like `CheckpointHook`
 HOOKS = Registry('hook')
 
+# manage all kinds of strategies like `NativeStrategy` and `DDPStrategy`
+STRATEGIES = Registry('strategy')
+
 # manage data-related modules
 DATASETS = Registry('dataset')
 DATA_SAMPLERS = Registry('data sampler')
 TRANSFORMS = Registry('transform')
 
 # mangage all kinds of modules inheriting `nn.Module`
 MODELS = Registry('model', build_model_from_cfg)
```

### Comparing `mmengine-0.7.4/mmengine/registry/utils.py` & `mmengine-0.8.0/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/runner/__init__.py` & `mmengine-0.8.0/mmengine/runner/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+from ._flexible_runner import FlexibleRunner
 from .amp import autocast
 from .base_loop import BaseLoop
 from .checkpoint import (CheckpointLoader, find_latest_checkpoint,
                          get_deprecated_model_names, get_external_models,
                          get_mmcls_models, get_state_dict,
                          get_torchvision_models, load_checkpoint,
                          load_state_dict, save_checkpoint, weights_to_cpu)
@@ -14,9 +15,9 @@
 
 __all__ = [
     'BaseLoop', 'load_state_dict', 'get_torchvision_models',
     'get_external_models', 'get_mmcls_models', 'get_deprecated_model_names',
     'CheckpointLoader', 'load_checkpoint', 'weights_to_cpu', 'get_state_dict',
     'save_checkpoint', 'EpochBasedTrainLoop', 'IterBasedTrainLoop', 'ValLoop',
     'TestLoop', 'Runner', 'get_priority', 'Priority', 'find_latest_checkpoint',
-    'autocast', 'LogProcessor', 'set_random_seed'
+    'autocast', 'LogProcessor', 'set_random_seed', 'FlexibleRunner'
 ]
```

### Comparing `mmengine-0.7.4/mmengine/runner/amp.py` & `mmengine-0.8.0/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/runner/base_loop.py` & `mmengine-0.8.0/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/runner/checkpoint.py` & `mmengine-0.8.0/mmengine/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/runner/log_processor.py` & `mmengine-0.8.0/mmengine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/runner/loops.py` & `mmengine-0.8.0/mmengine/runner/loops.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     def __init__(self,
                  runner,
                  dataloader: Union[DataLoader, Dict],
                  evaluator: Union[Evaluator, Dict, List],
                  fp16: bool = False) -> None:
         super().__init__(runner, dataloader)
 
-        if isinstance(evaluator, dict) or isinstance(evaluator, list):
+        if isinstance(evaluator, (dict, list)):
             self.evaluator = runner.build_evaluator(evaluator)  # type: ignore
         else:
             assert isinstance(evaluator, Evaluator), (
                 'evaluator must be one of dict, list or Evaluator instance, '
                 f'but got {type(evaluator)}.')
             self.evaluator = evaluator  # type: ignore
         if hasattr(self.dataloader.dataset, 'metainfo'):
```

### Comparing `mmengine-0.7.4/mmengine/runner/priority.py` & `mmengine-0.8.0/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/runner/runner.py` & `mmengine-0.8.0/mmengine/runner/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,16 +363,20 @@
             self._experiment_name = f'{filename_no_ext}_{self._timestamp}'
         else:
             self._experiment_name = self.timestamp
         self._log_dir = osp.join(self.work_dir, self.timestamp)
         mmengine.mkdir_or_exist(self._log_dir)
         # Used to reset registries location. See :meth:`Registry.build` for
         # more details.
-        self.default_scope = DefaultScope.get_instance(
-            self._experiment_name, scope_name=default_scope)
+        if default_scope is not None:
+            default_scope = DefaultScope.get_instance(  # type: ignore
+                self._experiment_name,
+                scope_name=default_scope)
+        self.default_scope = default_scope
+
         # Build log processor to format message.
         log_processor = dict() if log_processor is None else log_processor
         self.log_processor = self.build_log_processor(log_processor)
         # Since `get_instance` could return any subclass of ManagerMixin. The
         # corresponding attribute needs a type hint.
         self.logger = self.build_logger(log_level=log_level)
 
@@ -874,14 +878,15 @@
             # TODO: may use a more elegant way to get local device ID.
             model = MMDistributedDataParallel(
                 module=model,
                 device_ids=[int(os.environ['LOCAL_RANK'])],
                 broadcast_buffers=False,
                 find_unused_parameters=find_unused_parameters)
         else:
+            model_wrapper_cfg.setdefault('type', 'MMDistributedDataParallel')
             model_wrapper_type = MODEL_WRAPPERS.get(
                 model_wrapper_cfg.get('type'))  # type: ignore
             default_args: dict = dict()
             if issubclass(
                     model_wrapper_type,  # type: ignore
                     DistributedDataParallel):
                 default_args['device_ids'] = [int(os.environ['LOCAL_RANK'])]
@@ -1380,15 +1385,22 @@
 
         # build dataloader
         init_fn: Optional[partial]
 
         if 'worker_init_fn' in dataloader_cfg:
             worker_init_fn_cfg = dataloader_cfg.pop('worker_init_fn')
             worker_init_fn_type = worker_init_fn_cfg.pop('type')
-            worker_init_fn = FUNCTIONS.get(worker_init_fn_type)
+            if isinstance(worker_init_fn_type, str):
+                worker_init_fn = FUNCTIONS.get(worker_init_fn_type)
+            elif callable(worker_init_fn_type):
+                worker_init_fn = worker_init_fn_type
+            else:
+                raise TypeError(
+                    'type of worker_init_fn should be string or callable '
+                    f'object, but got {type(worker_init_fn_type)}')
             assert callable(worker_init_fn)
             init_fn = partial(worker_init_fn,
                               **worker_init_fn_cfg)  # type: ignore
         else:
             if seed is not None:
                 disable_subprocess_warning = dataloader_cfg.pop(
                     'disable_subprocess_warning', False)
@@ -1419,23 +1431,25 @@
         # However, in mmengine, if `collate_fn` is not defined in
         # dataloader_cfg, `pseudo_collate` will only convert the list of
         # samples into a dict without stacking the batch tensor.
         collate_fn_cfg = dataloader_cfg.pop('collate_fn',
                                             dict(type='pseudo_collate'))
         if isinstance(collate_fn_cfg, dict):
             collate_fn_type = collate_fn_cfg.pop('type')
-            collate_fn = FUNCTIONS.get(collate_fn_type)
+            if isinstance(collate_fn_type, str):
+                collate_fn = FUNCTIONS.get(collate_fn_type)
+            else:
+                collate_fn = collate_fn_type
             collate_fn = partial(collate_fn, **collate_fn_cfg)  # type: ignore
         elif callable(collate_fn_cfg):
             collate_fn = collate_fn_cfg
         else:
             raise TypeError(
                 'collate_fn should be a dict or callable object, but got '
                 f'{collate_fn_cfg}')
-
         data_loader = DataLoader(
             dataset=dataset,
             sampler=sampler if batch_sampler is None else None,
             batch_sampler=batch_sampler,
             collate_fn=collate_fn,
             worker_init_fn=init_fn,
             **dataloader_cfg)
@@ -1971,24 +1985,29 @@
         if 'config' in checkpoint['meta']:
             config = mmengine.Config.fromstring(
                 checkpoint['meta']['config'], file_format='.py')
             previous_gpu_ids = config.get('gpu_ids', None)
             if (previous_gpu_ids is not None and len(previous_gpu_ids) > 0
                     and len(previous_gpu_ids) != self._world_size):
                 # TODO, should we modify the iteration?
-                self.logger.info(
-                    'Number of GPU used for current experiment is not '
-                    'consistent with resuming from checkpoint')
                 if (self.auto_scale_lr is None
                         or not self.auto_scale_lr.get('enable', False)):
                     raise RuntimeError(
-                        'Cannot automatically rescale lr in resuming. Please '
-                        'make sure the number of GPU is consistent with the '
-                        'previous training state resuming from the checkpoint '
-                        'or set `enable` in `auto_scale_lr to False.')
+                        'Number of GPUs used for current experiment is not '
+                        'consistent with the checkpoint being resumed from. '
+                        'This will result in poor performance due to the '
+                        'learning rate. You must set the '
+                        '`auto_scale_lr` parameter for Runner and make '
+                        '`auto_scale_lr["enable"]=True`.')
+                else:
+                    self.logger.info(
+                        'Number of GPU used for current experiment is not '
+                        'consistent with resuming from checkpoint but the '
+                        'leaning rate will be adjusted according to the '
+                        f'setting in auto_scale_lr={self.auto_scale_lr}')
 
         # resume random seed
         resumed_seed = checkpoint['meta'].get('seed', None)
         current_seed = self._randomness_cfg.get('seed')
         if resumed_seed is not None and resumed_seed != current_seed:
             if current_seed is not None:
                 self.logger.warning(f'The value of random seed in the '
```

### Comparing `mmengine-0.7.4/mmengine/runner/utils.py` & `mmengine-0.8.0/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/structures/base_data_element.py` & `mmengine-0.8.0/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/structures/instance_data.py` & `mmengine-0.8.0/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/structures/label_data.py` & `mmengine-0.8.0/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/structures/pixel_data.py` & `mmengine-0.8.0/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/testing/__init__.py` & `mmengine-0.8.0/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/testing/_internal/distributed.py` & `mmengine-0.8.0/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/testing/compare.py` & `mmengine-0.8.0/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/testing/runner_test_case.py` & `mmengine-0.8.0/mmengine/testing/runner_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
         self.linear1 = nn.Linear(2, 2)
         self.linear2 = nn.Linear(2, 1)
 
     def forward(self, inputs, data_samples=None, mode='tensor'):
         if isinstance(inputs, list):
             inputs = torch.stack(inputs)
         if isinstance(data_samples, list):
-            data_sample = torch.stack(data_samples)
+            data_samples = torch.stack(data_samples)
         outputs = self.linear1(inputs)
         outputs = self.linear2(outputs)
 
         if mode == 'tensor':
             return outputs
         elif mode == 'loss':
-            loss = (data_sample - outputs).sum()
+            loss = (data_samples - outputs).sum()
             outputs = dict(loss=loss)
             return outputs
         elif mode == 'predict':
             return outputs
 
 
 class ToyDataset(Dataset):
```

### Comparing `mmengine-0.7.4/mmengine/utils/__init__.py` & `mmengine-0.8.0/mmengine/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .manager import ManagerMeta, ManagerMixin
 from .misc import (apply_to, check_prerequisites, concat_list,
-                   deprecated_api_warning, deprecated_function, has_method,
+                   deprecated_api_warning, deprecated_function,
+                   get_object_from_string, has_method,
                    import_modules_from_strings, is_list_of,
                    is_method_overridden, is_seq_of, is_str, is_tuple_of,
                    iter_cast, list_cast, requires_executable, requires_package,
                    slice_list, to_1tuple, to_2tuple, to_3tuple, to_4tuple,
                    to_ntuple, tuple_cast)
 from .package_utils import (call_command, get_installed_path, install_package,
                             is_installed)
@@ -24,9 +25,9 @@
     'scandir', 'deprecated_api_warning', 'import_modules_from_strings',
     'to_1tuple', 'to_2tuple', 'to_3tuple', 'to_4tuple', 'to_ntuple',
     'is_installed', 'call_command', 'get_installed_path', 'install_package',
     'is_abs', 'is_method_overridden', 'has_method', 'digit_version',
     'get_git_hash', 'ManagerMeta', 'ManagerMixin', 'Timer', 'check_time',
     'TimerError', 'ProgressBar', 'track_iter_progress',
     'track_parallel_progress', 'track_progress', 'deprecated_function',
-    'apply_to'
+    'apply_to', 'get_object_from_string'
 ]
```

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/hub.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/misc.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/trace.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.8.0/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/manager.py` & `mmengine-0.8.0/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/misc.py` & `mmengine-0.8.0/mmengine/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import re
 import subprocess
 import textwrap
 import warnings
 from collections import abc
 from importlib import import_module
-from inspect import getfullargspec
+from inspect import getfullargspec, ismodule
 from itertools import repeat
 from typing import Any, Callable, Optional, Type, Union
 
 
 # From PyTorch internals
 def _ntuple(n):
 
@@ -496,7 +496,47 @@
             new_docstring_parts = [deprecation_note, '\n\n', summary]
 
         wrapper.__doc__ = ''.join(new_docstring_parts)
 
         return wrapper
 
     return decorator
+
+
+def get_object_from_string(obj_name: str):
+    """Get object from name.
+
+    Args:
+        obj_name (str): The name of the object.
+
+    Examples:
+        >>> get_object_from_string('torch.optim.sgd.SGD')
+        >>> torch.optim.sgd.SGD
+    """
+    parts = iter(obj_name.split('.'))
+    module_name = next(parts)
+    # import module
+    while True:
+        try:
+            module = import_module(module_name)
+            part = next(parts)
+            # mmcv.ops has nms.py has nms function at the same time. So the
+            # function will have a higher priority
+            obj = getattr(module, part, None)
+            if obj is not None and not ismodule(obj):
+                break
+            module_name = f'{module_name}.{part}'
+        except StopIteration:
+            # if obj is a module
+            return module
+        except ImportError:
+            return None
+
+    # get class or attribute from module
+    while True:
+        try:
+            obj_cls = getattr(module, part)
+            part = next(parts)
+        except StopIteration:
+            return obj_cls
+        except AttributeError:
+            return None
```

### Comparing `mmengine-0.7.4/mmengine/utils/package_utils.py` & `mmengine-0.8.0/mmengine/utils/package_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import importlib
 import os.path as osp
 import subprocess
 
 
 def is_installed(package: str) -> bool:
     """Check package whether installed.
 
     Args:
         package (str): Name of package to be checked.
     """
     # When executing `import mmengine.runner`,
     # pkg_resources will be imported and it takes too much time.
     # Therefore, import it in function scope to save time.
+    import importlib.util
+
     import pkg_resources
     from pkg_resources import get_distribution
 
     # refresh the pkg_resources
     # more datails at https://github.com/pypa/setuptools/issues/373
     importlib.reload(pkg_resources)
     try:
         get_distribution(package)
         return True
     except pkg_resources.DistributionNotFound:
-        return False
+        spec = importlib.util.find_spec(package)
+        if spec is None:
+            return False
+        elif spec.origin is not None:
+            return True
+        else:
+            return False
 
 
 def get_installed_path(package: str) -> str:
     """Get installed path of package.
 
     Args:
         package (str): Name of package.
 
     Example:
         >>> get_installed_path('mmcls')
         >>> '.../lib/python3.7/site-packages/mmcls'
     """
-    from pkg_resources import get_distribution
+    import importlib.util
+
+    from pkg_resources import DistributionNotFound, get_distribution
 
     # if the package name is not the same as module name, module name should be
     # inferred. For example, mmcv-full is the package name, but mmcv is module
     # name. If we want to get the installed path of mmcv-full, we should concat
     # the pkg.location and module name
-    pkg = get_distribution(package)
+    try:
+        pkg = get_distribution(package)
+    except DistributionNotFound as e:
+        # if the package is not installed, package path set in PYTHONPATH
+        # can be detected by `find_spec`
+        spec = importlib.util.find_spec(package)
+        if spec is not None:
+            if spec.origin is not None:
+                return osp.dirname(spec.origin)
+            else:
+                # `get_installed_path` cannot get the installed path of
+                # namespace packages
+                raise RuntimeError(
+                    f'{package} is a namespace package, which is invalid '
+                    'for `get_install_path`')
+        else:
+            raise e
+
     possible_path = osp.join(pkg.location, package)
     if osp.exists(possible_path):
         return possible_path
     else:
         return osp.join(pkg.location, package2module(package))
```

### Comparing `mmengine-0.7.4/mmengine/utils/path.py` & `mmengine-0.8.0/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/progressbar.py` & `mmengine-0.8.0/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/timer.py` & `mmengine-0.8.0/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/utils/version_utils.py` & `mmengine-0.8.0/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/version.py` & `mmengine-0.8.0/mmengine/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.7.4'
+__version__ = '0.8.0'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.7.4/mmengine/visualization/utils.py` & `mmengine-0.8.0/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine/visualization/vis_backend.py` & `mmengine-0.8.0/mmengine/visualization/vis_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,18 @@
     @force_init_env
     def add_config(self, config: Config, **kwargs) -> None:
         """Record the config to wandb.
 
         Args:
             config (Config): The Config object
         """
-        self._wandb.config.update(dict(config))
+        assert isinstance(self._init_kwargs, dict)
+        allow_val_change = self._init_kwargs.get('allow_val_change', False)
+        self._wandb.config.update(
+            dict(config), allow_val_change=allow_val_change)
         self._wandb.run.log_code(name=self._log_code_name)
 
     @force_init_env
     def add_graph(self, model: torch.nn.Module, data_batch: Sequence[dict],
                   **kwargs) -> None:
         """Record the model graph.
```

### Comparing `mmengine-0.7.4/mmengine/visualization/visualizer.py` & `mmengine-0.8.0/mmengine/visualization/visualizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.7.4/mmengine.egg-info/PKG-INFO` & `mmengine-0.8.0/mmengine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6d 656e  : 2.1.Name: mmen
 00000020: 6769 6e65 0a56 6572 7369 6f6e 3a20 302e  gine.Version: 0.
-00000030: 372e 340a 5375 6d6d 6172 793a 2045 6e67  7.4.Summary: Eng
+00000030: 382e 300a 5375 6d6d 6172 793a 2045 6e67  8.0.Summary: Eng
 00000040: 696e 6520 6f66 204f 7065 6e4d 4d4c 6162  ine of OpenMMLab
 00000050: 2070 726f 6a65 6374 730a 486f 6d65 2d70   projects.Home-p
 00000060: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000070: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
 00000080: 6162 2f6d 6d65 6e67 696e 650a 4175 7468  ab/mmengine.Auth
 00000090: 6f72 3a20 4d4d 456e 6769 6e65 2041 7574  or: MMEngine Aut
 000000a0: 686f 7273 0a41 7574 686f 722d 656d 6169  hors.Author-emai
@@ -261,1018 +261,1067 @@
 00001040: 2f32 3139 3032 3631 3230 2d62 6137 3165  /219026120-ba71e
 00001050: 3438 622d 3665 3934 2d34 6264 342d 6234  48b-6e94-4bd4-b4
 00001060: 6539 2d62 3764 3137 3562 3565 3336 322e  e9-b7d175b5e362.
 00001070: 706e 6722 2077 6964 7468 3d22 3325 2220  png" width="3%" 
 00001080: 616c 743d 2222 202f 3e3c 2f61 3e0a 2020  alt="" /></a>.  
 00001090: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
 000010a0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-000010b0: 2049 6e74 726f 6475 6374 696f 6e0a 2020   Introduction.  
-000010c0: 2020 2020 2020 0a20 2020 2020 2020 204d        .        M
-000010d0: 4d45 6e67 696e 6520 6973 2061 2066 6f75  MEngine is a fou
-000010e0: 6e64 6174 696f 6e61 6c20 6c69 6272 6172  ndational librar
-000010f0: 7920 666f 7220 7472 6169 6e69 6e67 2064  y for training d
-00001100: 6565 7020 6c65 6172 6e69 6e67 206d 6f64  eep learning mod
-00001110: 656c 7320 6261 7365 6420 6f6e 2050 7954  els based on PyT
-00001120: 6f72 6368 2e20 4974 2070 726f 7669 6465  orch. It provide
-00001130: 7320 6120 736f 6c69 6420 656e 6769 6e65  s a solid engine
-00001140: 6572 696e 6720 666f 756e 6461 7469 6f6e  ering foundation
-00001150: 2061 6e64 2066 7265 6573 2064 6576 656c   and frees devel
-00001160: 6f70 6572 7320 6672 6f6d 2077 7269 7469  opers from writi
-00001170: 6e67 2072 6564 756e 6461 6e74 2063 6f64  ng redundant cod
-00001180: 6573 206f 6e20 776f 726b 666c 6f77 732e  es on workflows.
-00001190: 2049 7420 7365 7276 6573 2061 7320 7468   It serves as th
-000011a0: 6520 7472 6169 6e69 6e67 2065 6e67 696e  e training engin
-000011b0: 6520 6f66 2061 6c6c 204f 7065 6e4d 4d4c  e of all OpenMML
-000011c0: 6162 2063 6f64 6562 6173 6573 2c20 7768  ab codebases, wh
-000011d0: 6963 6820 7375 7070 6f72 7420 6875 6e64  ich support hund
-000011e0: 7265 6473 206f 6620 616c 676f 7269 7468  reds of algorith
-000011f0: 6d73 2069 6e20 7661 7269 6f75 7320 7265  ms in various re
-00001200: 7365 6172 6368 2061 7265 6173 2e20 4d6f  search areas. Mo
-00001210: 7265 6f76 6572 2c20 4d4d 456e 6769 6e65  reover, MMEngine
-00001220: 2069 7320 616c 736f 2067 656e 6572 6963   is also generic
-00001230: 2074 6f20 6265 2061 7070 6c69 6564 2074   to be applied t
-00001240: 6f20 6e6f 6e2d 4f70 656e 4d4d 4c61 6220  o non-OpenMMLab 
-00001250: 7072 6f6a 6563 7473 2e0a 2020 2020 2020  projects..      
-00001260: 2020 0a20 2020 2020 2020 204d 616a 6f72    .        Major
-00001270: 2066 6561 7475 7265 733a 0a20 2020 2020   features:.     
-00001280: 2020 200a 2020 2020 2020 2020 312e 202a     .        1. *
-00001290: 2a41 2075 6e69 7665 7273 616c 2061 6e64  *A universal and
-000012a0: 2070 6f77 6572 6675 6c20 7275 6e6e 6572   powerful runner
-000012b0: 2a2a 3a0a 2020 2020 2020 2020 0a20 2020  **:.        .   
-000012c0: 2020 2020 2020 2020 2d20 5375 7070 6f72          - Suppor
-000012d0: 7473 2074 7261 696e 696e 6720 6469 6666  ts training diff
-000012e0: 6572 656e 7420 7461 736b 7320 7769 7468  erent tasks with
-000012f0: 2061 2073 6d61 6c6c 2061 6d6f 756e 7420   a small amount 
-00001300: 6f66 2063 6f64 652c 2065 2e67 2e2c 2049  of code, e.g., I
-00001310: 6d61 6765 4e65 7420 6361 6e20 6265 2074  mageNet can be t
-00001320: 7261 696e 6564 2077 6974 6820 6f6e 6c79  rained with only
-00001330: 2038 3020 6c69 6e65 7320 6f66 2063 6f64   80 lines of cod
-00001340: 6520 2834 3030 206c 696e 6573 206f 6620  e (400 lines of 
-00001350: 7468 6520 6f72 6967 696e 616c 2050 7954  the original PyT
-00001360: 6f72 6368 2065 7861 6d70 6c65 292e 0a20  orch example).. 
-00001370: 2020 2020 2020 2020 2020 2d20 4561 7369            - Easi
-00001380: 6c79 2063 6f6d 7061 7469 626c 6520 7769  ly compatible wi
-00001390: 7468 206d 6f64 656c 7320 6672 6f6d 2070  th models from p
-000013a0: 6f70 756c 6172 2061 6c67 6f72 6974 686d  opular algorithm
-000013b0: 206c 6962 7261 7269 6573 2073 7563 6820   libraries such 
-000013c0: 6173 2054 494d 4d2c 2054 6f72 6368 5669  as TIMM, TorchVi
-000013d0: 7369 6f6e 2c20 616e 6420 4465 7465 6374  sion, and Detect
-000013e0: 726f 6e32 2e0a 2020 2020 2020 2020 0a20  ron2..        . 
-000013f0: 2020 2020 2020 2032 2e20 2a2a 4f70 656e         2. **Open
-00001400: 2061 7263 6869 7465 6374 7572 6520 7769   architecture wi
-00001410: 7468 2075 6e69 6669 6564 2069 6e74 6572  th unified inter
-00001420: 6661 6365 732a 2a3a 0a20 2020 2020 2020  faces**:.       
-00001430: 200a 2020 2020 2020 2020 2020 202d 2048   .           - H
-00001440: 616e 646c 6573 2064 6966 6665 7265 6e74  andles different
-00001450: 2061 6c67 6f72 6974 686d 2074 6173 6b73   algorithm tasks
-00001460: 2077 6974 6820 756e 6966 6965 6420 4150   with unified AP
-00001470: 4973 2c20 652e 672e 2c20 696d 706c 656d  Is, e.g., implem
-00001480: 656e 7420 6120 6d65 7468 6f64 2061 6e64  ent a method and
-00001490: 2061 7070 6c79 2069 7420 746f 2061 6c6c   apply it to all
-000014a0: 2063 6f6d 7061 7469 626c 6520 6d6f 6465   compatible mode
-000014b0: 6c73 2e0a 2020 2020 2020 2020 2020 202d  ls..           -
-000014c0: 2050 726f 7669 6465 7320 6120 756e 6966   Provides a unif
-000014d0: 6965 6420 6162 7374 7261 6374 696f 6e20  ied abstraction 
-000014e0: 666f 7220 7570 7065 722d 6c65 7665 6c20  for upper-level 
-000014f0: 616c 676f 7269 7468 6d20 6c69 6272 6172  algorithm librar
-00001500: 6965 732c 2077 6869 6368 2073 7570 706f  ies, which suppo
-00001510: 7274 7320 7661 7269 6f75 7320 6261 636b  rts various back
-00001520: 2d65 6e64 2064 6576 6963 6573 2073 7563  -end devices suc
-00001530: 6820 6173 204e 7669 6469 6120 4355 4441  h as Nvidia CUDA
-00001540: 2c20 4d61 6320 4d50 532c 2041 4d44 2c20  , Mac MPS, AMD, 
-00001550: 4d4c 552c 2061 6e64 206d 6f72 6520 666f  MLU, and more fo
-00001560: 7220 6d6f 6465 6c20 7472 6169 6e69 6e67  r model training
-00001570: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00001580: 2020 2033 2e20 2a2a 4375 7374 6f6d 697a     3. **Customiz
-00001590: 6162 6c65 2074 7261 696e 696e 6720 7072  able training pr
-000015a0: 6f63 6573 732a 2a3a 0a20 2020 2020 2020  ocess**:.       
-000015b0: 200a 2020 2020 2020 2020 2020 202d 2044   .           - D
-000015c0: 6566 696e 6573 2074 6865 2074 7261 696e  efines the train
-000015d0: 696e 6720 7072 6f63 6573 7320 6a75 7374  ing process just
-000015e0: 206c 696b 6520 706c 6179 696e 6720 7769   like playing wi
-000015f0: 7468 204c 6567 6f73 2e0a 2020 2020 2020  th Legos..      
-00001600: 2020 2020 202d 2050 726f 7669 6465 7320       - Provides 
-00001610: 7269 6368 2063 6f6d 706f 6e65 6e74 7320  rich components 
-00001620: 616e 6420 7374 7261 7465 6769 6573 2e0a  and strategies..
-00001630: 2020 2020 2020 2020 2020 202d 2043 6f6d             - Com
-00001640: 706c 6574 6520 636f 6e74 726f 6c73 206f  plete controls o
-00001650: 6e20 7468 6520 7472 6169 6e69 6e67 2070  n the training p
-00001660: 726f 6365 7373 2077 6974 6820 6469 6666  rocess with diff
-00001670: 6572 656e 7420 6c65 7665 6c73 206f 6620  erent levels of 
-00001680: 4150 4973 2e0a 2020 2020 2020 2020 0a20  APIs..        . 
-00001690: 2020 2020 2020 2023 2320 5768 6174 2773         ## What's
-000016a0: 204e 6577 0a20 2020 2020 2020 200a 2020   New.        .  
-000016b0: 2020 2020 2020 7630 2e37 2e34 2077 6173        v0.7.4 was
-000016c0: 2072 656c 6561 7365 6420 6f6e 2032 3032   released on 202
-000016d0: 332d 3036 2d30 332e 0a20 2020 2020 2020  3-06-03..       
-000016e0: 200a 2020 2020 2020 2020 2323 2320 4869   .        ### Hi
-000016f0: 6768 6c69 6768 7473 0a20 2020 2020 2020  ghlights.       
-00001700: 200a 2020 2020 2020 2020 2d20 5375 7070   .        - Supp
-00001710: 6f72 7420 7573 696e 6720 5b60 436c 6561  ort using [`Clea
-00001720: 724d 4c60 5d28 6874 7470 733a 2f2f 6d6d  rML`](https://mm
-00001730: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
-00001740: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001750: 636f 6d6d 6f6e 5f75 7361 6765 2f76 6973  common_usage/vis
-00001760: 7561 6c69 7a65 5f74 7261 696e 696e 675f  ualize_training_
-00001770: 6c6f 672e 6874 6d6c 2363 6c65 6172 6d6c  log.html#clearml
-00001780: 2920 746f 2072 6563 6f72 6420 6578 7065  ) to record expe
-00001790: 7269 6d65 6e74 2064 6174 610a 2020 2020  riment data.    
-000017a0: 2020 2020 2d20 4164 6420 5b60 536f 7068      - Add [`Soph
-000017b0: 6961 605d 2868 7474 7073 3a2f 2f6d 6d65  ia`](https://mme
-000017c0: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
-000017d0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f63  s.io/en/latest/c
-000017e0: 6f6d 6d6f 6e5f 7573 6167 652f 6265 7474  ommon_usage/bett
-000017f0: 6572 5f6f 7074 696d 697a 6572 732e 6874  er_optimizers.ht
-00001800: 6d6c 2373 6f70 6869 6129 206f 7074 696d  ml#sophia) optim
-00001810: 697a 6572 730a 2020 2020 2020 2020 0a20  izers.        . 
-00001820: 2020 2020 2020 2052 6561 6420 5b43 6861         Read [Cha
-00001830: 6e67 656c 6f67 5d28 2e2f 646f 6373 2f65  ngelog](./docs/e
-00001840: 6e2f 6e6f 7465 732f 6368 616e 6765 6c6f  n/notes/changelo
-00001850: 672e 6d64 2376 3037 342d 3036 3033 3230  g.md#v074-060320
-00001860: 3233 2920 666f 7220 6d6f 7265 2064 6574  23) for more det
-00001870: 6169 6c73 2e0a 2020 2020 2020 2020 0a20  ails..        . 
-00001880: 2020 2020 2020 2023 2320 496e 7374 616c         ## Instal
-00001890: 6c61 7469 6f6e 0a20 2020 2020 2020 200a  lation.        .
-000018a0: 2020 2020 2020 2020 4265 666f 7265 2069          Before i
-000018b0: 6e73 7461 6c6c 696e 6720 4d4d 456e 6769  nstalling MMEngi
-000018c0: 6e65 2c20 706c 6561 7365 2065 6e73 7572  ne, please ensur
-000018d0: 6520 7468 6174 2050 7954 6f72 6368 2068  e that PyTorch h
-000018e0: 6173 2062 6565 6e20 7375 6363 6573 7366  as been successf
-000018f0: 756c 6c79 2069 6e73 7461 6c6c 6564 2066  ully installed f
-00001900: 6f6c 6c6f 7769 6e67 2074 6865 205b 6f66  ollowing the [of
-00001910: 6669 6369 616c 2067 7569 6465 5d28 6874  ficial guide](ht
-00001920: 7470 733a 2f2f 7079 746f 7263 682e 6f72  tps://pytorch.or
-00001930: 672f 6765 742d 7374 6172 7465 642f 6c6f  g/get-started/lo
-00001940: 6361 6c6c 792f 292e 0a20 2020 2020 2020  cally/)..       
-00001950: 200a 2020 2020 2020 2020 496e 7374 616c   .        Instal
-00001960: 6c20 4d4d 456e 6769 6e65 0a20 2020 2020  l MMEngine.     
-00001970: 2020 200a 2020 2020 2020 2020 6060 6062     .        ```b
-00001980: 6173 680a 2020 2020 2020 2020 7069 7020  ash.        pip 
-00001990: 696e 7374 616c 6c20 2d55 206f 7065 6e6d  install -U openm
-000019a0: 696d 0a20 2020 2020 2020 206d 696d 2069  im.        mim i
-000019b0: 6e73 7461 6c6c 206d 6d65 6e67 696e 650a  nstall mmengine.
-000019c0: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
-000019d0: 2020 2020 0a20 2020 2020 2020 2056 6572      .        Ver
-000019e0: 6966 7920 7468 6520 696e 7374 616c 6c61  ify the installa
-000019f0: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
-00001a00: 2020 2020 2020 6060 6062 6173 680a 2020        ```bash.  
-00001a10: 2020 2020 2020 7079 7468 6f6e 202d 6320        python -c 
-00001a20: 2766 726f 6d20 6d6d 656e 6769 6e65 2e75  'from mmengine.u
-00001a30: 7469 6c73 2e64 6c5f 7574 696c 7320 696d  tils.dl_utils im
-00001a40: 706f 7274 2063 6f6c 6c65 6374 5f65 6e76  port collect_env
-00001a50: 3b70 7269 6e74 2863 6f6c 6c65 6374 5f65  ;print(collect_e
-00001a60: 6e76 2829 2927 0a20 2020 2020 2020 2060  nv())'.        `
-00001a70: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00001a80: 2020 2020 2323 2047 6574 2053 7461 7274      ## Get Start
-00001a90: 6564 0a20 2020 2020 2020 200a 2020 2020  ed.        .    
-00001aa0: 2020 2020 5461 6b69 6e67 2074 6865 2074      Taking the t
-00001ab0: 7261 696e 696e 6720 6f66 2061 2052 6573  raining of a Res
-00001ac0: 4e65 742d 3530 206d 6f64 656c 206f 6e20  Net-50 model on 
-00001ad0: 7468 6520 4349 4641 522d 3130 2064 6174  the CIFAR-10 dat
-00001ae0: 6173 6574 2061 7320 616e 2065 7861 6d70  aset as an examp
-00001af0: 6c65 2c20 7765 2077 696c 6c20 7573 6520  le, we will use 
-00001b00: 4d4d 456e 6769 6e65 2074 6f20 6275 696c  MMEngine to buil
-00001b10: 6420 6120 636f 6d70 6c65 7465 2c20 636f  d a complete, co
-00001b20: 6e66 6967 7572 6162 6c65 2074 7261 696e  nfigurable train
-00001b30: 696e 6720 616e 6420 7661 6c69 6461 7469  ing and validati
-00001b40: 6f6e 2070 726f 6365 7373 2069 6e20 6c65  on process in le
-00001b50: 7373 2074 6861 6e20 3830 206c 696e 6573  ss than 80 lines
-00001b60: 206f 6620 636f 6465 2e0a 2020 2020 2020   of code..      
-00001b70: 2020 0a20 2020 2020 2020 203c 6465 7461    .        <deta
-00001b80: 696c 733e 0a20 2020 2020 2020 203c 7375  ils>.        <su
-00001b90: 6d6d 6172 793e 4275 696c 6420 4d6f 6465  mmary>Build Mode
-00001ba0: 6c73 3c2f 7375 6d6d 6172 793e 0a20 2020  ls</summary>.   
-00001bb0: 2020 2020 200a 2020 2020 2020 2020 4669       .        Fi
-00001bc0: 7273 742c 2077 6520 6e65 6564 2074 6f20  rst, we need to 
-00001bd0: 6465 6669 6e65 2061 202a 2a6d 6f64 656c  define a **model
-00001be0: 2a2a 2077 6869 6368 2031 2920 696e 6865  ** which 1) inhe
-00001bf0: 7269 7473 2066 726f 6d20 6042 6173 654d  rits from `BaseM
-00001c00: 6f64 656c 6020 616e 6420 3229 2061 6363  odel` and 2) acc
-00001c10: 6570 7473 2061 6e20 6164 6469 7469 6f6e  epts an addition
-00001c20: 616c 2061 7267 756d 656e 7420 606d 6f64  al argument `mod
-00001c30: 6560 2069 6e20 7468 6520 6066 6f72 7761  e` in the `forwa
-00001c40: 7264 6020 6d65 7468 6f64 2c20 696e 2061  rd` method, in a
-00001c50: 6464 6974 696f 6e20 746f 2074 686f 7365  ddition to those
-00001c60: 2061 7267 756d 656e 7473 2072 656c 6174   arguments relat
-00001c70: 6564 2074 6f20 7468 6520 6461 7461 7365  ed to the datase
-00001c80: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-00001c90: 2020 2020 2d20 4475 7269 6e67 2074 7261      - During tra
-00001ca0: 696e 696e 672c 2074 6865 2076 616c 7565  ining, the value
-00001cb0: 206f 6620 606d 6f64 6560 2069 7320 226c   of `mode` is "l
-00001cc0: 6f73 7322 2c20 616e 6420 7468 6520 6066  oss", and the `f
-00001cd0: 6f72 7761 7264 6020 6d65 7468 6f64 2073  orward` method s
-00001ce0: 686f 756c 6420 7265 7475 726e 2061 2060  hould return a `
-00001cf0: 6469 6374 6020 636f 6e74 6169 6e69 6e67  dict` containing
-00001d00: 2074 6865 206b 6579 2022 6c6f 7373 222e   the key "loss".
-00001d10: 0a20 2020 2020 2020 202d 2044 7572 696e  .        - Durin
-00001d20: 6720 7661 6c69 6461 7469 6f6e 2c20 7468  g validation, th
-00001d30: 6520 7661 6c75 6520 6f66 2060 6d6f 6465  e value of `mode
-00001d40: 6020 6973 2022 7072 6564 6963 7422 2c20  ` is "predict", 
-00001d50: 616e 6420 7468 6520 666f 7277 6172 6420  and the forward 
-00001d60: 6d65 7468 6f64 2073 686f 756c 6420 7265  method should re
-00001d70: 7475 726e 2072 6573 756c 7473 2063 6f6e  turn results con
-00001d80: 7461 696e 696e 6720 626f 7468 2070 7265  taining both pre
-00001d90: 6469 6374 696f 6e73 2061 6e64 206c 6162  dictions and lab
-00001da0: 656c 732e 0a20 2020 2020 2020 200a 2020  els..        .  
-00001db0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00001dc0: 2020 2020 2020 2020 696d 706f 7274 2074          import t
-00001dd0: 6f72 6368 2e6e 6e2e 6675 6e63 7469 6f6e  orch.nn.function
-00001de0: 616c 2061 7320 460a 2020 2020 2020 2020  al as F.        
-00001df0: 696d 706f 7274 2074 6f72 6368 7669 7369  import torchvisi
-00001e00: 6f6e 0a20 2020 2020 2020 2066 726f 6d20  on.        from 
-00001e10: 6d6d 656e 6769 6e65 2e6d 6f64 656c 2069  mmengine.model i
-00001e20: 6d70 6f72 7420 4261 7365 4d6f 6465 6c0a  mport BaseModel.
-00001e30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001e40: 2063 6c61 7373 204d 4d52 6573 4e65 7435   class MMResNet5
-00001e50: 3028 4261 7365 4d6f 6465 6c29 3a0a 2020  0(BaseModel):.  
-00001e60: 2020 2020 2020 2020 2020 6465 6620 5f5f            def __
-00001e70: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-00001e80: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00001e90: 7065 7228 292e 5f5f 696e 6974 5f5f 2829  per().__init__()
-00001ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001eb0: 2073 656c 662e 7265 736e 6574 203d 2074   self.resnet = t
-00001ec0: 6f72 6368 7669 7369 6f6e 2e6d 6f64 656c  orchvision.model
-00001ed0: 732e 7265 736e 6574 3530 2829 0a20 2020  s.resnet50().   
-00001ee0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00001ef0: 2020 6465 6620 666f 7277 6172 6428 7365    def forward(se
-00001f00: 6c66 2c20 696d 6773 2c20 6c61 6265 6c73  lf, imgs, labels
-00001f10: 2c20 6d6f 6465 293a 0a20 2020 2020 2020  , mode):.       
-00001f20: 2020 2020 2020 2020 2078 203d 2073 656c           x = sel
-00001f30: 662e 7265 736e 6574 2869 6d67 7329 0a20  f.resnet(imgs). 
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001f50: 6620 6d6f 6465 203d 3d20 276c 6f73 7327  f mode == 'loss'
-00001f60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001f70: 2020 2020 2020 7265 7475 726e 207b 276c        return {'l
-00001f80: 6f73 7327 3a20 462e 6372 6f73 735f 656e  oss': F.cross_en
-00001f90: 7472 6f70 7928 782c 206c 6162 656c 7329  tropy(x, labels)
-00001fa0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00001fb0: 2020 656c 6966 206d 6f64 6520 3d3d 2027    elif mode == '
-00001fc0: 7072 6564 6963 7427 3a0a 2020 2020 2020  predict':.      
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001fe0: 7475 726e 2078 2c20 6c61 6265 6c73 0a20  turn x, labels. 
-00001ff0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00002000: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
-00002010: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
-00002020: 2020 2020 2020 2020 3c64 6574 6169 6c73          <details
-00002030: 3e0a 2020 2020 2020 2020 3c73 756d 6d61  >.        <summa
-00002040: 7279 3e42 7569 6c64 2044 6174 6173 6574  ry>Build Dataset
-00002050: 733c 2f73 756d 6d61 7279 3e0a 2020 2020  s</summary>.    
-00002060: 2020 2020 0a20 2020 2020 2020 204e 6578      .        Nex
-00002070: 742c 2077 6520 6e65 6564 2074 6f20 6372  t, we need to cr
-00002080: 6561 7465 202a 2a44 6174 6173 6574 2a2a  eate **Dataset**
-00002090: 7320 616e 6420 2a2a 4461 7461 4c6f 6164  s and **DataLoad
-000020a0: 6572 2a2a 7320 666f 7220 7472 6169 6e69  er**s for traini
-000020b0: 6e67 2061 6e64 2076 616c 6964 6174 696f  ng and validatio
-000020c0: 6e2e 0a20 2020 2020 2020 2049 6e20 7468  n..        In th
-000020d0: 6973 2063 6173 652c 2077 6520 7369 6d70  is case, we simp
-000020e0: 6c79 2075 7365 2062 7569 6c74 2d69 6e20  ly use built-in 
-000020f0: 6461 7461 7365 7473 2073 7570 706f 7274  datasets support
-00002100: 6564 2069 6e20 546f 7263 6856 6973 696f  ed in TorchVisio
-00002110: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00002120: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
-00002130: 2020 2020 2020 696d 706f 7274 2074 6f72        import tor
-00002140: 6368 7669 7369 6f6e 2e74 7261 6e73 666f  chvision.transfo
-00002150: 726d 7320 6173 2074 7261 6e73 666f 726d  rms as transform
-00002160: 730a 2020 2020 2020 2020 6672 6f6d 2074  s.        from t
-00002170: 6f72 6368 2e75 7469 6c73 2e64 6174 6120  orch.utils.data 
-00002180: 696d 706f 7274 2044 6174 614c 6f61 6465  import DataLoade
-00002190: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-000021a0: 2020 206e 6f72 6d5f 6366 6720 3d20 6469     norm_cfg = di
-000021b0: 6374 286d 6561 6e3d 5b30 2e34 3931 2c20  ct(mean=[0.491, 
-000021c0: 302e 3438 322c 2030 2e34 3437 5d2c 2073  0.482, 0.447], s
-000021d0: 7464 3d5b 302e 3230 322c 2030 2e31 3939  td=[0.202, 0.199
-000021e0: 2c20 302e 3230 315d 290a 2020 2020 2020  , 0.201]).      
-000021f0: 2020 7472 6169 6e5f 6461 7461 6c6f 6164    train_dataload
-00002200: 6572 203d 2044 6174 614c 6f61 6465 7228  er = DataLoader(
-00002210: 6261 7463 685f 7369 7a65 3d33 322c 0a20  batch_size=32,. 
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002240: 2020 2020 2073 6875 6666 6c65 3d54 7275       shuffle=Tru
-00002250: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
-00002280: 3d74 6f72 6368 7669 7369 6f6e 2e64 6174  =torchvision.dat
-00002290: 6173 6574 732e 4349 4641 5231 3028 0a20  asets.CIFAR10(. 
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2057 6861 7427 7320 4e65 770a 2020 2020   What's New.    
+000010c0: 2020 2020 0a20 2020 2020 2020 2076 302e      .        v0.
+000010d0: 382e 3020 7761 7320 7265 6c65 6173 6564  8.0 was released
+000010e0: 206f 6e20 3230 3233 2d30 362d 3330 2e0a   on 2023-06-30..
+000010f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001100: 2048 6967 686c 6967 6874 733a 0a20 2020   Highlights:.   
+00001110: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00001120: 5375 7070 6f72 7420 7472 6169 6e69 6e67  Support training
+00001130: 2077 6974 6820 5b46 5344 505d 2868 7474   with [FSDP](htt
+00001140: 7073 3a2f 2f70 7974 6f72 6368 2e6f 7267  ps://pytorch.org
+00001150: 2f74 7574 6f72 6961 6c73 2f69 6e74 6572  /tutorials/inter
+00001160: 6d65 6469 6174 652f 4653 4450 5f61 6461  mediate/FSDP_ada
+00001170: 766e 6365 645f 7475 746f 7269 616c 2e68  vnced_tutorial.h
+00001180: 746d 6c3f 6869 6768 6c69 6768 743d 6673  tml?highlight=fs
+00001190: 6470 2920 616e 6420 5b44 6565 7053 7065  dp) and [DeepSpe
+000011a0: 6564 5d28 6874 7470 733a 2f2f 7777 772e  ed](https://www.
+000011b0: 6465 6570 7370 6565 642e 6169 2f29 2e20  deepspeed.ai/). 
+000011c0: 5265 6665 7220 746f 2074 6865 205b 6578  Refer to the [ex
+000011d0: 616d 706c 655d 2868 7474 7073 3a2f 2f67  ample](https://g
+000011e0: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+000011f0: 6d6c 6162 2f6d 6d65 6e67 696e 652f 626c  mlab/mmengine/bl
+00001200: 6f62 2f6d 6169 6e2f 6578 616d 706c 6573  ob/main/examples
+00001210: 2f64 6973 7472 6962 7574 6564 5f74 7261  /distributed_tra
+00001220: 696e 696e 675f 7769 7468 5f66 6c65 7869  ining_with_flexi
+00001230: 626c 655f 7275 6e6e 6572 2e70 7929 2066  ble_runner.py) f
+00001240: 6f72 206d 6f72 6520 6465 7461 696c 6564  or more detailed
+00001250: 2075 7361 6765 732e 0a20 2020 2020 2020   usages..       
+00001260: 200a 2020 2020 2020 2020 2d20 496e 7472   .        - Intr
+00001270: 6f64 7563 6520 7468 6520 7075 7265 2050  oduce the pure P
+00001280: 7974 686f 6e20 7374 796c 6520 636f 6e66  ython style conf
+00001290: 6967 7572 6174 696f 6e20 6669 6c65 3a0a  iguration file:.
+000012a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000012b0: 2020 202d 2053 7570 706f 7274 206e 6176     - Support nav
+000012c0: 6967 6174 696e 6720 746f 2062 6173 6520  igating to base 
+000012d0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+000012e0: 6c65 2069 6e20 4944 450a 2020 2020 2020  le in IDE.      
+000012f0: 2020 2020 2d20 5375 7070 6f72 7420 6e61      - Support na
+00001300: 7669 6761 7469 6e67 2074 6f20 6261 7365  vigating to base
+00001310: 2076 6172 6961 626c 6520 696e 2049 4445   variable in IDE
+00001320: 0a20 2020 2020 2020 2020 202d 2053 7570  .          - Sup
+00001330: 706f 7274 206e 6176 6967 6174 696e 6720  port navigating 
+00001340: 746f 2073 6f75 7263 6520 636f 6465 206f  to source code o
+00001350: 6620 636c 6173 7320 696e 2049 4445 0a20  f class in IDE. 
+00001360: 2020 2020 2020 2020 202d 2053 7570 706f           - Suppo
+00001370: 7274 2069 6e68 6572 6974 696e 6720 7477  rt inheriting tw
+00001380: 6f20 636f 6e66 6967 7572 6174 696f 6e20  o configuration 
+00001390: 6669 6c65 7320 636f 6e74 6169 6e69 6e67  files containing
+000013a0: 2074 6865 2073 616d 6520 6669 656c 640a   the same field.
+000013b0: 2020 2020 2020 2020 2020 2d20 4c6f 6164            - Load
+000013c0: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+000013d0: 6f6e 2066 696c 6520 7769 7468 6f75 7420  on file without 
+000013e0: 6f74 6865 7220 7468 6972 642d 7061 7274  other third-part
+000013f0: 7920 7265 7175 6972 656d 656e 7473 0a20  y requirements. 
+00001400: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001410: 2020 5265 6665 7220 746f 2074 6865 205b    Refer to the [
+00001420: 7475 746f 7269 616c 5d28 6874 7470 733a  tutorial](https:
+00001430: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+00001440: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001450: 6573 742f 6164 7661 6e63 6564 5f74 7574  est/advanced_tut
+00001460: 6f72 6961 6c73 2f63 6f6e 6669 672e 6874  orials/config.ht
+00001470: 6d6c 2361 2d70 7572 652d 7079 7468 6f6e  ml#a-pure-python
+00001480: 2d73 7479 6c65 2d63 6f6e 6669 6775 7261  -style-configura
+00001490: 7469 6f6e 2d66 696c 652d 6265 7461 2920  tion-file-beta) 
+000014a0: 666f 7220 6d6f 7265 2064 6574 6169 6c65  for more detaile
+000014b0: 6420 7573 6167 6573 2e0a 2020 2020 2020  d usages..      
+000014c0: 2020 0a20 2020 2020 2020 2020 2021 5b6e    .          ![n
+000014d0: 6577 2d63 6f6e 6669 672d 656e 5d28 6874  ew-config-en](ht
+000014e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000014f0: 2f6f 7065 6e2d 6d6d 6c61 622f 6d6d 656e  /open-mmlab/mmen
+00001500: 6769 6e65 2f61 7373 6574 732f 3537 3536  gine/assets/5756
+00001510: 3636 3330 2f37 6562 3431 3734 382d 3933  6630/7eb41748-93
+00001520: 3734 2d34 3838 662d 3930 3165 2d66 6364  74-488f-901e-fcd
+00001530: 3766 3064 3363 3861 3129 0a20 2020 2020  7f0d3c8a1).     
+00001540: 2020 200a 2020 2020 2020 2020 5265 6164     .        Read
+00001550: 205b 4368 616e 6765 6c6f 675d 282e 2f64   [Changelog](./d
+00001560: 6f63 732f 656e 2f6e 6f74 6573 2f63 6861  ocs/en/notes/cha
+00001570: 6e67 656c 6f67 2e6d 6423 7630 3830 2d30  ngelog.md#v080-0
+00001580: 3633 3032 3032 3329 2066 6f72 206d 6f72  6302023) for mor
+00001590: 6520 6465 7461 696c 732e 0a20 2020 2020  e details..     
+000015a0: 2020 200a 2020 2020 2020 2020 2323 2049     .        ## I
+000015b0: 6e74 726f 6475 6374 696f 6e0a 2020 2020  ntroduction.    
+000015c0: 2020 2020 0a20 2020 2020 2020 204d 4d45      .        MME
+000015d0: 6e67 696e 6520 6973 2061 2066 6f75 6e64  ngine is a found
+000015e0: 6174 696f 6e61 6c20 6c69 6272 6172 7920  ational library 
+000015f0: 666f 7220 7472 6169 6e69 6e67 2064 6565  for training dee
+00001600: 7020 6c65 6172 6e69 6e67 206d 6f64 656c  p learning model
+00001610: 7320 6261 7365 6420 6f6e 2050 7954 6f72  s based on PyTor
+00001620: 6368 2e20 4974 2070 726f 7669 6465 7320  ch. It provides 
+00001630: 6120 736f 6c69 6420 656e 6769 6e65 6572  a solid engineer
+00001640: 696e 6720 666f 756e 6461 7469 6f6e 2061  ing foundation a
+00001650: 6e64 2066 7265 6573 2064 6576 656c 6f70  nd frees develop
+00001660: 6572 7320 6672 6f6d 2077 7269 7469 6e67  ers from writing
+00001670: 2072 6564 756e 6461 6e74 2063 6f64 6573   redundant codes
+00001680: 206f 6e20 776f 726b 666c 6f77 732e 2049   on workflows. I
+00001690: 7420 7365 7276 6573 2061 7320 7468 6520  t serves as the 
+000016a0: 7472 6169 6e69 6e67 2065 6e67 696e 6520  training engine 
+000016b0: 6f66 2061 6c6c 204f 7065 6e4d 4d4c 6162  of all OpenMMLab
+000016c0: 2063 6f64 6562 6173 6573 2c20 7768 6963   codebases, whic
+000016d0: 6820 7375 7070 6f72 7420 6875 6e64 7265  h support hundre
+000016e0: 6473 206f 6620 616c 676f 7269 7468 6d73  ds of algorithms
+000016f0: 2069 6e20 7661 7269 6f75 7320 7265 7365   in various rese
+00001700: 6172 6368 2061 7265 6173 2e20 4d6f 7265  arch areas. More
+00001710: 6f76 6572 2c20 4d4d 456e 6769 6e65 2069  over, MMEngine i
+00001720: 7320 616c 736f 2067 656e 6572 6963 2074  s also generic t
+00001730: 6f20 6265 2061 7070 6c69 6564 2074 6f20  o be applied to 
+00001740: 6e6f 6e2d 4f70 656e 4d4d 4c61 6220 7072  non-OpenMMLab pr
+00001750: 6f6a 6563 7473 2e0a 2020 2020 2020 2020  ojects..        
+00001760: 0a20 2020 2020 2020 204d 616a 6f72 2066  .        Major f
+00001770: 6561 7475 7265 733a 0a20 2020 2020 2020  eatures:.       
+00001780: 200a 2020 2020 2020 2020 312e 202a 2a41   .        1. **A
+00001790: 2075 6e69 7665 7273 616c 2061 6e64 2070   universal and p
+000017a0: 6f77 6572 6675 6c20 7275 6e6e 6572 2a2a  owerful runner**
+000017b0: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+000017c0: 2020 2020 2020 2d20 5375 7070 6f72 7473        - Supports
+000017d0: 2074 7261 696e 696e 6720 6469 6666 6572   training differ
+000017e0: 656e 7420 7461 736b 7320 7769 7468 2061  ent tasks with a
+000017f0: 2073 6d61 6c6c 2061 6d6f 756e 7420 6f66   small amount of
+00001800: 2063 6f64 652c 2065 2e67 2e2c 2049 6d61   code, e.g., Ima
+00001810: 6765 4e65 7420 6361 6e20 6265 2074 7261  geNet can be tra
+00001820: 696e 6564 2077 6974 6820 6f6e 6c79 2038  ined with only 8
+00001830: 3020 6c69 6e65 7320 6f66 2063 6f64 6520  0 lines of code 
+00001840: 2834 3030 206c 696e 6573 206f 6620 7468  (400 lines of th
+00001850: 6520 6f72 6967 696e 616c 2050 7954 6f72  e original PyTor
+00001860: 6368 2065 7861 6d70 6c65 292e 0a20 2020  ch example)..   
+00001870: 2020 2020 2020 2020 2d20 4561 7369 6c79          - Easily
+00001880: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
+00001890: 206d 6f64 656c 7320 6672 6f6d 2070 6f70   models from pop
+000018a0: 756c 6172 2061 6c67 6f72 6974 686d 206c  ular algorithm l
+000018b0: 6962 7261 7269 6573 2073 7563 6820 6173  ibraries such as
+000018c0: 2054 494d 4d2c 2054 6f72 6368 5669 7369   TIMM, TorchVisi
+000018d0: 6f6e 2c20 616e 6420 4465 7465 6374 726f  on, and Detectro
+000018e0: 6e32 2e0a 2020 2020 2020 2020 0a20 2020  n2..        .   
+000018f0: 2020 2020 2032 2e20 2a2a 4f70 656e 2061       2. **Open a
+00001900: 7263 6869 7465 6374 7572 6520 7769 7468  rchitecture with
+00001910: 2075 6e69 6669 6564 2069 6e74 6572 6661   unified interfa
+00001920: 6365 732a 2a3a 0a20 2020 2020 2020 200a  ces**:.        .
+00001930: 2020 2020 2020 2020 2020 202d 2048 616e             - Han
+00001940: 646c 6573 2064 6966 6665 7265 6e74 2061  dles different a
+00001950: 6c67 6f72 6974 686d 2074 6173 6b73 2077  lgorithm tasks w
+00001960: 6974 6820 756e 6966 6965 6420 4150 4973  ith unified APIs
+00001970: 2c20 652e 672e 2c20 696d 706c 656d 656e  , e.g., implemen
+00001980: 7420 6120 6d65 7468 6f64 2061 6e64 2061  t a method and a
+00001990: 7070 6c79 2069 7420 746f 2061 6c6c 2063  pply it to all c
+000019a0: 6f6d 7061 7469 626c 6520 6d6f 6465 6c73  ompatible models
+000019b0: 2e0a 2020 2020 2020 2020 2020 202d 2050  ..           - P
+000019c0: 726f 7669 6465 7320 6120 756e 6966 6965  rovides a unifie
+000019d0: 6420 6162 7374 7261 6374 696f 6e20 666f  d abstraction fo
+000019e0: 7220 7570 7065 722d 6c65 7665 6c20 616c  r upper-level al
+000019f0: 676f 7269 7468 6d20 6c69 6272 6172 6965  gorithm librarie
+00001a00: 732c 2077 6869 6368 2073 7570 706f 7274  s, which support
+00001a10: 7320 7661 7269 6f75 7320 6261 636b 2d65  s various back-e
+00001a20: 6e64 2064 6576 6963 6573 2073 7563 6820  nd devices such 
+00001a30: 6173 204e 7669 6469 6120 4355 4441 2c20  as Nvidia CUDA, 
+00001a40: 4d61 6320 4d50 532c 2041 4d44 2c20 4d4c  Mac MPS, AMD, ML
+00001a50: 552c 2061 6e64 206d 6f72 6520 666f 7220  U, and more for 
+00001a60: 6d6f 6465 6c20 7472 6169 6e69 6e67 2e0a  model training..
+00001a70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001a80: 2033 2e20 2a2a 4375 7374 6f6d 697a 6162   3. **Customizab
+00001a90: 6c65 2074 7261 696e 696e 6720 7072 6f63  le training proc
+00001aa0: 6573 732a 2a3a 0a20 2020 2020 2020 200a  ess**:.        .
+00001ab0: 2020 2020 2020 2020 2020 202d 2044 6566             - Def
+00001ac0: 696e 6573 2074 6865 2074 7261 696e 696e  ines the trainin
+00001ad0: 6720 7072 6f63 6573 7320 6a75 7374 206c  g process just l
+00001ae0: 696b 6520 706c 6179 696e 6720 7769 7468  ike playing with
+00001af0: 204c 6567 6f73 2e0a 2020 2020 2020 2020   Legos..        
+00001b00: 2020 202d 2050 726f 7669 6465 7320 7269     - Provides ri
+00001b10: 6368 2063 6f6d 706f 6e65 6e74 7320 616e  ch components an
+00001b20: 6420 7374 7261 7465 6769 6573 2e0a 2020  d strategies..  
+00001b30: 2020 2020 2020 2020 202d 2043 6f6d 706c           - Compl
+00001b40: 6574 6520 636f 6e74 726f 6c73 206f 6e20  ete controls on 
+00001b50: 7468 6520 7472 6169 6e69 6e67 2070 726f  the training pro
+00001b60: 6365 7373 2077 6974 6820 6469 6666 6572  cess with differ
+00001b70: 656e 7420 6c65 7665 6c73 206f 6620 4150  ent levels of AP
+00001b80: 4973 2e0a 2020 2020 2020 2020 0a20 2020  Is..        .   
+00001b90: 2020 2020 2023 2320 496e 7374 616c 6c61       ## Installa
+00001ba0: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
+00001bb0: 2020 2020 2020 4265 666f 7265 2069 6e73        Before ins
+00001bc0: 7461 6c6c 696e 6720 4d4d 456e 6769 6e65  talling MMEngine
+00001bd0: 2c20 706c 6561 7365 2065 6e73 7572 6520  , please ensure 
+00001be0: 7468 6174 2050 7954 6f72 6368 2068 6173  that PyTorch has
+00001bf0: 2062 6565 6e20 7375 6363 6573 7366 756c   been successful
+00001c00: 6c79 2069 6e73 7461 6c6c 6564 2066 6f6c  ly installed fol
+00001c10: 6c6f 7769 6e67 2074 6865 205b 6f66 6669  lowing the [offi
+00001c20: 6369 616c 2067 7569 6465 5d28 6874 7470  cial guide](http
+00001c30: 733a 2f2f 7079 746f 7263 682e 6f72 672f  s://pytorch.org/
+00001c40: 6765 742d 7374 6172 7465 642f 6c6f 6361  get-started/loca
+00001c50: 6c6c 792f 292e 0a20 2020 2020 2020 200a  lly/)..        .
+00001c60: 2020 2020 2020 2020 496e 7374 616c 6c20          Install 
+00001c70: 4d4d 456e 6769 6e65 0a20 2020 2020 2020  MMEngine.       
+00001c80: 200a 2020 2020 2020 2020 6060 6062 6173   .        ```bas
+00001c90: 680a 2020 2020 2020 2020 7069 7020 696e  h.        pip in
+00001ca0: 7374 616c 6c20 2d55 206f 7065 6e6d 696d  stall -U openmim
+00001cb0: 0a20 2020 2020 2020 206d 696d 2069 6e73  .        mim ins
+00001cc0: 7461 6c6c 206d 6d65 6e67 696e 650a 2020  tall mmengine.  
+00001cd0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001ce0: 2020 0a20 2020 2020 2020 2056 6572 6966    .        Verif
+00001cf0: 7920 7468 6520 696e 7374 616c 6c61 7469  y the installati
+00001d00: 6f6e 0a20 2020 2020 2020 200a 2020 2020  on.        .    
+00001d10: 2020 2020 6060 6062 6173 680a 2020 2020      ```bash.    
+00001d20: 2020 2020 7079 7468 6f6e 202d 6320 2766      python -c 'f
+00001d30: 726f 6d20 6d6d 656e 6769 6e65 2e75 7469  rom mmengine.uti
+00001d40: 6c73 2e64 6c5f 7574 696c 7320 696d 706f  ls.dl_utils impo
+00001d50: 7274 2063 6f6c 6c65 6374 5f65 6e76 3b70  rt collect_env;p
+00001d60: 7269 6e74 2863 6f6c 6c65 6374 5f65 6e76  rint(collect_env
+00001d70: 2829 2927 0a20 2020 2020 2020 2060 6060  ())'.        ```
+00001d80: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001d90: 2020 2323 2047 6574 2053 7461 7274 6564    ## Get Started
+00001da0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001db0: 2020 5461 6b69 6e67 2074 6865 2074 7261    Taking the tra
+00001dc0: 696e 696e 6720 6f66 2061 2052 6573 4e65  ining of a ResNe
+00001dd0: 742d 3530 206d 6f64 656c 206f 6e20 7468  t-50 model on th
+00001de0: 6520 4349 4641 522d 3130 2064 6174 6173  e CIFAR-10 datas
+00001df0: 6574 2061 7320 616e 2065 7861 6d70 6c65  et as an example
+00001e00: 2c20 7765 2077 696c 6c20 7573 6520 4d4d  , we will use MM
+00001e10: 456e 6769 6e65 2074 6f20 6275 696c 6420  Engine to build 
+00001e20: 6120 636f 6d70 6c65 7465 2c20 636f 6e66  a complete, conf
+00001e30: 6967 7572 6162 6c65 2074 7261 696e 696e  igurable trainin
+00001e40: 6720 616e 6420 7661 6c69 6461 7469 6f6e  g and validation
+00001e50: 2070 726f 6365 7373 2069 6e20 6c65 7373   process in less
+00001e60: 2074 6861 6e20 3830 206c 696e 6573 206f   than 80 lines o
+00001e70: 6620 636f 6465 2e0a 2020 2020 2020 2020  f code..        
+00001e80: 0a20 2020 2020 2020 203c 6465 7461 696c  .        <detail
+00001e90: 733e 0a20 2020 2020 2020 203c 7375 6d6d  s>.        <summ
+00001ea0: 6172 793e 4275 696c 6420 4d6f 6465 6c73  ary>Build Models
+00001eb0: 3c2f 7375 6d6d 6172 793e 0a20 2020 2020  </summary>.     
+00001ec0: 2020 200a 2020 2020 2020 2020 4669 7273     .        Firs
+00001ed0: 742c 2077 6520 6e65 6564 2074 6f20 6465  t, we need to de
+00001ee0: 6669 6e65 2061 202a 2a6d 6f64 656c 2a2a  fine a **model**
+00001ef0: 2077 6869 6368 2031 2920 696e 6865 7269   which 1) inheri
+00001f00: 7473 2066 726f 6d20 6042 6173 654d 6f64  ts from `BaseMod
+00001f10: 656c 6020 616e 6420 3229 2061 6363 6570  el` and 2) accep
+00001f20: 7473 2061 6e20 6164 6469 7469 6f6e 616c  ts an additional
+00001f30: 2061 7267 756d 656e 7420 606d 6f64 6560   argument `mode`
+00001f40: 2069 6e20 7468 6520 6066 6f72 7761 7264   in the `forward
+00001f50: 6020 6d65 7468 6f64 2c20 696e 2061 6464  ` method, in add
+00001f60: 6974 696f 6e20 746f 2074 686f 7365 2061  ition to those a
+00001f70: 7267 756d 656e 7473 2072 656c 6174 6564  rguments related
+00001f80: 2074 6f20 7468 6520 6461 7461 7365 742e   to the dataset.
+00001f90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001fa0: 2020 2d20 4475 7269 6e67 2074 7261 696e    - During train
+00001fb0: 696e 672c 2074 6865 2076 616c 7565 206f  ing, the value o
+00001fc0: 6620 606d 6f64 6560 2069 7320 226c 6f73  f `mode` is "los
+00001fd0: 7322 2c20 616e 6420 7468 6520 6066 6f72  s", and the `for
+00001fe0: 7761 7264 6020 6d65 7468 6f64 2073 686f  ward` method sho
+00001ff0: 756c 6420 7265 7475 726e 2061 2060 6469  uld return a `di
+00002000: 6374 6020 636f 6e74 6169 6e69 6e67 2074  ct` containing t
+00002010: 6865 206b 6579 2022 6c6f 7373 222e 0a20  he key "loss".. 
+00002020: 2020 2020 2020 202d 2044 7572 696e 6720         - During 
+00002030: 7661 6c69 6461 7469 6f6e 2c20 7468 6520  validation, the 
+00002040: 7661 6c75 6520 6f66 2060 6d6f 6465 6020  value of `mode` 
+00002050: 6973 2022 7072 6564 6963 7422 2c20 616e  is "predict", an
+00002060: 6420 7468 6520 666f 7277 6172 6420 6d65  d the forward me
+00002070: 7468 6f64 2073 686f 756c 6420 7265 7475  thod should retu
+00002080: 726e 2072 6573 756c 7473 2063 6f6e 7461  rn results conta
+00002090: 696e 696e 6720 626f 7468 2070 7265 6469  ining both predi
+000020a0: 6374 696f 6e73 2061 6e64 206c 6162 656c  ctions and label
+000020b0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+000020c0: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
+000020d0: 2020 2020 2020 696d 706f 7274 2074 6f72        import tor
+000020e0: 6368 2e6e 6e2e 6675 6e63 7469 6f6e 616c  ch.nn.functional
+000020f0: 2061 7320 460a 2020 2020 2020 2020 696d   as F.        im
+00002100: 706f 7274 2074 6f72 6368 7669 7369 6f6e  port torchvision
+00002110: 0a20 2020 2020 2020 2066 726f 6d20 6d6d  .        from mm
+00002120: 656e 6769 6e65 2e6d 6f64 656c 2069 6d70  engine.model imp
+00002130: 6f72 7420 4261 7365 4d6f 6465 6c0a 2020  ort BaseModel.  
+00002140: 2020 2020 2020 0a20 2020 2020 2020 2063        .        c
+00002150: 6c61 7373 204d 4d52 6573 4e65 7435 3028  lass MMResNet50(
+00002160: 4261 7365 4d6f 6465 6c29 3a0a 2020 2020  BaseModel):.    
+00002170: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
+00002180: 6974 5f5f 2873 656c 6629 3a0a 2020 2020  it__(self):.    
+00002190: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+000021a0: 7228 292e 5f5f 696e 6974 5f5f 2829 0a20  r().__init__(). 
+000021b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000021c0: 656c 662e 7265 736e 6574 203d 2074 6f72  elf.resnet = tor
+000021d0: 6368 7669 7369 6f6e 2e6d 6f64 656c 732e  chvision.models.
+000021e0: 7265 736e 6574 3530 2829 0a20 2020 2020  resnet50().     
+000021f0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+00002200: 6465 6620 666f 7277 6172 6428 7365 6c66  def forward(self
+00002210: 2c20 696d 6773 2c20 6c61 6265 6c73 2c20  , imgs, labels, 
+00002220: 6d6f 6465 293a 0a20 2020 2020 2020 2020  mode):.         
+00002230: 2020 2020 2020 2078 203d 2073 656c 662e         x = self.
+00002240: 7265 736e 6574 2869 6d67 7329 0a20 2020  resnet(imgs).   
+00002250: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002260: 6d6f 6465 203d 3d20 276c 6f73 7327 3a0a  mode == 'loss':.
+00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002280: 2020 2020 7265 7475 726e 207b 276c 6f73      return {'los
+00002290: 7327 3a20 462e 6372 6f73 735f 656e 7472  s': F.cross_entr
+000022a0: 6f70 7928 782c 206c 6162 656c 7329 7d0a  opy(x, labels)}.
 000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2020 2020 2020 2027 6461 7461 2f63           'data/c
-000022d0: 6966 6172 3130 272c 0a20 2020 2020 2020  ifar10',.       
-000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2074 7261 696e 3d54 7275 652c 0a20     train=True,. 
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 2020 2020 2020 2064 6f77 6e6c 6f61           downloa
-00002340: 643d 5472 7565 2c0a 2020 2020 2020 2020  d=True,.        
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 7472 616e 7366 6f72 6d3d 7472 616e    transform=tran
-00002380: 7366 6f72 6d73 2e43 6f6d 706f 7365 285b  sforms.Compose([
-00002390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000023c0: 7261 6e73 666f 726d 732e 5261 6e64 6f6d  ransforms.Random
-000023d0: 4372 6f70 2833 322c 2070 6164 6469 6e67  Crop(32, padding
-000023e0: 3d34 292c 0a20 2020 2020 2020 2020 2020  =4),.           
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2074 7261 6e73 666f 726d 732e 5261     transforms.Ra
-00002420: 6e64 6f6d 486f 7269 7a6f 6e74 616c 466c  ndomHorizontalFl
-00002430: 6970 2829 2c0a 2020 2020 2020 2020 2020  ip(),.          
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 2020 2020 7472 616e 7366 6f72 6d73 2e54      transforms.T
-00002470: 6f54 656e 736f 7228 292c 0a20 2020 2020  oTensor(),.     
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-000024b0: 726d 732e 4e6f 726d 616c 697a 6528 2a2a  rms.Normalize(**
-000024c0: 6e6f 726d 5f63 6667 290a 2020 2020 2020  norm_cfg).      
-000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: 2020 2020 5d29 2929 0a20 2020 2020 2020      ]))).       
-00002500: 2076 616c 5f64 6174 616c 6f61 6465 7220   val_dataloader 
-00002510: 3d20 4461 7461 4c6f 6164 6572 2862 6174  = DataLoader(bat
-00002520: 6368 5f73 697a 653d 3332 2c0a 2020 2020  ch_size=32,.    
+000022c0: 656c 6966 206d 6f64 6520 3d3d 2027 7072  elif mode == 'pr
+000022d0: 6564 6963 7427 3a0a 2020 2020 2020 2020  edict':.        
+000022e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000022f0: 726e 2078 2c20 6c61 6265 6c73 0a20 2020  rn x, labels.   
+00002300: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+00002310: 200a 2020 2020 2020 2020 3c2f 6465 7461   .        </deta
+00002320: 696c 733e 0a20 2020 2020 2020 200a 2020  ils>.        .  
+00002330: 2020 2020 2020 3c64 6574 6169 6c73 3e0a        <details>.
+00002340: 2020 2020 2020 2020 3c73 756d 6d61 7279          <summary
+00002350: 3e42 7569 6c64 2044 6174 6173 6574 733c  >Build Datasets<
+00002360: 2f73 756d 6d61 7279 3e0a 2020 2020 2020  /summary>.      
+00002370: 2020 0a20 2020 2020 2020 204e 6578 742c    .        Next,
+00002380: 2077 6520 6e65 6564 2074 6f20 6372 6561   we need to crea
+00002390: 7465 202a 2a44 6174 6173 6574 2a2a 7320  te **Dataset**s 
+000023a0: 616e 6420 2a2a 4461 7461 4c6f 6164 6572  and **DataLoader
+000023b0: 2a2a 7320 666f 7220 7472 6169 6e69 6e67  **s for training
+000023c0: 2061 6e64 2076 616c 6964 6174 696f 6e2e   and validation.
+000023d0: 0a20 2020 2020 2020 2049 6e20 7468 6973  .        In this
+000023e0: 2063 6173 652c 2077 6520 7369 6d70 6c79   case, we simply
+000023f0: 2075 7365 2062 7569 6c74 2d69 6e20 6461   use built-in da
+00002400: 7461 7365 7473 2073 7570 706f 7274 6564  tasets supported
+00002410: 2069 6e20 546f 7263 6856 6973 696f 6e2e   in TorchVision.
+00002420: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002430: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+00002440: 2020 2020 696d 706f 7274 2074 6f72 6368      import torch
+00002450: 7669 7369 6f6e 2e74 7261 6e73 666f 726d  vision.transform
+00002460: 7320 6173 2074 7261 6e73 666f 726d 730a  s as transforms.
+00002470: 2020 2020 2020 2020 6672 6f6d 2074 6f72          from tor
+00002480: 6368 2e75 7469 6c73 2e64 6174 6120 696d  ch.utils.data im
+00002490: 706f 7274 2044 6174 614c 6f61 6465 720a  port DataLoader.
+000024a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000024b0: 206e 6f72 6d5f 6366 6720 3d20 6469 6374   norm_cfg = dict
+000024c0: 286d 6561 6e3d 5b30 2e34 3931 2c20 302e  (mean=[0.491, 0.
+000024d0: 3438 322c 2030 2e34 3437 5d2c 2073 7464  482, 0.447], std
+000024e0: 3d5b 302e 3230 322c 2030 2e31 3939 2c20  =[0.202, 0.199, 
+000024f0: 302e 3230 315d 290a 2020 2020 2020 2020  0.201]).        
+00002500: 7472 6169 6e5f 6461 7461 6c6f 6164 6572  train_dataloader
+00002510: 203d 2044 6174 614c 6f61 6465 7228 6261   = DataLoader(ba
+00002520: 7463 685f 7369 7a65 3d33 322c 0a20 2020  tch_size=32,.   
 00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 7368 7566 666c 653d 4661 6c73 652c 0a20  shuffle=False,. 
-00002560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 2020 2073 6875 6666 6c65 3d54 7275 652c     shuffle=True,
+00002560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002580: 2020 2064 6174 6173 6574 3d74 6f72 6368     dataset=torch
-00002590: 7669 7369 6f6e 2e64 6174 6173 6574 732e  vision.datasets.
-000025a0: 4349 4641 5231 3028 0a20 2020 2020 2020  CIFAR10(.       
+00002580: 2020 2020 2020 2064 6174 6173 6574 3d74         dataset=t
+00002590: 6f72 6368 7669 7369 6f6e 2e64 6174 6173  orchvision.datas
+000025a0: 6574 732e 4349 4641 5231 3028 0a20 2020  ets.CIFAR10(.   
 000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2027 6461 7461 2f63 6966 6172 3130 272c   'data/cifar10',
-000025e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000025d0: 2020 2020 2020 2027 6461 7461 2f63 6966         'data/cif
+000025e0: 6172 3130 272c 0a20 2020 2020 2020 2020  ar10',.         
 000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 2020 2020 2020 2074 7261 696e 3d46           train=F
-00002610: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2074 7261 696e 3d54 7275 652c 0a20 2020   train=True,.   
 00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2020 2020 2020 646f                do
-00002640: 776e 6c6f 6164 3d54 7275 652c 0a20 2020  wnload=True,.   
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 2064 6f77 6e6c 6f61 643d         download=
+00002650: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
 00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 2020 2074 7261 6e73 666f 726d 3d74       transform=t
-00002680: 7261 6e73 666f 726d 732e 436f 6d70 6f73  ransforms.Compos
-00002690: 6528 5b0a 2020 2020 2020 2020 2020 2020  e([.            
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 7472 616e 7366 6f72 6d3d 7472 616e 7366  transform=transf
+00002690: 6f72 6d73 2e43 6f6d 706f 7365 285b 0a20  orms.Compose([. 
 000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 7472 616e 7366 6f72 6d73 2e54 6f54 656e  transforms.ToTen
-000026d0: 736f 7228 292c 0a20 2020 2020 2020 2020  sor(),.         
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 2074 7261 6e73 666f 726d 732e 4e6f     transforms.No
-00002710: 726d 616c 697a 6528 2a2a 6e6f 726d 5f63  rmalize(**norm_c
-00002720: 6667 290a 2020 2020 2020 2020 2020 2020  fg).            
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2020 2020 2020 2020 2020 2020 5d29 2929              ])))
-00002750: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00002760: 2020 2020 200a 2020 2020 2020 2020 3c2f       .        </
-00002770: 6465 7461 696c 733e 0a20 2020 2020 2020  details>.       
-00002780: 200a 2020 2020 2020 2020 3c64 6574 6169   .        <detai
-00002790: 6c73 3e0a 2020 2020 2020 2020 3c73 756d  ls>.        <sum
-000027a0: 6d61 7279 3e42 7569 6c64 204d 6574 7269  mary>Build Metri
-000027b0: 6373 3c2f 7375 6d6d 6172 793e 0a20 2020  cs</summary>.   
-000027c0: 2020 2020 200a 2020 2020 2020 2020 546f       .        To
-000027d0: 2076 616c 6964 6174 6520 616e 6420 7465   validate and te
-000027e0: 7374 2074 6865 206d 6f64 656c 2c20 7765  st the model, we
-000027f0: 206e 6565 6420 746f 2064 6566 696e 6520   need to define 
-00002800: 6120 2a2a 4d65 7472 6963 2a2a 2063 616c  a **Metric** cal
-00002810: 6c65 6420 6163 6375 7261 6379 2074 6f20  led accuracy to 
-00002820: 6576 616c 7561 7465 2074 6865 206d 6f64  evaluate the mod
-00002830: 656c 2e20 5468 6973 206d 6574 7269 6320  el. This metric 
-00002840: 6e65 6564 7320 746f 2069 6e68 6572 6974  needs to inherit
-00002850: 2066 726f 6d20 6042 6173 654d 6574 7269   from `BaseMetri
-00002860: 6360 2061 6e64 2069 6d70 6c65 6d65 6e74  c` and implement
-00002870: 7320 7468 6520 6070 726f 6365 7373 6020  s the `process` 
-00002880: 616e 6420 6063 6f6d 7075 7465 5f6d 6574  and `compute_met
-00002890: 7269 6373 6020 6d65 7468 6f64 732e 0a20  rics` methods.. 
-000028a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000028b0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-000028c0: 2020 6672 6f6d 206d 6d65 6e67 696e 652e    from mmengine.
-000028d0: 6576 616c 7561 746f 7220 696d 706f 7274  evaluator import
-000028e0: 2042 6173 654d 6574 7269 630a 2020 2020   BaseMetric.    
-000028f0: 2020 2020 0a20 2020 2020 2020 2063 6c61      .        cla
-00002900: 7373 2041 6363 7572 6163 7928 4261 7365  ss Accuracy(Base
-00002910: 4d65 7472 6963 293a 0a20 2020 2020 2020  Metric):.       
-00002920: 2020 2020 2064 6566 2070 726f 6365 7373       def process
-00002930: 2873 656c 662c 2064 6174 615f 6261 7463  (self, data_batc
-00002940: 682c 2064 6174 615f 7361 6d70 6c65 7329  h, data_samples)
-00002950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002960: 2020 7363 6f72 652c 2067 7420 3d20 6461    score, gt = da
-00002970: 7461 5f73 616d 706c 6573 0a20 2020 2020  ta_samples.     
-00002980: 2020 2020 2020 2020 2020 2023 2053 6176             # Sav
-00002990: 6520 7468 6520 7265 7375 6c74 7320 6f66  e the results of
-000029a0: 2061 2062 6174 6368 2074 6f20 6073 656c   a batch to `sel
-000029b0: 662e 7265 7375 6c74 7360 0a20 2020 2020  f.results`.     
-000029c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000029d0: 7265 7375 6c74 732e 6170 7065 6e64 287b  results.append({
-000029e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029f0: 2020 2020 2027 6261 7463 685f 7369 7a65       'batch_size
-00002a00: 273a 206c 656e 2867 7429 2c0a 2020 2020  ': len(gt),.    
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2763 6f72 7265 6374 273a 2028 7363 6f72  'correct': (scor
-00002a30: 652e 6172 676d 6178 2864 696d 3d31 2920  e.argmax(dim=1) 
-00002a40: 3d3d 2067 7429 2e73 756d 2829 2e63 7075  == gt).sum().cpu
-00002a50: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00002a60: 2020 2020 7d29 0a20 2020 2020 2020 2020      }).         
-00002a70: 2020 2064 6566 2063 6f6d 7075 7465 5f6d     def compute_m
-00002a80: 6574 7269 6373 2873 656c 662c 2072 6573  etrics(self, res
-00002a90: 756c 7473 293a 0a20 2020 2020 2020 2020  ults):.         
-00002aa0: 2020 2020 2020 2074 6f74 616c 5f63 6f72         total_cor
-00002ab0: 7265 6374 203d 2073 756d 2869 7465 6d5b  rect = sum(item[
-00002ac0: 2763 6f72 7265 6374 275d 2066 6f72 2069  'correct'] for i
-00002ad0: 7465 6d20 696e 2072 6573 756c 7473 290a  tem in results).
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 746f 7461 6c5f 7369 7a65 203d 2073 756d  total_size = sum
-00002b00: 2869 7465 6d5b 2762 6174 6368 5f73 697a  (item['batch_siz
-00002b10: 6527 5d20 666f 7220 6974 656d 2069 6e20  e'] for item in 
-00002b20: 7265 7375 6c74 7329 0a20 2020 2020 2020  results).       
-00002b30: 2020 2020 2020 2020 2023 2052 6574 7572           # Retur
-00002b40: 6e73 2061 2064 6963 7469 6f6e 6172 7920  ns a dictionary 
-00002b50: 7769 7468 2074 6865 2072 6573 756c 7473  with the results
-00002b60: 206f 6620 7468 6520 6576 616c 7561 7465   of the evaluate
-00002b70: 6420 6d65 7472 6963 732c 0a20 2020 2020  d metrics,.     
-00002b80: 2020 2020 2020 2020 2020 2023 2077 6865             # whe
-00002b90: 7265 2074 6865 206b 6579 2069 7320 7468  re the key is th
-00002ba0: 6520 6e61 6d65 206f 6620 7468 6520 6d65  e name of the me
-00002bb0: 7472 6963 0a20 2020 2020 2020 2020 2020  tric.           
-00002bc0: 2020 2020 2072 6574 7572 6e20 6469 6374       return dict
-00002bd0: 2861 6363 7572 6163 793d 3130 3020 2a20  (accuracy=100 * 
-00002be0: 746f 7461 6c5f 636f 7272 6563 7420 2f20  total_correct / 
-00002bf0: 746f 7461 6c5f 7369 7a65 290a 2020 2020  total_size).    
-00002c00: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00002c10: 0a20 2020 2020 2020 203c 2f64 6574 6169  .        </detai
-00002c20: 6c73 3e0a 2020 2020 2020 2020 0a20 2020  ls>.        .   
-00002c30: 2020 2020 203c 6465 7461 696c 733e 0a20       <details>. 
-00002c40: 2020 2020 2020 203c 7375 6d6d 6172 793e         <summary>
-00002c50: 4275 696c 6420 6120 5275 6e6e 6572 3c2f  Build a Runner</
-00002c60: 7375 6d6d 6172 793e 0a20 2020 2020 2020  summary>.       
-00002c70: 200a 2020 2020 2020 2020 4669 6e61 6c6c   .        Finall
-00002c80: 792c 2077 6520 6361 6e20 636f 6e73 7472  y, we can constr
-00002c90: 7563 7420 6120 2a2a 5275 6e6e 6572 2a2a  uct a **Runner**
-00002ca0: 2077 6974 6820 7072 6576 696f 7573 6c79   with previously
-00002cb0: 2064 6566 696e 6564 2060 4d6f 6465 6c60   defined `Model`
-00002cc0: 2c20 6044 6174 614c 6f61 6465 7260 2c20  , `DataLoader`, 
-00002cd0: 616e 6420 604d 6574 7269 6373 602c 2077  and `Metrics`, w
-00002ce0: 6974 6820 736f 6d65 206f 7468 6572 2063  ith some other c
-00002cf0: 6f6e 6669 6773 2c20 6173 2073 686f 776e  onfigs, as shown
-00002d00: 2062 656c 6f77 2e0a 2020 2020 2020 2020   below..        
-00002d10: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
-00002d20: 6f6e 0a20 2020 2020 2020 2066 726f 6d20  on.        from 
-00002d30: 746f 7263 682e 6f70 7469 6d20 696d 706f  torch.optim impo
-00002d40: 7274 2053 4744 0a20 2020 2020 2020 2066  rt SGD.        f
-00002d50: 726f 6d20 6d6d 656e 6769 6e65 2e72 756e  rom mmengine.run
-00002d60: 6e65 7220 696d 706f 7274 2052 756e 6e65  ner import Runne
-00002d70: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-00002d80: 2020 2072 756e 6e65 7220 3d20 5275 6e6e     runner = Runn
-00002d90: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00002da0: 6d6f 6465 6c3d 4d4d 5265 734e 6574 3530  model=MMResNet50
-00002db0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00002dc0: 776f 726b 5f64 6972 3d27 2e2f 776f 726b  work_dir='./work
-00002dd0: 5f64 6972 272c 0a20 2020 2020 2020 2020  _dir',.         
-00002de0: 2020 2074 7261 696e 5f64 6174 616c 6f61     train_dataloa
-00002df0: 6465 723d 7472 6169 6e5f 6461 7461 6c6f  der=train_datalo
-00002e00: 6164 6572 2c0a 2020 2020 2020 2020 2020  ader,.          
-00002e10: 2020 2320 6120 7772 6170 7065 7220 746f    # a wrapper to
-00002e20: 2065 7865 6375 7465 2062 6163 6b20 7072   execute back pr
-00002e30: 6f70 6167 6174 696f 6e20 616e 6420 6772  opagation and gr
-00002e40: 6164 6965 6e74 2075 7064 6174 652c 2065  adient update, e
-00002e50: 7463 2e0a 2020 2020 2020 2020 2020 2020  tc..            
-00002e60: 6f70 7469 6d5f 7772 6170 7065 723d 6469  optim_wrapper=di
-00002e70: 6374 286f 7074 696d 697a 6572 3d64 6963  ct(optimizer=dic
-00002e80: 7428 7479 7065 3d53 4744 2c20 6c72 3d30  t(type=SGD, lr=0
-00002e90: 2e30 3031 2c20 6d6f 6d65 6e74 756d 3d30  .001, momentum=0
-00002ea0: 2e39 2929 2c0a 2020 2020 2020 2020 2020  .9)),.          
-00002eb0: 2020 2320 7365 7420 736f 6d65 2074 7261    # set some tra
-00002ec0: 696e 696e 6720 636f 6e66 6967 7320 6c69  ining configs li
-00002ed0: 6b65 2065 706f 6368 730a 2020 2020 2020  ke epochs.      
-00002ee0: 2020 2020 2020 7472 6169 6e5f 6366 673d        train_cfg=
-00002ef0: 6469 6374 2862 795f 6570 6f63 683d 5472  dict(by_epoch=Tr
-00002f00: 7565 2c20 6d61 785f 6570 6f63 6873 3d35  ue, max_epochs=5
-00002f10: 2c20 7661 6c5f 696e 7465 7276 616c 3d31  , val_interval=1
-00002f20: 292c 0a20 2020 2020 2020 2020 2020 2076  ),.            v
-00002f30: 616c 5f64 6174 616c 6f61 6465 723d 7661  al_dataloader=va
-00002f40: 6c5f 6461 7461 6c6f 6164 6572 2c0a 2020  l_dataloader,.  
-00002f50: 2020 2020 2020 2020 2020 7661 6c5f 6366            val_cf
-00002f60: 673d 6469 6374 2829 2c0a 2020 2020 2020  g=dict(),.      
-00002f70: 2020 2020 2020 7661 6c5f 6576 616c 7561        val_evalua
-00002f80: 746f 723d 6469 6374 2874 7970 653d 4163  tor=dict(type=Ac
-00002f90: 6375 7261 6379 292c 0a20 2020 2020 2020  curacy),.       
-00002fa0: 2029 0a20 2020 2020 2020 2060 6060 0a20   ).        ```. 
-00002fb0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002fc0: 3c2f 6465 7461 696c 733e 0a20 2020 2020  </details>.     
-00002fd0: 2020 200a 2020 2020 2020 2020 3c64 6574     .        <det
-00002fe0: 6169 6c73 3e0a 2020 2020 2020 2020 3c73  ails>.        <s
-00002ff0: 756d 6d61 7279 3e4c 6175 6e63 6820 5472  ummary>Launch Tr
-00003000: 6169 6e69 6e67 3c2f 7375 6d6d 6172 793e  aining</summary>
-00003010: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003020: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00003030: 2020 2020 7275 6e6e 6572 2e74 7261 696e      runner.train
-00003040: 2829 0a20 2020 2020 2020 2060 6060 0a20  ().        ```. 
-00003050: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003060: 3c2f 6465 7461 696c 733e 0a20 2020 2020  </details>.     
-00003070: 2020 200a 2020 2020 2020 2020 2323 204c     .        ## L
-00003080: 6561 726e 204d 6f72 650a 2020 2020 2020  earn More.      
-00003090: 2020 0a20 2020 2020 2020 203c 6465 7461    .        <deta
-000030a0: 696c 733e 0a20 2020 2020 2020 203c 7375  ils>.        <su
-000030b0: 6d6d 6172 793e 5475 746f 7269 616c 733c  mmary>Tutorials<
-000030c0: 2f73 756d 6d61 7279 3e0a 2020 2020 2020  /summary>.      
-000030d0: 2020 0a20 2020 2020 2020 202d 205b 5275    .        - [Ru
-000030e0: 6e6e 6572 5d28 6874 7470 733a 2f2f 6d6d  nner](https://mm
-000030f0: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
-00003100: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00003110: 7475 746f 7269 616c 732f 7275 6e6e 6572  tutorials/runner
-00003120: 2e68 746d 6c29 0a20 2020 2020 2020 202d  .html).        -
-00003130: 205b 4461 7461 7365 7420 616e 6420 4461   [Dataset and Da
-00003140: 7461 4c6f 6164 6572 5d28 6874 7470 733a  taLoader](https:
-00003150: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
-00003160: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00003170: 6573 742f 7475 746f 7269 616c 732f 6461  est/tutorials/da
-00003180: 7461 7365 742e 6874 6d6c 290a 2020 2020  taset.html).    
-00003190: 2020 2020 2d20 5b4d 6f64 656c 5d28 6874      - [Model](ht
-000031a0: 7470 733a 2f2f 6d6d 656e 6769 6e65 2e72  tps://mmengine.r
-000031b0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000031c0: 2f6c 6174 6573 742f 7475 746f 7269 616c  /latest/tutorial
-000031d0: 732f 6d6f 6465 6c2e 6874 6d6c 290a 2020  s/model.html).  
-000031e0: 2020 2020 2020 2d20 5b45 7661 6c75 6174        - [Evaluat
-000031f0: 696f 6e5d 2868 7474 7073 3a2f 2f6d 6d65  ion](https://mme
-00003200: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
-00003210: 732e 696f 2f65 6e2f 6c61 7465 7374 2f74  s.io/en/latest/t
-00003220: 7574 6f72 6961 6c73 2f65 7661 6c75 6174  utorials/evaluat
-00003230: 696f 6e2e 6874 6d6c 290a 2020 2020 2020  ion.html).      
-00003240: 2020 2d20 5b4f 7074 696d 5772 6170 7065    - [OptimWrappe
-00003250: 725d 2868 7474 7073 3a2f 2f6d 6d65 6e67  r](https://mmeng
-00003260: 696e 652e 7265 6164 7468 6564 6f63 732e  ine.readthedocs.
-00003270: 696f 2f65 6e2f 6c61 7465 7374 2f74 7574  io/en/latest/tut
-00003280: 6f72 6961 6c73 2f6f 7074 696d 5f77 7261  orials/optim_wra
-00003290: 7070 6572 2e68 746d 6c29 0a20 2020 2020  pper.html).     
-000032a0: 2020 202d 205b 5061 7261 6d65 7465 7220     - [Parameter 
-000032b0: 5363 6865 6475 6c65 725d 2868 7474 7073  Scheduler](https
-000032c0: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-000032d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000032e0: 7465 7374 2f74 7574 6f72 6961 6c73 2f70  test/tutorials/p
-000032f0: 6172 616d 5f73 6368 6564 756c 6572 2e68  aram_scheduler.h
-00003300: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-00003310: 486f 6f6b 5d28 6874 7470 733a 2f2f 6d6d  Hook](https://mm
-00003320: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
-00003330: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00003340: 7475 746f 7269 616c 732f 686f 6f6b 2e68  tutorials/hook.h
-00003350: 746d 6c29 0a20 2020 2020 2020 200a 2020  tml).        .  
-00003360: 2020 2020 2020 3c2f 6465 7461 696c 733e        </details>
-00003370: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003380: 2020 3c64 6574 6169 6c73 3e0a 2020 2020    <details>.    
-00003390: 2020 2020 3c73 756d 6d61 7279 3e41 6476      <summary>Adv
-000033a0: 616e 6365 6420 7475 746f 7269 616c 733c  anced tutorials<
-000033b0: 2f73 756d 6d61 7279 3e0a 2020 2020 2020  /summary>.      
-000033c0: 2020 0a20 2020 2020 2020 202d 205b 5265    .        - [Re
-000033d0: 6769 7374 7279 5d28 6874 7470 733a 2f2f  gistry](https://
-000033e0: 6d6d 656e 6769 6e65 2e72 6561 6474 6865  mmengine.readthe
-000033f0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00003400: 742f 6164 7661 6e63 6564 5f74 7574 6f72  t/advanced_tutor
-00003410: 6961 6c73 2f72 6567 6973 7472 792e 6874  ials/registry.ht
-00003420: 6d6c 290a 2020 2020 2020 2020 2d20 5b43  ml).        - [C
-00003430: 6f6e 6669 675d 2868 7474 7073 3a2f 2f6d  onfig](https://m
-00003440: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-00003450: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00003460: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
-00003470: 616c 732f 636f 6e66 6967 2e68 746d 6c29  als/config.html)
-00003480: 0a20 2020 2020 2020 202d 205b 4261 7365  .        - [Base
-00003490: 4461 7461 7365 745d 2868 7474 7073 3a2f  Dataset](https:/
-000034a0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-000034b0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-000034c0: 7374 2f61 6476 616e 6365 645f 7475 746f  st/advanced_tuto
-000034d0: 7269 616c 732f 6261 7365 6461 7461 7365  rials/basedatase
-000034e0: 742e 6874 6d6c 290a 2020 2020 2020 2020  t.html).        
-000034f0: 2d20 5b44 6174 6120 5472 616e 7366 6f72  - [Data Transfor
-00003500: 6d5d 2868 7474 7073 3a2f 2f6d 6d65 6e67  m](https://mmeng
+000026c0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000026d0: 6e73 666f 726d 732e 5261 6e64 6f6d 4372  nsforms.RandomCr
+000026e0: 6f70 2833 322c 2070 6164 6469 6e67 3d34  op(32, padding=4
+000026f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002720: 2074 7261 6e73 666f 726d 732e 5261 6e64   transforms.Rand
+00002730: 6f6d 486f 7269 7a6f 6e74 616c 466c 6970  omHorizontalFlip
+00002740: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 7472 616e 7366 6f72 6d73 2e54 6f54    transforms.ToT
+00002780: 656e 736f 7228 292c 0a20 2020 2020 2020  ensor(),.       
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000027c0: 732e 4e6f 726d 616c 697a 6528 2a2a 6e6f  s.Normalize(**no
+000027d0: 726d 5f63 6667 290a 2020 2020 2020 2020  rm_cfg).        
+000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002800: 2020 5d29 2929 0a20 2020 2020 2020 2076    ]))).        v
+00002810: 616c 5f64 6174 616c 6f61 6465 7220 3d20  al_dataloader = 
+00002820: 4461 7461 4c6f 6164 6572 2862 6174 6368  DataLoader(batch
+00002830: 5f73 697a 653d 3332 2c0a 2020 2020 2020  _size=32,.      
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+00002860: 7566 666c 653d 4661 6c73 652c 0a20 2020  uffle=False,.   
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2064 6174 6173 6574 3d74 6f72 6368 7669   dataset=torchvi
+000028a0: 7369 6f6e 2e64 6174 6173 6574 732e 4349  sion.datasets.CI
+000028b0: 4641 5231 3028 0a20 2020 2020 2020 2020  FAR10(.         
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000028e0: 6461 7461 2f63 6966 6172 3130 272c 0a20  data/cifar10',. 
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 2020 2074 7261 696e 3d46 616c         train=Fal
+00002920: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 2020 2020 2020 646f 776e              down
+00002950: 6c6f 6164 3d54 7275 652c 0a20 2020 2020  load=True,.     
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2074 7261 6e73 666f 726d 3d74 7261     transform=tra
+00002990: 6e73 666f 726d 732e 436f 6d70 6f73 6528  nsforms.Compose(
+000029a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029c0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000029d0: 616e 7366 6f72 6d73 2e54 6f54 656e 736f  ansforms.ToTenso
+000029e0: 7228 292c 0a20 2020 2020 2020 2020 2020  r(),.           
+000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 2074 7261 6e73 666f 726d 732e 4e6f 726d   transforms.Norm
+00002a20: 616c 697a 6528 2a2a 6e6f 726d 5f63 6667  alize(**norm_cfg
+00002a30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 2020 2020 2020 2020 2020 5d29 2929 0a20            ]))). 
+00002a60: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00002a70: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
+00002a80: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
+00002a90: 2020 2020 2020 2020 3c64 6574 6169 6c73          <details
+00002aa0: 3e0a 2020 2020 2020 2020 3c73 756d 6d61  >.        <summa
+00002ab0: 7279 3e42 7569 6c64 204d 6574 7269 6373  ry>Build Metrics
+00002ac0: 3c2f 7375 6d6d 6172 793e 0a20 2020 2020  </summary>.     
+00002ad0: 2020 200a 2020 2020 2020 2020 546f 2076     .        To v
+00002ae0: 616c 6964 6174 6520 616e 6420 7465 7374  alidate and test
+00002af0: 2074 6865 206d 6f64 656c 2c20 7765 206e   the model, we n
+00002b00: 6565 6420 746f 2064 6566 696e 6520 6120  eed to define a 
+00002b10: 2a2a 4d65 7472 6963 2a2a 2063 616c 6c65  **Metric** calle
+00002b20: 6420 6163 6375 7261 6379 2074 6f20 6576  d accuracy to ev
+00002b30: 616c 7561 7465 2074 6865 206d 6f64 656c  aluate the model
+00002b40: 2e20 5468 6973 206d 6574 7269 6320 6e65  . This metric ne
+00002b50: 6564 7320 746f 2069 6e68 6572 6974 2066  eds to inherit f
+00002b60: 726f 6d20 6042 6173 654d 6574 7269 6360  rom `BaseMetric`
+00002b70: 2061 6e64 2069 6d70 6c65 6d65 6e74 7320   and implements 
+00002b80: 7468 6520 6070 726f 6365 7373 6020 616e  the `process` an
+00002b90: 6420 6063 6f6d 7075 7465 5f6d 6574 7269  d `compute_metri
+00002ba0: 6373 6020 6d65 7468 6f64 732e 0a20 2020  cs` methods..   
+00002bb0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
+00002bc0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00002bd0: 6672 6f6d 206d 6d65 6e67 696e 652e 6576  from mmengine.ev
+00002be0: 616c 7561 746f 7220 696d 706f 7274 2042  aluator import B
+00002bf0: 6173 654d 6574 7269 630a 2020 2020 2020  aseMetric.      
+00002c00: 2020 0a20 2020 2020 2020 2063 6c61 7373    .        class
+00002c10: 2041 6363 7572 6163 7928 4261 7365 4d65   Accuracy(BaseMe
+00002c20: 7472 6963 293a 0a20 2020 2020 2020 2020  tric):.         
+00002c30: 2020 2064 6566 2070 726f 6365 7373 2873     def process(s
+00002c40: 656c 662c 2064 6174 615f 6261 7463 682c  elf, data_batch,
+00002c50: 2064 6174 615f 7361 6d70 6c65 7329 3a0a   data_samples):.
+00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c70: 7363 6f72 652c 2067 7420 3d20 6461 7461  score, gt = data
+00002c80: 5f73 616d 706c 6573 0a20 2020 2020 2020  _samples.       
+00002c90: 2020 2020 2020 2020 2023 2053 6176 6520           # Save 
+00002ca0: 7468 6520 7265 7375 6c74 7320 6f66 2061  the results of a
+00002cb0: 2062 6174 6368 2074 6f20 6073 656c 662e   batch to `self.
+00002cc0: 7265 7375 6c74 7360 0a20 2020 2020 2020  results`.       
+00002cd0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00002ce0: 7375 6c74 732e 6170 7065 6e64 287b 0a20  sults.append({. 
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2027 6261 7463 685f 7369 7a65 273a     'batch_size':
+00002d10: 206c 656e 2867 7429 2c0a 2020 2020 2020   len(gt),.      
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+00002d30: 6f72 7265 6374 273a 2028 7363 6f72 652e  orrect': (score.
+00002d40: 6172 676d 6178 2864 696d 3d31 2920 3d3d  argmax(dim=1) ==
+00002d50: 2067 7429 2e73 756d 2829 2e63 7075 2829   gt).sum().cpu()
+00002d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002d70: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
+00002d80: 2064 6566 2063 6f6d 7075 7465 5f6d 6574   def compute_met
+00002d90: 7269 6373 2873 656c 662c 2072 6573 756c  rics(self, resul
+00002da0: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+00002db0: 2020 2020 2074 6f74 616c 5f63 6f72 7265       total_corre
+00002dc0: 6374 203d 2073 756d 2869 7465 6d5b 2763  ct = sum(item['c
+00002dd0: 6f72 7265 6374 275d 2066 6f72 2069 7465  orrect'] for ite
+00002de0: 6d20 696e 2072 6573 756c 7473 290a 2020  m in results).  
+00002df0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00002e00: 7461 6c5f 7369 7a65 203d 2073 756d 2869  tal_size = sum(i
+00002e10: 7465 6d5b 2762 6174 6368 5f73 697a 6527  tem['batch_size'
+00002e20: 5d20 666f 7220 6974 656d 2069 6e20 7265  ] for item in re
+00002e30: 7375 6c74 7329 0a20 2020 2020 2020 2020  sults).         
+00002e40: 2020 2020 2020 2023 2052 6574 7572 6e73         # Returns
+00002e50: 2061 2064 6963 7469 6f6e 6172 7920 7769   a dictionary wi
+00002e60: 7468 2074 6865 2072 6573 756c 7473 206f  th the results o
+00002e70: 6620 7468 6520 6576 616c 7561 7465 6420  f the evaluated 
+00002e80: 6d65 7472 6963 732c 0a20 2020 2020 2020  metrics,.       
+00002e90: 2020 2020 2020 2020 2023 2077 6865 7265           # where
+00002ea0: 2074 6865 206b 6579 2069 7320 7468 6520   the key is the 
+00002eb0: 6e61 6d65 206f 6620 7468 6520 6d65 7472  name of the metr
+00002ec0: 6963 0a20 2020 2020 2020 2020 2020 2020  ic.             
+00002ed0: 2020 2072 6574 7572 6e20 6469 6374 2861     return dict(a
+00002ee0: 6363 7572 6163 793d 3130 3020 2a20 746f  ccuracy=100 * to
+00002ef0: 7461 6c5f 636f 7272 6563 7420 2f20 746f  tal_correct / to
+00002f00: 7461 6c5f 7369 7a65 290a 2020 2020 2020  tal_size).      
+00002f10: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00002f20: 2020 2020 2020 203c 2f64 6574 6169 6c73         </details
+00002f30: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
+00002f40: 2020 203c 6465 7461 696c 733e 0a20 2020     <details>.   
+00002f50: 2020 2020 203c 7375 6d6d 6172 793e 4275       <summary>Bu
+00002f60: 696c 6420 6120 5275 6e6e 6572 3c2f 7375  ild a Runner</su
+00002f70: 6d6d 6172 793e 0a20 2020 2020 2020 200a  mmary>.        .
+00002f80: 2020 2020 2020 2020 4669 6e61 6c6c 792c          Finally,
+00002f90: 2077 6520 6361 6e20 636f 6e73 7472 7563   we can construc
+00002fa0: 7420 6120 2a2a 5275 6e6e 6572 2a2a 2077  t a **Runner** w
+00002fb0: 6974 6820 7072 6576 696f 7573 6c79 2064  ith previously d
+00002fc0: 6566 696e 6564 2060 4d6f 6465 6c60 2c20  efined `Model`, 
+00002fd0: 6044 6174 614c 6f61 6465 7260 2c20 616e  `DataLoader`, an
+00002fe0: 6420 604d 6574 7269 6373 602c 2077 6974  d `Metrics`, wit
+00002ff0: 6820 736f 6d65 206f 7468 6572 2063 6f6e  h some other con
+00003000: 6669 6773 2c20 6173 2073 686f 776e 2062  figs, as shown b
+00003010: 656c 6f77 2e0a 2020 2020 2020 2020 0a20  elow..        . 
+00003020: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00003030: 0a20 2020 2020 2020 2066 726f 6d20 746f  .        from to
+00003040: 7263 682e 6f70 7469 6d20 696d 706f 7274  rch.optim import
+00003050: 2053 4744 0a20 2020 2020 2020 2066 726f   SGD.        fro
+00003060: 6d20 6d6d 656e 6769 6e65 2e72 756e 6e65  m mmengine.runne
+00003070: 7220 696d 706f 7274 2052 756e 6e65 720a  r import Runner.
+00003080: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003090: 2072 756e 6e65 7220 3d20 5275 6e6e 6572   runner = Runner
+000030a0: 280a 2020 2020 2020 2020 2020 2020 6d6f  (.            mo
+000030b0: 6465 6c3d 4d4d 5265 734e 6574 3530 2829  del=MMResNet50()
+000030c0: 2c0a 2020 2020 2020 2020 2020 2020 776f  ,.            wo
+000030d0: 726b 5f64 6972 3d27 2e2f 776f 726b 5f64  rk_dir='./work_d
+000030e0: 6972 272c 0a20 2020 2020 2020 2020 2020  ir',.           
+000030f0: 2074 7261 696e 5f64 6174 616c 6f61 6465   train_dataloade
+00003100: 723d 7472 6169 6e5f 6461 7461 6c6f 6164  r=train_dataload
+00003110: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00003120: 2320 6120 7772 6170 7065 7220 746f 2065  # a wrapper to e
+00003130: 7865 6375 7465 2062 6163 6b20 7072 6f70  xecute back prop
+00003140: 6167 6174 696f 6e20 616e 6420 6772 6164  agation and grad
+00003150: 6965 6e74 2075 7064 6174 652c 2065 7463  ient update, etc
+00003160: 2e0a 2020 2020 2020 2020 2020 2020 6f70  ..            op
+00003170: 7469 6d5f 7772 6170 7065 723d 6469 6374  tim_wrapper=dict
+00003180: 286f 7074 696d 697a 6572 3d64 6963 7428  (optimizer=dict(
+00003190: 7479 7065 3d53 4744 2c20 6c72 3d30 2e30  type=SGD, lr=0.0
+000031a0: 3031 2c20 6d6f 6d65 6e74 756d 3d30 2e39  01, momentum=0.9
+000031b0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+000031c0: 2320 7365 7420 736f 6d65 2074 7261 696e  # set some train
+000031d0: 696e 6720 636f 6e66 6967 7320 6c69 6b65  ing configs like
+000031e0: 2065 706f 6368 730a 2020 2020 2020 2020   epochs.        
+000031f0: 2020 2020 7472 6169 6e5f 6366 673d 6469      train_cfg=di
+00003200: 6374 2862 795f 6570 6f63 683d 5472 7565  ct(by_epoch=True
+00003210: 2c20 6d61 785f 6570 6f63 6873 3d35 2c20  , max_epochs=5, 
+00003220: 7661 6c5f 696e 7465 7276 616c 3d31 292c  val_interval=1),
+00003230: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00003240: 5f64 6174 616c 6f61 6465 723d 7661 6c5f  _dataloader=val_
+00003250: 6461 7461 6c6f 6164 6572 2c0a 2020 2020  dataloader,.    
+00003260: 2020 2020 2020 2020 7661 6c5f 6366 673d          val_cfg=
+00003270: 6469 6374 2829 2c0a 2020 2020 2020 2020  dict(),.        
+00003280: 2020 2020 7661 6c5f 6576 616c 7561 746f      val_evaluato
+00003290: 723d 6469 6374 2874 7970 653d 4163 6375  r=dict(type=Accu
+000032a0: 7261 6379 292c 0a20 2020 2020 2020 2029  racy),.        )
+000032b0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+000032c0: 2020 2020 200a 2020 2020 2020 2020 3c2f       .        </
+000032d0: 6465 7461 696c 733e 0a20 2020 2020 2020  details>.       
+000032e0: 200a 2020 2020 2020 2020 3c64 6574 6169   .        <detai
+000032f0: 6c73 3e0a 2020 2020 2020 2020 3c73 756d  ls>.        <sum
+00003300: 6d61 7279 3e4c 6175 6e63 6820 5472 6169  mary>Launch Trai
+00003310: 6e69 6e67 3c2f 7375 6d6d 6172 793e 0a20  ning</summary>. 
+00003320: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003330: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00003340: 2020 7275 6e6e 6572 2e74 7261 696e 2829    runner.train()
+00003350: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00003360: 2020 2020 200a 2020 2020 2020 2020 3c2f       .        </
+00003370: 6465 7461 696c 733e 0a20 2020 2020 2020  details>.       
+00003380: 200a 2020 2020 2020 2020 2323 204c 6561   .        ## Lea
+00003390: 726e 204d 6f72 650a 2020 2020 2020 2020  rn More.        
+000033a0: 0a20 2020 2020 2020 203c 6465 7461 696c  .        <detail
+000033b0: 733e 0a20 2020 2020 2020 203c 7375 6d6d  s>.        <summ
+000033c0: 6172 793e 5475 746f 7269 616c 733c 2f73  ary>Tutorials</s
+000033d0: 756d 6d61 7279 3e0a 2020 2020 2020 2020  ummary>.        
+000033e0: 0a20 2020 2020 2020 202d 205b 5275 6e6e  .        - [Runn
+000033f0: 6572 5d28 6874 7470 733a 2f2f 6d6d 656e  er](https://mmen
+00003400: 6769 6e65 2e72 6561 6474 6865 646f 6373  gine.readthedocs
+00003410: 2e69 6f2f 656e 2f6c 6174 6573 742f 7475  .io/en/latest/tu
+00003420: 746f 7269 616c 732f 7275 6e6e 6572 2e68  torials/runner.h
+00003430: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
+00003440: 4461 7461 7365 7420 616e 6420 4461 7461  Dataset and Data
+00003450: 4c6f 6164 6572 5d28 6874 7470 733a 2f2f  Loader](https://
+00003460: 6d6d 656e 6769 6e65 2e72 6561 6474 6865  mmengine.readthe
+00003470: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00003480: 742f 7475 746f 7269 616c 732f 6461 7461  t/tutorials/data
+00003490: 7365 742e 6874 6d6c 290a 2020 2020 2020  set.html).      
+000034a0: 2020 2d20 5b4d 6f64 656c 5d28 6874 7470    - [Model](http
+000034b0: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
+000034c0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000034d0: 6174 6573 742f 7475 746f 7269 616c 732f  atest/tutorials/
+000034e0: 6d6f 6465 6c2e 6874 6d6c 290a 2020 2020  model.html).    
+000034f0: 2020 2020 2d20 5b45 7661 6c75 6174 696f      - [Evaluatio
+00003500: 6e5d 2868 7474 7073 3a2f 2f6d 6d65 6e67  n](https://mmeng
 00003510: 696e 652e 7265 6164 7468 6564 6f63 732e  ine.readthedocs.
-00003520: 696f 2f65 6e2f 6c61 7465 7374 2f61 6476  io/en/latest/adv
-00003530: 616e 6365 645f 7475 746f 7269 616c 732f  anced_tutorials/
-00003540: 6461 7461 5f74 7261 6e73 666f 726d 2e68  data_transform.h
-00003550: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-00003560: 5765 6967 6874 2049 6e69 7469 616c 697a  Weight Initializ
-00003570: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6d  ation](https://m
-00003580: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-00003590: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000035a0: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
-000035b0: 616c 732f 696e 6974 6961 6c69 7a65 2e68  als/initialize.h
-000035c0: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-000035d0: 5669 7375 616c 697a 6174 696f 6e5d 2868  Visualization](h
-000035e0: 7474 7073 3a2f 2f6d 6d65 6e67 696e 652e  ttps://mmengine.
-000035f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00003600: 6e2f 6c61 7465 7374 2f61 6476 616e 6365  n/latest/advance
-00003610: 645f 7475 746f 7269 616c 732f 7669 7375  d_tutorials/visu
-00003620: 616c 697a 6174 696f 6e2e 6874 6d6c 290a  alization.html).
-00003630: 2020 2020 2020 2020 2d20 5b41 6273 7472          - [Abstr
-00003640: 6163 7420 4461 7461 2045 6c65 6d65 6e74  act Data Element
-00003650: 5d28 6874 7470 733a 2f2f 6d6d 656e 6769  ](https://mmengi
-00003660: 6e65 2e72 6561 6474 6865 646f 6373 2e69  ne.readthedocs.i
-00003670: 6f2f 656e 2f6c 6174 6573 742f 6164 7661  o/en/latest/adva
-00003680: 6e63 6564 5f74 7574 6f72 6961 6c73 2f64  nced_tutorials/d
-00003690: 6174 615f 656c 656d 656e 742e 6874 6d6c  ata_element.html
-000036a0: 290a 2020 2020 2020 2020 2d20 5b44 6973  ).        - [Dis
-000036b0: 7472 6962 7574 696f 6e20 436f 6d6d 756e  tribution Commun
-000036c0: 6963 6174 696f 6e5d 2868 7474 7073 3a2f  ication](https:/
-000036d0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-000036e0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-000036f0: 7374 2f61 6476 616e 6365 645f 7475 746f  st/advanced_tuto
-00003700: 7269 616c 732f 6469 7374 7269 6275 7465  rials/distribute
-00003710: 642e 6874 6d6c 290a 2020 2020 2020 2020  d.html).        
-00003720: 2d20 5b4c 6f67 6769 6e67 5d28 6874 7470  - [Logging](http
-00003730: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
-00003740: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00003750: 6174 6573 742f 6164 7661 6e63 6564 5f74  atest/advanced_t
-00003760: 7574 6f72 6961 6c73 2f6c 6f67 6769 6e67  utorials/logging
-00003770: 2e68 746d 6c29 0a20 2020 2020 2020 202d  .html).        -
-00003780: 205b 4669 6c65 2049 4f5d 2868 7474 7073   [File IO](https
-00003790: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-000037a0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000037b0: 7465 7374 2f61 6476 616e 6365 645f 7475  test/advanced_tu
-000037c0: 746f 7269 616c 732f 6669 6c65 696f 2e68  torials/fileio.h
-000037d0: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-000037e0: 476c 6f62 616c 206d 616e 6167 6572 2028  Global manager (
-000037f0: 4d61 6e61 6765 724d 6978 696e 295d 2868  ManagerMixin)](h
-00003800: 7474 7073 3a2f 2f6d 6d65 6e67 696e 652e  ttps://mmengine.
-00003810: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00003820: 6e2f 6c61 7465 7374 2f61 6476 616e 6365  n/latest/advance
-00003830: 645f 7475 746f 7269 616c 732f 6d61 6e61  d_tutorials/mana
-00003840: 6765 725f 6d69 7869 6e2e 6874 6d6c 290a  ger_mixin.html).
-00003850: 2020 2020 2020 2020 2d20 5b55 7365 206d          - [Use m
-00003860: 6f64 756c 6573 2066 726f 6d20 6f74 6865  odules from othe
-00003870: 7220 6c69 6272 6172 6965 735d 2868 7474  r libraries](htt
-00003880: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
-00003890: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-000038a0: 6c61 7465 7374 2f61 6476 616e 6365 645f  latest/advanced_
-000038b0: 7475 746f 7269 616c 732f 6372 6f73 735f  tutorials/cross_
-000038c0: 6c69 6272 6172 792e 6874 6d6c 290a 2020  library.html).  
-000038d0: 2020 2020 2020 2d20 5b54 6573 7420 5469        - [Test Ti
-000038e0: 6d65 2041 6775 6d65 6e74 6174 696f 6e5d  me Agumentation]
-000038f0: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
-00003900: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00003910: 2f65 6e2f 6c61 7465 7374 2f61 6476 616e  /en/latest/advan
-00003920: 6365 645f 7475 746f 7269 616c 732f 7465  ced_tutorials/te
-00003930: 7374 5f74 696d 655f 6175 676d 656e 7461  st_time_augmenta
-00003940: 7469 6f6e 2e68 746d 6c29 0a20 2020 2020  tion.html).     
-00003950: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
-00003960: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
-00003970: 2020 2020 2020 2020 3c64 6574 6169 6c73          <details
-00003980: 3e0a 2020 2020 2020 2020 3c73 756d 6d61  >.        <summa
-00003990: 7279 3e45 7861 6d70 6c65 733c 2f73 756d  ry>Examples</sum
-000039a0: 6d61 7279 3e0a 2020 2020 2020 2020 0a20  mary>.        . 
-000039b0: 2020 2020 2020 202d 205b 5472 6169 6e20         - [Train 
-000039c0: 6120 4741 4e5d 2868 7474 7073 3a2f 2f6d  a GAN](https://m
-000039d0: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-000039e0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000039f0: 2f65 7861 6d70 6c65 732f 7472 6169 6e5f  /examples/train_
-00003a00: 615f 6761 6e2e 6874 6d6c 290a 2020 2020  a_gan.html).    
-00003a10: 2020 2020 0a20 2020 2020 2020 203c 2f64      .        </d
-00003a20: 6574 6169 6c73 3e0a 2020 2020 2020 2020  etails>.        
-00003a30: 0a20 2020 2020 2020 203c 6465 7461 696c  .        <detail
-00003a40: 733e 0a20 2020 2020 2020 203c 7375 6d6d  s>.        <summ
-00003a50: 6172 793e 436f 6d6d 6f6e 2055 7361 6765  ary>Common Usage
-00003a60: 3c2f 7375 6d6d 6172 793e 0a20 2020 2020  </summary>.     
-00003a70: 2020 200a 2020 2020 2020 2020 2d20 5b52     .        - [R
-00003a80: 6573 756d 6520 5472 6169 6e69 6e67 5d28  esume Training](
-00003a90: 6874 7470 733a 2f2f 6d6d 656e 6769 6e65  https://mmengine
-00003aa0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00003ab0: 656e 2f6c 6174 6573 742f 636f 6d6d 6f6e  en/latest/common
-00003ac0: 5f75 7361 6765 2f72 6573 756d 655f 7472  _usage/resume_tr
-00003ad0: 6169 6e69 6e67 2e68 746d 6c29 0a20 2020  aining.html).   
-00003ae0: 2020 2020 202d 205b 5370 6565 6420 7570       - [Speed up
-00003af0: 2054 7261 696e 696e 675d 2868 7474 7073   Training](https
-00003b00: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-00003b10: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00003b20: 7465 7374 2f63 6f6d 6d6f 6e5f 7573 6167  test/common_usag
-00003b30: 652f 7370 6565 645f 7570 5f74 7261 696e  e/speed_up_train
-00003b40: 696e 672e 6874 6d6c 290a 2020 2020 2020  ing.html).      
-00003b50: 2020 2d20 5b53 6176 6520 4d65 6d6f 7279    - [Save Memory
-00003b60: 206f 6e20 4750 555d 2868 7474 7073 3a2f   on GPU](https:/
-00003b70: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00003b80: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003b90: 7374 2f63 6f6d 6d6f 6e5f 7573 6167 652f  st/common_usage/
-00003ba0: 7361 7665 5f67 7075 5f6d 656d 6f72 792e  save_gpu_memory.
-00003bb0: 6874 6d6c 290a 2020 2020 2020 2020 0a20  html).        . 
-00003bc0: 2020 2020 2020 203c 2f64 6574 6169 6c73         </details
-00003bd0: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
-00003be0: 2020 203c 6465 7461 696c 733e 0a20 2020     <details>.   
-00003bf0: 2020 2020 203c 7375 6d6d 6172 793e 4465       <summary>De
-00003c00: 7369 676e 3c2f 7375 6d6d 6172 793e 0a20  sign</summary>. 
-00003c10: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003c20: 2d20 5b48 6f6f 6b5d 2868 7474 7073 3a2f  - [Hook](https:/
-00003c30: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00003c40: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003c50: 7374 2f64 6573 6967 6e2f 686f 6f6b 2e68  st/design/hook.h
-00003c60: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
-00003c70: 5275 6e6e 6572 5d28 6874 7470 733a 2f2f  Runner](https://
-00003c80: 6d6d 656e 6769 6e65 2e72 6561 6474 6865  mmengine.readthe
-00003c90: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00003ca0: 742f 6465 7369 676e 2f72 756e 6e65 722e  t/design/runner.
-00003cb0: 6874 6d6c 290a 2020 2020 2020 2020 2d20  html).        - 
-00003cc0: 5b45 7661 6c75 6174 696f 6e5d 2868 7474  [Evaluation](htt
-00003cd0: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
-00003ce0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00003cf0: 6c61 7465 7374 2f64 6573 6967 6e2f 6576  latest/design/ev
-00003d00: 616c 7561 7469 6f6e 2e68 746d 6c29 0a20  aluation.html). 
-00003d10: 2020 2020 2020 202d 205b 5669 7375 616c         - [Visual
-00003d20: 697a 6174 696f 6e5d 2868 7474 7073 3a2f  ization](https:/
-00003d30: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00003d40: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003d50: 7374 2f64 6573 6967 6e2f 7669 7375 616c  st/design/visual
-00003d60: 697a 6174 696f 6e2e 6874 6d6c 290a 2020  ization.html).  
-00003d70: 2020 2020 2020 2d20 5b4c 6f67 6769 6e67        - [Logging
-00003d80: 5d28 6874 7470 733a 2f2f 6d6d 656e 6769  ](https://mmengi
-00003d90: 6e65 2e72 6561 6474 6865 646f 6373 2e69  ne.readthedocs.i
-00003da0: 6f2f 656e 2f6c 6174 6573 742f 6465 7369  o/en/latest/desi
-00003db0: 676e 2f6c 6f67 6769 6e67 2e68 746d 6c29  gn/logging.html)
-00003dc0: 0a20 2020 2020 2020 202d 205b 496e 6665  .        - [Infe
-00003dd0: 725d 2868 7474 7073 3a2f 2f6d 6d65 6e67  r](https://mmeng
-00003de0: 696e 652e 7265 6164 7468 6564 6f63 732e  ine.readthedocs.
-00003df0: 696f 2f65 6e2f 6c61 7465 7374 2f64 6573  io/en/latest/des
-00003e00: 6967 6e2f 696e 6665 722e 6874 6d6c 290a  ign/infer.html).
-00003e10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003e20: 203c 2f64 6574 6169 6c73 3e0a 2020 2020   </details>.    
-00003e30: 2020 2020 0a20 2020 2020 2020 203c 6465      .        <de
-00003e40: 7461 696c 733e 0a20 2020 2020 2020 203c  tails>.        <
-00003e50: 7375 6d6d 6172 793e 4d69 6772 6174 696f  summary>Migratio
-00003e60: 6e20 6775 6964 653c 2f73 756d 6d61 7279  n guide</summary
-00003e70: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
-00003e80: 2020 202d 205b 4d69 6772 6174 6520 5275     - [Migrate Ru
-00003e90: 6e6e 6572 2066 726f 6d20 4d4d 4356 2074  nner from MMCV t
-00003ea0: 6f20 4d4d 456e 6769 6e65 5d28 6874 7470  o MMEngine](http
-00003eb0: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
-00003ec0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00003ed0: 6174 6573 742f 6d69 6772 6174 696f 6e2f  atest/migration/
-00003ee0: 7275 6e6e 6572 2e68 746d 6c29 0a20 2020  runner.html).   
-00003ef0: 2020 2020 202d 205b 4d69 6772 6174 6520       - [Migrate 
-00003f00: 486f 6f6b 2066 726f 6d20 4d4d 4356 2074  Hook from MMCV t
-00003f10: 6f20 4d4d 456e 6769 6e65 5d28 6874 7470  o MMEngine](http
-00003f20: 733a 2f2f 6d6d 656e 6769 6e65 2e72 6561  s://mmengine.rea
-00003f30: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00003f40: 6174 6573 742f 6d69 6772 6174 696f 6e2f  atest/migration/
-00003f50: 686f 6f6b 2e68 746d 6c29 0a20 2020 2020  hook.html).     
-00003f60: 2020 202d 205b 4d69 6772 6174 6520 4d6f     - [Migrate Mo
-00003f70: 6465 6c20 6672 6f6d 204d 4d43 5620 746f  del from MMCV to
-00003f80: 204d 4d45 6e67 696e 655d 2868 7474 7073   MMEngine](https
-00003f90: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
-00003fa0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00003fb0: 7465 7374 2f6d 6967 7261 7469 6f6e 2f6d  test/migration/m
-00003fc0: 6f64 656c 2e68 746d 6c29 0a20 2020 2020  odel.html).     
-00003fd0: 2020 202d 205b 4d69 6772 6174 6520 5061     - [Migrate Pa
-00003fe0: 7261 6d65 7465 7220 5363 6865 6475 6c65  rameter Schedule
-00003ff0: 7220 6672 6f6d 204d 4d43 5620 746f 204d  r from MMCV to M
-00004000: 4d45 6e67 696e 655d 2868 7474 7073 3a2f  MEngine](https:/
-00004010: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
-00004020: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00004030: 7374 2f6d 6967 7261 7469 6f6e 2f70 6172  st/migration/par
-00004040: 616d 5f73 6368 6564 756c 6572 2e68 746d  am_scheduler.htm
-00004050: 6c29 0a20 2020 2020 2020 202d 205b 4d69  l).        - [Mi
-00004060: 6772 6174 6520 4461 7461 2054 7261 6e73  grate Data Trans
-00004070: 666f 726d 2074 6f20 4f70 656e 4d4d 4c61  form to OpenMMLa
-00004080: 6220 322e 305d 2868 7474 7073 3a2f 2f6d  b 2.0](https://m
-00004090: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
-000040a0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000040b0: 2f6d 6967 7261 7469 6f6e 2f74 7261 6e73  /migration/trans
-000040c0: 666f 726d 2e68 746d 6c29 0a20 2020 2020  form.html).     
-000040d0: 2020 200a 2020 2020 2020 2020 3c2f 6465     .        </de
-000040e0: 7461 696c 733e 0a20 2020 2020 2020 200a  tails>.        .
-000040f0: 2020 2020 2020 2020 2323 2043 6f6e 7472          ## Contr
-00004100: 6962 7574 696e 670a 2020 2020 2020 2020  ibuting.        
-00004110: 0a20 2020 2020 2020 2057 6520 6170 7072  .        We appr
-00004120: 6563 6961 7465 2061 6c6c 2063 6f6e 7472  eciate all contr
-00004130: 6962 7574 696f 6e73 2074 6f20 696d 7072  ibutions to impr
-00004140: 6f76 6520 4d4d 456e 6769 6e65 2e20 506c  ove MMEngine. Pl
-00004150: 6561 7365 2072 6566 6572 2074 6f20 5b43  ease refer to [C
-00004160: 4f4e 5452 4942 5554 494e 472e 6d64 5d28  ONTRIBUTING.md](
-00004170: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
-00004180: 2066 6f72 2074 6865 2063 6f6e 7472 6962   for the contrib
-00004190: 7574 696e 6720 6775 6964 656c 696e 652e  uting guideline.
-000041a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000041b0: 2020 2323 2043 6974 6174 696f 6e0a 2020    ## Citation.  
-000041c0: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
-000041d0: 6620 796f 7520 6669 6e64 2074 6869 7320  f you find this 
-000041e0: 7072 6f6a 6563 7420 7573 6566 756c 2069  project useful i
-000041f0: 6e20 796f 7572 2072 6573 6561 7263 682c  n your research,
-00004200: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
-00004210: 2063 6974 653a 0a20 2020 2020 2020 200a   cite:.        .
-00004220: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
-00004230: 2020 2020 4061 7274 6963 6c65 7b6d 6d65      @article{mme
-00004240: 6e67 696e 6532 3032 322c 0a20 2020 2020  ngine2022,.     
-00004250: 2020 2020 2074 6974 6c65 2020 203d 207b       title   = {
-00004260: 7b4d 4d45 6e67 696e 657d 3a20 4f70 656e  {MMEngine}: Open
-00004270: 4d4d 4c61 6220 466f 756e 6461 7469 6f6e  MMLab Foundation
-00004280: 616c 204c 6962 7261 7279 2066 6f72 2054  al Library for T
-00004290: 7261 696e 696e 6720 4465 6570 204c 6561  raining Deep Lea
-000042a0: 726e 696e 6720 4d6f 6465 6c73 7d2c 0a20  rning Models},. 
-000042b0: 2020 2020 2020 2020 2061 7574 686f 7220           author 
-000042c0: 203d 207b 4d4d 456e 6769 6e65 2043 6f6e   = {MMEngine Con
-000042d0: 7472 6962 7574 6f72 737d 2c0a 2020 2020  tributors},.    
-000042e0: 2020 2020 2020 686f 7770 7562 6c69 7368        howpublish
-000042f0: 6564 203d 207b 5c75 726c 7b68 7474 7073  ed = {\url{https
-00004300: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f70  ://github.com/op
-00004310: 656e 2d6d 6d6c 6162 2f6d 6d65 6e67 696e  en-mmlab/mmengin
-00004320: 657d 7d2c 0a20 2020 2020 2020 2020 2079  e}},.          y
-00004330: 6561 723d 7b32 3032 327d 0a20 2020 2020  ear={2022}.     
-00004340: 2020 207d 0a20 2020 2020 2020 2060 6060     }.        ```
-00004350: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004360: 2020 2323 204c 6963 656e 7365 0a20 2020    ## License.   
-00004370: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-00004380: 6973 2070 726f 6a65 6374 2069 7320 7265  is project is re
-00004390: 6c65 6173 6564 2075 6e64 6572 2074 6865  leased under the
-000043a0: 205b 4170 6163 6865 2032 2e30 206c 6963   [Apache 2.0 lic
-000043b0: 656e 7365 5d28 4c49 4345 4e53 4529 2e0a  ense](LICENSE)..
-000043c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000043d0: 2023 2320 5072 6f6a 6563 7473 2069 6e20   ## Projects in 
-000043e0: 4f70 656e 4d4d 4c61 620a 2020 2020 2020  OpenMMLab.      
-000043f0: 2020 0a20 2020 2020 2020 202d 205b 4d49    .        - [MI
-00004400: 4d5d 2868 7474 7073 3a2f 2f67 6974 6875  M](https://githu
-00004410: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
-00004420: 2f6d 696d 293a 204d 494d 2069 6e73 7461  /mim): MIM insta
-00004430: 6c6c 7320 4f70 656e 4d4d 4c61 6220 7061  lls OpenMMLab pa
-00004440: 636b 6167 6573 2e0a 2020 2020 2020 2020  ckages..        
-00004450: 2d20 5b4d 4d43 565d 2868 7474 7073 3a2f  - [MMCV](https:/
-00004460: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004470: 2d6d 6d6c 6162 2f6d 6d63 7629 3a20 4f70  -mmlab/mmcv): Op
-00004480: 656e 4d4d 4c61 6220 666f 756e 6461 7469  enMMLab foundati
-00004490: 6f6e 616c 206c 6962 7261 7279 2066 6f72  onal library for
-000044a0: 2063 6f6d 7075 7465 7220 7669 7369 6f6e   computer vision
-000044b0: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d45  ..        - [MME
-000044c0: 7661 6c5d 2868 7474 7073 3a2f 2f67 6974  val](https://git
-000044d0: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
-000044e0: 6162 2f6d 6d65 7661 6c29 3a20 4120 756e  ab/mmeval): A un
-000044f0: 6966 6965 6420 6576 616c 7561 7469 6f6e  ified evaluation
-00004500: 206c 6962 7261 7279 2066 6f72 206d 756c   library for mul
-00004510: 7469 706c 6520 6d61 6368 696e 6520 6c65  tiple machine le
-00004520: 6172 6e69 6e67 206c 6962 7261 7269 6573  arning libraries
-00004530: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d50  ..        - [MMP
-00004540: 7265 5472 6169 6e5d 2868 7474 7073 3a2f  reTrain](https:/
-00004550: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004560: 2d6d 6d6c 6162 2f6d 6d70 7265 7472 6169  -mmlab/mmpretrai
-00004570: 6e29 3a20 4f70 656e 4d4d 4c61 6220 7072  n): OpenMMLab pr
-00004580: 652d 7472 6169 6e69 6e67 2074 6f6f 6c62  e-training toolb
-00004590: 6f78 2061 6e64 2062 656e 6368 6d61 726b  ox and benchmark
-000045a0: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d61  ..        - [MMa
-000045b0: 6769 635d 2868 7474 7073 3a2f 2f67 6974  gic](https://git
-000045c0: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
-000045d0: 6162 2f6d 6d61 6769 6329 3a20 4f70 656e  ab/mmagic): Open
-000045e0: 2a2a 4d4d 2a2a 4c61 6220 2a2a 412a 2a64  **MM**Lab **A**d
-000045f0: 7661 6e63 6564 2c20 2a2a 472a 2a65 6e65  vanced, **G**ene
-00004600: 7261 7469 7665 2061 6e64 202a 2a49 2a2a  rative and **I**
-00004610: 6e74 656c 6c69 6765 6e74 202a 2a43 2a2a  ntelligent **C**
-00004620: 7265 6174 696f 6e20 746f 6f6c 626f 782e  reation toolbox.
-00004630: 0a20 2020 2020 2020 202d 205b 4d4d 4465  .        - [MMDe
-00004640: 7465 6374 696f 6e5d 2868 7474 7073 3a2f  tection](https:/
-00004650: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004660: 2d6d 6d6c 6162 2f6d 6d64 6574 6563 7469  -mmlab/mmdetecti
-00004670: 6f6e 293a 204f 7065 6e4d 4d4c 6162 2064  on): OpenMMLab d
-00004680: 6574 6563 7469 6f6e 2074 6f6f 6c62 6f78  etection toolbox
-00004690: 2061 6e64 2062 656e 6368 6d61 726b 2e0a   and benchmark..
-000046a0: 2020 2020 2020 2020 2d20 5b4d 4d59 4f4c          - [MMYOL
-000046b0: 4f5d 2868 7474 7073 3a2f 2f67 6974 6875  O](https://githu
-000046c0: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
-000046d0: 2f6d 6d79 6f6c 6f29 3a20 4f70 656e 4d4d  /mmyolo): OpenMM
-000046e0: 4c61 6220 594f 4c4f 2073 6572 6965 7320  Lab YOLO series 
-000046f0: 746f 6f6c 626f 7820 616e 6420 6265 6e63  toolbox and benc
-00004700: 686d 6172 6b2e 0a20 2020 2020 2020 202d  hmark..        -
-00004710: 205b 4d4d 4465 7465 6374 696f 6e33 445d   [MMDetection3D]
-00004720: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00004730: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
-00004740: 6d64 6574 6563 7469 6f6e 3364 293a 204f  mdetection3d): O
-00004750: 7065 6e4d 4d4c 6162 2773 206e 6578 742d  penMMLab's next-
-00004760: 6765 6e65 7261 7469 6f6e 2070 6c61 7466  generation platf
-00004770: 6f72 6d20 666f 7220 6765 6e65 7261 6c20  orm for general 
-00004780: 3344 206f 626a 6563 7420 6465 7465 6374  3D object detect
-00004790: 696f 6e2e 0a20 2020 2020 2020 202d 205b  ion..        - [
-000047a0: 4d4d 526f 7461 7465 5d28 6874 7470 733a  MMRotate](https:
-000047b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7065  //github.com/ope
-000047c0: 6e2d 6d6d 6c61 622f 6d6d 726f 7461 7465  n-mmlab/mmrotate
-000047d0: 293a 204f 7065 6e4d 4d4c 6162 2072 6f74  ): OpenMMLab rot
-000047e0: 6174 6564 206f 626a 6563 7420 6465 7465  ated object dete
-000047f0: 6374 696f 6e20 746f 6f6c 626f 7820 616e  ction toolbox an
-00004800: 6420 6265 6e63 686d 6172 6b2e 0a20 2020  d benchmark..   
-00004810: 2020 2020 202d 205b 4d4d 5472 6163 6b69       - [MMTracki
-00004820: 6e67 5d28 6874 7470 733a 2f2f 6769 7468  ng](https://gith
-00004830: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
-00004840: 622f 6d6d 7472 6163 6b69 6e67 293a 204f  b/mmtracking): O
-00004850: 7065 6e4d 4d4c 6162 2076 6964 656f 2070  penMMLab video p
-00004860: 6572 6365 7074 696f 6e20 746f 6f6c 626f  erception toolbo
-00004870: 7820 616e 6420 6265 6e63 686d 6172 6b2e  x and benchmark.
-00004880: 0a20 2020 2020 2020 202d 205b 4d4d 506f  .        - [MMPo
-00004890: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
-000048a0: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
-000048b0: 622f 6d6d 706f 7365 293a 204f 7065 6e4d  b/mmpose): OpenM
-000048c0: 4d4c 6162 2070 6f73 6520 6573 7469 6d61  MLab pose estima
-000048d0: 7469 6f6e 2074 6f6f 6c62 6f78 2061 6e64  tion toolbox and
-000048e0: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
-000048f0: 2020 2020 2d20 5b4d 4d53 6567 6d65 6e74      - [MMSegment
-00004900: 6174 696f 6e5d 2868 7474 7073 3a2f 2f67  ation](https://g
-00004910: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
-00004920: 6d6c 6162 2f6d 6d73 6567 6d65 6e74 6174  mlab/mmsegmentat
-00004930: 696f 6e29 3a20 4f70 656e 4d4d 4c61 6220  ion): OpenMMLab 
-00004940: 7365 6d61 6e74 6963 2073 6567 6d65 6e74  semantic segment
-00004950: 6174 696f 6e20 746f 6f6c 626f 7820 616e  ation toolbox an
-00004960: 6420 6265 6e63 686d 6172 6b2e 0a20 2020  d benchmark..   
-00004970: 2020 2020 202d 205b 4d4d 4f43 525d 2868       - [MMOCR](h
-00004980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004990: 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d 6d6f  m/open-mmlab/mmo
-000049a0: 6372 293a 204f 7065 6e4d 4d4c 6162 2074  cr): OpenMMLab t
-000049b0: 6578 7420 6465 7465 6374 696f 6e2c 2072  ext detection, r
-000049c0: 6563 6f67 6e69 7469 6f6e 2c20 616e 6420  ecognition, and 
-000049d0: 756e 6465 7273 7461 6e64 696e 6720 746f  understanding to
-000049e0: 6f6c 626f 782e 0a20 2020 2020 2020 202d  olbox..        -
-000049f0: 205b 4d4d 4875 6d61 6e33 445d 2868 7474   [MMHuman3D](htt
-00004a00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004a10: 6f70 656e 2d6d 6d6c 6162 2f6d 6d68 756d  open-mmlab/mmhum
-00004a20: 616e 3364 293a 204f 7065 6e4d 4d4c 6162  an3d): OpenMMLab
-00004a30: 2033 4420 6875 6d61 6e20 7061 7261 6d65   3D human parame
-00004a40: 7472 6963 206d 6f64 656c 2074 6f6f 6c62  tric model toolb
-00004a50: 6f78 2061 6e64 2062 656e 6368 6d61 726b  ox and benchmark
-00004a60: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d53  ..        - [MMS
-00004a70: 656c 6653 7570 5d28 6874 7470 733a 2f2f  elfSup](https://
-00004a80: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e2d  github.com/open-
-00004a90: 6d6d 6c61 622f 6d6d 7365 6c66 7375 7029  mmlab/mmselfsup)
-00004aa0: 3a20 4f70 656e 4d4d 4c61 6220 7365 6c66  : OpenMMLab self
-00004ab0: 2d73 7570 6572 7669 7365 6420 6c65 6172  -supervised lear
-00004ac0: 6e69 6e67 2074 6f6f 6c62 6f78 2061 6e64  ning toolbox and
-00004ad0: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
-00004ae0: 2020 2020 2d20 5b4d 4d46 6577 5368 6f74      - [MMFewShot
-00004af0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004b00: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
-00004b10: 6d6d 6665 7773 686f 7429 3a20 4f70 656e  mmfewshot): Open
-00004b20: 4d4d 4c61 6220 6665 7773 686f 7420 6c65  MMLab fewshot le
-00004b30: 6172 6e69 6e67 2074 6f6f 6c62 6f78 2061  arning toolbox a
-00004b40: 6e64 2062 656e 6368 6d61 726b 2e0a 2020  nd benchmark..  
-00004b50: 2020 2020 2020 2d20 5b4d 4d41 6374 696f        - [MMActio
-00004b60: 6e32 5d28 6874 7470 733a 2f2f 6769 7468  n2](https://gith
-00004b70: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
-00004b80: 622f 6d6d 6163 7469 6f6e 3229 3a20 4f70  b/mmaction2): Op
-00004b90: 656e 4d4d 4c61 6227 7320 6e65 7874 2d67  enMMLab's next-g
-00004ba0: 656e 6572 6174 696f 6e20 6163 7469 6f6e  eneration action
-00004bb0: 2075 6e64 6572 7374 616e 6469 6e67 2074   understanding t
-00004bc0: 6f6f 6c62 6f78 2061 6e64 2062 656e 6368  oolbox and bench
-00004bd0: 6d61 726b 2e0a 2020 2020 2020 2020 2d20  mark..        - 
-00004be0: 5b4d 4d46 6c6f 775d 2868 7474 7073 3a2f  [MMFlow](https:/
-00004bf0: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
-00004c00: 2d6d 6d6c 6162 2f6d 6d66 6c6f 7729 3a20  -mmlab/mmflow): 
-00004c10: 4f70 656e 4d4d 4c61 6220 6f70 7469 6361  OpenMMLab optica
-00004c20: 6c20 666c 6f77 2074 6f6f 6c62 6f78 2061  l flow toolbox a
-00004c30: 6e64 2062 656e 6368 6d61 726b 2e0a 2020  nd benchmark..  
-00004c40: 2020 2020 2020 2d20 5b4d 4d44 6570 6c6f        - [MMDeplo
-00004c50: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00004c60: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
-00004c70: 2f6d 6d64 6570 6c6f 7929 3a20 4f70 656e  /mmdeploy): Open
-00004c80: 4d4d 4c61 6220 6d6f 6465 6c20 6465 706c  MMLab model depl
-00004c90: 6f79 6d65 6e74 2066 7261 6d65 776f 726b  oyment framework
-00004ca0: 2e0a 2020 2020 2020 2020 2d20 5b4d 4d52  ..        - [MMR
-00004cb0: 617a 6f72 5d28 6874 7470 733a 2f2f 6769  azor](https://gi
-00004cc0: 7468 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d  thub.com/open-mm
-00004cd0: 6c61 622f 6d6d 7261 7a6f 7229 3a20 4f70  lab/mmrazor): Op
-00004ce0: 656e 4d4d 4c61 6220 6d6f 6465 6c20 636f  enMMLab model co
-00004cf0: 6d70 7265 7373 696f 6e20 746f 6f6c 626f  mpression toolbo
-00004d00: 7820 616e 6420 6265 6e63 686d 6172 6b2e  x and benchmark.
-00004d10: 0a20 2020 2020 2020 202d 205b 506c 6179  .        - [Play
-00004d20: 6772 6f75 6e64 5d28 6874 7470 733a 2f2f  ground](https://
-00004d30: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e2d  github.com/open-
-00004d40: 6d6d 6c61 622f 706c 6179 6772 6f75 6e64  mmlab/playground
-00004d50: 293a 2041 2063 656e 7472 616c 2068 7562  ): A central hub
-00004d60: 2066 6f72 2067 6174 6865 7269 6e67 2061   for gathering a
-00004d70: 6e64 2073 686f 7763 6173 696e 6720 616d  nd showcasing am
-00004d80: 617a 696e 6720 7072 6f6a 6563 7473 2062  azing projects b
-00004d90: 7569 6c74 2075 706f 6e20 4f70 656e 4d4d  uilt upon OpenMM
-00004da0: 4c61 622e 0a20 2020 2020 2020 200a 506c  Lab..        .Pl
-00004db0: 6174 666f 726d 3a20 554e 4b4e 4f57 4e0a  atform: UNKNOWN.
-00004dc0: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
-00004dd0: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00004de0: 3a20 3420 2d20 4265 7461 0a43 6c61 7373  : 4 - Beta.Class
-00004df0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00004e00: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00004e10: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
-00004e20: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
-00004e30: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00004e40: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00004e50: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
-00004e60: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00004e70: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00004e80: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
-00004e90: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00004ea0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00004eb0: 686f 6e20 3a3a 2033 2e37 0a43 6c61 7373  hon :: 3.7.Class
-00004ec0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00004ed0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00004ee0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
-00004ef0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00004f00: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00004f10: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-00004f20: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00004f30: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00004f40: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00004f50: 300a 436c 6173 7369 6669 6572 3a20 546f  0.Classifier: To
-00004f60: 7069 6320 3a3a 2055 7469 6c69 7469 6573  pic :: Utilities
-00004f70: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-00004f80: 3a20 3e3d 332e 370a 4465 7363 7269 7074  : >=3.7.Descript
-00004f90: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00004fa0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00004fb0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00004fc0: 616c 6c0a 5072 6f76 6964 6573 2d45 7874  all.Provides-Ext
-00004fd0: 7261 3a20 7465 7374 730a                 ra: tests.
+00003520: 696f 2f65 6e2f 6c61 7465 7374 2f74 7574  io/en/latest/tut
+00003530: 6f72 6961 6c73 2f65 7661 6c75 6174 696f  orials/evaluatio
+00003540: 6e2e 6874 6d6c 290a 2020 2020 2020 2020  n.html).        
+00003550: 2d20 5b4f 7074 696d 5772 6170 7065 725d  - [OptimWrapper]
+00003560: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
+00003570: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00003580: 2f65 6e2f 6c61 7465 7374 2f74 7574 6f72  /en/latest/tutor
+00003590: 6961 6c73 2f6f 7074 696d 5f77 7261 7070  ials/optim_wrapp
+000035a0: 6572 2e68 746d 6c29 0a20 2020 2020 2020  er.html).       
+000035b0: 202d 205b 5061 7261 6d65 7465 7220 5363   - [Parameter Sc
+000035c0: 6865 6475 6c65 725d 2868 7474 7073 3a2f  heduler](https:/
+000035d0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+000035e0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000035f0: 7374 2f74 7574 6f72 6961 6c73 2f70 6172  st/tutorials/par
+00003600: 616d 5f73 6368 6564 756c 6572 2e68 746d  am_scheduler.htm
+00003610: 6c29 0a20 2020 2020 2020 202d 205b 486f  l).        - [Ho
+00003620: 6f6b 5d28 6874 7470 733a 2f2f 6d6d 656e  ok](https://mmen
+00003630: 6769 6e65 2e72 6561 6474 6865 646f 6373  gine.readthedocs
+00003640: 2e69 6f2f 656e 2f6c 6174 6573 742f 7475  .io/en/latest/tu
+00003650: 746f 7269 616c 732f 686f 6f6b 2e68 746d  torials/hook.htm
+00003660: 6c29 0a20 2020 2020 2020 200a 2020 2020  l).        .    
+00003670: 2020 2020 3c2f 6465 7461 696c 733e 0a20      </details>. 
+00003680: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003690: 3c64 6574 6169 6c73 3e0a 2020 2020 2020  <details>.      
+000036a0: 2020 3c73 756d 6d61 7279 3e41 6476 616e    <summary>Advan
+000036b0: 6365 6420 7475 746f 7269 616c 733c 2f73  ced tutorials</s
+000036c0: 756d 6d61 7279 3e0a 2020 2020 2020 2020  ummary>.        
+000036d0: 0a20 2020 2020 2020 202d 205b 5265 6769  .        - [Regi
+000036e0: 7374 7279 5d28 6874 7470 733a 2f2f 6d6d  stry](https://mm
+000036f0: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
+00003700: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00003710: 6164 7661 6e63 6564 5f74 7574 6f72 6961  advanced_tutoria
+00003720: 6c73 2f72 6567 6973 7472 792e 6874 6d6c  ls/registry.html
+00003730: 290a 2020 2020 2020 2020 2d20 5b43 6f6e  ).        - [Con
+00003740: 6669 675d 2868 7474 7073 3a2f 2f6d 6d65  fig](https://mme
+00003750: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+00003760: 732e 696f 2f65 6e2f 6c61 7465 7374 2f61  s.io/en/latest/a
+00003770: 6476 616e 6365 645f 7475 746f 7269 616c  dvanced_tutorial
+00003780: 732f 636f 6e66 6967 2e68 746d 6c29 0a20  s/config.html). 
+00003790: 2020 2020 2020 202d 205b 4261 7365 4461         - [BaseDa
+000037a0: 7461 7365 745d 2868 7474 7073 3a2f 2f6d  taset](https://m
+000037b0: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+000037c0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000037d0: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
+000037e0: 616c 732f 6261 7365 6461 7461 7365 742e  als/basedataset.
+000037f0: 6874 6d6c 290a 2020 2020 2020 2020 2d20  html).        - 
+00003800: 5b44 6174 6120 5472 616e 7366 6f72 6d5d  [Data Transform]
+00003810: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
+00003820: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00003830: 2f65 6e2f 6c61 7465 7374 2f61 6476 616e  /en/latest/advan
+00003840: 6365 645f 7475 746f 7269 616c 732f 6461  ced_tutorials/da
+00003850: 7461 5f74 7261 6e73 666f 726d 2e68 746d  ta_transform.htm
+00003860: 6c29 0a20 2020 2020 2020 202d 205b 5765  l).        - [We
+00003870: 6967 6874 2049 6e69 7469 616c 697a 6174  ight Initializat
+00003880: 696f 6e5d 2868 7474 7073 3a2f 2f6d 6d65  ion](https://mme
+00003890: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+000038a0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f61  s.io/en/latest/a
+000038b0: 6476 616e 6365 645f 7475 746f 7269 616c  dvanced_tutorial
+000038c0: 732f 696e 6974 6961 6c69 7a65 2e68 746d  s/initialize.htm
+000038d0: 6c29 0a20 2020 2020 2020 202d 205b 5669  l).        - [Vi
+000038e0: 7375 616c 697a 6174 696f 6e5d 2868 7474  sualization](htt
+000038f0: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
+00003900: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00003910: 6c61 7465 7374 2f61 6476 616e 6365 645f  latest/advanced_
+00003920: 7475 746f 7269 616c 732f 7669 7375 616c  tutorials/visual
+00003930: 697a 6174 696f 6e2e 6874 6d6c 290a 2020  ization.html).  
+00003940: 2020 2020 2020 2d20 5b41 6273 7472 6163        - [Abstrac
+00003950: 7420 4461 7461 2045 6c65 6d65 6e74 5d28  t Data Element](
+00003960: 6874 7470 733a 2f2f 6d6d 656e 6769 6e65  https://mmengine
+00003970: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00003980: 656e 2f6c 6174 6573 742f 6164 7661 6e63  en/latest/advanc
+00003990: 6564 5f74 7574 6f72 6961 6c73 2f64 6174  ed_tutorials/dat
+000039a0: 615f 656c 656d 656e 742e 6874 6d6c 290a  a_element.html).
+000039b0: 2020 2020 2020 2020 2d20 5b44 6973 7472          - [Distr
+000039c0: 6962 7574 696f 6e20 436f 6d6d 756e 6963  ibution Communic
+000039d0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6d  ation](https://m
+000039e0: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+000039f0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003a00: 2f61 6476 616e 6365 645f 7475 746f 7269  /advanced_tutori
+00003a10: 616c 732f 6469 7374 7269 6275 7465 642e  als/distributed.
+00003a20: 6874 6d6c 290a 2020 2020 2020 2020 2d20  html).        - 
+00003a30: 5b4c 6f67 6769 6e67 5d28 6874 7470 733a  [Logging](https:
+00003a40: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+00003a50: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00003a60: 6573 742f 6164 7661 6e63 6564 5f74 7574  est/advanced_tut
+00003a70: 6f72 6961 6c73 2f6c 6f67 6769 6e67 2e68  orials/logging.h
+00003a80: 746d 6c29 0a20 2020 2020 2020 202d 205b  tml).        - [
+00003a90: 4669 6c65 2049 4f5d 2868 7474 7073 3a2f  File IO](https:/
+00003aa0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+00003ab0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00003ac0: 7374 2f61 6476 616e 6365 645f 7475 746f  st/advanced_tuto
+00003ad0: 7269 616c 732f 6669 6c65 696f 2e68 746d  rials/fileio.htm
+00003ae0: 6c29 0a20 2020 2020 2020 202d 205b 476c  l).        - [Gl
+00003af0: 6f62 616c 206d 616e 6167 6572 2028 4d61  obal manager (Ma
+00003b00: 6e61 6765 724d 6978 696e 295d 2868 7474  nagerMixin)](htt
+00003b10: 7073 3a2f 2f6d 6d65 6e67 696e 652e 7265  ps://mmengine.re
+00003b20: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00003b30: 6c61 7465 7374 2f61 6476 616e 6365 645f  latest/advanced_
+00003b40: 7475 746f 7269 616c 732f 6d61 6e61 6765  tutorials/manage
+00003b50: 725f 6d69 7869 6e2e 6874 6d6c 290a 2020  r_mixin.html).  
+00003b60: 2020 2020 2020 2d20 5b55 7365 206d 6f64        - [Use mod
+00003b70: 756c 6573 2066 726f 6d20 6f74 6865 7220  ules from other 
+00003b80: 6c69 6272 6172 6965 735d 2868 7474 7073  libraries](https
+00003b90: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
+00003ba0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00003bb0: 7465 7374 2f61 6476 616e 6365 645f 7475  test/advanced_tu
+00003bc0: 746f 7269 616c 732f 6372 6f73 735f 6c69  torials/cross_li
+00003bd0: 6272 6172 792e 6874 6d6c 290a 2020 2020  brary.html).    
+00003be0: 2020 2020 2d20 5b54 6573 7420 5469 6d65      - [Test Time
+00003bf0: 2041 6775 6d65 6e74 6174 696f 6e5d 2868   Agumentation](h
+00003c00: 7474 7073 3a2f 2f6d 6d65 6e67 696e 652e  ttps://mmengine.
+00003c10: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00003c20: 6e2f 6c61 7465 7374 2f61 6476 616e 6365  n/latest/advance
+00003c30: 645f 7475 746f 7269 616c 732f 7465 7374  d_tutorials/test
+00003c40: 5f74 696d 655f 6175 676d 656e 7461 7469  _time_augmentati
+00003c50: 6f6e 2e68 746d 6c29 0a20 2020 2020 2020  on.html).       
+00003c60: 200a 2020 2020 2020 2020 3c2f 6465 7461   .        </deta
+00003c70: 696c 733e 0a20 2020 2020 2020 200a 2020  ils>.        .  
+00003c80: 2020 2020 2020 3c64 6574 6169 6c73 3e0a        <details>.
+00003c90: 2020 2020 2020 2020 3c73 756d 6d61 7279          <summary
+00003ca0: 3e45 7861 6d70 6c65 733c 2f73 756d 6d61  >Examples</summa
+00003cb0: 7279 3e0a 2020 2020 2020 2020 0a20 2020  ry>.        .   
+00003cc0: 2020 2020 202d 205b 5472 6169 6e20 6120       - [Train a 
+00003cd0: 4741 4e5d 2868 7474 7073 3a2f 2f6d 6d65  GAN](https://mme
+00003ce0: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+00003cf0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f65  s.io/en/latest/e
+00003d00: 7861 6d70 6c65 732f 7472 6169 6e5f 615f  xamples/train_a_
+00003d10: 6761 6e2e 6874 6d6c 290a 2020 2020 2020  gan.html).      
+00003d20: 2020 0a20 2020 2020 2020 203c 2f64 6574    .        </det
+00003d30: 6169 6c73 3e0a 2020 2020 2020 2020 0a20  ails>.        . 
+00003d40: 2020 2020 2020 203c 6465 7461 696c 733e         <details>
+00003d50: 0a20 2020 2020 2020 203c 7375 6d6d 6172  .        <summar
+00003d60: 793e 436f 6d6d 6f6e 2055 7361 6765 3c2f  y>Common Usage</
+00003d70: 7375 6d6d 6172 793e 0a20 2020 2020 2020  summary>.       
+00003d80: 200a 2020 2020 2020 2020 2d20 5b52 6573   .        - [Res
+00003d90: 756d 6520 5472 6169 6e69 6e67 5d28 6874  ume Training](ht
+00003da0: 7470 733a 2f2f 6d6d 656e 6769 6e65 2e72  tps://mmengine.r
+00003db0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00003dc0: 2f6c 6174 6573 742f 636f 6d6d 6f6e 5f75  /latest/common_u
+00003dd0: 7361 6765 2f72 6573 756d 655f 7472 6169  sage/resume_trai
+00003de0: 6e69 6e67 2e68 746d 6c29 0a20 2020 2020  ning.html).     
+00003df0: 2020 202d 205b 5370 6565 6420 7570 2054     - [Speed up T
+00003e00: 7261 696e 696e 675d 2868 7474 7073 3a2f  raining](https:/
+00003e10: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+00003e20: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00003e30: 7374 2f63 6f6d 6d6f 6e5f 7573 6167 652f  st/common_usage/
+00003e40: 7370 6565 645f 7570 5f74 7261 696e 696e  speed_up_trainin
+00003e50: 672e 6874 6d6c 290a 2020 2020 2020 2020  g.html).        
+00003e60: 2d20 5b53 6176 6520 4d65 6d6f 7279 206f  - [Save Memory o
+00003e70: 6e20 4750 555d 2868 7474 7073 3a2f 2f6d  n GPU](https://m
+00003e80: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00003e90: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003ea0: 2f63 6f6d 6d6f 6e5f 7573 6167 652f 7361  /common_usage/sa
+00003eb0: 7665 5f67 7075 5f6d 656d 6f72 792e 6874  ve_gpu_memory.ht
+00003ec0: 6d6c 290a 2020 2020 2020 2020 0a20 2020  ml).        .   
+00003ed0: 2020 2020 203c 2f64 6574 6169 6c73 3e0a       </details>.
+00003ee0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003ef0: 203c 6465 7461 696c 733e 0a20 2020 2020   <details>.     
+00003f00: 2020 203c 7375 6d6d 6172 793e 4465 7369     <summary>Desi
+00003f10: 676e 3c2f 7375 6d6d 6172 793e 0a20 2020  gn</summary>.   
+00003f20: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00003f30: 5b48 6f6f 6b5d 2868 7474 7073 3a2f 2f6d  [Hook](https://m
+00003f40: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00003f50: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003f60: 2f64 6573 6967 6e2f 686f 6f6b 2e68 746d  /design/hook.htm
+00003f70: 6c29 0a20 2020 2020 2020 202d 205b 5275  l).        - [Ru
+00003f80: 6e6e 6572 5d28 6874 7470 733a 2f2f 6d6d  nner](https://mm
+00003f90: 656e 6769 6e65 2e72 6561 6474 6865 646f  engine.readthedo
+00003fa0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00003fb0: 6465 7369 676e 2f72 756e 6e65 722e 6874  design/runner.ht
+00003fc0: 6d6c 290a 2020 2020 2020 2020 2d20 5b45  ml).        - [E
+00003fd0: 7661 6c75 6174 696f 6e5d 2868 7474 7073  valuation](https
+00003fe0: 3a2f 2f6d 6d65 6e67 696e 652e 7265 6164  ://mmengine.read
+00003ff0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00004000: 7465 7374 2f64 6573 6967 6e2f 6576 616c  test/design/eval
+00004010: 7561 7469 6f6e 2e68 746d 6c29 0a20 2020  uation.html).   
+00004020: 2020 2020 202d 205b 5669 7375 616c 697a       - [Visualiz
+00004030: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6d  ation](https://m
+00004040: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00004050: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00004060: 2f64 6573 6967 6e2f 7669 7375 616c 697a  /design/visualiz
+00004070: 6174 696f 6e2e 6874 6d6c 290a 2020 2020  ation.html).    
+00004080: 2020 2020 2d20 5b4c 6f67 6769 6e67 5d28      - [Logging](
+00004090: 6874 7470 733a 2f2f 6d6d 656e 6769 6e65  https://mmengine
+000040a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+000040b0: 656e 2f6c 6174 6573 742f 6465 7369 676e  en/latest/design
+000040c0: 2f6c 6f67 6769 6e67 2e68 746d 6c29 0a20  /logging.html). 
+000040d0: 2020 2020 2020 202d 205b 496e 6665 725d         - [Infer]
+000040e0: 2868 7474 7073 3a2f 2f6d 6d65 6e67 696e  (https://mmengin
+000040f0: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00004100: 2f65 6e2f 6c61 7465 7374 2f64 6573 6967  /en/latest/desig
+00004110: 6e2f 696e 6665 722e 6874 6d6c 290a 2020  n/infer.html).  
+00004120: 2020 2020 2020 0a20 2020 2020 2020 203c        .        <
+00004130: 2f64 6574 6169 6c73 3e0a 2020 2020 2020  /details>.      
+00004140: 2020 0a20 2020 2020 2020 203c 6465 7461    .        <deta
+00004150: 696c 733e 0a20 2020 2020 2020 203c 7375  ils>.        <su
+00004160: 6d6d 6172 793e 4d69 6772 6174 696f 6e20  mmary>Migration 
+00004170: 6775 6964 653c 2f73 756d 6d61 7279 3e0a  guide</summary>.
+00004180: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004190: 202d 205b 4d69 6772 6174 6520 5275 6e6e   - [Migrate Runn
+000041a0: 6572 2066 726f 6d20 4d4d 4356 2074 6f20  er from MMCV to 
+000041b0: 4d4d 456e 6769 6e65 5d28 6874 7470 733a  MMEngine](https:
+000041c0: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+000041d0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+000041e0: 6573 742f 6d69 6772 6174 696f 6e2f 7275  est/migration/ru
+000041f0: 6e6e 6572 2e68 746d 6c29 0a20 2020 2020  nner.html).     
+00004200: 2020 202d 205b 4d69 6772 6174 6520 486f     - [Migrate Ho
+00004210: 6f6b 2066 726f 6d20 4d4d 4356 2074 6f20  ok from MMCV to 
+00004220: 4d4d 456e 6769 6e65 5d28 6874 7470 733a  MMEngine](https:
+00004230: 2f2f 6d6d 656e 6769 6e65 2e72 6561 6474  //mmengine.readt
+00004240: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00004250: 6573 742f 6d69 6772 6174 696f 6e2f 686f  est/migration/ho
+00004260: 6f6b 2e68 746d 6c29 0a20 2020 2020 2020  ok.html).       
+00004270: 202d 205b 4d69 6772 6174 6520 4d6f 6465   - [Migrate Mode
+00004280: 6c20 6672 6f6d 204d 4d43 5620 746f 204d  l from MMCV to M
+00004290: 4d45 6e67 696e 655d 2868 7474 7073 3a2f  MEngine](https:/
+000042a0: 2f6d 6d65 6e67 696e 652e 7265 6164 7468  /mmengine.readth
+000042b0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000042c0: 7374 2f6d 6967 7261 7469 6f6e 2f6d 6f64  st/migration/mod
+000042d0: 656c 2e68 746d 6c29 0a20 2020 2020 2020  el.html).       
+000042e0: 202d 205b 4d69 6772 6174 6520 5061 7261   - [Migrate Para
+000042f0: 6d65 7465 7220 5363 6865 6475 6c65 7220  meter Scheduler 
+00004300: 6672 6f6d 204d 4d43 5620 746f 204d 4d45  from MMCV to MME
+00004310: 6e67 696e 655d 2868 7474 7073 3a2f 2f6d  ngine](https://m
+00004320: 6d65 6e67 696e 652e 7265 6164 7468 6564  mengine.readthed
+00004330: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00004340: 2f6d 6967 7261 7469 6f6e 2f70 6172 616d  /migration/param
+00004350: 5f73 6368 6564 756c 6572 2e68 746d 6c29  _scheduler.html)
+00004360: 0a20 2020 2020 2020 202d 205b 4d69 6772  .        - [Migr
+00004370: 6174 6520 4461 7461 2054 7261 6e73 666f  ate Data Transfo
+00004380: 726d 2074 6f20 4f70 656e 4d4d 4c61 6220  rm to OpenMMLab 
+00004390: 322e 305d 2868 7474 7073 3a2f 2f6d 6d65  2.0](https://mme
+000043a0: 6e67 696e 652e 7265 6164 7468 6564 6f63  ngine.readthedoc
+000043b0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6d  s.io/en/latest/m
+000043c0: 6967 7261 7469 6f6e 2f74 7261 6e73 666f  igration/transfo
+000043d0: 726d 2e68 746d 6c29 0a20 2020 2020 2020  rm.html).       
+000043e0: 200a 2020 2020 2020 2020 3c2f 6465 7461   .        </deta
+000043f0: 696c 733e 0a20 2020 2020 2020 200a 2020  ils>.        .  
+00004400: 2020 2020 2020 2323 2043 6f6e 7472 6962        ## Contrib
+00004410: 7574 696e 670a 2020 2020 2020 2020 0a20  uting.        . 
+00004420: 2020 2020 2020 2057 6520 6170 7072 6563         We apprec
+00004430: 6961 7465 2061 6c6c 2063 6f6e 7472 6962  iate all contrib
+00004440: 7574 696f 6e73 2074 6f20 696d 7072 6f76  utions to improv
+00004450: 6520 4d4d 456e 6769 6e65 2e20 506c 6561  e MMEngine. Plea
+00004460: 7365 2072 6566 6572 2074 6f20 5b43 4f4e  se refer to [CON
+00004470: 5452 4942 5554 494e 472e 6d64 5d28 434f  TRIBUTING.md](CO
+00004480: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
+00004490: 6f72 2074 6865 2063 6f6e 7472 6962 7574  or the contribut
+000044a0: 696e 6720 6775 6964 656c 696e 652e 0a20  ing guideline.. 
+000044b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000044c0: 2323 2043 6974 6174 696f 6e0a 2020 2020  ## Citation.    
+000044d0: 2020 2020 0a20 2020 2020 2020 2049 6620      .        If 
+000044e0: 796f 7520 6669 6e64 2074 6869 7320 7072  you find this pr
+000044f0: 6f6a 6563 7420 7573 6566 756c 2069 6e20  oject useful in 
+00004500: 796f 7572 2072 6573 6561 7263 682c 2070  your research, p
+00004510: 6c65 6173 6520 636f 6e73 6964 6572 2063  lease consider c
+00004520: 6974 653a 0a20 2020 2020 2020 200a 2020  ite:.        .  
+00004530: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00004540: 2020 4061 7274 6963 6c65 7b6d 6d65 6e67    @article{mmeng
+00004550: 696e 6532 3032 322c 0a20 2020 2020 2020  ine2022,.       
+00004560: 2020 2074 6974 6c65 2020 203d 207b 7b4d     title   = {{M
+00004570: 4d45 6e67 696e 657d 3a20 4f70 656e 4d4d  MEngine}: OpenMM
+00004580: 4c61 6220 466f 756e 6461 7469 6f6e 616c  Lab Foundational
+00004590: 204c 6962 7261 7279 2066 6f72 2054 7261   Library for Tra
+000045a0: 696e 696e 6720 4465 6570 204c 6561 726e  ining Deep Learn
+000045b0: 696e 6720 4d6f 6465 6c73 7d2c 0a20 2020  ing Models},.   
+000045c0: 2020 2020 2020 2061 7574 686f 7220 203d         author  =
+000045d0: 207b 4d4d 456e 6769 6e65 2043 6f6e 7472   {MMEngine Contr
+000045e0: 6962 7574 6f72 737d 2c0a 2020 2020 2020  ibutors},.      
+000045f0: 2020 2020 686f 7770 7562 6c69 7368 6564      howpublished
+00004600: 203d 207b 5c75 726c 7b68 7474 7073 3a2f   = {\url{https:/
+00004610: 2f67 6974 6875 622e 636f 6d2f 6f70 656e  /github.com/open
+00004620: 2d6d 6d6c 6162 2f6d 6d65 6e67 696e 657d  -mmlab/mmengine}
+00004630: 7d2c 0a20 2020 2020 2020 2020 2079 6561  },.          yea
+00004640: 723d 7b32 3032 327d 0a20 2020 2020 2020  r={2022}.       
+00004650: 207d 0a20 2020 2020 2020 2060 6060 0a20   }.        ```. 
+00004660: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00004670: 2323 204c 6963 656e 7365 0a20 2020 2020  ## License.     
+00004680: 2020 200a 2020 2020 2020 2020 5468 6973     .        This
+00004690: 2070 726f 6a65 6374 2069 7320 7265 6c65   project is rele
+000046a0: 6173 6564 2075 6e64 6572 2074 6865 205b  ased under the [
+000046b0: 4170 6163 6865 2032 2e30 206c 6963 656e  Apache 2.0 licen
+000046c0: 7365 5d28 4c49 4345 4e53 4529 2e0a 2020  se](LICENSE)..  
+000046d0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000046e0: 2320 5072 6f6a 6563 7473 2069 6e20 4f70  # Projects in Op
+000046f0: 656e 4d4d 4c61 620a 2020 2020 2020 2020  enMMLab.        
+00004700: 0a20 2020 2020 2020 202d 205b 4d49 4d5d  .        - [MIM]
+00004710: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004720: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
+00004730: 696d 293a 204d 494d 2069 6e73 7461 6c6c  im): MIM install
+00004740: 7320 4f70 656e 4d4d 4c61 6220 7061 636b  s OpenMMLab pack
+00004750: 6167 6573 2e0a 2020 2020 2020 2020 2d20  ages..        - 
+00004760: 5b4d 4d43 565d 2868 7474 7073 3a2f 2f67  [MMCV](https://g
+00004770: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004780: 6d6c 6162 2f6d 6d63 7629 3a20 4f70 656e  mlab/mmcv): Open
+00004790: 4d4d 4c61 6220 666f 756e 6461 7469 6f6e  MMLab foundation
+000047a0: 616c 206c 6962 7261 7279 2066 6f72 2063  al library for c
+000047b0: 6f6d 7075 7465 7220 7669 7369 6f6e 2e0a  omputer vision..
+000047c0: 2020 2020 2020 2020 2d20 5b4d 4d45 7661          - [MMEva
+000047d0: 6c5d 2868 7474 7073 3a2f 2f67 6974 6875  l](https://githu
+000047e0: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
+000047f0: 2f6d 6d65 7661 6c29 3a20 4120 756e 6966  /mmeval): A unif
+00004800: 6965 6420 6576 616c 7561 7469 6f6e 206c  ied evaluation l
+00004810: 6962 7261 7279 2066 6f72 206d 756c 7469  ibrary for multi
+00004820: 706c 6520 6d61 6368 696e 6520 6c65 6172  ple machine lear
+00004830: 6e69 6e67 206c 6962 7261 7269 6573 2e0a  ning libraries..
+00004840: 2020 2020 2020 2020 2d20 5b4d 4d50 7265          - [MMPre
+00004850: 5472 6169 6e5d 2868 7474 7073 3a2f 2f67  Train](https://g
+00004860: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004870: 6d6c 6162 2f6d 6d70 7265 7472 6169 6e29  mlab/mmpretrain)
+00004880: 3a20 4f70 656e 4d4d 4c61 6220 7072 652d  : OpenMMLab pre-
+00004890: 7472 6169 6e69 6e67 2074 6f6f 6c62 6f78  training toolbox
+000048a0: 2061 6e64 2062 656e 6368 6d61 726b 2e0a   and benchmark..
+000048b0: 2020 2020 2020 2020 2d20 5b4d 4d61 6769          - [MMagi
+000048c0: 635d 2868 7474 7073 3a2f 2f67 6974 6875  c](https://githu
+000048d0: 622e 636f 6d2f 6f70 656e 2d6d 6d6c 6162  b.com/open-mmlab
+000048e0: 2f6d 6d61 6769 6329 3a20 4f70 656e 2a2a  /mmagic): Open**
+000048f0: 4d4d 2a2a 4c61 6220 2a2a 412a 2a64 7661  MM**Lab **A**dva
+00004900: 6e63 6564 2c20 2a2a 472a 2a65 6e65 7261  nced, **G**enera
+00004910: 7469 7665 2061 6e64 202a 2a49 2a2a 6e74  tive and **I**nt
+00004920: 656c 6c69 6765 6e74 202a 2a43 2a2a 7265  elligent **C**re
+00004930: 6174 696f 6e20 746f 6f6c 626f 782e 0a20  ation toolbox.. 
+00004940: 2020 2020 2020 202d 205b 4d4d 4465 7465         - [MMDete
+00004950: 6374 696f 6e5d 2868 7474 7073 3a2f 2f67  ction](https://g
+00004960: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004970: 6d6c 6162 2f6d 6d64 6574 6563 7469 6f6e  mlab/mmdetection
+00004980: 293a 204f 7065 6e4d 4d4c 6162 2064 6574  ): OpenMMLab det
+00004990: 6563 7469 6f6e 2074 6f6f 6c62 6f78 2061  ection toolbox a
+000049a0: 6e64 2062 656e 6368 6d61 726b 2e0a 2020  nd benchmark..  
+000049b0: 2020 2020 2020 2d20 5b4d 4d59 4f4c 4f5d        - [MMYOLO]
+000049c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000049d0: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
+000049e0: 6d79 6f6c 6f29 3a20 4f70 656e 4d4d 4c61  myolo): OpenMMLa
+000049f0: 6220 594f 4c4f 2073 6572 6965 7320 746f  b YOLO series to
+00004a00: 6f6c 626f 7820 616e 6420 6265 6e63 686d  olbox and benchm
+00004a10: 6172 6b2e 0a20 2020 2020 2020 202d 205b  ark..        - [
+00004a20: 4d4d 4465 7465 6374 696f 6e33 445d 2868  MMDetection3D](h
+00004a30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004a40: 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d 6d64  m/open-mmlab/mmd
+00004a50: 6574 6563 7469 6f6e 3364 293a 204f 7065  etection3d): Ope
+00004a60: 6e4d 4d4c 6162 2773 206e 6578 742d 6765  nMMLab's next-ge
+00004a70: 6e65 7261 7469 6f6e 2070 6c61 7466 6f72  neration platfor
+00004a80: 6d20 666f 7220 6765 6e65 7261 6c20 3344  m for general 3D
+00004a90: 206f 626a 6563 7420 6465 7465 6374 696f   object detectio
+00004aa0: 6e2e 0a20 2020 2020 2020 202d 205b 4d4d  n..        - [MM
+00004ab0: 526f 7461 7465 5d28 6874 7470 733a 2f2f  Rotate](https://
+00004ac0: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e2d  github.com/open-
+00004ad0: 6d6d 6c61 622f 6d6d 726f 7461 7465 293a  mmlab/mmrotate):
+00004ae0: 204f 7065 6e4d 4d4c 6162 2072 6f74 6174   OpenMMLab rotat
+00004af0: 6564 206f 626a 6563 7420 6465 7465 6374  ed object detect
+00004b00: 696f 6e20 746f 6f6c 626f 7820 616e 6420  ion toolbox and 
+00004b10: 6265 6e63 686d 6172 6b2e 0a20 2020 2020  benchmark..     
+00004b20: 2020 202d 205b 4d4d 5472 6163 6b69 6e67     - [MMTracking
+00004b30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004b40: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
+00004b50: 6d6d 7472 6163 6b69 6e67 293a 204f 7065  mmtracking): Ope
+00004b60: 6e4d 4d4c 6162 2076 6964 656f 2070 6572  nMMLab video per
+00004b70: 6365 7074 696f 6e20 746f 6f6c 626f 7820  ception toolbox 
+00004b80: 616e 6420 6265 6e63 686d 6172 6b2e 0a20  and benchmark.. 
+00004b90: 2020 2020 2020 202d 205b 4d4d 506f 7365         - [MMPose
+00004ba0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004bb0: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
+00004bc0: 6d6d 706f 7365 293a 204f 7065 6e4d 4d4c  mmpose): OpenMML
+00004bd0: 6162 2070 6f73 6520 6573 7469 6d61 7469  ab pose estimati
+00004be0: 6f6e 2074 6f6f 6c62 6f78 2061 6e64 2062  on toolbox and b
+00004bf0: 656e 6368 6d61 726b 2e0a 2020 2020 2020  enchmark..      
+00004c00: 2020 2d20 5b4d 4d53 6567 6d65 6e74 6174    - [MMSegmentat
+00004c10: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
+00004c20: 6875 622e 636f 6d2f 6f70 656e 2d6d 6d6c  hub.com/open-mml
+00004c30: 6162 2f6d 6d73 6567 6d65 6e74 6174 696f  ab/mmsegmentatio
+00004c40: 6e29 3a20 4f70 656e 4d4d 4c61 6220 7365  n): OpenMMLab se
+00004c50: 6d61 6e74 6963 2073 6567 6d65 6e74 6174  mantic segmentat
+00004c60: 696f 6e20 746f 6f6c 626f 7820 616e 6420  ion toolbox and 
+00004c70: 6265 6e63 686d 6172 6b2e 0a20 2020 2020  benchmark..     
+00004c80: 2020 202d 205b 4d4d 4f43 525d 2868 7474     - [MMOCR](htt
+00004c90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004ca0: 6f70 656e 2d6d 6d6c 6162 2f6d 6d6f 6372  open-mmlab/mmocr
+00004cb0: 293a 204f 7065 6e4d 4d4c 6162 2074 6578  ): OpenMMLab tex
+00004cc0: 7420 6465 7465 6374 696f 6e2c 2072 6563  t detection, rec
+00004cd0: 6f67 6e69 7469 6f6e 2c20 616e 6420 756e  ognition, and un
+00004ce0: 6465 7273 7461 6e64 696e 6720 746f 6f6c  derstanding tool
+00004cf0: 626f 782e 0a20 2020 2020 2020 202d 205b  box..        - [
+00004d00: 4d4d 4875 6d61 6e33 445d 2868 7474 7073  MMHuman3D](https
+00004d10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f70  ://github.com/op
+00004d20: 656e 2d6d 6d6c 6162 2f6d 6d68 756d 616e  en-mmlab/mmhuman
+00004d30: 3364 293a 204f 7065 6e4d 4d4c 6162 2033  3d): OpenMMLab 3
+00004d40: 4420 6875 6d61 6e20 7061 7261 6d65 7472  D human parametr
+00004d50: 6963 206d 6f64 656c 2074 6f6f 6c62 6f78  ic model toolbox
+00004d60: 2061 6e64 2062 656e 6368 6d61 726b 2e0a   and benchmark..
+00004d70: 2020 2020 2020 2020 2d20 5b4d 4d53 656c          - [MMSel
+00004d80: 6653 7570 5d28 6874 7470 733a 2f2f 6769  fSup](https://gi
+00004d90: 7468 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d  thub.com/open-mm
+00004da0: 6c61 622f 6d6d 7365 6c66 7375 7029 3a20  lab/mmselfsup): 
+00004db0: 4f70 656e 4d4d 4c61 6220 7365 6c66 2d73  OpenMMLab self-s
+00004dc0: 7570 6572 7669 7365 6420 6c65 6172 6e69  upervised learni
+00004dd0: 6e67 2074 6f6f 6c62 6f78 2061 6e64 2062  ng toolbox and b
+00004de0: 656e 6368 6d61 726b 2e0a 2020 2020 2020  enchmark..      
+00004df0: 2020 2d20 5b4d 4d46 6577 5368 6f74 5d28    - [MMFewShot](
+00004e00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004e10: 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f 6d6d  om/open-mmlab/mm
+00004e20: 6665 7773 686f 7429 3a20 4f70 656e 4d4d  fewshot): OpenMM
+00004e30: 4c61 6220 6665 7773 686f 7420 6c65 6172  Lab fewshot lear
+00004e40: 6e69 6e67 2074 6f6f 6c62 6f78 2061 6e64  ning toolbox and
+00004e50: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
+00004e60: 2020 2020 2d20 5b4d 4d41 6374 696f 6e32      - [MMAction2
+00004e70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004e80: 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61 622f  .com/open-mmlab/
+00004e90: 6d6d 6163 7469 6f6e 3229 3a20 4f70 656e  mmaction2): Open
+00004ea0: 4d4d 4c61 6227 7320 6e65 7874 2d67 656e  MMLab's next-gen
+00004eb0: 6572 6174 696f 6e20 6163 7469 6f6e 2075  eration action u
+00004ec0: 6e64 6572 7374 616e 6469 6e67 2074 6f6f  nderstanding too
+00004ed0: 6c62 6f78 2061 6e64 2062 656e 6368 6d61  lbox and benchma
+00004ee0: 726b 2e0a 2020 2020 2020 2020 2d20 5b4d  rk..        - [M
+00004ef0: 4d46 6c6f 775d 2868 7474 7073 3a2f 2f67  MFlow](https://g
+00004f00: 6974 6875 622e 636f 6d2f 6f70 656e 2d6d  ithub.com/open-m
+00004f10: 6d6c 6162 2f6d 6d66 6c6f 7729 3a20 4f70  mlab/mmflow): Op
+00004f20: 656e 4d4d 4c61 6220 6f70 7469 6361 6c20  enMMLab optical 
+00004f30: 666c 6f77 2074 6f6f 6c62 6f78 2061 6e64  flow toolbox and
+00004f40: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
+00004f50: 2020 2020 2d20 5b4d 4d44 6570 6c6f 795d      - [MMDeploy]
+00004f60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004f70: 636f 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d  com/open-mmlab/m
+00004f80: 6d64 6570 6c6f 7929 3a20 4f70 656e 4d4d  mdeploy): OpenMM
+00004f90: 4c61 6220 6d6f 6465 6c20 6465 706c 6f79  Lab model deploy
+00004fa0: 6d65 6e74 2066 7261 6d65 776f 726b 2e0a  ment framework..
+00004fb0: 2020 2020 2020 2020 2d20 5b4d 4d52 617a          - [MMRaz
+00004fc0: 6f72 5d28 6874 7470 733a 2f2f 6769 7468  or](https://gith
+00004fd0: 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d 6c61  ub.com/open-mmla
+00004fe0: 622f 6d6d 7261 7a6f 7229 3a20 4f70 656e  b/mmrazor): Open
+00004ff0: 4d4d 4c61 6220 6d6f 6465 6c20 636f 6d70  MMLab model comp
+00005000: 7265 7373 696f 6e20 746f 6f6c 626f 7820  ression toolbox 
+00005010: 616e 6420 6265 6e63 686d 6172 6b2e 0a20  and benchmark.. 
+00005020: 2020 2020 2020 202d 205b 506c 6179 6772         - [Playgr
+00005030: 6f75 6e64 5d28 6874 7470 733a 2f2f 6769  ound](https://gi
+00005040: 7468 7562 2e63 6f6d 2f6f 7065 6e2d 6d6d  thub.com/open-mm
+00005050: 6c61 622f 706c 6179 6772 6f75 6e64 293a  lab/playground):
+00005060: 2041 2063 656e 7472 616c 2068 7562 2066   A central hub f
+00005070: 6f72 2067 6174 6865 7269 6e67 2061 6e64  or gathering and
+00005080: 2073 686f 7763 6173 696e 6720 616d 617a   showcasing amaz
+00005090: 696e 6720 7072 6f6a 6563 7473 2062 7569  ing projects bui
+000050a0: 6c74 2075 706f 6e20 4f70 656e 4d4d 4c61  lt upon OpenMMLa
+000050b0: 622e 0a20 2020 2020 2020 200a 506c 6174  b..        .Plat
+000050c0: 666f 726d 3a20 554e 4b4e 4f57 4e0a 436c  form: UNKNOWN.Cl
+000050d0: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
+000050e0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000050f0: 3420 2d20 4265 7461 0a43 6c61 7373 6966  4 - Beta.Classif
+00005100: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
+00005110: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00005120: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
+00005130: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+00005140: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00005150: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00005160: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
+00005170: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00005180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00005190: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+000051a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000051b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000051c0: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
+000051d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000051e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000051f0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00005200: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00005210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00005220: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00005230: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00005240: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00005250: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00005260: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00005270: 6320 3a3a 2055 7469 6c69 7469 6573 0a52  c :: Utilities.R
+00005280: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+00005290: 3e3d 332e 370a 4465 7363 7269 7074 696f  >=3.7.Descriptio
+000052a0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+000052b0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
+000052c0: 6f76 6964 6573 2d45 7874 7261 3a20 616c  ovides-Extra: al
+000052d0: 6c0a 5072 6f76 6964 6573 2d45 7874 7261  l.Provides-Extra
+000052e0: 3a20 7465 7374 730a                      : tests.
```

### Comparing `mmengine-0.7.4/mmengine.egg-info/SOURCES.txt` & `mmengine-0.8.0/mmengine.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 mmengine/__init__.py
 mmengine/version.py
 mmengine.egg-info/PKG-INFO
 mmengine.egg-info/SOURCES.txt
 mmengine.egg-info/dependency_links.txt
 mmengine.egg-info/requires.txt
 mmengine.egg-info/top_level.txt
+mmengine/_strategy/__init__.py
+mmengine/_strategy/base.py
+mmengine/_strategy/deepspeed.py
+mmengine/_strategy/distributed.py
+mmengine/_strategy/fsdp.py
+mmengine/_strategy/single_device.py
+mmengine/_strategy/utils.py
 mmengine/analysis/__init__.py
 mmengine/analysis/complexity_analysis.py
 mmengine/analysis/jit_analysis.py
 mmengine/analysis/jit_handles.py
 mmengine/analysis/print_helper.py
 mmengine/config/__init__.py
 mmengine/config/config.py
+mmengine/config/lazy.py
 mmengine/config/utils.py
 mmengine/dataset/__init__.py
 mmengine/dataset/base_dataset.py
 mmengine/dataset/dataset_wrapper.py
 mmengine/dataset/sampler.py
 mmengine/dataset/utils.py
 mmengine/device/__init__.py
@@ -82,22 +90,25 @@
 mmengine/model/test_time_aug.py
 mmengine/model/utils.py
 mmengine/model/weight_init.py
 mmengine/model/base_model/__init__.py
 mmengine/model/base_model/base_model.py
 mmengine/model/base_model/data_preprocessor.py
 mmengine/model/wrappers/__init__.py
+mmengine/model/wrappers/_deepspeed.py
 mmengine/model/wrappers/distributed.py
 mmengine/model/wrappers/fully_sharded_distributed.py
 mmengine/model/wrappers/seperate_distributed.py
 mmengine/model/wrappers/utils.py
 mmengine/optim/__init__.py
 mmengine/optim/optimizer/__init__.py
+mmengine/optim/optimizer/_deepspeed.py
 mmengine/optim/optimizer/amp_optimizer_wrapper.py
 mmengine/optim/optimizer/apex_optimizer_wrapper.py
+mmengine/optim/optimizer/base.py
 mmengine/optim/optimizer/builder.py
 mmengine/optim/optimizer/default_constructor.py
 mmengine/optim/optimizer/optimizer_wrapper.py
 mmengine/optim/optimizer/optimizer_wrapper_dict.py
 mmengine/optim/optimizer/zero_optimizer.py
 mmengine/optim/scheduler/__init__.py
 mmengine/optim/scheduler/lr_scheduler.py
@@ -106,14 +117,15 @@
 mmengine/registry/__init__.py
 mmengine/registry/build_functions.py
 mmengine/registry/default_scope.py
 mmengine/registry/registry.py
 mmengine/registry/root.py
 mmengine/registry/utils.py
 mmengine/runner/__init__.py
+mmengine/runner/_flexible_runner.py
 mmengine/runner/amp.py
 mmengine/runner/base_loop.py
 mmengine/runner/checkpoint.py
 mmengine/runner/log_processor.py
 mmengine/runner/loops.py
 mmengine/runner/priority.py
 mmengine/runner/runner.py
```

### Comparing `mmengine-0.7.4/setup.py` & `mmengine-0.8.0/setup.py`

 * *Files identical despite different names*

