# Comparing `tmp/SELDOMpy-0.6.8.tar.gz` & `tmp/SELDOMpy-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.6.8.tar", last modified: Mon Jul  3 17:21:58 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.6.9.tar", last modified: Mon Jul  3 17:25:53 2023, max compression
```

## Comparing `SELDOMpy-0.6.8.tar` & `SELDOMpy-0.6.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 17:21:58.244865 SELDOMpy-0.6.8/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.8/LICENSE.txt
--rw-rw-rw-   0        0        0      601 2023-07-03 17:21:58.244865 SELDOMpy-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 17:21:58.121880 SELDOMpy-0.6.8/SELDOMpy/
--rw-rw-rw-   0        0        0      390 2023-07-03 07:13:49.000000 SELDOMpy-0.6.8/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:21:58.223836 SELDOMpy-0.6.8/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.8/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.8/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.8/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.8/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.8/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.8/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.8/SELDOMpy/optimization.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.8/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.8/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     5618 2023-07-03 17:21:17.000000 SELDOMpy-0.6.8/SELDOMpy/setup.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.8/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.8/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:21:58.226834 SELDOMpy-0.6.8/SELDOMpy/src/
--rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/AMIGO_model.c
--rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/AMIGO_model_stats.c
--rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/AMIGO_problem.c
--rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.6.8/SELDOMpy/src/__init__.py
--rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.6.8/SELDOMpy/src/anODEModel.c
--rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodea.c
--rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodea_io.c
--rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes.c
--rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_band.c
--rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_bandpre.c
--rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_bbdpre.c
--rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_dense.c
--rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_diag.c
--rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_direct.c
--rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_io.c
--rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_spbcgs.c
--rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_spgmr.c
--rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_spils.c
--rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/cvodes_sptfqmr.c
--rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.6.8/SELDOMpy/src/decimal2binary.c
--rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/dhc.c
--rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/findStates.c
--rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/fnvector_serial.c
--rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/getAdjacencyMatrix.c
--rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/getNumBits.c
--rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/getNumInputs.c
--rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/getStateIndex.c
--rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/getTruthTables.c
--rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/get_count_bits.c
--rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/get_input_index.c
--rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/get_support_truth_tables.c
--rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/get_truth_tables_index.c
--rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/hill_function.c
--rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/linear_transfer_function.c
--rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/normHill.c
--rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/nvector_serial.c
--rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/printAdjMat.c
--rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/printInterMat.c
--rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/printNminiTerms.c
--rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/printTruthTables.c
--rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.6.8/SELDOMpy/src/sim_logic_ode.c
--rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/simulate_amigo_model.c
--rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_band.c
--rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_dense.c
--rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_direct.c
--rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_iterative.c
--rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_math.c
--rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_nvector.c
--rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_spbcgs.c
--rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_spgmr.c
--rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.6.8/SELDOMpy/src/sundials_sptfqmr.c
-drwxrwxrwx   0        0        0        0 2023-07-03 17:21:58.127850 SELDOMpy-0.6.8/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      601 2023-07-03 17:21:57.000000 SELDOMpy-0.6.8/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3493 2023-07-03 17:21:57.000000 SELDOMpy-0.6.8/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 17:21:57.000000 SELDOMpy-0.6.8/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-03 17:21:57.000000 SELDOMpy-0.6.8/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-03 17:21:57.000000 SELDOMpy-0.6.8/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-03 17:21:58.246837 SELDOMpy-0.6.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 17:25:53.619741 SELDOMpy-0.6.9/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      601 2023-07-03 17:25:53.619741 SELDOMpy-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 17:25:53.509760 SELDOMpy-0.6.9/SELDOMpy/
+-rw-rw-rw-   0        0        0      390 2023-07-03 07:13:49.000000 SELDOMpy-0.6.9/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:25:53.603744 SELDOMpy-0.6.9/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.9/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.9/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.9/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.9/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.9/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.9/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.9/SELDOMpy/optimization.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.9/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.9/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.9/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.9/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:25:53.605748 SELDOMpy-0.6.9/SELDOMpy/src/
+-rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/AMIGO_model.c
+-rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/AMIGO_model_stats.c
+-rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/AMIGO_problem.c
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.6.9/SELDOMpy/src/__init__.py
+-rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.6.9/SELDOMpy/src/anODEModel.c
+-rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodea.c
+-rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodea_io.c
+-rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes.c
+-rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_band.c
+-rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_bandpre.c
+-rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_bbdpre.c
+-rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_dense.c
+-rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_diag.c
+-rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_direct.c
+-rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_io.c
+-rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_spbcgs.c
+-rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_spgmr.c
+-rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_spils.c
+-rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/cvodes_sptfqmr.c
+-rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.6.9/SELDOMpy/src/decimal2binary.c
+-rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/dhc.c
+-rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/findStates.c
+-rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/fnvector_serial.c
+-rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/getAdjacencyMatrix.c
+-rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/getNumBits.c
+-rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/getNumInputs.c
+-rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/getStateIndex.c
+-rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/getTruthTables.c
+-rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/get_count_bits.c
+-rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/get_input_index.c
+-rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/get_support_truth_tables.c
+-rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/get_truth_tables_index.c
+-rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/hill_function.c
+-rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/linear_transfer_function.c
+-rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/normHill.c
+-rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/nvector_serial.c
+-rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/printAdjMat.c
+-rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/printInterMat.c
+-rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/printNminiTerms.c
+-rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/printTruthTables.c
+-rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.6.9/SELDOMpy/src/sim_logic_ode.c
+-rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/simulate_amigo_model.c
+-rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_band.c
+-rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_dense.c
+-rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_direct.c
+-rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_iterative.c
+-rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_math.c
+-rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_nvector.c
+-rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_spbcgs.c
+-rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_spgmr.c
+-rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.6.9/SELDOMpy/src/sundials_sptfqmr.c
+drwxrwxrwx   0        0        0        0 2023-07-03 17:25:53.521754 SELDOMpy-0.6.9/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      601 2023-07-03 17:25:53.000000 SELDOMpy-0.6.9/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3484 2023-07-03 17:25:53.000000 SELDOMpy-0.6.9/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 17:25:53.000000 SELDOMpy-0.6.9/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-03 17:25:53.000000 SELDOMpy-0.6.9/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-03 17:25:53.000000 SELDOMpy-0.6.9/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-03 17:25:53.620728 SELDOMpy-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     5612 2023-07-03 17:25:08.000000 SELDOMpy-0.6.9/setup.py
```

### Comparing `SELDOMpy-0.6.8/LICENSE.txt` & `SELDOMpy-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/PKG-INFO` & `SELDOMpy-0.6.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.6.8
+Version: 0.6.9
 Summary: hardware acceleration
 Home-page: https://github.com/voxy/accel.git
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `SELDOMpy-0.6.8/SELDOMpy/buildmim.py` & `SELDOMpy-0.6.9/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/extras.py` & `SELDOMpy-0.6.9/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/gen_exps.py` & `SELDOMpy-0.6.9/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.6.9/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.6.9/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/optimization.py` & `SELDOMpy-0.6.9/SELDOMpy/optimization.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/plot_results.py` & `SELDOMpy-0.6.9/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.6.9/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/setup.py` & `SELDOMpy-0.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # If you do change the License,
 # remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-with io.open(os.path.join(here, '../README.md'), encoding='utf-8') as f:
+with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
@@ -55,15 +55,15 @@
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
             self.status('Removing previous builds…')
-            rmtree(os.path.join(here, '../dist'))
+            rmtree(os.path.join(here, 'dist'))
         except OSError:
             pass
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPi via Twine…')
@@ -78,15 +78,15 @@
 
 extra_link_args = ["-shared", "-lxilinxopencl", "-lpthread", "-lrt",
                    "-L/opt/Xilinx/SDx/2017.1.op/runtime/lib/x86_64", "-lstdc++", ]
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version='0.6.8',
+    version='0.6.9',
     description=DESCRIPTION,
     long_description=long_description,
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     packages=find_packages(exclude=('tests',)),
     ext_modules=[Extension(
```

