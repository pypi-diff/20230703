# Comparing `tmp/macq-0.3.6.tar.gz` & `tmp/macq-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macq-0.3.6.tar", last modified: Fri Jun 30 15:36:21 2023, max compression
+gzip compressed data, was "macq-0.3.7.tar", last modified: Mon Jul  3 16:10:36 2023, max compression
```

## Comparing `macq-0.3.6.tar` & `macq-0.3.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.637668 macq-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 15:35:55.000000 macq-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-30 15:36:21.637668 macq-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-30 15:35:55.000000 macq-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.625668 macq-0.3.6/macq/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 15:35:55.000000 macq-0.3.6/macq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.629668 macq-0.3.6/macq/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/amdn.py
--rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/arms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/learned_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/learned_fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    34948 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/locm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-06-30 15:35:55.000000 macq-0.3.6/macq/extract/slaf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.629668 macq-0.3.6/macq/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.629668 macq-0.3.6/macq/generate/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/pddl/fd_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/pddl/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/pddl/planning_domains_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/pddl/random_goal_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/pddl/trace_from_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/pddl/vanilla_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-30 15:35:55.000000 macq-0.3.6/macq/generate/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.633668 macq-0.3.6/macq/observation/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/action_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/atomic_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/id_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/identity_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/noisy_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/noisy_partial_disordered_parallel_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/noisy_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/observed_tracelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-30 15:35:55.000000 macq-0.3.6/macq/observation/partial_observation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.633668 macq-0.3.6/macq/trace/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/disordered_parallel_actions_observation_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/partial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-30 15:35:55.000000 macq-0.3.6/macq/trace/trace_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.637668 macq-0.3.6/macq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/common_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/complex_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/pysat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/tokenization_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/tokenization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/trace_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-30 15:35:55.000000 macq-0.3.6/macq/utils/trace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.625668 macq-0.3.6/macq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-30 15:36:21.000000 macq-0.3.6/macq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-30 15:36:21.000000 macq-0.3.6/macq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:36:21.000000 macq-0.3.6/macq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-30 15:36:21.000000 macq-0.3.6/macq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 15:36:21.000000 macq-0.3.6/macq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 15:35:55.000000 macq-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:36:21.637668 macq-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-30 15:35:55.000000 macq-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:36:21.637668 macq-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-30 15:35:55.000000 macq-0.3.6/tests/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.823550 macq-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 16:10:14.000000 macq-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-03 16:10:36.823550 macq-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-03 16:10:14.000000 macq-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.815550 macq-0.3.7/macq/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 16:10:14.000000 macq-0.3.7/macq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.819550 macq-0.3.7/macq/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/amdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/arms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/learned_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/learned_fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34948 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/locm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23733 2023-07-03 16:10:14.000000 macq-0.3.7/macq/extract/slaf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.819550 macq-0.3.7/macq/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.819550 macq-0.3.7/macq/generate/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/pddl/fd_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/pddl/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/pddl/planning_domains_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/pddl/random_goal_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/pddl/trace_from_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/pddl/vanilla_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-03 16:10:14.000000 macq-0.3.7/macq/generate/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.823550 macq-0.3.7/macq/observation/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/action_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/atomic_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/id_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/identity_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/noisy_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/noisy_partial_disordered_parallel_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/noisy_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/observed_tracelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-03 16:10:14.000000 macq-0.3.7/macq/observation/partial_observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.823550 macq-0.3.7/macq/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/disordered_parallel_actions_observation_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/partial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-03 16:10:14.000000 macq-0.3.7/macq/trace/trace_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.823550 macq-0.3.7/macq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/complex_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/tokenization_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/tokenization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/trace_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-03 16:10:14.000000 macq-0.3.7/macq/utils/trace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.815550 macq-0.3.7/macq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-03 16:10:36.000000 macq-0.3.7/macq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-03 16:10:36.000000 macq-0.3.7/macq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:10:36.000000 macq-0.3.7/macq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 16:10:36.000000 macq-0.3.7/macq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 16:10:36.000000 macq-0.3.7/macq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 16:10:14.000000 macq-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:10:36.823550 macq-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-03 16:10:14.000000 macq-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:10:36.823550 macq-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-03 16:10:14.000000 macq-0.3.7/tests/test_readme.py
```

### Comparing `macq-0.3.6/LICENSE` & `macq-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/PKG-INFO` & `macq-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.6
+Version: 0.3.7
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.6/README.md` & `macq-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/__init__.py` & `macq-0.3.7/macq/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/amdn.py` & `macq-0.3.7/macq/extract/amdn.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/arms.py` & `macq-0.3.7/macq/extract/arms.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/exceptions.py` & `macq-0.3.7/macq/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/extract.py` & `macq-0.3.7/macq/extract/extract.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/learned_action.py` & `macq-0.3.7/macq/extract/learned_action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/learned_fluent.py` & `macq-0.3.7/macq/extract/learned_fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/locm.py` & `macq-0.3.7/macq/extract/locm.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/model.py` & `macq-0.3.7/macq/extract/model.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/observer.py` & `macq-0.3.7/macq/extract/observer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/extract/slaf.py` & `macq-0.3.7/macq/extract/slaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,15 @@
                             )
                     """If the fluent is not observed to be either true or false (it is missing), then nothing happens."""
                 # display current updates
                 if debug_mode:
                     print("Update according to observations.")
                     for obj in to_obs:
                         f_str = raw_fluent_factored[obj]["fluent"].name
