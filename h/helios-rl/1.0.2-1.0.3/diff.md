# Comparing `tmp/helios-rl-1.0.2.tar.gz` & `tmp/helios-rl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-rl-1.0.2.tar", last modified: Mon Jul  3 10:47:59 2023, max compression
+gzip compressed data, was "helios-rl-1.0.3.tar", last modified: Mon Jul  3 19:13:26 2023, max compression
```

## Comparing `helios-rl-1.0.2.tar` & `helios-rl-1.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.798752 helios-rl-1.0.2/
--rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.2/LICENSE
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 10:47:59.798130 helios-rl-1.0.2/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.2/README.md
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.752691 helios-rl-1.0.2/helios_rl/
--rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.759491 helios-rl-1.0.2/helios_rl/adapters/
--rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/adapters/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.766120 helios-rl-1.0.2/helios_rl/agents/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/agent_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.2/helios_rl/agents/neural_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/random_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/table_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)    19502 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/analysis.py
--rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/config.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/config_local.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.775479 helios-rl-1.0.2/helios_rl/encoders/
--rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/encoder_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/observable_objects_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/poss_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/poss_state_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/prior_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.2/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.779492 helios-rl-1.0.2/helios_rl/environment_setup/
--rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/environment_setup/helios_info.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/environment_setup/imports.py
--rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/environment_setup/results_table.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.784467 helios-rl-1.0.2/helios_rl/evaluation/
--rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/evaluation/combined_variance_visual.py
--rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/evaluation/convergence_measure.py
--rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/evaluation/tabular_output.py
--rw-r--r--   0 p97070po   (502) staff       (20)    20998 2023-07-03 10:46:56.000000 helios-rl-1.0.2/helios_rl/evaluation/visual_output.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.796299 helios-rl-1.0.2/helios_rl/experiments/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/experience_sampling.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instr_input.py
--rw-r--r--   0 p97070po   (502) staff       (20)    30150 2023-05-19 16:23:14.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search.py
--rw-r--r--   0 p97070po   (502) staff       (20)    26701 2023-06-22 10:50:29.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search_mlp.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.2/helios_rl/experiments/standard.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/supervised_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/unsupervised_instruction_following.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.758485 helios-rl-1.0.2/helios_rl.egg-info/
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/SOURCES.txt
--rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/dependency_links.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/requires.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/top_level.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-03 10:47:59.798941 helios-rl-1.0.2/setup.cfg
--rw-r--r--   0 p97070po   (502) staff       (20)      764 2023-07-03 10:47:05.000000 helios-rl-1.0.2/setup.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.966077 helios-rl-1.0.3/
+-rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.3/LICENSE
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 19:13:26.965343 helios-rl-1.0.3/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.3/README.md
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.920840 helios-rl-1.0.3/helios_rl/
+-rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.927291 helios-rl-1.0.3/helios_rl/adapters/
+-rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/adapters/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.934282 helios-rl-1.0.3/helios_rl/agents/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/agents/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/agents/agent_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.3/helios_rl/agents/neural_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/agents/random_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/agents/table_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    19502 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/analysis.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/config.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/config_local.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.943114 helios-rl-1.0.3/helios_rl/encoders/
+-rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/encoders/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/encoders/encoder_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/encoders/observable_objects_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/encoders/poss_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/encoders/poss_state_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/encoders/prior_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.3/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.946852 helios-rl-1.0.3/helios_rl/environment_setup/
+-rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/environment_setup/helios_info.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/environment_setup/imports.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/environment_setup/results_table.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.952305 helios-rl-1.0.3/helios_rl/evaluation/
+-rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/evaluation/combined_variance_visual.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/evaluation/convergence_measure.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/evaluation/tabular_output.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    20998 2023-07-03 10:46:56.000000 helios-rl-1.0.3/helios_rl/evaluation/visual_output.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.964017 helios-rl-1.0.3/helios_rl/experiments/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/experiments/experience_sampling.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/experiments/helios_instr_input.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    32072 2023-07-03 19:12:13.000000 helios-rl-1.0.3/helios_rl/experiments/helios_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.3/helios_rl/experiments/helios_instruction_search.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    27274 2023-07-03 19:04:14.000000 helios-rl-1.0.3/helios_rl/experiments/helios_instruction_search_mlp.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.3/helios_rl/experiments/standard.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/experiments/supervised_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.3/helios_rl/experiments/unsupervised_instruction_following.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 19:13:26.926306 helios-rl-1.0.3/helios_rl.egg-info/
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 19:13:26.000000 helios-rl-1.0.3/helios_rl.egg-info/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-03 19:13:26.000000 helios-rl-1.0.3/helios_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-03 19:13:26.000000 helios-rl-1.0.3/helios_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-03 19:13:26.000000 helios-rl-1.0.3/helios_rl.egg-info/requires.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-03 19:13:26.000000 helios-rl-1.0.3/helios_rl.egg-info/top_level.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-03 19:13:26.966279 helios-rl-1.0.3/setup.cfg
+-rw-r--r--   0 p97070po   (502) staff       (20)      767 2023-07-03 19:10:59.000000 helios-rl-1.0.3/setup.py
```

### Comparing `helios-rl-1.0.2/LICENSE` & `helios-rl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/README.md` & `helios-rl-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/__init__.py` & `helios-rl-1.0.3/helios_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/adapters/__init__.py` & `helios-rl-1.0.3/helios_rl/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/agents/agent_abstract.py` & `helios-rl-1.0.3/helios_rl/agents/agent_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/agents/neural_q_agent.py` & `helios-rl-1.0.3/helios_rl/agents/neural_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/agents/random_agent.py` & `helios-rl-1.0.3/helios_rl/agents/random_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/agents/table_q_agent.py` & `helios-rl-1.0.3/helios_rl/agents/table_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/analysis.py` & `helios-rl-1.0.3/helios_rl/analysis.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/config.py` & `helios-rl-1.0.3/helios_rl/config.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/config_local.py` & `helios-rl-1.0.3/helios_rl/config_local.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/encoders/__init__.py` & `helios-rl-1.0.3/helios_rl/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/encoders/encoder_abstract.py` & `helios-rl-1.0.3/helios_rl/encoders/encoder_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/encoders/observable_objects_encoded.py` & `helios-rl-1.0.3/helios_rl/encoders/observable_objects_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/encoders/poss_actions_encoded.py` & `helios-rl-1.0.3/helios_rl/encoders/poss_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/encoders/poss_state_encoded.py` & `helios-rl-1.0.3/helios_rl/encoders/poss_state_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/encoders/prior_actions_encoded.py` & `helios-rl-1.0.3/helios_rl/encoders/prior_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py` & `helios-rl-1.0.3/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/environment_setup/helios_info.py` & `helios-rl-1.0.3/helios_rl/environment_setup/helios_info.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/environment_setup/imports.py` & `helios-rl-1.0.3/helios_rl/environment_setup/imports.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/environment_setup/results_table.py` & `helios-rl-1.0.3/helios_rl/environment_setup/results_table.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/evaluation/combined_variance_visual.py` & `helios-rl-1.0.3/helios_rl/evaluation/combined_variance_visual.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/evaluation/convergence_measure.py` & `helios-rl-1.0.3/helios_rl/evaluation/convergence_measure.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/evaluation/visual_output.py` & `helios-rl-1.0.3/helios_rl/evaluation/visual_output.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/experiments/helios_instr_input.py` & `helios-rl-1.0.3/helios_rl/experiments/helios_instr_input.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/experiments/helios_instruction_following.py` & `helios-rl-1.0.3/helios_rl/experiments/helios_instruction_following.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,26 @@
                         for live_sample_batch in range(0, live_sample_batch_count-1):
                             print("--- Live Interaction Batch Num", live_sample_batch+1)
                             # ---- 
                             # Train for sub instr plan
                             start = str(env_start).split(".")[0]
                             i=0
                             while True:
