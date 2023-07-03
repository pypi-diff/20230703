# Comparing `tmp/helios-rl-1.0.1.tar.gz` & `tmp/helios-rl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-rl-1.0.1.tar", last modified: Mon Jul  3 08:53:43 2023, max compression
+gzip compressed data, was "helios-rl-1.0.2.tar", last modified: Mon Jul  3 10:47:59 2023, max compression
```

## Comparing `helios-rl-1.0.1.tar` & `helios-rl-1.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.367125 helios-rl-1.0.1/
--rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.1/LICENSE
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 08:53:43.366562 helios-rl-1.0.1/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.1/README.md
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.323681 helios-rl-1.0.1/helios_rl/
--rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.329632 helios-rl-1.0.1/helios_rl/adapters/
--rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/adapters/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.335758 helios-rl-1.0.1/helios_rl/agents/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/agents/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/agents/agent_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.1/helios_rl/agents/neural_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/agents/random_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/agents/table_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)    19502 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/analysis.py
--rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/config.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/config_local.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.343854 helios-rl-1.0.1/helios_rl/encoders/
--rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/encoders/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/encoders/encoder_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/encoders/observable_objects_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/encoders/poss_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/encoders/poss_state_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/encoders/prior_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.1/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.347816 helios-rl-1.0.1/helios_rl/environment_setup/
--rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/environment_setup/helios_info.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/environment_setup/imports.py
--rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/environment_setup/results_table.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.352203 helios-rl-1.0.1/helios_rl/evaluation/
--rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/evaluation/combined_variance_visual.py
--rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/evaluation/convergence_measure.py
--rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/evaluation/tabular_output.py
--rw-r--r--   0 p97070po   (502) staff       (20)    20983 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/evaluation/visual_output.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.365176 helios-rl-1.0.1/helios_rl/experiments/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/experiments/experience_sampling.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/experiments/helios_instr_input.py
--rw-r--r--   0 p97070po   (502) staff       (20)    30150 2023-05-19 16:23:14.000000 helios-rl-1.0.1/helios_rl/experiments/helios_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.1/helios_rl/experiments/helios_instruction_search.py
--rw-r--r--   0 p97070po   (502) staff       (20)    26701 2023-06-22 10:50:29.000000 helios-rl-1.0.1/helios_rl/experiments/helios_instruction_search_mlp.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.1/helios_rl/experiments/standard.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/experiments/supervised_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.1/helios_rl/experiments/unsupervised_instruction_following.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 08:53:43.328699 helios-rl-1.0.1/helios_rl.egg-info/
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 08:53:43.000000 helios-rl-1.0.1/helios_rl.egg-info/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-03 08:53:43.000000 helios-rl-1.0.1/helios_rl.egg-info/SOURCES.txt
--rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-03 08:53:43.000000 helios-rl-1.0.1/helios_rl.egg-info/dependency_links.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-03 08:53:43.000000 helios-rl-1.0.1/helios_rl.egg-info/requires.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-03 08:53:43.000000 helios-rl-1.0.1/helios_rl.egg-info/top_level.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-03 08:53:43.367272 helios-rl-1.0.1/setup.cfg
--rw-r--r--   0 p97070po   (502) staff       (20)      764 2023-07-03 08:53:12.000000 helios-rl-1.0.1/setup.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.798752 helios-rl-1.0.2/
+-rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.2/LICENSE
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 10:47:59.798130 helios-rl-1.0.2/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.2/README.md
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.752691 helios-rl-1.0.2/helios_rl/
+-rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.759491 helios-rl-1.0.2/helios_rl/adapters/
+-rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/adapters/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.766120 helios-rl-1.0.2/helios_rl/agents/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/agent_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.2/helios_rl/agents/neural_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/random_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/agents/table_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    19502 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/analysis.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/config.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/config_local.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.775479 helios-rl-1.0.2/helios_rl/encoders/
+-rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/encoder_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/observable_objects_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/poss_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/poss_state_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/encoders/prior_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.2/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.779492 helios-rl-1.0.2/helios_rl/environment_setup/
+-rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/environment_setup/helios_info.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/environment_setup/imports.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/environment_setup/results_table.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.784467 helios-rl-1.0.2/helios_rl/evaluation/
+-rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/evaluation/combined_variance_visual.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/evaluation/convergence_measure.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/evaluation/tabular_output.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    20998 2023-07-03 10:46:56.000000 helios-rl-1.0.2/helios_rl/evaluation/visual_output.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.796299 helios-rl-1.0.2/helios_rl/experiments/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/experience_sampling.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instr_input.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    30150 2023-05-19 16:23:14.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    26701 2023-06-22 10:50:29.000000 helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search_mlp.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.2/helios_rl/experiments/standard.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/supervised_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.2/helios_rl/experiments/unsupervised_instruction_following.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-03 10:47:59.758485 helios-rl-1.0.2/helios_rl.egg-info/
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/requires.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-03 10:47:59.000000 helios-rl-1.0.2/helios_rl.egg-info/top_level.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-03 10:47:59.798941 helios-rl-1.0.2/setup.cfg
+-rw-r--r--   0 p97070po   (502) staff       (20)      764 2023-07-03 10:47:05.000000 helios-rl-1.0.2/setup.py
```

### Comparing `helios-rl-1.0.1/LICENSE` & `helios-rl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/README.md` & `helios-rl-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/__init__.py` & `helios-rl-1.0.2/helios_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/adapters/__init__.py` & `helios-rl-1.0.2/helios_rl/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/agents/agent_abstract.py` & `helios-rl-1.0.2/helios_rl/agents/agent_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/agents/neural_q_agent.py` & `helios-rl-1.0.2/helios_rl/agents/neural_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/agents/random_agent.py` & `helios-rl-1.0.2/helios_rl/agents/random_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/agents/table_q_agent.py` & `helios-rl-1.0.2/helios_rl/agents/table_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/analysis.py` & `helios-rl-1.0.2/helios_rl/analysis.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/config.py` & `helios-rl-1.0.2/helios_rl/config.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/config_local.py` & `helios-rl-1.0.2/helios_rl/config_local.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/encoders/__init__.py` & `helios-rl-1.0.2/helios_rl/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/encoders/encoder_abstract.py` & `helios-rl-1.0.2/helios_rl/encoders/encoder_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/encoders/observable_objects_encoded.py` & `helios-rl-1.0.2/helios_rl/encoders/observable_objects_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/encoders/poss_actions_encoded.py` & `helios-rl-1.0.2/helios_rl/encoders/poss_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/encoders/poss_state_encoded.py` & `helios-rl-1.0.2/helios_rl/encoders/poss_state_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/encoders/prior_actions_encoded.py` & `helios-rl-1.0.2/helios_rl/encoders/prior_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py` & `helios-rl-1.0.2/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/environment_setup/helios_info.py` & `helios-rl-1.0.2/helios_rl/environment_setup/helios_info.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/environment_setup/imports.py` & `helios-rl-1.0.2/helios_rl/environment_setup/imports.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/environment_setup/results_table.py` & `helios-rl-1.0.2/helios_rl/environment_setup/results_table.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/evaluation/combined_variance_visual.py` & `helios-rl-1.0.2/helios_rl/evaluation/combined_variance_visual.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/evaluation/convergence_measure.py` & `helios-rl-1.0.2/helios_rl/evaluation/convergence_measure.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/evaluation/visual_output.py` & `helios-rl-1.0.2/helios_rl/evaluation/visual_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 ci_L=np.mean(window_reward)
                 ci_U=np.mean(window_reward)
             # CI produces error if all values the same
             elif np.count_nonzero(window_reward == window_reward[0]) == len(window_reward):
                 ci_L=np.mean(window_reward)
                 ci_U=np.mean(window_reward)
             else:
