# Comparing `tmp/refuel-autolabel-0.0.6.tar.gz` & `tmp/refuel-autolabel-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-autolabel-0.0.6.tar", last modified: Fri Jun 30 23:17:00 2023, max compression
+gzip compressed data, was "refuel-autolabel-0.0.7.tar", last modified: Mon Jul  3 03:33:57 2023, max compression
```

## Comparing `refuel-autolabel-0.0.6.tar` & `refuel-autolabel-0.0.7.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.617916 refuel-autolabel-0.0.6/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/LICENSE
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10361 2023-06-30 23:17:00.617696 refuel-autolabel-0.0.6/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8337 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/README.md
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2247 2023-06-30 23:16:32.000000 refuel-autolabel-0.0.6/pyproject.toml
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-30 23:17:00.617963 refuel-autolabel-0.0.6/setup.cfg
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.602635 refuel-autolabel-0.0.6/src/
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.604749 refuel-autolabel-0.0.6/src/autolabel/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/__init__.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.605527 refuel-autolabel-0.0.6/src/autolabel/cache/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/cache/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/cache/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/cache/sqlalchemy_cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.6/src/autolabel/confidence.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.606230 refuel-autolabel-0.0.6/src/autolabel/configs/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/configs/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1401 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/configs/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7569 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/configs/config.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4114 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/configs/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.607915 refuel-autolabel-0.0.6/src/autolabel/data_models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/annotation.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/dataset.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/task.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/task_run.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.608439 refuel-autolabel-0.0.6/src/autolabel/database/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/database/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      679 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/database/engine.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/database/state_manager.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8085 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/dataset_loader.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.609102 refuel-autolabel-0.0.6/src/autolabel/few_shot/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3233 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/few_shot/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/few_shot/fixed_example_selector.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/few_shot/vector_store.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19705 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/labeler.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.610564 refuel-autolabel-0.0.6/src/autolabel/models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/models/anthropic.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3132 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/models/hf_pipeline.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5682 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/models/openai.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3920 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/models/palm.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3575 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/models/refuel.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4685 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.612509 refuel-autolabel-0.0.6/src/autolabel/tasks/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1298 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4319 2023-06-22 05:07:53.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7409 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7419 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/entity_matching.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8221 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/multilabel_classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12627 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/named_entity_recognition.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7508 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/question_answering.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/utils.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9773 2023-06-22 21:40:05.000000 refuel-autolabel-0.0.6/src/autolabel/utils.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.617432 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10361 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1652 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      863 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/requires.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/top_level.txt
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.294360 refuel-autolabel-0.0.7/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/LICENSE
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10384 2023-07-03 03:33:57.294155 refuel-autolabel-0.0.7/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8337 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/README.md
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2303 2023-07-03 03:32:59.000000 refuel-autolabel-0.0.7/pyproject.toml
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-07-03 03:33:57.294419 refuel-autolabel-0.0.7/setup.cfg
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.280809 refuel-autolabel-0.0.7/src/
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.284286 refuel-autolabel-0.0.7/src/autolabel/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/__init__.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.285054 refuel-autolabel-0.0.7/src/autolabel/cache/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/cache/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/cache/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/cache/sqlalchemy_cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.7/src/autolabel/confidence.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.286283 refuel-autolabel-0.0.7/src/autolabel/configs/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/configs/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1401 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/configs/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7569 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/configs/config.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4114 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/configs/schema.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.287918 refuel-autolabel-0.0.7/src/autolabel/data_models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/annotation.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/dataset.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/task.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/data_models/task_run.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.288496 refuel-autolabel-0.0.7/src/autolabel/database/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/database/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      643 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/database/engine.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.7/src/autolabel/database/state_manager.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8085 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/dataset_loader.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.289063 refuel-autolabel-0.0.7/src/autolabel/few_shot/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3233 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/few_shot/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/few_shot/fixed_example_selector.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/few_shot/vector_store.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19705 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/labeler.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.291076 refuel-autolabel-0.0.7/src/autolabel/models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2107 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/models/anthropic.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.7/src/autolabel/models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1959 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/models/cohere.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3132 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/models/hf_pipeline.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5682 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/models/openai.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3920 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/models/palm.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3575 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/models/refuel.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4707 2023-07-03 02:09:47.000000 refuel-autolabel-0.0.7/src/autolabel/schema.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.293133 refuel-autolabel-0.0.7/src/autolabel/tasks/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1298 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4319 2023-06-22 05:07:53.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7409 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/classification.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7419 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/entity_matching.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8221 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/multilabel_classification.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12627 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/named_entity_recognition.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7508 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/question_answering.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.7/src/autolabel/tasks/utils.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9773 2023-06-22 21:40:05.000000 refuel-autolabel-0.0.7/src/autolabel/utils.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-07-03 03:33:57.293951 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10384 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1683 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      903 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/requires.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-07-03 03:33:57.000000 refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/top_level.txt
```

### Comparing `refuel-autolabel-0.0.6/LICENSE` & `refuel-autolabel-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/PKG-INFO` & `refuel-autolabel-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.6
+Version: 0.0.7
 Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: openai
 Provides-Extra: anthropic
 Provides-Extra: huggingface
 Provides-Extra: google