### Comparing `SELDOMpy-0.6.8/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.6.9/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.6.9/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/AMIGO_model.c` & `SELDOMpy-0.6.9/SELDOMpy/src/AMIGO_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/AMIGO_problem.c` & `SELDOMpy-0.6.9/SELDOMpy/src/AMIGO_problem.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/anODEModel.c` & `SELDOMpy-0.6.9/SELDOMpy/src/anODEModel.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodea.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodea.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodea_io.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodea_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_band.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_bandpre.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_bandpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_bbdpre.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_bbdpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_dense.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_diag.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_diag.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_direct.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_io.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_spbcgs.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_spgmr.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_spils.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_spils.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/cvodes_sptfqmr.c` & `SELDOMpy-0.6.9/SELDOMpy/src/cvodes_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/dhc.c` & `SELDOMpy-0.6.9/SELDOMpy/src/dhc.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/findStates.c` & `SELDOMpy-0.6.9/SELDOMpy/src/findStates.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/fnvector_serial.c` & `SELDOMpy-0.6.9/SELDOMpy/src/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/getAdjacencyMatrix.c` & `SELDOMpy-0.6.9/SELDOMpy/src/getAdjacencyMatrix.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/getStateIndex.c` & `SELDOMpy-0.6.9/SELDOMpy/src/getStateIndex.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/getTruthTables.c` & `SELDOMpy-0.6.9/SELDOMpy/src/getTruthTables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/get_support_truth_tables.c` & `SELDOMpy-0.6.9/SELDOMpy/src/get_support_truth_tables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/get_truth_tables_index.c` & `SELDOMpy-0.6.9/SELDOMpy/src/get_truth_tables_index.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/nvector_serial.c` & `SELDOMpy-0.6.9/SELDOMpy/src/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/printNminiTerms.c` & `SELDOMpy-0.6.9/SELDOMpy/src/printNminiTerms.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sim_logic_ode.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sim_logic_ode.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/simulate_amigo_model.c` & `SELDOMpy-0.6.9/SELDOMpy/src/simulate_amigo_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_band.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_dense.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_direct.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_iterative.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_math.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_math.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_nvector.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_spbcgs.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_spgmr.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy/src/sundials_sptfqmr.c` & `SELDOMpy-0.6.9/SELDOMpy/src/sundials_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.8/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.6.9/SELDOMpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.6.8
+Version: 0.6.9
 Summary: hardware acceleration
 Home-page: https://github.com/voxy/accel.git
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `SELDOMpy-0.6.8/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.6.9/SELDOMpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE.txt
 README.md
 setup.cfg
+setup.py
 SELDOMpy/__init__.py
 SELDOMpy/buildmim.py
 SELDOMpy/extras.py
 SELDOMpy/gen_exps.py
 SELDOMpy/getLBODEmodel.py
 SELDOMpy/getRandomLBODEmodel.py
 SELDOMpy/optimization.py
 SELDOMpy/plot_results.py
 SELDOMpy/reduce_fun.py
-SELDOMpy/setup.py
 SELDOMpy/simulate_logic_based_ode.py
 SELDOMpy/simulate_logic_based_ode_obs.py
 SELDOMpy.egg-info/PKG-INFO
 SELDOMpy.egg-info/SOURCES.txt
 SELDOMpy.egg-info/dependency_links.txt
 SELDOMpy.egg-info/requires.txt
 SELDOMpy.egg-info/top_level.txt
```

