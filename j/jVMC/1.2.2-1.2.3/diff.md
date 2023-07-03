# Comparing `tmp/jVMC-1.2.2.tar.gz` & `tmp/jVMC-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jVMC-1.2.2.tar", last modified: Wed Jun 14 08:48:26 2023, max compression
+gzip compressed data, was "jVMC-1.2.3.tar", last modified: Mon Jul  3 11:50:25 2023, max compression
```

## Comparing `jVMC-1.2.2.tar` & `jVMC-1.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 08:48:12.000000 jVMC-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-14 08:48:26.857486 jVMC-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-14 08:48:12.000000 jVMC-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.853486 jVMC-1.2.2/jVMC/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/global_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/mpi_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.853486 jVMC-1.2.2/jVMC/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/activation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/ffn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/rbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/rnn1d_general.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/rnn2d_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/sym_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/nets/two_nets_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/jVMC/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/branch_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/operator/povm.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/jVMC/util/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/minsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/output_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/symmetries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/tdvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-06-14 08:48:12.000000 jVMC-1.2.2/jVMC/vqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.853486 jVMC-1.2.2/jVMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 08:48:26.000000 jVMC-1.2.2/jVMC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:48:26.857486 jVMC-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-14 08:48:12.000000 jVMC-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:26.857486 jVMC-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/minsr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/mpi_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/nets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/operator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/povm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/stats_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/stepper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/symmetries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/tdvp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-06-14 08:48:12.000000 jVMC-1.2.2/tests/vqs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.298665 jVMC-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 11:50:15.000000 jVMC-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-03 11:50:25.298665 jVMC-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-03 11:50:15.000000 jVMC-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/global_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/mpi_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/activation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/rbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/rnn1d_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/rnn2d_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/sym_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/two_nets_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/branch_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/povm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/minsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/output_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/symmetries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/tdvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/vqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:50:25.298665 jVMC-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-03 11:50:15.000000 jVMC-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.298665 jVMC-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/minsr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/mpi_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/nets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/operator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/povm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/stepper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/symmetries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/tdvp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/vqs_test.py
```

### Comparing `jVMC-1.2.2/LICENSE` & `jVMC-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/PKG-INFO` & `jVMC-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jVMC
-Version: 1.2.2
+Version: 1.2.3
 Summary: jVMC: Versatile and performant variational Monte Carlo
 Home-page: https://jvmc.readthedocs.io/en/latest/#
 Author: Markus Schmitt, Moritz Reh
 Author-email: markus.schmitt@uni-koeln.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jVMC-1.2.2/README.md` & `jVMC-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/global_defs.py` & `jVMC-1.2.3/jVMC/global_defs.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/mpi_wrapper.py` & `jVMC-1.2.3/jVMC/mpi_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/activation_functions.py` & `jVMC-1.2.3/jVMC/nets/activation_functions.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/cnn.py` & `jVMC-1.2.3/jVMC/nets/cnn.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/ffn.py` & `jVMC-1.2.3/jVMC/nets/ffn.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/initializers.py` & `jVMC-1.2.3/jVMC/nets/initializers.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/rbm.py` & `jVMC-1.2.3/jVMC/nets/rbm.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/rnn1d_general.py` & `jVMC-1.2.3/jVMC/nets/rnn1d_general.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/rnn2d_general.py` & `jVMC-1.2.3/jVMC/nets/rnn2d_general.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/sym_wrapper.py` & `jVMC-1.2.3/jVMC/nets/sym_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/nets/two_nets_wrapper.py` & `jVMC-1.2.3/jVMC/nets/two_nets_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/operator/base.py` & `jVMC-1.2.3/jVMC/operator/base.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/operator/branch_free.py` & `jVMC-1.2.3/jVMC/operator/branch_free.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/operator/povm.py` & `jVMC-1.2.3/jVMC/operator/povm.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/sampler.py` & `jVMC-1.2.3/jVMC/sampler.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/stats.py` & `jVMC-1.2.3/jVMC/stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,52 +38,52 @@
 
     global statsPmapDevices
 
     if jVMC.global_defs.pmap_devices_updated(statsPmapDevices):
 
         statsPmapDevices = global_defs.myPmapDevices
 
