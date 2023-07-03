# Comparing `tmp/evolvepy-1.0.0.tar.gz` & `tmp/evolvepy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Github\evolvepy\dist\tmpmupax50n\evolvepy-1.0.0.tar", last modified: Thu Jan 13 18:52:02 2022, max compression
+gzip compressed data, was "D:\Github\evolvepy\dist\.tmp-w_o0q4k8\evolvepy-2.0.0.tar", last modified: Mon Jul  3 00:29:19 2023, max compression
```

## Comparing `evolvepy-1.0.0.tar` & `evolvepy-2.0.0.tar`

### file list

```diff
@@ -1,66 +1,90 @@
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.212771 evolvepy-1.0.0/
--rw-rw-rw-   0        0        0     1102 2022-01-04 20:19:16.000000 evolvepy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4057 2022-01-13 18:52:02.212771 evolvepy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2949 2022-01-13 02:45:43.000000 evolvepy-1.0.0/README.md
--rw-rw-rw-   0        0        0      108 2021-10-17 19:38:36.000000 evolvepy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1361 2022-01-13 18:52:02.213773 evolvepy-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.158772 evolvepy-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.167772 evolvepy-1.0.0/src/evolvepy/
--rw-rw-rw-   0        0        0      115 2022-01-04 00:45:43.000000 evolvepy-1.0.0/src/evolvepy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.190771 evolvepy-1.0.0/src/evolvepy/callbacks/
--rw-rw-rw-   0        0        0      423 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/callbacks/__init__.py
--rw-rw-rw-   0        0        0     3732 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/callbacks/callback.py
--rw-rw-rw-   0        0        0     8750 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/callbacks/dynamic_mutation.py
--rw-rw-rw-   0        0        0     3366 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/callbacks/incremental_evolution.py
--rw-rw-rw-   0        0        0    10585 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/callbacks/logger.py
--rw-rw-rw-   0        0        0     4504 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/configurable.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.195772 evolvepy-1.0.0/src/evolvepy/evaluator/
--rw-rw-rw-   0        0        0      350 2022-01-13 01:39:08.000000 evolvepy-1.0.0/src/evolvepy/evaluator/__init__.py
--rw-rw-rw-   0        0        0     2217 2022-01-13 02:03:15.000000 evolvepy-1.0.0/src/evolvepy/evaluator/aggregator.py
--rw-rw-rw-   0        0        0     3909 2022-01-13 02:07:31.000000 evolvepy-1.0.0/src/evolvepy/evaluator/cache.py
--rw-rw-rw-   0        0        0     3008 2022-01-13 01:47:44.000000 evolvepy-1.0.0/src/evolvepy/evaluator/dispatcher.py
--rw-rw-rw-   0        0        0     3071 2022-01-13 01:43:55.000000 evolvepy-1.0.0/src/evolvepy/evaluator/evaluator.py
--rw-rw-rw-   0        0        0     4276 2022-01-13 02:31:09.000000 evolvepy-1.0.0/src/evolvepy/evaluator/function_evaluator.py
--rw-rw-rw-   0        0        0     6314 2022-01-13 02:26:10.000000 evolvepy-1.0.0/src/evolvepy/evaluator/process_evaluator.py
--rw-rw-rw-   0        0        0     3019 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/evolver.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.200772 evolvepy-1.0.0/src/evolvepy/generator/
--rw-rw-rw-   0        0        0      467 2022-01-13 00:32:37.000000 evolvepy-1.0.0/src/evolvepy/generator/__init__.py
--rw-rw-rw-   0        0        0     6524 2022-01-13 02:27:20.000000 evolvepy-1.0.0/src/evolvepy/generator/basic_layers.py
--rw-rw-rw-   0        0        0     2854 2022-01-13 01:55:17.000000 evolvepy-1.0.0/src/evolvepy/generator/combine.py
--rw-rw-rw-   0        0        0     4116 2022-01-13 02:23:13.000000 evolvepy-1.0.0/src/evolvepy/generator/context.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.202771 evolvepy-1.0.0/src/evolvepy/generator/crossover/
--rw-rw-rw-   0        0        0      174 2022-01-12 21:44:27.000000 evolvepy-1.0.0/src/evolvepy/generator/crossover/__init__.py
--rw-rw-rw-   0        0        0     1665 2022-01-12 21:51:30.000000 evolvepy-1.0.0/src/evolvepy/generator/crossover/crossover.py
--rw-rw-rw-   0        0        0     2742 2022-01-13 18:35:19.000000 evolvepy-1.0.0/src/evolvepy/generator/descriptor.py
--rw-rw-rw-   0        0        0     4484 2022-01-13 18:35:19.000000 evolvepy-1.0.0/src/evolvepy/generator/firstgen.py
--rw-rw-rw-   0        0        0     7080 2022-01-13 18:35:19.000000 evolvepy-1.0.0/src/evolvepy/generator/generator.py
--rw-rw-rw-   0        0        0     7960 2022-01-13 18:35:19.000000 evolvepy-1.0.0/src/evolvepy/generator/layer.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.204772 evolvepy-1.0.0/src/evolvepy/generator/mutation/
--rw-rw-rw-   0        0        0      301 2022-01-12 21:42:25.000000 evolvepy-1.0.0/src/evolvepy/generator/mutation/__init__.py
--rw-rw-rw-   0        0        0     1095 2022-01-12 21:48:55.000000 evolvepy-1.0.0/src/evolvepy/generator/mutation/binary_mutation.py
--rw-rw-rw-   0        0        0     6132 2022-01-12 23:39:34.000000 evolvepy-1.0.0/src/evolvepy/generator/mutation/mutation.py
--rw-rw-rw-   0        0        0     2325 2022-01-12 22:45:05.000000 evolvepy-1.0.0/src/evolvepy/generator/mutation/numeric_mutation.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.205771 evolvepy-1.0.0/src/evolvepy/generator/selection/
--rw-rw-rw-   0        0        0      174 2022-01-12 23:10:28.000000 evolvepy-1.0.0/src/evolvepy/generator/selection/__init__.py
--rw-rw-rw-   0        0        0     2887 2022-01-13 00:09:05.000000 evolvepy-1.0.0/src/evolvepy/generator/selection/selection.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.206771 evolvepy-1.0.0/src/evolvepy/integrations/
--rw-rw-rw-   0        0        0       57 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.207771 evolvepy-1.0.0/src/evolvepy/integrations/gym/
--rw-rw-rw-   0        0        0      116 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/gym/__init__.py
--rw-rw-rw-   0        0        0     3492 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/gym/gym.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.209773 evolvepy-1.0.0/src/evolvepy/integrations/tf_keras/
--rw-rw-rw-   0        0        0      240 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/tf_keras/__init__.py
--rw-rw-rw-   0        0        0    13733 2022-01-12 21:44:28.000000 evolvepy-1.0.0/src/evolvepy/integrations/tf_keras/tf_keras.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.210773 evolvepy-1.0.0/src/evolvepy/integrations/unity_gym/
--rw-rw-rw-   0        0        0      149 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/unity_gym/__init__.py
--rw-rw-rw-   0        0        0     1268 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/unity_gym/unity.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.211773 evolvepy-1.0.0/src/evolvepy/integrations/wandb/
--rw-rw-rw-   0        0        0      107 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/wandb/__init__.py
--rw-rw-rw-   0        0        0     4038 2022-01-12 21:08:07.000000 evolvepy-1.0.0/src/evolvepy/integrations/wandb/wandb.py
-drwxrwxrwx   0        0        0        0 2022-01-13 18:52:02.187773 evolvepy-1.0.0/src/evolvepy.egg-info/
--rw-rw-rw-   0        0        0        1 2021-12-21 18:43:41.000000 evolvepy-1.0.0/src/evolvepy.egg-info/.gitignore
--rw-rw-rw-   0        0        0     4057 2022-01-13 18:52:02.000000 evolvepy-1.0.0/src/evolvepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1836 2022-01-13 18:52:02.000000 evolvepy-1.0.0/src/evolvepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-13 18:52:02.000000 evolvepy-1.0.0/src/evolvepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2022-01-13 18:52:02.000000 evolvepy-1.0.0/src/evolvepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-01-13 18:52:02.000000 evolvepy-1.0.0/src/evolvepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.617926 evolvepy-2.0.0/
+-rw-rw-rw-   0        0        0     1102 2022-01-04 20:19:16.000000 evolvepy-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4406 2023-07-03 00:29:19.617926 evolvepy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3298 2022-01-13 20:37:44.000000 evolvepy-2.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-17 19:38:36.000000 evolvepy-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1404 2023-07-03 00:29:19.624019 evolvepy-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.552782 evolvepy-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.561782 evolvepy-2.0.0/src/evolvepy/
+-rw-rw-rw-   0        0        0      115 2022-01-04 00:45:43.000000 evolvepy-2.0.0/src/evolvepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.582899 evolvepy-2.0.0/src/evolvepy/callbacks/
+-rw-rw-rw-   0        0        0      423 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     5583 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/callbacks/callback.py
+-rw-rw-rw-   0        0        0     8750 2023-06-27 21:09:01.000000 evolvepy-2.0.0/src/evolvepy/callbacks/dynamic_mutation.py
+-rw-rw-rw-   0        0        0     3366 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/callbacks/incremental_evolution.py
+-rw-rw-rw-   0        0        0    10585 2023-06-27 21:08:46.000000 evolvepy-2.0.0/src/evolvepy/callbacks/logger.py
+-rw-rw-rw-   0        0        0     4504 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/configurable.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.586578 evolvepy-2.0.0/src/evolvepy/evaluator/
+-rw-rw-rw-   0        0        0      348 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/evaluator/__init__.py
+-rw-rw-rw-   0        0        0     2213 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/evaluator/aggregator.py
+-rw-rw-rw-   0        0        0     4747 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/evaluator/cache.py
+-rw-rw-rw-   0        0        0     3159 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/evaluator/evaluator.py
+-rw-rw-rw-   0        0        0     4843 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/evaluator/function_evaluator.py
+-rw-rw-rw-   0        0        0     3583 2023-07-02 22:16:18.000000 evolvepy-2.0.0/src/evolvepy/evaluator/multiple.py
+-rw-rw-rw-   0        0        0     6797 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/evaluator/process_evaluator.py
+-rw-rw-rw-   0        0        0     4944 2023-07-02 22:18:16.000000 evolvepy-2.0.0/src/evolvepy/evolver.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.592789 evolvepy-2.0.0/src/evolvepy/generator/
+-rw-rw-rw-   0        0        0      467 2022-01-13 00:32:37.000000 evolvepy-2.0.0/src/evolvepy/generator/__init__.py
+-rw-rw-rw-   0        0        0     6525 2023-07-02 23:33:03.000000 evolvepy-2.0.0/src/evolvepy/generator/basic_layers.py
+-rw-rw-rw-   0        0        0     2864 2023-07-02 23:33:03.000000 evolvepy-2.0.0/src/evolvepy/generator/combine.py
+-rw-rw-rw-   0        0        0     4295 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/generator/context.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.593706 evolvepy-2.0.0/src/evolvepy/generator/crossover/
+-rw-rw-rw-   0        0        0      174 2022-01-12 21:44:27.000000 evolvepy-2.0.0/src/evolvepy/generator/crossover/__init__.py
+-rw-rw-rw-   0        0        0     1902 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/generator/crossover/crossover.py
+-rw-rw-rw-   0        0        0     2742 2022-01-13 18:35:19.000000 evolvepy-2.0.0/src/evolvepy/generator/descriptor.py
+-rw-rw-rw-   0        0        0     4489 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/generator/firstgen.py
+-rw-rw-rw-   0        0        0     7166 2023-07-02 23:33:03.000000 evolvepy-2.0.0/src/evolvepy/generator/generator.py
+-rw-rw-rw-   0        0        0     8577 2023-07-02 23:33:03.000000 evolvepy-2.0.0/src/evolvepy/generator/layer.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.596696 evolvepy-2.0.0/src/evolvepy/generator/mutation/
+-rw-rw-rw-   0        0        0      301 2022-01-12 21:42:25.000000 evolvepy-2.0.0/src/evolvepy/generator/mutation/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/generator/mutation/binary_mutation.py
+-rw-rw-rw-   0        0        0     6152 2023-07-02 23:33:03.000000 evolvepy-2.0.0/src/evolvepy/generator/mutation/mutation.py
+-rw-rw-rw-   0        0        0     2496 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/generator/mutation/numeric_mutation.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.597696 evolvepy-2.0.0/src/evolvepy/generator/selection/
+-rw-rw-rw-   0        0        0      174 2022-01-12 23:10:28.000000 evolvepy-2.0.0/src/evolvepy/generator/selection/__init__.py
+-rw-rw-rw-   0        0        0     3128 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/generator/selection/selection.py
+-rw-rw-rw-   0        0        0     3612 2023-07-02 23:33:03.000000 evolvepy-2.0.0/src/evolvepy/generator/thread_pool.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.598696 evolvepy-2.0.0/src/evolvepy/integrations/
+-rw-rw-rw-   0        0        0       57 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.599697 evolvepy-2.0.0/src/evolvepy/integrations/gym/
+-rw-rw-rw-   0        0        0      116 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/gym/__init__.py
+-rw-rw-rw-   0        0        0     3492 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/gym/gym.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.602697 evolvepy-2.0.0/src/evolvepy/integrations/nvtx/
+-rw-rw-rw-   0        0        0      149 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/integrations/nvtx/__init__.py
+-rw-rw-rw-   0        0        0      569 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/integrations/nvtx/annotate_se.py
+-rw-rw-rw-   0        0        0      111 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/integrations/nvtx/colors.py
+-rw-rw-rw-   0        0        0      430 2023-07-02 16:47:25.000000 evolvepy-2.0.0/src/evolvepy/integrations/nvtx/mock.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.603697 evolvepy-2.0.0/src/evolvepy/integrations/ray/
+-rw-rw-rw-   0        0        0      129 2023-07-02 23:25:00.000000 evolvepy-2.0.0/src/evolvepy/integrations/ray/__init__.py
+-rw-rw-rw-   0        0        0     4031 2023-07-02 23:25:00.000000 evolvepy-2.0.0/src/evolvepy/integrations/ray/distributed_evaluator.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.604697 evolvepy-2.0.0/src/evolvepy/integrations/tf_keras/
+-rw-rw-rw-   0        0        0      240 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/tf_keras/__init__.py
+-rw-rw-rw-   0        0        0    13733 2023-06-12 20:02:31.000000 evolvepy-2.0.0/src/evolvepy/integrations/tf_keras/tf_keras.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.605697 evolvepy-2.0.0/src/evolvepy/integrations/unity_gym/
+-rw-rw-rw-   0        0        0      149 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/unity_gym/__init__.py
+-rw-rw-rw-   0        0        0     1268 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/unity_gym/unity.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.606695 evolvepy-2.0.0/src/evolvepy/integrations/wandb/
+-rw-rw-rw-   0        0        0      107 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/wandb/__init__.py
+-rw-rw-rw-   0        0        0     4038 2022-01-12 21:08:07.000000 evolvepy-2.0.0/src/evolvepy/integrations/wandb/wandb.py
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.578899 evolvepy-2.0.0/src/evolvepy.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-12-21 18:43:41.000000 evolvepy-2.0.0/src/evolvepy.egg-info/.gitignore
+-rw-rw-rw-   0        0        0     4406 2023-07-03 00:29:19.000000 evolvepy-2.0.0/src/evolvepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2502 2023-07-03 00:29:19.000000 evolvepy-2.0.0/src/evolvepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 00:29:19.000000 evolvepy-2.0.0/src/evolvepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      243 2023-07-03 00:29:19.000000 evolvepy-2.0.0/src/evolvepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 00:29:19.000000 evolvepy-2.0.0/src/evolvepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 00:29:19.616927 evolvepy-2.0.0/tests/
+-rw-rw-rw-   0        0        0     1844 2022-01-12 21:44:28.000000 evolvepy-2.0.0/tests/test_combine_layer.py
+-rw-rw-rw-   0        0        0     1155 2022-01-04 00:45:43.000000 evolvepy-2.0.0/tests/test_configurable.py
+-rw-rw-rw-   0        0        0     2029 2022-01-12 21:44:28.000000 evolvepy-2.0.0/tests/test_context.py
+-rw-rw-rw-   0        0        0      745 2022-01-12 21:44:28.000000 evolvepy-2.0.0/tests/test_crossover.py
+-rw-rw-rw-   0        0        0     3323 2022-01-04 00:45:43.000000 evolvepy-2.0.0/tests/test_dynamic_mutation.py
+-rw-rw-rw-   0        0        0     4885 2022-01-05 15:19:42.000000 evolvepy-2.0.0/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0     4639 2022-01-12 21:44:28.000000 evolvepy-2.0.0/tests/test_generator.py
+-rw-rw-rw-   0        0        0     2052 2022-01-12 21:44:28.000000 evolvepy-2.0.0/tests/test_incremental_evolution.py
+-rw-rw-rw-   0        0        0     3640 2023-07-02 23:33:03.000000 evolvepy-2.0.0/tests/test_layer.py
+-rw-rw-rw-   0        0        0     1638 2022-01-04 00:45:43.000000 evolvepy-2.0.0/tests/test_logger.py
+-rw-rw-rw-   0        0        0     1142 2022-01-12 21:44:28.000000 evolvepy-2.0.0/tests/test_mutation.py
+-rw-rw-rw-   0        0        0     1992 2022-01-12 21:44:28.000000 evolvepy-2.0.0/tests/test_mutation_layer.py
+-rw-rw-rw-   0        0        0      701 2022-01-13 18:43:50.000000 evolvepy-2.0.0/tests/test_random_predation.py
+-rw-rw-rw-   0        0        0     1096 2022-01-12 13:55:20.000000 evolvepy-2.0.0/tests/test_selection.py
```

### Comparing `evolvepy-1.0.0/LICENSE` & `evolvepy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/PKG-INFO` & `evolvepy-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 Metadata-Version: 2.1
 Name: evolvepy