-                                if start in self.known_instructions_dict[(agent_type+'_'+adapter)]:
+                                # Only allow insutrction up until total limi
+                                # - Prevents it being given more episodes than flat
+                                # - Prevents cyclic instruction paths
+                                if int(number_training_episodes*self.instruction_episode_ratio)<=(number_training_episodes-total_instr_episodes):
+                                    # Override with trained agent if goal seen previously
+                                    if goal in self.trained_agents[str(agent_type) + '_' + str(adapter)]:
+                                        live_env.agent = self.trained_agents[str(agent_type) + '_' + str(adapter)][goal].clone()
+                                        # Reset exploration parameter between seeds so to not get 'trapped'
+                                        live_env.agent.exploration_parameter_reset()
+                                    break
+                                
+                                elif start in self.known_instructions_dict[(agent_type+'_'+adapter)]:
                                     i+=1
                                     max_count = 0
                                     for end in self.known_instructions_dict[(agent_type+'_'+adapter)][start]:
                                         if self.known_instructions_dict[(agent_type+'_'+adapter)][start][end] > max_count:
                                             max_count = self.known_instructions_dict[(agent_type+'_'+adapter)][start][end]
                                             instr = start + "---" + end
                                             print("Sub-instr: ", instr)
@@ -304,15 +315,26 @@
                         start = str(env_start).split(".")[0]
                         i=0
                         total_instr_episodes = 0
                         instr_results = None
                         while True:
                             i+=1
                             max_count = 0