+                        phi = raw_fluent_factored[f_str]
                         print("\nfluent: " + f_str)
                         print("\npossible expl. for fluent being true:")
                         for f in phi["pos expl"]:
                             if f == top:
                                 print("true")
                             elif f == bottom:
                                 print("false")
@@ -411,14 +412,15 @@
                         SLAF.__remove_subsumed_clauses(phi["neutral"])
                 # display current updates
                 if debug_mode:
                     if a:
                         print("\nAction taken: " + str(a) + "\n")
                         for obj in to_obs:
                             f_str = raw_fluent_factored[obj]["fluent"].name
+                            phi = raw_fluent_factored[f_str]
                             print("\nfluent: " + f_str)
                             print(
                                 "\npossible expl. for fluent being true after "
                                 + str(a)
                                 + ":"
                             )
                             for f in phi["pos expl"]:
```

### Comparing `macq-0.3.6/macq/generate/csv.py` & `macq-0.3.7/macq/generate/csv.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/generate/pddl/fd_random_walk.py` & `macq-0.3.7/macq/generate/pddl/fd_random_walk.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/generate/pddl/generator.py` & `macq-0.3.7/macq/generate/pddl/generator.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/generate/pddl/planning_domains_api.py` & `macq-0.3.7/macq/generate/pddl/planning_domains_api.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/generate/pddl/random_goal_sampling.py` & `macq-0.3.7/macq/generate/pddl/random_goal_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/generate/pddl/trace_from_goal.py` & `macq-0.3.7/macq/generate/pddl/trace_from_goal.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/generate/pddl/vanilla_sampling.py` & `macq-0.3.7/macq/generate/pddl/vanilla_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/generate/plan.py` & `macq-0.3.7/macq/generate/plan.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/__init__.py` & `macq-0.3.7/macq/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/action_observation.py` & `macq-0.3.7/macq/observation/action_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/atomic_partial_observation.py` & `macq-0.3.7/macq/observation/atomic_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/identity_observation.py` & `macq-0.3.7/macq/observation/identity_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/noisy_observation.py` & `macq-0.3.7/macq/observation/noisy_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/noisy_partial_disordered_parallel_observation.py` & `macq-0.3.7/macq/observation/noisy_partial_disordered_parallel_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/noisy_partial_observation.py` & `macq-0.3.7/macq/observation/noisy_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/observation.py` & `macq-0.3.7/macq/observation/observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/observed_tracelist.py` & `macq-0.3.7/macq/observation/observed_tracelist.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/observation/partial_observation.py` & `macq-0.3.7/macq/observation/partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/__init__.py` & `macq-0.3.7/macq/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/action.py` & `macq-0.3.7/macq/trace/action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/disordered_parallel_actions_observation_lists.py` & `macq-0.3.7/macq/trace/disordered_parallel_actions_observation_lists.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/fluent.py` & `macq-0.3.7/macq/trace/fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/state.py` & `macq-0.3.7/macq/trace/state.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/step.py` & `macq-0.3.7/macq/trace/step.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/trace.py` & `macq-0.3.7/macq/trace/trace.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/trace/trace_list.py` & `macq-0.3.7/macq/trace/trace_list.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/utils/__init__.py` & `macq-0.3.7/macq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/utils/progress.py` & `macq-0.3.7/macq/utils/progress.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/utils/pysat.py` & `macq-0.3.7/macq/utils/pysat.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/utils/timer.py` & `macq-0.3.7/macq/utils/timer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/utils/trace_errors.py` & `macq-0.3.7/macq/utils/trace_errors.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq/utils/trace_utils.py` & `macq-0.3.7/macq/utils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/macq.egg-info/PKG-INFO` & `macq-0.3.7/macq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.6
+Version: 0.3.7
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.6/macq.egg-info/SOURCES.txt` & `macq-0.3.7/macq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macq-0.3.6/setup.py` & `macq-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.6"
+VERSION = "0.3.7"
 
 NAME = "macq"
 
 DESCRIPTION = "Action model acquisition from state trace data."
 
 DEPENDENCIES = [
     "tarski",
```

### Comparing `macq-0.3.6/tests/test_readme.py` & `macq-0.3.7/tests/test_readme.py`

 * *Files identical despite different names*