-Version: 1.0.0
+Version: 2.0.0
 Summary: EvolvePy is a Python module created to allow the easy creation and execution of evolutionary algorithms.
 Home-page: https://github.com/EltonCN/evolvepy
 Author: EltonCN, João Bonucci, Thiago Lacerda
 Author-email: elton.nascimento@students.ic.unicamp.br, j218733@dac.unicamp.br, t244712@dac.unicamp.br
 License: MIT
 Project-URL: Bug Tracker, https://github.com/EltonCN/evolvepy/issues
 Project-URL: Documentation, https://eltoncn.github.io/evolvepy
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: unity
 Provides-Extra: wandb
 Provides-Extra: gym
+Provides-Extra: ray
 Provides-Extra: tensorflow
 Provides-Extra: all_integrations
 Provides-Extra: doc_generation
 License-File: LICENSE
 
-[![](https://img.shields.io/pypi/v/evolvepy?style=for-the-badge)]() [![](https://img.shields.io/github/license/EltonCN/evolvepy?style=for-the-badge)](https://github.com/EltonCN/evolvepy/blob/main/LICENSE)
+[![](https://img.shields.io/pypi/v/evolvepy?style=for-the-badge)](https://pypi.org/project/evolvepy) [![](https://img.shields.io/pypi/l/evolvepy?style=for-the-badge)](https://github.com/EltonCN/evolvepy/blob/main/LICENSE) [![](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EltonCN/evolvepy)
 
 # EvolvePy
 
 EvolvePy is a Python module created to allow the easy creation and execution of evolutionary algorithms.
 
 **Documentation**: [EvolvePy's documentation](https://eltoncn.github.io/evolvepy/_build/html/index.html).
 
+Presentation video (Portuguese, click on the image):
+[![Presentation Video](/Thumbnail.png)](https://www.youtube.com/watch?v=Hfo1XkzEcis&list=PLXcCIm-yDGGfBveHj_f_31GkythkJpeUl&index=1)
+
 ## Features
 
-(Links to example using feature)
+(Links to example using the feature)
 
 - Allows to create complex individual generators using different strategies:
-  - [Crossover](/examples/1%20-%20Simple%20EA.ipynb) (one-point, n-point, mean)
-  - Mutation ([sum](/examples/1%20-%20Simple%20EA.ipynb), multiplication, binary)
-  - Dynamic mutation
-  - [Elitism](/examples/2%20-%20Elitism.ipynb)
-  - [Randomic predation](/examples/6%20-%20Random%20Predation.ipynb)
-  - [Incremental evolution](/examples/5%20-%20Incremental%20Evolution.ipynb)
+  - [Crossover](/examples/Simple%20EA.ipynb) (one-point, n-point, mean)
+  - Mutation ([sum](/examples/Simple%20EA.ipynb), multiplication, [binary](/examples/3-CNF-SAT.ipynb))
+  - [Dynamic mutation](/examples/Dynamic%20Mutation.ipynb)
+  - [Elitism](/examples/Elitism.ipynb)
+  - [Randomic predation](/examples/Random%20Predation.ipynb)
+  - [Incremental evolution](/examples/Incremental%20Evolution.ipynb)
 - Define individuals with different chromosomes, with different types, ranges, sizes and parameters in the generator.
-- Evaluate individuals using [simple functions](/examples/1%20-%20Simple%20EA.ipynb)  or [multiple processes](/examples/Car%20PID%20Control.ipynb).
+- Evaluate individuals using [simple functions](/examples/Simple%20EA.ipynb)  or [multiple processes](/examples/Car%20PID%20Control.ipynb).
   - [Fitness cache](/examples/Car%20PID%20Control.ipynb) to avoid evaluate the same individual several times.
   - Fitness functions with different scores, which can be aggregated with different strategies.
   - [Evaluate the same individual several times to avoid noise](/examples/Car%20PID%20Control.ipynb).
-- [Log the evolution data to analyze later](/examples/4%20-%20Logger.ipynb).
+- [Log the evolution data to analyze later](/examples/Logger.ipynb).
 - Integrations with other modules:
-  - [Wandb](/examples/4%20-%20Logger.ipynb)
+  - [Wandb](/examples/Logger.ipynb)
   - [Tensorflow/Keras](/examples/TF-Keras%20Integration.ipynb)
   - [Gym](/examples/Reinforcement%20Learning.ipynb)
   - [Unity ML Agents](/examples/Unity%20ML%20Agents%20-%203DBall.ipynb) (using Gym)
 
 ## Installation
 
 - EvolvePy can be installed using pip:
@@ -89,8 +92,7 @@
 ## Authors
 
 Created by students from Unicamp's Institute of Computing (IC-Unicamp) as a project for the [evolutionary systems subject](https://gitlab.com/simoesusp/disciplinas/tree/master/SSC0713-Sistemas-Evolutivos-Aplicados-a-Robotica) at ICMC-USP, taught by prof. Eduardo do Valle Simoes.
 
 - [EltonCN](https://github.com/EltonCN)
 - [João Bonucci](https://github.com/Joao-Pedro-MB)
 - [Thiago Lacerda](https://github.com/ThiagoDSL)
-
```

### Comparing `evolvepy-1.0.0/README.md` & `evolvepy-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-[![](https://img.shields.io/pypi/v/evolvepy?style=for-the-badge)]() [![](https://img.shields.io/github/license/EltonCN/evolvepy?style=for-the-badge)](https://github.com/EltonCN/evolvepy/blob/main/LICENSE)
+[![](https://img.shields.io/pypi/v/evolvepy?style=for-the-badge)](https://pypi.org/project/evolvepy) [![](https://img.shields.io/pypi/l/evolvepy?style=for-the-badge)](https://github.com/EltonCN/evolvepy/blob/main/LICENSE) [![](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EltonCN/evolvepy)
 
 # EvolvePy
 
 EvolvePy is a Python module created to allow the easy creation and execution of evolutionary algorithms.
 
 **Documentation**: [EvolvePy's documentation](https://eltoncn.github.io/evolvepy/_build/html/index.html).
 
+Presentation video (Portuguese, click on the image):
+[![Presentation Video](/Thumbnail.png)](https://www.youtube.com/watch?v=Hfo1XkzEcis&list=PLXcCIm-yDGGfBveHj_f_31GkythkJpeUl&index=1)
+
 ## Features
 
-(Links to example using feature)
+(Links to example using the feature)
 
 - Allows to create complex individual generators using different strategies:
-  - [Crossover](/examples/1%20-%20Simple%20EA.ipynb) (one-point, n-point, mean)
-  - Mutation ([sum](/examples/1%20-%20Simple%20EA.ipynb), multiplication, binary)
-  - Dynamic mutation
-  - [Elitism](/examples/2%20-%20Elitism.ipynb)
-  - [Randomic predation](/examples/6%20-%20Random%20Predation.ipynb)
-  - [Incremental evolution](/examples/5%20-%20Incremental%20Evolution.ipynb)
+  - [Crossover](/examples/Simple%20EA.ipynb) (one-point, n-point, mean)
+  - Mutation ([sum](/examples/Simple%20EA.ipynb), multiplication, [binary](/examples/3-CNF-SAT.ipynb))
+  - [Dynamic mutation](/examples/Dynamic%20Mutation.ipynb)
+  - [Elitism](/examples/Elitism.ipynb)
+  - [Randomic predation](/examples/Random%20Predation.ipynb)
+  - [Incremental evolution](/examples/Incremental%20Evolution.ipynb)
 - Define individuals with different chromosomes, with different types, ranges, sizes and parameters in the generator.
-- Evaluate individuals using [simple functions](/examples/1%20-%20Simple%20EA.ipynb)  or [multiple processes](/examples/Car%20PID%20Control.ipynb).
+- Evaluate individuals using [simple functions](/examples/Simple%20EA.ipynb)  or [multiple processes](/examples/Car%20PID%20Control.ipynb).
   - [Fitness cache](/examples/Car%20PID%20Control.ipynb) to avoid evaluate the same individual several times.
   - Fitness functions with different scores, which can be aggregated with different strategies.
   - [Evaluate the same individual several times to avoid noise](/examples/Car%20PID%20Control.ipynb).
-- [Log the evolution data to analyze later](/examples/4%20-%20Logger.ipynb).
+- [Log the evolution data to analyze later](/examples/Logger.ipynb).
 - Integrations with other modules:
-  - [Wandb](/examples/4%20-%20Logger.ipynb)
+  - [Wandb](/examples/Logger.ipynb)
   - [Tensorflow/Keras](/examples/TF-Keras%20Integration.ipynb)
   - [Gym](/examples/Reinforcement%20Learning.ipynb)
   - [Unity ML Agents](/examples/Unity%20ML%20Agents%20-%203DBall.ipynb) (using Gym)
 
 ## Installation
 
 - EvolvePy can be installed using pip:
```

### Comparing `evolvepy-1.0.0/setup.cfg` & `evolvepy-2.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 766f 6c76 6570 790d 0a76 6572   = evolvepy..ver
-00000020: 7369 6f6e 203d 2031 2e30 2e30 0d0a 6175  sion = 1.0.0..au
+00000020: 7369 6f6e 203d 2032 2e30 2e30 0d0a 6175  sion = 2.0.0..au
 00000030: 7468 6f72 203d 2045 6c74 6f6e 434e 2c20  thor = EltonCN, 
 00000040: 4a6f c3a3 6f20 426f 6e75 6363 692c 2054  Jo..o Bonucci, T
 00000050: 6869 6167 6f20 4c61 6365 7264 610d 0a61  hiago Lacerda..a
 00000060: 7574 686f 725f 656d 6169 6c20 3d20 656c  uthor_email = el
 00000070: 746f 6e2e 6e61 7363 696d 656e 746f 4073  ton.nascimento@s
 00000080: 7475 6465 6e74 732e 6963 2e75 6e69 6361  tudents.ic.unica
 00000090: 6d70 2e62 722c 206a 3231 3837 3333 4064  mp.br, j218733@d
@@ -57,30 +57,32 @@
 00000380: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
 00000390: 7461 203d 2054 7275 650d 0a70 6163 6b61  ta = True..packa
 000003a0: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
 000003b0: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
 000003c0: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
 000003d0: 6972 6573 203d 203e 3d33 2e37 0d0a 696e  ires = >=3.7..in
 000003e0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000003f0: 200d 0a09 6e75 6d70 7920 3d3d 2031 2e32   ...numpy == 1.2
+000003f0: 200d 0a09 6e75 6d70 7920 3e3d 2031 2e32   ...numpy >= 1.2
 00000400: 300d 0a09 6e75 6d62 610d 0a0d 0a5b 6f70  0...numba....[op
 00000410: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
 00000420: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
 00000430: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  c....[options.ex
 00000440: 7472 6173 5f72 6571 7569 7265 5d0d 0a75  tras_require]..u
 00000450: 6e69 7479 203d 206d 6c61 6765 6e74 733e  nity = mlagents>
 00000460: 3d30 2e32 372e 303b 2067 796d 5f75 6e69  =0.27.0; gym_uni
 00000470: 7479 3b20 6779 6d0d 0a77 616e 6462 203d  ty; gym..wandb =
 00000480: 2077 616e 6462 0d0a 6779 6d20 3d20 6779   wandb..gym = gy
-00000490: 6d0d 0a74 656e 736f 7266 6c6f 7720 3d20  m..tensorflow = 
-000004a0: 7465 6e73 6f72 666c 6f77 0d0a 616c 6c5f  tensorflow..all_
-000004b0: 696e 7465 6772 6174 696f 6e73 203d 206d  integrations = m
-000004c0: 6c61 6765 6e74 733e 3d30 2e32 372e 303b  lagents>=0.27.0;
-000004d0: 2067 796d 5f75 6e69 7479 3b20 6779 6d3b   gym_unity; gym;
-000004e0: 2077 616e 6462 3b20 7465 6e73 6f72 666c   wandb; tensorfl
-000004f0: 6f77 0d0a 646f 635f 6765 6e65 7261 7469  ow..doc_generati
-00000500: 6f6e 203d 2073 7068 696e 783b 206d 3272  on = sphinx; m2r
-00000510: 323b 2073 7068 696e 785f 7274 645f 7468  2; sphinx_rtd_th
-00000520: 656d 650d 0a0d 0a5b 6567 675f 696e 666f  eme....[egg_info
-00000530: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000540: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000550: 0a                                       .
+00000490: 6d3c 3d30 2e32 312e 300d 0a72 6179 203d  m<=0.21.0..ray =
+000004a0: 2072 6179 2023 2064 6973 7472 6962 7574   ray # distribut
+000004b0: 6564 2065 7661 6c75 6174 6f72 0d0a 7465  ed evaluator..te
+000004c0: 6e73 6f72 666c 6f77 203d 2074 656e 736f  nsorflow = tenso
+000004d0: 7266 6c6f 770d 0a61 6c6c 5f69 6e74 6567  rflow..all_integ
+000004e0: 7261 7469 6f6e 7320 3d20 6d6c 6167 656e  rations = mlagen
+000004f0: 7473 3e3d 302e 3237 2e30 3b20 6779 6d5f  ts>=0.27.0; gym_
+00000500: 756e 6974 793b 2067 796d 3b20 7761 6e64  unity; gym; wand
+00000510: 623b 2074 656e 736f 7266 6c6f 770d 0a64  b; tensorflow..d
+00000520: 6f63 5f67 656e 6572 6174 696f 6e20 3d20  oc_generation = 
+00000530: 7370 6869 6e78 3b20 6d32 7232 3b20 7370  sphinx; m2r2; sp
+00000540: 6869 6e78 5f72 7464 5f74 6865 6d65 0d0a  hinx_rtd_theme..
+00000550: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000560: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000570: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `evolvepy-1.0.0/src/evolvepy/callbacks/callback.py` & `evolvepy-2.0.0/src/evolvepy/callbacks/callback.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import Dict, List
 import numpy as np
 from evolvepy.configurable import Configurable
 
 from evolvepy.generator import Generator
 from evolvepy.evaluator import Evaluator
+from evolvepy.integrations import nvtx
 
 class Callback(Configurable):
     '''
     Base Callback class.
 
     Callbacks are objects that can be called upon during evolution to change its behavior.
     '''
@@ -85,15 +86,65 @@
         
         for callback in value:
             if not isinstance(callback, Callback):
                 raise ValueError("All callbacks elements must be a evolvepy Callback instance.")
         
         self._callbacks = value
 
+    #To call in Evolver
+
+    def _on_start(self) -> None:
+        '''
+        Called when evolution start.
+        '''
+        range_name = "{0}_start".format(self.name)
+        with nvtx.annotate_se(range_name, domain="evolvepy", category="callback", color=nvtx.callback_color):
+            self.on_start()
+
+    def _on_generator_start(self) -> None:
+        '''
+        Called before generator run.
+        '''
+        range_name = "{0}_generator_start".format(self.name)
+        with nvtx.annotate_se(range_name, domain="evolvepy", category="callback", color=nvtx.callback_color):
+            self.on_generator_start()
         
+
+    def _on_generator_end(self, population:np.ndarray) -> None:
+        '''
+        Called after generator run, before evaluator.
+
+        Args:
+            population (np.ndarray): The generated population.
+        '''
+        range_name = "{0}_generator_end".format(self.name)
+        with nvtx.annotate_se(range_name, domain="evolvepy", category="callback", color=nvtx.callback_color):
+            self.on_generator_end(population)
+
+    def _on_evaluator_end(self, fitness:np.ndarray) -> None:
+        '''
+        Called after evaluator run.
+
+        Args:
+            fitness (np.ndarray): The population fitness.
+        '''
+        range_name = "{0}_evaluator_end".format(self.name)
+        with nvtx.annotate_se(range_name, domain="evolvepy", category="callback", color=nvtx.callback_color):
+            self.on_evaluator_end(fitness)
+
+    def _on_stop(self) -> None:
+        '''
+        Called on evolution end.
+        '''
+        range_name = "{0}_stop".format(self.name)
+        with nvtx.annotate_se(range_name, domain="evolvepy", category="callback", color=nvtx.callback_color):
+            self.on_stop()
+
+
+    #To override
     def on_start(self) -> None:
         '''
         Called when evolution start.
         '''
         pass
 
     def on_generator_start(self) -> None:
```

### Comparing `evolvepy-1.0.0/src/evolvepy/callbacks/dynamic_mutation.py` & `evolvepy-2.0.0/src/evolvepy/callbacks/dynamic_mutation.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/callbacks/incremental_evolution.py` & `evolvepy-2.0.0/src/evolvepy/callbacks/incremental_evolution.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/callbacks/logger.py` & `evolvepy-2.0.0/src/evolvepy/callbacks/logger.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/configurable.py` & `evolvepy-2.0.0/src/evolvepy/configurable.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/evaluator/aggregator.py` & `evolvepy-2.0.0/src/evolvepy/evaluator/aggregator.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         dynamic_parameters = {"weights":True}
 
         super().__init__(evaluator, parameters=parameters, dynamic_parameters=dynamic_parameters)
         
         self._mode = mode
         self._n_scores = 1
 
-    def __call__(self, population:np.ndarray) -> np.ndarray:
+    def call(self, population:np.ndarray) -> np.ndarray:
         '''
         Evaluates a population aggregating the scores.
 
         Args:
             population (np.ndarray): Population to be evaluated.
 
         Returns:
```

### Comparing `evolvepy-1.0.0/src/evolvepy/evaluator/evaluator.py` & `evolvepy-2.0.0/src/evolvepy/evaluator/evaluator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Union
 
 import numpy as np
 
 from evolvepy.configurable import Configurable
+from evolvepy.integrations import nvtx
 
 class Evaluator(Configurable, ABC):
     '''
     Base evaluator class.
 
     Must be inherited to be used.
     '''
     
-    def __init__(self, n_scores:int=1, individual_per_call:int = 1, other_parameters:Dict[str,object]=None, dynamic_parameters:Dict[str,bool]=None) -> None:
+    def __init__(self, n_scores:int=1, individual_per_call:int = 1, other_parameters:Dict[str,object]=None, dynamic_parameters:Dict[str,bool]=None, name:str=None) -> None:
         '''
         Evalutor constructor.
 
         Args:
             n_scores (int, optional): Number of scores generated when evaluating an individual. Defaults to 1.
             individual_per_call (int, optional): Number of individuals that are evaluated at each call. Defaults to 1.
             other_parameters (Dict[str,object], optional): Other parameters defined by the inheritor class. Defaults to None.
@@ -25,39 +26,45 @@
         
         if other_parameters is None:
             other_parameters={}
         
         other_parameters["n_scores"] = n_scores
         other_parameters["individual_per_call"] = individual_per_call
 
-        super().__init__(other_parameters, dynamic_parameters)
+        super().__init__(other_parameters, dynamic_parameters, name=name)
 
         self._individual_per_call = individual_per_call
         self._n_scores = n_scores
         self._scores : np.ndarray = None
 
-    @abstractmethod
     def __call__(self, population:np.ndarray) -> np.ndarray:
         '''
         Evaluates the population.
 
         Args:
             population (np.ndarray): Population to be evaluated.
 
         Returns:
             np.ndarray: Population fitness
         '''
-        ...
+        with nvtx.annotate_se(self.name, domain="evolvepy", category="evaluator", color=nvtx.evaluator_color):
+            fitness = self.call(population)
+
+        return fitness
 
     @property
     def scores(self) -> np.ndarray:
         '''
         Scores of the last evaluated individuals.
         '''
         return self._scores
+    
+    @abstractmethod
+    def call(self, population:np.ndarray) -> np.ndarray:
+        ...
 
 class EvaluationStage(Evaluator):
     '''
     An evaluation stage. Allows you to modify the behavior of an evaluator.
 
     Can be chained with other stages.
     '''
@@ -69,20 +76,12 @@
         Args:
             evaluator (Evaluator): Evaluator that will be modified.
             parameters (Dict[str, object], optional): Evaluator parameters. Defaults to None.
             dynamic_parameters (Dict[str, bool], optional): Evaluator dynamic parameters description. Defaults to None.
         '''
         super().__init__(evaluator._n_scores, evaluator._individual_per_call, other_parameters=parameters, dynamic_parameters=dynamic_parameters)
         self._evaluator = evaluator
-    
 
-    def __call__(self, population:np.ndarray) -> np.ndarray:
-        '''
-        Evaluates the population using the evaluator.
-
-        Args:
-            population (np.ndarray): Population to be evaluated.
-
-        Returns:
-            np.ndarray: Population fitness.
-        '''
-        return self._evaluator(population)
+        
+    
+    def call(self, population:np.ndarray) -> np.ndarray:
+        return self._evaluator(population)
```

### Comparing `evolvepy-1.0.0/src/evolvepy/evaluator/function_evaluator.py` & `evolvepy-2.0.0/src/evolvepy/evaluator/function_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,32 +4,26 @@
 from numba.np.ufunc import parallel
 from .evaluator import Evaluator
 
 import numpy as np
 from numpy.typing import ArrayLike
 import numba
 
-PYTHON = 0
-JIT = 1
-NJIT = 2
-JIT_PARALLEL = 3
-NJIT_PARALLEL = 3
-
 class FunctionEvaluator(Evaluator):
     '''
     Evaluates individuals using a simple function.
     '''
 
     PYTHON = 0
     JIT = 1
     NJIT = 2
     JIT_PARALLEL = 3
     NJIT_PARALLEL = 4
 
-    def __init__(self, function:Callable[[np.ndarray], ArrayLike], n_scores:int=1, mode:int=NJIT, individual_per_call:int = 1) -> None:
+    def __init__(self, function:Callable[[np.ndarray], ArrayLike], n_scores:int=1, mode:int=NJIT, individual_per_call:int = 1, name:str=None, n_thread:int=None) -> None:
         '''
         FunctionEvaluator constructor.
 
         Args:
             function (Callable[[np.ndarray], ArrayLike]): Function that will be used to evaluate individuals.
             n_scores (int, optional): Number of scores generated for each individual. Defaults to 1.
             mode (int, optional): In which compilation mode to use the fitness function. Defaults to FunctionEvaluator.NJIT.
@@ -37,49 +31,63 @@
                                 PYTHON: No JIT compilation
                                 JIT: With Numba JIT compilation
                                 NJIT: With Numba No Python mode.
                                 JIT_PARALLEL: With JIT and parallel assessments.
                                 NJIT_PARALLEL: With NJIT and parallel assessments.
             individual_per_call (int, optional): Number of individuals that are evaluated at each function call. Defaults to 1.
         '''
-        super().__init__(n_scores, individual_per_call, other_parameters={"evaluation_function_name":function.__name__})
+        other_parameters = {"evaluation_function_name":function.__name__, "mode":mode}
+        if mode == FunctionEvaluator.JIT_PARALLEL or mode == FunctionEvaluator.NJIT_PARALLEL:
+            other_parameters["n_thread"] = n_thread
+
+        super().__init__(n_scores, individual_per_call, other_parameters, name=name)
 
-        if mode == JIT:
+        if mode == FunctionEvaluator.JIT:
             self._function = numba.jit()(function)
-            self._static_call = numba.jit()(FunctionEvaluator.call)
-        elif mode == NJIT:
+            self._static_call = numba.jit()(FunctionEvaluator.static_call)
+        elif mode == FunctionEvaluator.NJIT:
             self._function = numba.njit()(function)
-            self._static_call = numba.njit()(FunctionEvaluator.call)
-        elif mode == JIT_PARALLEL:
+            self._static_call = numba.njit()(FunctionEvaluator.static_call)
+        elif mode == FunctionEvaluator.JIT_PARALLEL:
             self._function = numba.jit(parallel=True)(function)
-            self._static_call = numba.jit(parallel=True)(FunctionEvaluator.call)
-        elif mode == NJIT_PARALLEL:
+            self._static_call = numba.jit(parallel=True)(FunctionEvaluator.static_call)
+        elif mode == FunctionEvaluator.NJIT_PARALLEL:
             self._function = numba.njit(parallel=True)(function)
-            self._static_call = numba.njit(parallel=True)(FunctionEvaluator.call)
+            self._static_call = numba.njit(parallel=True)(FunctionEvaluator.static_call)
         else:
             self._function = function
-            self._static_call = FunctionEvaluator.call
+            self._static_call = FunctionEvaluator.static_call
 
         self._mode = mode
+        self._n_thread = n_thread
+        
 
-    def __call__(self, population: np.ndarray) -> np.ndarray:
+    def call(self, population: np.ndarray) -> np.ndarray:
         '''
         Evaluates a population using the fitness function.
 
         Args:
             population (np.ndarray): Population to be evaluated.
 
         Returns:
             np.ndarray: Population fitness.
         '''
+        if self._n_thread is not None:
+            orig_num_threads = numba.get_num_threads()
+            numba.set_num_threads(self._n_thread)
+
         self._scores  = self._static_call(self._function, self._individual_per_call, self._n_scores, population)
+
+        if self._n_thread is not None:
+            numba.set_num_threads(orig_num_threads)
+
         return self._scores
 
     @staticmethod
-    def call(function:Callable, individual_per_call:int, n_scores:int, population:np.ndarray) -> np.ndarray:
+    def static_call(function:Callable, individual_per_call:int, n_scores:int, population:np.ndarray) -> np.ndarray:
         '''
         Call the fitness function in the desired mode.
 
         Static method to enable just-in-time compilation using Numba.
 
         Args:
             function (Callable): Function that will be used to evaluate individuals.
```

### Comparing `evolvepy-1.0.0/src/evolvepy/evaluator/process_evaluator.py` & `evolvepy-2.0.0/src/evolvepy/evaluator/process_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, Type
 import multiprocessing as mp
 from abc import ABC, abstractmethod
 
 import numpy as np
 
 from .evaluator import Evaluator
+from evolvepy.integrations import nvtx
 
 class ProcessFitnessFunction(ABC):
     '''
     Base class of fitness function to be used to evaluate individuals in parallel with multiple processes.
 
     It must be inherited in a class that will implement the evaluation.
     '''
@@ -30,18 +31,24 @@
         Args:
             individuals (np.ndarray): Individuals who will be evaluated
 
         Returns:
             np.ndarray: Individuals fitness.
         '''
         if not self._setted or self._reset:
-            self.setup()
-            self._setted = True
+            range_name = "{0}_setup".format(self.__class__.__name__)
+            with nvtx.annotate_se(range_name, domain="evolvepy", category="evaluator", color=nvtx.evaluator_color):
+                self.setup()
+                self._setted = True
         
-        return self.evaluate(individuals)
+        range_name = "{0}_evaluation".format(self.__class__.__name__)
+        with nvtx.annotate_se(range_name, domain="evolvepy", category="evaluator", color=nvtx.evaluator_color):
+            fitness = self.evaluate(individuals)
+        
+        return fitness 
 
 
     @abstractmethod
     def setup(self) -> None:
         '''
         Method that prepares the evaluator to evaluate individuals.
 
@@ -87,15 +94,15 @@
 
 class ProcessEvaluator(Evaluator):
     '''
     Evaluates individuals using multiple process.
 
     '''
 
-    def __init__(self, fitness_function:Type[ProcessFitnessFunction], n_process:int=None, timeout:int=None, n_scores: int = 1, individual_per_call: int = 1, args:Dict[str, object]=None) -> None:
+    def __init__(self, fitness_function:Type[ProcessFitnessFunction], n_process:int=None, timeout:int=None, n_scores: int = 1, individual_per_call: int = 1, args:Dict[str, object]=None, name:str=None) -> None:
         '''
         ProcessEvaluator constructor.
 
         Args:
             fitness_function (Type[ProcessFitnessFunction]): Class that will be used to evaluate individuals.
             n_process (int, optional): Number of process to use. Defaults to None (same number as cpu_count).
             timeout (int, optional): Maximum time to wait for a new evaluation. Defaults to None (infinity).
@@ -103,15 +110,15 @@
             individual_per_call (int, optional): Number of individuals that the fitness function receives. Defaults to 1.
             args (Dict[str, object], optional): Other arguments for the fitness_function constructor. Defaults to None.
         '''
         if n_process is None:
             n_process = mp.cpu_count()
         
         other_parameters={"evaluation_function_name":fitness_function.__name__, "n_process":n_process, "timeout":timeout}
-        super().__init__(n_scores=n_scores, individual_per_call=individual_per_call, other_parameters=other_parameters)
+        super().__init__(n_scores=n_scores, individual_per_call=individual_per_call, other_parameters=other_parameters, name=name)
 
         self._fitness_function = fitness_function
         self._n_process = n_process
         self._timeout = timeout
 
         self._process = []
         self._individuals_queue = mp.Queue()
@@ -137,15 +144,15 @@
                             daemon=True)
             p.start()
             self._process.append(p)
         
         self._setted = True
 
 
-    def __call__(self, population: np.ndarray) -> np.ndarray:
+    def call(self, population: np.ndarray) -> np.ndarray:
         '''
         Evaluates the population
 
         Args:
             population (np.ndarray): Population to be evaluated.
 
         Raises:
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/basic_layers.py` & `evolvepy-2.0.0/src/evolvepy/generator/basic_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 		'''
 		Initialize the Filter from the top layer
 
 		Args:
 			n_to_pass (int): Number of best individuals selected.
 			name (strig): Name of the layer.
 		'''
-		parameters = {"n_to_pass":n_to_pass}
+		parameters = {"n_to_pass":int(n_to_pass)}
 		dynamic_parameters = {"n_to_pass":True}
 		super().__init__(name=name, parameters=parameters, dynamic_parameters=dynamic_parameters)
 
 	def call(self, population: np.ndarray, fitness: np.ndarray, context:Context) -> Tuple[np.ndarray, np.ndarray]:
 		'''
 		Generic call to funcion to use the class as funtion call
 
@@ -65,15 +65,14 @@
 			parameters (Dict(string, string)): parameters for the function
 			dynamic_parameters (Dit(string, string)): dinamic parameters of the function
 
 		Returns:
 			n_to_pass (int): Number of best individuals selected
 		'''
 		n_to_pass = self.parameters["n_to_pass"]
-		
 		return population[0:n_to_pass], fitness[0:n_to_pass]
 
 class Block(Layer):
 	'''
 	Block a determined chromosome for the next layers
 	'''
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/combine.py` & `evolvepy-2.0.0/src/evolvepy/generator/combine.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         '''
         Generic call for combine function
         '''
         return CombineLayer.combine(chromosomes, fitness, self._selection_function, self._crossover_function, self._n_combine)
 
     
     @staticmethod
-    @numba.njit()#parallel=True)
+    @numba.njit(nogil=True)#parallel=True)
     def combine(chromosomes:np.ndarray, fitness:np.ndarray, selection_function:Callable, crossover_function:Callable, n_combine:int):
         '''
         Combine two or more layers
 
         Args:
             chromossomes (np.ndarray): Array of chromosomes
             fitness (np.ndarray): Array of inidividuals fitness
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/context.py` & `evolvepy-2.0.0/src/evolvepy/generator/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Union
 
+from evolvepy.integrations import nvtx
+
 class Context:
     '''
     Layer to pass the context and restrictions from the previous layers
     '''
     default_values = ["sorted", "_sorted", "blocked", "_chromosome_names", "chromosome_names", "_values", "have_value", "copy", "_block_all", "block_all", "population_size", "_population_size"]
 
     def __init__(self, population_size:int, chromosome_names:Union[List[str], None]=None, sorted=False):
@@ -109,23 +111,24 @@
         '''
         Returns if name if within the registered values
         '''
         if name in self._values or name in Context.default_values:
             return True
         else:
             return False
-
+    
     def copy(self) -> Context:
         '''
         Create a copy of this instance
         '''
-        context = Context(self.population_size, self.chromosome_names, self.sorted)
-        
-        if isinstance(self.blocked, bool):
-            context.blocked = self.blocked
-        else:
-            context.blocked = dict(zip(self.blocked.keys(), self.blocked.values()))
-        
-        context._values = dict(zip(self._values.keys(), self._values.values()))
+        with nvtx.annotate_se(domain="evolvepy", category="generator", color=nvtx.generator_color):
+            context = Context(self.population_size, self.chromosome_names, self.sorted)
+            
+            if isinstance(self.blocked, bool):
+                context.blocked = self.blocked
+            else:
+                context.blocked = dict(zip(self.blocked.keys(), self.blocked.values()))
+            
+            context._values = dict(zip(self._values.keys(), self._values.values()))
 
         return context
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/descriptor.py` & `evolvepy-2.0.0/src/evolvepy/generator/descriptor.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/firstgen.py` & `evolvepy-2.0.0/src/evolvepy/generator/firstgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 		chromosome_range = self._chromosome_ranges[index]
 
 
 		if dtype.base.char in np.typecodes["AllFloat"]:
 			chromosome = np.random.rand(population_size, n_gene)
 			chromosome *= chromosome_range[1] - chromosome_range[0]
 			chromosome += chromosome_range[0]
-		elif dtype.char in np.typecodes["AllInteger"]:
+		elif dtype.base.char in np.typecodes["AllInteger"]:
 			chromosome = np.random.randint(chromosome_range[0], chromosome_range[1], shape)
 		else:
 			chromosome = np.random.choice([0, 1], shape).astype(np.bool_)
 
 		return chromosome
 	
 	def __call__(self, population: Union[ArrayLike, None], fitness: Union[ArrayLike, None] = None, context: Union[Context, None] = None) -> np.ndarray:
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/generator.py` & `evolvepy-2.0.0/src/evolvepy/generator/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 from numpy.typing import ArrayLike, DTypeLike
 
 from evolvepy.generator.context import Context
 from evolvepy.generator.layer import Layer
 from evolvepy.generator.firstgen import FirstGenLayer
 from evolvepy.generator.descriptor import Descriptor
+from evolvepy.generator.thread_pool import ThreadPool
 
 class Generator:
 	'''
 	Main class of the pipeline, it defines the layers oder, bifurcations and parameters
 	'''
 
 	def __init__(self, layers:Union[None, List[Layer]]=None, first_layer:Layer=None, last_layer:Layer=None, descriptor:Optional[Descriptor]=None):    
@@ -220,14 +221,16 @@
 		
 		context = Context(population_size, self._descriptor.chromosome_names)
 
 		if self._population is not None and len(self._population) > population_size:
 			self._population = self._population[:population_size]
 
 		self._layers[0](self._population, self._fitness, context)
+
+		ThreadPool.wait_for_end()
 		
 		if len(self._layers[-1].population) != population_size:
 			raise RuntimeError("The generator generated a population with wrong size. Expected "+str(population_size)+", got "+str(len(self._layers[-1].population)))
 
 		self._population = self._layers[-1].population
 
 		return self._population
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/layer.py` & `evolvepy-2.0.0/src/evolvepy/generator/layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from numpy.typing import ArrayLike
 
 from evolvepy.configurable import Configurable
 from evolvepy.generator.context import Context
+from evolvepy.integrations import nvtx
+from evolvepy.generator.thread_pool import ThreadPool
 
 class Layer(Configurable):
 	'''
 	Base Layer class with essential properties and methods, can be used as base for especialized layers of as simple layer in the pipeline
 	'''
 
 
@@ -100,29 +102,35 @@
 			fitness (np.ndarray): Fitness array
 			context (Context): Context object for the next layers
 
 		Returns:
 			population (np.ndarray): New population array
 			fitness (np.ndarray): New fitness array
 		'''         
+		profile_range = nvtx.start_range(self.name, domain="evolvepy", category="generator_layer", color=nvtx.generator_color)
 
 		if not (population is None and fitness is None):
 			population = np.asarray(population)
 
 			if fitness is None:
 				fitness = np.zeros(len(population), dtype=np.float32)
 			fitness = np.asarray(fitness).flatten()
 
 			if context is None:
 				context = Context(len(population), population.dtype.names)
 
 			if not context.block_all:
+				operation_profile_range = nvtx.start_range(self.name+"_call", domain="evolvepy", category="generator_layer", color=nvtx.generator_color)
+				
 				population, fitness = self.call(population, fitness, context)
+				
+				nvtx.end_range(operation_profile_range)
+				
+		nvtx.end_range(profile_range)
 
-		
 		self.send_next(population, fitness, context)
 		
 
 		self._context = context
 
 		return population, fitness
 
@@ -138,16 +146,19 @@
 		self._population = population
 		self._fitness = fitness
 
 		for layer in self._next:
 			next_context = context
 			if len(self._next) != 1:
 				next_context = next_context.copy()
-				
-			layer(population, fitness, next_context)
+				job = (layer, population, fitness, next_context)
+				ThreadPool.add_job(job)
+			else:
+				layer(population, fitness, next_context)
+			
 
 	def call(self, population:np.ndarray, fitness:np.ndarray, context:Context) -> Tuple[np.ndarray, np.ndarray]:
 		return population, fitness
 
 
 class Concatenate(Layer):
 	'''
@@ -244,25 +255,31 @@
 		Returns:
 			population (np.ndarray): New population array
 			fitness (np.ndarray): New fitness array
 		'''   
 
 		result = population.copy()
 
-		if self._chromosome_names is None: # Without specified name
-			if len(population.dtype) == 0 and not context.blocked: # and only one chromosome
-				result = self.call_chromosomes(population, fitness, context, None)
-			else:
-				for name in population.dtype.names: # and multiple chrmossomes
-					if not context.blocked[name]:
-						result[name] = self.call_chromosomes(population[name], fitness, context, name)
+		if len(population.dtype) == 0 and not context.blocked:
+			result = self.call_chromosomes(population, fitness, context, None)
+			
 		else:
-			for name in self._chromosome_names:
+			dim_to_operate = population.dtype.names
+
+			if self._chromosome_names is not None:
+				dim_to_operate = self._chromosome_names
+			
+			for name in dim_to_operate:
 				if not context.blocked[name]:
-						result[name] = self.call_chromosomes(population[name], fitness, context, name)
+					range_name = "{0}_{1}".format(self.name, name)
+					profile_range = nvtx.start_range(range_name, domain="evolvepy", category="generator_layer", color=nvtx.generator_color)
+					
+					result[name] = self.call_chromosomes(population[name], fitness, context, name)
+					
+					nvtx.end_range(profile_range)
 
 
 		return result, fitness
 	
 	#?????
 	def call_chromosomes(self, chromosomes:np.ndarray, fitness:np.ndarray, context:Context, name:Optional[str]) -> np.ndarray:
 		return chromosomes
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/mutation/mutation.py` & `evolvepy-2.0.0/src/evolvepy/generator/mutation/mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         existence_rate = self.parameters["existence_rate"]
         gene_rate = self.parameters["gene_rate"]
         mutation_range = (self.parameters["mutation_range_min"], self.parameters["mutation_range_max"])
 
         return NumericMutationLayer.mutate(chromosomes, self._mutation_function, existence_rate, gene_rate, mutation_range)
 
     @staticmethod
-    @numba.njit()#parallel=True)
+    @numba.njit(nogil=True)#parallel=True)
     def mutate(chromosomes:np.ndarray, mutation_function:Callable, existence_rate:float, gene_rate:float, mutation_range:Tuple[float, float]):
         '''
         Generic caller to a mutation function passed as parameters.
 
         Args:
             chromosomes (np.ArrayLike): Array of chromosomes
             existence_rate (float): Probability of first mutation
@@ -112,15 +112,15 @@
         existence_rate = self.parameters["existence_rate"]
         gene_rate = self.parameters["gene_rate"]
 
 
         return BinaryMutationLayer.mutate(chromosomes, self._mutation_function, existence_rate, gene_rate)
 
     @staticmethod
-    @numba.njit()
+    @numba.njit(nogil=True)
     def mutate(chromosomes:np.ndarray, mutation_function:Callable, existence_rate:float, gene_rate:float):
         '''
         Generic caller to a mutation function passed as parameters.
 
         Args:
             chromosomes (np.ArrayLike): array of chromosomes
             existence_rate (float): probability of first mutation
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/mutation/numeric_mutation.py` & `evolvepy-2.0.0/src/evolvepy/generator/mutation/numeric_mutation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from numba.core.utils import chain_exception
 import numpy as np
 from numpy.typing import ArrayLike
 import numba
 from typing import Tuple
+from evolvepy.integrations import nvtx
 
-
+#@nvtx.annotate(domain="evolvepy", category="generator_operator")
 @numba.njit
 def sum_mutation(chromosome:ArrayLike, existence_rate:float, gene_rate:float, mutation_range:Tuple[float, float]):
     '''
     It takes a chromosome and add a random value between the mutation range to its gene, then repeats the process with
     the given probability.
 
     Args:
@@ -31,14 +32,15 @@
 
             index = np.random.randint(0, chromosome.shape[0])
             new_chromosome[index] = chromosome[index] + np.random.uniform(mutation_range[0], mutation_range[1])
             count += 1
 
     return new_chromosome
 
+@nvtx.annotate(domain="evolvepy", category="generator_operator")
 def mul_mutation(chromosome:ArrayLike, existence_rate:float, gene_rate:float, mutation_range:Tuple[float, float]):
     '''
     It takes a chromosome and multiply a random value between the mutation range to its gene, then repeats the process with
     the given probability.
 
     Args:
         chromosome (np.ArrayLike): array of chromosomes
```

### Comparing `evolvepy-1.0.0/src/evolvepy/generator/selection/selection.py` & `evolvepy-2.0.0/src/evolvepy/generator/selection/selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import numpy as np
 from numpy.typing import ArrayLike
 from numpy.random import choice
 import numba
 
+from evolvepy.integrations import nvtx
+
 @numba.njit(fastmath=True)
 def isin(val, arr):
     for i in range(arr.shape[0]):
         if arr[i] == val:
             return True
     return False
 
+#@nvtx.annotate(domain="evolvepy", category="generator_operator")
 @numba.njit
 def tournament(fitness_array:ArrayLike, n_selection:int) -> np.ndarray:
 	'''
 	Select the best individuals in a one vs one test.
 		
 	Args:
 		fitness_array (np.typing.ArrayLike): Array with evaluated fitness from the generation
@@ -40,14 +43,15 @@
 			else:
 				best_index = index2
 
 		selected[i] = best_index
 
 	return selected
 
+@nvtx.annotate(domain="evolvepy", category="generator_operator")
 @numba.njit
 def roulette(fitness_array:ArrayLike, n_selection:int) -> np.ndarray:
 	'''
 	Select the best individuals stocaticaly with the probability of beign chosen
 	equivalent to the individual fitness.
 	
 	Args:
@@ -77,14 +81,15 @@
 		while index == -1 or (isin(index, selected)):
 			index = indexs[np.searchsorted(cumsum, np.random.random(), side="right")]
 
 		selected[i] = index
 		
 	return selected
 
+@nvtx.annotate(domain="evolvepy", category="generator_operator")
 @numba.njit
 def rank(fitness_array:ArrayLike, n_selection:int) -> np.ndarray:
     '''
 	Select the n best individuals assuming the fitness_array is decreasingly sorted.
     
 	Args:
     	fitness_array (np.typing.ArrayLike): array with evaluated fitness from the generation
```

### Comparing `evolvepy-1.0.0/src/evolvepy/integrations/gym/gym.py` & `evolvepy-2.0.0/src/evolvepy/integrations/gym/gym.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/integrations/tf_keras/tf_keras.py` & `evolvepy-2.0.0/src/evolvepy/integrations/tf_keras/tf_keras.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/integrations/unity_gym/unity.py` & `evolvepy-2.0.0/src/evolvepy/integrations/unity_gym/unity.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy/integrations/wandb/wandb.py` & `evolvepy-2.0.0/src/evolvepy/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `evolvepy-1.0.0/src/evolvepy.egg-info/PKG-INFO` & `evolvepy-2.0.0/src/evolvepy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 Metadata-Version: 2.1
 Name: evolvepy
-Version: 1.0.0
+Version: 2.0.0
 Summary: EvolvePy is a Python module created to allow the easy creation and execution of evolutionary algorithms.
 Home-page: https://github.com/EltonCN/evolvepy
 Author: EltonCN, João Bonucci, Thiago Lacerda
 Author-email: elton.nascimento@students.ic.unicamp.br, j218733@dac.unicamp.br, t244712@dac.unicamp.br
 License: MIT
 Project-URL: Bug Tracker, https://github.com/EltonCN/evolvepy/issues
 Project-URL: Documentation, https://eltoncn.github.io/evolvepy
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: unity
 Provides-Extra: wandb
 Provides-Extra: gym
+Provides-Extra: ray
 Provides-Extra: tensorflow
 Provides-Extra: all_integrations
 Provides-Extra: doc_generation
 License-File: LICENSE
 
-[![](https://img.shields.io/pypi/v/evolvepy?style=for-the-badge)]() [![](https://img.shields.io/github/license/EltonCN/evolvepy?style=for-the-badge)](https://github.com/EltonCN/evolvepy/blob/main/LICENSE)
+[![](https://img.shields.io/pypi/v/evolvepy?style=for-the-badge)](https://pypi.org/project/evolvepy) [![](https://img.shields.io/pypi/l/evolvepy?style=for-the-badge)](https://github.com/EltonCN/evolvepy/blob/main/LICENSE) [![](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EltonCN/evolvepy)
 
 # EvolvePy
 
 EvolvePy is a Python module created to allow the easy creation and execution of evolutionary algorithms.
 
 **Documentation**: [EvolvePy's documentation](https://eltoncn.github.io/evolvepy/_build/html/index.html).
 
+Presentation video (Portuguese, click on the image):
+[![Presentation Video](/Thumbnail.png)](https://www.youtube.com/watch?v=Hfo1XkzEcis&list=PLXcCIm-yDGGfBveHj_f_31GkythkJpeUl&index=1)
+
 ## Features
 
-(Links to example using feature)
+(Links to example using the feature)
 
 - Allows to create complex individual generators using different strategies:
-  - [Crossover](/examples/1%20-%20Simple%20EA.ipynb) (one-point, n-point, mean)
-  - Mutation ([sum](/examples/1%20-%20Simple%20EA.ipynb), multiplication, binary)
-  - Dynamic mutation
-  - [Elitism](/examples/2%20-%20Elitism.ipynb)
-  - [Randomic predation](/examples/6%20-%20Random%20Predation.ipynb)
-  - [Incremental evolution](/examples/5%20-%20Incremental%20Evolution.ipynb)
+  - [Crossover](/examples/Simple%20EA.ipynb) (one-point, n-point, mean)
+  - Mutation ([sum](/examples/Simple%20EA.ipynb), multiplication, [binary](/examples/3-CNF-SAT.ipynb))
+  - [Dynamic mutation](/examples/Dynamic%20Mutation.ipynb)
+  - [Elitism](/examples/Elitism.ipynb)
+  - [Randomic predation](/examples/Random%20Predation.ipynb)
+  - [Incremental evolution](/examples/Incremental%20Evolution.ipynb)
 - Define individuals with different chromosomes, with different types, ranges, sizes and parameters in the generator.
-- Evaluate individuals using [simple functions](/examples/1%20-%20Simple%20EA.ipynb)  or [multiple processes](/examples/Car%20PID%20Control.ipynb).
+- Evaluate individuals using [simple functions](/examples/Simple%20EA.ipynb)  or [multiple processes](/examples/Car%20PID%20Control.ipynb).
   - [Fitness cache](/examples/Car%20PID%20Control.ipynb) to avoid evaluate the same individual several times.
   - Fitness functions with different scores, which can be aggregated with different strategies.
   - [Evaluate the same individual several times to avoid noise](/examples/Car%20PID%20Control.ipynb).
-- [Log the evolution data to analyze later](/examples/4%20-%20Logger.ipynb).
+- [Log the evolution data to analyze later](/examples/Logger.ipynb).
 - Integrations with other modules:
-  - [Wandb](/examples/4%20-%20Logger.ipynb)
+  - [Wandb](/examples/Logger.ipynb)
   - [Tensorflow/Keras](/examples/TF-Keras%20Integration.ipynb)
   - [Gym](/examples/Reinforcement%20Learning.ipynb)
   - [Unity ML Agents](/examples/Unity%20ML%20Agents%20-%203DBall.ipynb) (using Gym)
 
 ## Installation
 
 - EvolvePy can be installed using pip:
@@ -89,8 +92,7 @@
 ## Authors
 
 Created by students from Unicamp's Institute of Computing (IC-Unicamp) as a project for the [evolutionary systems subject](https://gitlab.com/simoesusp/disciplinas/tree/master/SSC0713-Sistemas-Evolutivos-Aplicados-a-Robotica) at ICMC-USP, taught by prof. Eduardo do Valle Simoes.
 
 - [EltonCN](https://github.com/EltonCN)
 - [João Bonucci](https://github.com/Joao-Pedro-MB)
 - [Thiago Lacerda](https://github.com/ThiagoDSL)
-
```