-                            if start in self.known_instructions_dict[(agent_type+'_'+adapter)]:
+                            # Only allow insutrction up until total limi
+                            # - Prevents it being given more episodes than flat
+                            # - Prevents cyclic instruction paths
+                            if int(number_training_episodes*self.instruction_episode_ratio)<=(number_training_episodes-total_instr_episodes):
+                                # Override with trained agent if goal seen previously
+                                if goal in self.trained_agents[str(agent_type) + '_' + str(adapter)]:
+                                    live_env.agent = self.trained_agents[str(agent_type) + '_' + str(adapter)][goal].clone()
+                                    # Reset exploration parameter between seeds so to not get 'trapped'
+                                    live_env.agent.exploration_parameter_reset()
+                                break
+                            
+                            elif start in self.known_instructions_dict[(agent_type+'_'+adapter)]:
                                 for end in self.known_instructions_dict[(agent_type+'_'+adapter)][start]:
                                     if self.known_instructions_dict[(agent_type+'_'+adapter)][start][end] > max_count:
                                         max_count = self.known_instructions_dict[(agent_type+'_'+adapter)][start][end]
                                         instr = start + "---" + end
                                         print("Sub-instr: ", instr)
                                         
                                 # Instructions use fewer epispdes, lower bound to 10
```

### Comparing `helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search.py` & `helios-rl-1.0.3/helios_rl/experiments/helios_instruction_search.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search_mlp.py` & `helios-rl-1.0.3/helios_rl/experiments/helios_instruction_search_mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
                         if i == 0:
                             instruction = str(sample_env.start_obs).split(".")[0] + "---" + instr
                         else:
                             instruction = instructions[i-1] + "---" + instr
                         
                         instr_description = instr_descriptions[i]
                         
-                        if type(instr_description) != type(List[str]):
+                        if type(instr_description) == type(''):
                             instr_description = instr_description.split('.')
                             instr_description = list(filter(None, instr_description))
                         # Create tensor vector of description
                         instruction_vector = self.enc.encode(instr_description)
                         # EXPLORE TO FIND LOCATION OF SUB-GOAL
                         sub_goal = None
                         # ---------------------------
@@ -259,36 +259,38 @@
                                     sim = self.instr_feedback_layer(t_state, instruction_vector)
                                     if sim > max_sim:
                                         max_sim  = sim
                                         sub_goal_max = obs_state
                                         sub_goal_max_t = t_state
                                     if sim >= self.sim_threshold:
                                         sub_goal = obs_state # Sub-Goal code
+                                        sub_goal_t = t_state
                                         sub_goal_list.append(sub_goal)
                 
-                                # TODO: OR if none above threshold within (1-threshold%) of max sim
+                                # OR if none above threshold within (1-threshold%) of max sim
                                 if max_sim < self.sim_threshold:
                                     sub_goal = sub_goal_max