+Provides-Extra: cohere
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
 
 <h4 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.6 Summary: Label,
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.7 Summary: Label,
 clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -17,16 +17,16 @@
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/refuel-ai/
 autolabel Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
-Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
-File: LICENSE [Refuel logo]
+Provides-Extra: huggingface Provides-Extra: google Provides-Extra: cohere
+Provides-Extra: all License-File: LICENSE [Refuel logo]
                 *** Discord | Twitter | Website | Benchmark ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
```

### Comparing `refuel-autolabel-0.0.6/README.md` & `refuel-autolabel-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/pyproject.toml` & `refuel-autolabel-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "refuel-autolabel"
-version = "0.0.6"
+version = "0.0.7"
 description = "Label, clean and enrich text datasets with LLMs"
 readme = "README.md"
 authors = [{ name = "Refuel.ai", email = "support@refuel.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -67,26 +67,30 @@
 huggingface = [
     "transformers >= 4.25.0",
     "sentence_transformers"
 ]
 google = [
     "google-cloud-aiplatform>=1.25.0"
 ]
+cohere = [
+    "cohere>=4.11.2"
+]
 all = [
     "black",
     "bumpver",
     "pip-tools",
     "pytest",
     "pytest-mock",
     "pre-commit",
     "openai >= 0.27.4",
     "tiktoken >= 0.3.3",
     "anthropic == 0.2.6",
     "transformers >= 4.25.0",
     "google-cloud-aiplatform>=1.25.0",
+    "cohere>=4.11.2",
     "sentence_transformers"
 ]
 
 [project.urls]
 Homepage = "https://github.com/refuel-ai/autolabel"
 
 [tool.black]
```

### Comparing `refuel-autolabel-0.0.6/src/autolabel/cache/base.py` & `refuel-autolabel-0.0.7/src/autolabel/cache/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/cache/sqlalchemy_cache.py` & `refuel-autolabel-0.0.7/src/autolabel/cache/sqlalchemy_cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/confidence.py` & `refuel-autolabel-0.0.7/src/autolabel/confidence.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/configs/base.py` & `refuel-autolabel-0.0.7/src/autolabel/configs/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/configs/config.py` & `refuel-autolabel-0.0.7/src/autolabel/configs/config.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/configs/schema.py` & `refuel-autolabel-0.0.7/src/autolabel/configs/schema.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/data_models/annotation.py` & `refuel-autolabel-0.0.7/src/autolabel/data_models/annotation.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/data_models/cache.py` & `refuel-autolabel-0.0.7/src/autolabel/data_models/cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/data_models/dataset.py` & `refuel-autolabel-0.0.7/src/autolabel/data_models/dataset.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/data_models/task.py` & `refuel-autolabel-0.0.7/src/autolabel/data_models/task.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/data_models/task_run.py` & `refuel-autolabel-0.0.7/src/autolabel/data_models/task_run.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/database/engine.py` & `refuel-autolabel-0.0.7/src/autolabel/database/engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Optional
+
 from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
-from os.path import join, expanduser
 
 DB_ENGINE = None
 
 # This creates one global ".autolabel.db" in your home directory.
 # Having one global SQLite database in ~ is a poor idea, since
 # SQLite cannot handle multiple simultaneous writes (if you have
 # several different labeling jobs going on).
```

### Comparing `refuel-autolabel-0.0.6/src/autolabel/database/state_manager.py` & `refuel-autolabel-0.0.7/src/autolabel/database/state_manager.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/dataset_loader.py` & `refuel-autolabel-0.0.7/src/autolabel/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/few_shot/__init__.py` & `refuel-autolabel-0.0.7/src/autolabel/few_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/few_shot/fixed_example_selector.py` & `refuel-autolabel-0.0.7/src/autolabel/few_shot/fixed_example_selector.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/few_shot/vector_store.py` & `refuel-autolabel-0.0.7/src/autolabel/few_shot/vector_store.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/labeler.py` & `refuel-autolabel-0.0.7/src/autolabel/labeler.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/models/__init__.py` & `refuel-autolabel-0.0.7/src/autolabel/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,18 @@
                 from .refuel import RefuelLLM
 
                 model_cls = RefuelLLM
             elif model_provider == ModelProvider.GOOGLE:
                 from .palm import PaLMLLM
 
                 model_cls = PaLMLLM
+            elif model_provider == ModelProvider.COHERE:
+                from .cohere import CohereLLM
+
+                model_cls = CohereLLM
             else:
                 raise ValueError
         except ValueError as e:
             logger.error(
                 f"{config.provider()} is not in the list of supported providers: \
                 {list(ModelProvider.__members__.keys())}"
             )
```

### Comparing `refuel-autolabel-0.0.6/src/autolabel/models/anthropic.py` & `refuel-autolabel-0.0.7/src/autolabel/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/models/base.py` & `refuel-autolabel-0.0.7/src/autolabel/models/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/models/hf_pipeline.py` & `refuel-autolabel-0.0.7/src/autolabel/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/models/openai.py` & `refuel-autolabel-0.0.7/src/autolabel/models/openai.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/models/palm.py` & `refuel-autolabel-0.0.7/src/autolabel/models/palm.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/models/refuel.py` & `refuel-autolabel-0.0.7/src/autolabel/models/refuel.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/schema.py` & `refuel-autolabel-0.0.7/src/autolabel/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     """Enum containing all LLM providers currently supported by autolabeler"""
 
     OPENAI = "openai"
     ANTHROPIC = "anthropic"
     HUGGINGFACE_PIPELINE = "huggingface_pipeline"
     REFUEL = "refuel"
     GOOGLE = "google"
+    COHERE = "cohere"
 
 
 class TaskType(str, Enum):
     """Enum containing all the types of tasks that autolabeler currently supports"""
 
     CLASSIFICATION = "classification"
     NAMED_ENTITY_RECOGNITION = "named_entity_recognition"
```

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/__init__.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/base.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/classification.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/entity_matching.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/entity_matching.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/multilabel_classification.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/named_entity_recognition.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/question_answering.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/question_answering.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/tasks/utils.py` & `refuel-autolabel-0.0.7/src/autolabel/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/autolabel/utils.py` & `refuel-autolabel-0.0.7/src/autolabel/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/PKG-INFO` & `refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.6
+Version: 0.0.7
 Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: openai
 Provides-Extra: anthropic
 Provides-Extra: huggingface
 Provides-Extra: google
+Provides-Extra: cohere
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
 
 <h4 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.6 Summary: Label,
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.7 Summary: Label,
 clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -17,16 +17,16 @@
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/refuel-ai/
 autolabel Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
-Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
-File: LICENSE [Refuel logo]
+Provides-Extra: huggingface Provides-Extra: google Provides-Extra: cohere
+Provides-Extra: all License-File: LICENSE [Refuel logo]
                 *** Discord | Twitter | Website | Benchmark ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
```

### Comparing `refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/SOURCES.txt` & `refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/autolabel/database/state_manager.py
 src/autolabel/few_shot/__init__.py
 src/autolabel/few_shot/fixed_example_selector.py
 src/autolabel/few_shot/vector_store.py
 src/autolabel/models/__init__.py
 src/autolabel/models/anthropic.py
 src/autolabel/models/base.py
+src/autolabel/models/cohere.py
 src/autolabel/models/hf_pipeline.py
 src/autolabel/models/openai.py
 src/autolabel/models/palm.py
 src/autolabel/models/refuel.py
 src/autolabel/tasks/__init__.py
 src/autolabel/tasks/base.py
 src/autolabel/tasks/classification.py
```

### Comparing `refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/requires.txt` & `refuel-autolabel-0.0.7/src/refuel_autolabel.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -26,19 +26,23 @@
 pytest-mock
 pre-commit
 openai>=0.27.4
 tiktoken>=0.3.3
 anthropic==0.2.6
 transformers>=4.25.0
 google-cloud-aiplatform>=1.25.0
+cohere>=4.11.2
 sentence_transformers
 
 [anthropic]
 anthropic==0.2.6
 
+[cohere]
+cohere>=4.11.2
+
 [dev]
 black
 bumpver
 mkdocs
 mkdocs-autorefs
 mkdocs-jupyter
 mkdocs-material
```