-        _mean_helper = pmap_for_my_devices(lambda data, w: jnp.tensordot(w, data, axes=(0,0)), in_axes=(0, 0))
-        _data_prep = pmap_for_my_devices(lambda data, w, mean: jax.vmap(lambda d, w, m: jnp.sqrt(w) * (d - m), in_axes=(0,0,None))(data, w, mean), in_axes=(0, 0, None))
-        _covar_helper = pmap_for_my_devices(
+        _mean_helper = jVMC.global_defs.pmap_for_my_devices(lambda data, w: jnp.tensordot(w, data, axes=(0,0)), in_axes=(0, 0))
+        _data_prep = jVMC.global_defs.pmap_for_my_devices(lambda data, w, mean: jax.vmap(lambda d, w, m: jnp.sqrt(w) * (d - m), in_axes=(0,0,None))(data, w, mean), in_axes=(0, 0, None))
+        _covar_helper = jVMC.global_defs.pmap_for_my_devices(
                                 lambda data1, data2:
                                     jnp.tensordot(
                                         jnp.conj(data1),
                                         data2, axes=(0,0)), 
                                 in_axes=(0, 0)
                                 )
-        _covar_var_helper = pmap_for_my_devices(
+        _covar_var_helper = jVMC.global_defs.pmap_for_my_devices(
                                     lambda data1, data2, w: 
                                         jnp.sum(
                                             jnp.abs( 
                                                 jax.vmap(lambda a,b: jnp.outer(a,b))(jnp.conj(data1), data2),
                                             )**2 / w[...,None,None],
                                             axis=0),
                                     in_axes=(0, 0, 0)
                                     )
-        _covar_data_helper = pmap_for_my_devices(lambda data1, data2, w: jax.vmap(lambda a,b,w: jnp.outer(a,b) / w)(jnp.conj(data1), data2, w), in_axes=(0, 0, 0))
-        _trafo_helper_1 = pmap_for_my_devices(
+        _covar_data_helper = jVMC.global_defs.pmap_for_my_devices(lambda data1, data2, w: jax.vmap(lambda a,b,w: jnp.outer(a,b) / w)(jnp.conj(data1), data2, w), in_axes=(0, 0, 0))
+        _trafo_helper_1 = jVMC.global_defs.pmap_for_my_devices(
                                 lambda data, w, mean, f: f(
                                     jax.vmap(lambda x,y: x/jnp.sqrt(y), in_axes=(0,0))(data, w) 
                                     + mean
                                     ), 
                                 in_axes=(0, 0, None), static_broadcasted_argnums=(3,))
-        _trafo_helper_2 = pmap_for_my_devices(
+        _trafo_helper_2 = jVMC.global_defs.pmap_for_my_devices(
                                 lambda data, w, mean, v, f: 
                                     jnp.matmul(v, 
                                                 f(
                                                 jax.vmap(lambda x,y: x/jnp.sqrt(y), in_axes=(0,0))(data, w) 
                                                 + mean
                                                 )
                                     ), 
                                 in_axes=(0, 0, None, None), static_broadcasted_argnums=(4,))
-        _select_helper = pmap_for_my_devices( lambda ix,g: jax.vmap(lambda ix,g: g[ix], in_axes=(None, 0))(ix,g), in_axes=(None, 0) )
-        _get_subset_helper = pmap_for_my_devices(lambda x, ixs: x[slice(*ixs)], in_axes=(0,), static_broadcasted_argnums=(1,))
-        _subset_mean_helper = pmap_for_my_devices(lambda d, w, m: jnp.tensordot(jnp.sqrt(w), d, axes=(0,0)) + m, in_axes=(0,0,None))
-        _subset_data_prep = pmap_for_my_devices(jax.vmap(lambda d, w, m1, m2: d+jnp.sqrt(w)*(m1-m2), in_axes=(0,0,None,None)), in_axes=(0,0,None,None))
+        _select_helper = jVMC.global_defs.pmap_for_my_devices( lambda ix,g: jax.vmap(lambda ix,g: g[ix], in_axes=(None, 0))(ix,g), in_axes=(None, 0) )
+        _get_subset_helper = jVMC.global_defs.pmap_for_my_devices(lambda x, ixs: x[slice(*ixs)], in_axes=(0,), static_broadcasted_argnums=(1,))
+        _subset_mean_helper = jVMC.global_defs.pmap_for_my_devices(lambda d, w, m: jnp.tensordot(jnp.sqrt(w), d, axes=(0,0)) + m, in_axes=(0,0,None))
+        _subset_data_prep = jVMC.global_defs.pmap_for_my_devices(jax.vmap(lambda d, w, m1, m2: d+jnp.sqrt(w)*(m1-m2), in_axes=(0,0,None,None)), in_axes=(0,0,None,None))
 
 
 class SampledObs():
     """This class implements the computation of statistics from Monte Carlo or exact samples.
 
     Initializer arguments:
         * ``observations``: Observations :math:`O_n` in the sample. The array must have a leading device \
```

### Comparing `jVMC-1.2.2/jVMC/util/minsr.py` & `jVMC-1.2.3/jVMC/util/minsr.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/util/output_manager.py` & `jVMC-1.2.3/jVMC/util/output_manager.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/util/stepper.py` & `jVMC-1.2.3/jVMC/util/stepper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/util/symmetries.py` & `jVMC-1.2.3/jVMC/util/symmetries.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/util/tdvp.py` & `jVMC-1.2.3/jVMC/util/tdvp.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/util/util.py` & `jVMC-1.2.3/jVMC/util/util.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC/vqs.py` & `jVMC-1.2.3/jVMC/vqs.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/jVMC.egg-info/PKG-INFO` & `jVMC-1.2.3/jVMC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jVMC
-Version: 1.2.2
+Version: 1.2.3
 Summary: jVMC: Versatile and performant variational Monte Carlo
 Home-page: https://jvmc.readthedocs.io/en/latest/#
 Author: Markus Schmitt, Moritz Reh
 Author-email: markus.schmitt@uni-koeln.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jVMC-1.2.2/jVMC.egg-info/SOURCES.txt` & `jVMC-1.2.3/jVMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/setup.py` & `jVMC-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/minsr_test.py` & `jVMC-1.2.3/tests/minsr_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/mpi_wrapper_test.py` & `jVMC-1.2.3/tests/mpi_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/nets_test.py` & `jVMC-1.2.3/tests/nets_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/operator_test.py` & `jVMC-1.2.3/tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/povm_test.py` & `jVMC-1.2.3/tests/povm_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/sampler_test.py` & `jVMC-1.2.3/tests/sampler_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/stats_test.py` & `jVMC-1.2.3/tests/stats_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/stepper_test.py` & `jVMC-1.2.3/tests/stepper_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/symmetries_test.py` & `jVMC-1.2.3/tests/symmetries_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/tdvp_test.py` & `jVMC-1.2.3/tests/tdvp_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.2/tests/vqs_test.py` & `jVMC-1.2.3/tests/vqs_test.py`

 * *Files identical despite different names*