-                                    sub_goal_list.append(sub_goal)
-                                    sub_goal_t = sub_goal_max_t
-                                    # for obs_state in self.observed_states:
-                                    #     str_state = self.observed_states[obs_state]
-                                    #     #str_state_stacked = ' '.join(str_state)
-                                    #     t_state = self.enc.encode(str_state)
-                                    #     # ---
-                                    #     total_sim = 0
-                                    #     # Average sim across each sentence in instruction vs state
-                                    #     for i,instr_sentence in enumerate(instruction_vector):
-                                    #         feedback_layer_sent = feedback_layer[i]
-                                    #         for state_sentence in t_state:
-                                    #             total_sim+=self.cos(torch.add(state_sentence, feedback_layer_sent), instr_sentence) 
-                                    #     sim = total_sim.item()/(len(instruction_vector)*len(t_state))
-                                    #     if sim >= max_sim*(self.sim_threshold):
-                                    #         sub_goal = obs_state # Temp Sub-Goal as most known similar
-                                    #         sub_goal_list.append(sub_goal)
+                                    sub_goal_t = sub_goal_max_t                                    
+                                    # Find all states that have same sim as max
+                                    for obs_state in self.observed_states:
+                                        str_state = self.observed_states[obs_state]
+                                        #str_state_stacked = ' '.join(str_state)
+                                        t_state = self.enc.encode(str_state)
+                                        # ---
+                                        total_sim = 0
+                                        # Average sim across each sentence in instruction vs state
+                                        dim_count = 0
+                                        for idx,instr_sentence in enumerate(instruction_vector):
+                                            feedback_layer_sent = feedback_layer[idx]
+                                            for state_sentence in t_state:
+                                                total_sim+=self.cos(torch.add(state_sentence, feedback_layer_sent), instr_sentence)
+                                                dim_count+=1
+                                        sim = 0 if dim_count==0 else total_sim.item()/dim_count
+                                        if sim >= (max_sim):
+                                            sub_goal_list.append(obs_state)
 
                                 if max_sim < self.sim_threshold:
                                     print("Minimum sim for observed states to match instruction not found, using best match instead. Best match sim value = ", max_sim )
                             # If adapter is poor to match to instruction vector none of them observed states match
                             if (max_sim<-1)|(sub_goal is None):#|(max_sim>1):
                                 print("All observed states result in similarity outside bounds (i.e. strongly opposite vectors to instruction). Re-starting Search.")
                                 print("Max sim found = ", max_sim)
@@ -297,21 +299,28 @@
                             elif (sim_delta<0.05)|(search_count>=5):
                                 print("Change in sim less than or equal to delta cap or search cap reached, assume goal-state not observed. Re-starting Search.")
                                 if simulated_instr_goal:
                                     print("-- Known sub_goal position: ", simulated_instr_goal)
                                 print("-- Best match: ", sub_goal_max)
                                 sub_goal = None
                                 self.observed_states = {}
+                                search_count = 0
                             else:
                                 if not simulated_instr_goal:
                                     print(" ")
                                     print("===========")
                                     print("Instruction: ", instr)
                                     print(sub_goal)
                                     print("Best match state for instruction \n ______ \n Adapted form: \n\t - ", self.observed_states[sub_goal], " \n Engine observation: \n\t - " , sub_goal)
+                                    print("Full list of matching states...",)
+                                    for s_g in sub_goal_list:
+                                        print(self.observed_states[s_g], ": ", s_g)
+                                    print("")
+                                    print("Tensor check: Size of Instruction vs Best match: ", instruction_vector.size(), " --- ", sub_goal_t.size())
+                                    print("")
                                     feedback = input("-- Does this match the expectation instruction outcome? (Y/N)")
                                     feedback_count+=1 
                                 else:
                                     if type(simulated_instr_goal[0]) != type(sub_goal_max):
                                         print("- ERROR: Typing of simulated sub-goal check does not match typing of state from environment, please correct this.")
                                         print(type(simulated_instr_goal[0])," - ", type(sub_goal_max))
                                         #print("Observed States Examples: ", self.observed_states(list(self.observed_states.keys())[0:5]))
```

### Comparing `helios-rl-1.0.2/helios_rl/experiments/standard.py` & `helios-rl-1.0.3/helios_rl/experiments/standard.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/experiments/supervised_instruction_following.py` & `helios-rl-1.0.3/helios_rl/experiments/supervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl/experiments/unsupervised_instruction_following.py` & `helios-rl-1.0.3/helios_rl/experiments/unsupervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/helios_rl.egg-info/SOURCES.txt` & `helios-rl-1.0.3/helios_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.2/setup.py` & `helios-rl-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='helios-rl',
-    version='1.0.2',
+    version='1.0.3',
     packages=[
         'helios_rl', 
         'helios_rl.adapters', 
         'helios_rl.agents', 
         'helios_rl.encoders', 
         'helios_rl.environment_setup', 
         'helios_rl.evaluation', 
@@ -20,9 +20,9 @@
         'numpy',
         'pandas',
         'matplotlib',
         'seaborn',
         'scipy',
         'torch',
         'sentence-transformers'
-    ]
-)
+    ] 
+)
```