-                ci_L, ci_U = st.t.interval(alpha=0.95, df=len(window_reward)-1, loc=np.mean(window_reward), scale=st.sem(window_reward))
+                ci_L, ci_U = st.t.interval(confidence=0.95, df=len(window_reward)-1, loc=np.mean(window_reward), scale=st.sem(window_reward))
 
             reward_delta.append(mean)
             ci_L_lst.append(ci_L)
             ci_U_lst.append(ci_U)
     
         x =  self.results_data['episode']
         y = np.array(reward_delta)
@@ -145,15 +145,15 @@
                 ci_L=np.mean(window_reward)
                 ci_U=np.mean(window_reward)
             # CI produces error if all values the same
             elif np.count_nonzero(window_reward == window_reward[0]) == len(window_reward):
                 ci_L=np.mean(window_reward)
                 ci_U=np.mean(window_reward)
             else:
-                ci_L, ci_U = st.t.interval(alpha=0.95, df=len(window_reward)-1, loc=np.mean(window_reward), scale=st.sem(window_reward))
+                ci_L, ci_U = st.t.interval(confidence=0.95, df=len(window_reward)-1, loc=np.mean(window_reward), scale=st.sem(window_reward))
 
             reward_delta.append(mean)
             ci_L_lst.append(ci_L)
             ci_U_lst.append(ci_U)
     
         x =  self.results_data['episode']
         y = np.array(reward_delta)
@@ -396,15 +396,15 @@
                 ci_L=np.mean(window_reward)
                 ci_U=np.mean(window_reward)
             # CI produces error if all values the same
             elif np.count_nonzero(window_reward == window_reward[0]) == len(window_reward):
                 ci_L=np.mean(window_reward)
                 ci_U=np.mean(window_reward)
             else:
-                ci_L, ci_U = st.t.interval(alpha=0.95, df=len(window_reward)-1, loc=np.mean(window_reward), scale=st.sem(window_reward))
+                ci_L, ci_U = st.t.interval(confidence=0.95, df=len(window_reward)-1, loc=np.mean(window_reward), scale=st.sem(window_reward))
 
             reward_delta.append(mean)
             ci_L_lst.append(ci_L)
             ci_U_lst.append(ci_U)
     
         x =  self.results_data['episode']
         y = np.array(reward_delta)
```

### Comparing `helios-rl-1.0.1/helios_rl/experiments/helios_instr_input.py` & `helios-rl-1.0.2/helios_rl/experiments/helios_instr_input.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/experiments/helios_instruction_following.py` & `helios-rl-1.0.2/helios_rl/experiments/helios_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/experiments/helios_instruction_search.py` & `helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/experiments/helios_instruction_search_mlp.py` & `helios-rl-1.0.2/helios_rl/experiments/helios_instruction_search_mlp.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/experiments/standard.py` & `helios-rl-1.0.2/helios_rl/experiments/standard.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/experiments/supervised_instruction_following.py` & `helios-rl-1.0.2/helios_rl/experiments/supervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl/experiments/unsupervised_instruction_following.py` & `helios-rl-1.0.2/helios_rl/experiments/unsupervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/helios_rl.egg-info/SOURCES.txt` & `helios-rl-1.0.2/helios_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.1/setup.py` & `helios-rl-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='helios-rl',
-    version='1.0.1',
+    version='1.0.2',
     packages=[
         'helios_rl', 
         'helios_rl.adapters', 
         'helios_rl.agents', 
         'helios_rl.encoders', 
         'helios_rl.environment_setup', 
         'helios_rl.evaluation',
```

