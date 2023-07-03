# Comparing `tmp/uqtestfuns-0.2.0.tar.gz` & `tmp/uqtestfuns-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uqtestfuns-0.2.0.tar", last modified: Mon Jun 26 17:18:56 2023, max compression
+gzip compressed data, was "uqtestfuns-0.3.0.tar", last modified: Mon Jul  3 15:36:51 2023, max compression
```

## Comparing `uqtestfuns-0.2.0.tar` & `uqtestfuns-0.3.0.tar`

### file list

```diff
@@ -1,70 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9012 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.910832 uqtestfuns-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.910832 uqtestfuns-0.2.0/src/uqtestfuns/
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.914831 uqtestfuns-0.2.0/src/uqtestfuns/core/
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.914831 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (122)     8331 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/probabilistic_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     6077 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.918831 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5984 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (122)     6845 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6394 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py
--rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py
--rw-r--r--   0 runner    (1001) docker     (122)     9350 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py
--rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3875 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/uqtestfun.py
--rw-r--r--   0 runner    (1001) docker     (122)    15916 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/uqtestfun_abc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/global_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     8816 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.918831 uqtestfuns-0.2.0/src/uqtestfuns/meta/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    12619 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/metaspec.py
--rw-r--r--   0 runner    (1001) docker     (122)     7364 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/uqmetatestfun.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/
--rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3321 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/ackley.py
--rw-r--r--   0 runner    (1001) docker     (122)     4792 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/borehole.py
--rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/bratley1992.py
--rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/damped_oscillator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/flood.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/forrester.py
--rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/franke.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/gramacy2007.py
--rw-r--r--   0 runner    (1001) docker     (122)     3668 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/ishigami.py
--rw-r--r--   0 runner    (1001) docker     (122)     7421 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/mclain.py
--rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/oakley2002.py
--rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/otl_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/piston.py
--rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sobol_g.py
--rw-r--r--   0 runner    (1001) docker     (122)     7550 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sulfur.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/welch1992.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/wing_weight.py
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.914831 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/tests/test_list_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9012 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.476695 uqtestfuns-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns/
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8331 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/probabilistic_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6077 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.484695 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5984 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6845 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6394 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9350 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3875 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15916 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun_abc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/global_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8816 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.484695 uqtestfuns-0.3.0/src/uqtestfuns/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12619 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/metaspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7364 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/meta/uqmetatestfun.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3321 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ackley.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4792 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/borehole.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/bratley1992.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3753 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/cantilever_beam_2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/circular_pipe_crack.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10303 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/damped_oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/flood.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/forrester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/four_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/franke.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/gayton_hat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/gramacy2007.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/hyper_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3668 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ishigami.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7421 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/mclain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/oakley2002.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/otl_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/piston.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9619 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sobol_g.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/speed_reducer_shaft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7550 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sulfur.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/welch1992.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/test_functions/wing_weight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/src/uqtestfuns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.480695 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2767 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-03 15:36:51.000000 uqtestfuns-0.3.0/src/uqtestfuns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 15:36:51.488695 uqtestfuns-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-07-03 15:36:42.000000 uqtestfuns-0.3.0/tests/test_list_functions.py
```

### Comparing `uqtestfuns-0.2.0/LICENSE` & `uqtestfuns-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/PKG-INFO` & `uqtestfuns-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uqtestfuns
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 Home-page: https://github.com/damar-wicaksono/uqtestfuns
 Author: Damar Wicaksono
 Author-email: damar.wicaksono@outlook.com
 License: MIT
 Platform: ANY
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7703922-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7703922)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8109901-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8109901)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
```

### Comparing `uqtestfuns-0.2.0/README.md` & `uqtestfuns-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7703922-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7703922)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8109901-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8109901)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
```

### Comparing `uqtestfuns-0.2.0/setup.cfg` & `uqtestfuns-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uqtestfuns
-version = 0.2.0
+version = 0.3.0
 url = https://github.com/damar-wicaksono/uqtestfuns
 author = Damar Wicaksono
 author_email = damar.wicaksono@outlook.com
 description = A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 long_description = file: README.md
 long_description_content_type = text/markdown
 platform = ANY
```

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/__init__.py` & `uqtestfuns-0.3.0/src/uqtestfuns/__init__.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/input_spec.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/input_spec.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/probabilistic_input.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/probabilistic_input.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distribution.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distribution.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/utils.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/prob_input/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/uqtestfun.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/uqtestfun_abc.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/uqtestfun_abc.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/core/utils.py` & `uqtestfuns-0.3.0/src/uqtestfuns/core/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/helpers.py` & `uqtestfuns-0.3.0/src/uqtestfuns/helpers.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/meta/basis_functions.py` & `uqtestfuns-0.3.0/src/uqtestfuns/meta/basis_functions.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/meta/metaspec.py` & `uqtestfuns-0.3.0/src/uqtestfuns/meta/metaspec.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/meta/uqmetatestfun.py` & `uqtestfuns-0.3.0/src/uqtestfuns/meta/uqmetatestfun.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/__init__.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 """
 The init for the 'test_functions' subpackage of UQTestFuns.
 """
 from .ackley import Ackley
 from .borehole import Borehole
 from .bratley1992 import Bratley1992a, Bratley1992b, Bratley1992c, Bratley1992d
-from .damped_oscillator import DampedOscillator
+from .cantilever_beam_2d import CantileverBeam2D
+from .circular_pipe_crack import CircularPipeCrack
+from .damped_oscillator import DampedOscillator, DampedOscillatorReliability
 from .flood import Flood
 from .forrester import Forrester2008
+from .four_branch import FourBranch
 from .franke import Franke1, Franke2, Franke3, Franke4, Franke5, Franke6
+from .gayton_hat import GaytonHat
 from .gramacy2007 import Gramacy1DSine
+from .hyper_sphere import HyperSphere
 from .ishigami import Ishigami
 from .oakley2002 import Oakley1D
 from .otl_circuit import OTLCircuit
 from .mclain import McLainS1, McLainS2, McLainS3, McLainS4, McLainS5
 from .piston import Piston
 from .sobol_g import SobolG
+from .speed_reducer_shaft import SpeedReducerShaft
 from .sulfur import Sulfur
 from .welch1992 import Welch1992
 from .wing_weight import WingWeight
 
 # NOTE: Import the new test function implementation class from its respective
 # module manually here and update the list below.
 
 __all__ = [
     "Ackley",
     "Borehole",
     "Bratley1992a",
     "Bratley1992b",
     "Bratley1992c",
     "Bratley1992d",
+    "CantileverBeam2D",
+    "CircularPipeCrack",
     "DampedOscillator",
+    "DampedOscillatorReliability",
     "Flood",
     "Forrester2008",
+    "FourBranch",
     "Franke1",
     "Franke2",
     "Franke3",
     "Franke4",
     "Franke5",
     "Franke6",
+    "GaytonHat",
     "Gramacy1DSine",
+    "HyperSphere",
     "Ishigami",
     "Oakley1D",
     "OTLCircuit",
     "McLainS1",
     "McLainS2",
     "McLainS3",
     "McLainS4",
     "McLainS5",
     "Piston",
     "SobolG",
+    "SpeedReducerShaft",
     "Sulfur",
     "Welch1992",
     "WingWeight",
 ]
```

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/ackley.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ackley.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/borehole.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/borehole.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/bratley1992.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/bratley1992.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/damped_oscillator.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/damped_oscillator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 """
 Module with an implementation of the damped oscillator model.
 
 The damped oscillator model is a seven-dimensional scalar-valued function
 that computes the relative displacement of a secondary spring
 under a white noise base acceleration.
 The model was first proposed in [1] and used in the context of reliability
-analysis in [2] and [3]. Note, however, that the reliability analysis
-variant differs from this base model.
+analysis in, for examples, [2], [3], [4], and [5].
+Note, however, that the reliability analysis variant differs
+from the base model.
 Used in the context of reliability analysis,
 the model also includes additional parameters related to a capacity factor and
 load such that the performance function can be computed.
 
 The damped oscillator model is based on a two-degree-of-freedom
 primary-secondary mechanical system characterized by two masses, two springs,
 and the corresponding damping ratios.
 
 References
 ----------
 1. Takeru Igusa and Armen Der Kiureghian, “Dynamic characterization of
    two‐degree‐of‐freedom equipment‐structure systems,”
    Journal of Engineering Mechanics, vol. 111, no. 1, pp. 1–19, 1985.
    DOI: 10.1061/(ASCE)0733-9399(1985)111:1(1)
-2. Armen Der Kiureghian and Mario De Stefano, “Efficient algorithm for
+2. Armen Der Kiureghian and Mario De Stefano, "An efficient algorithm for
+   second-order reliability analysis," Department of Civil and Environmental
+   Engineering, University of California, Berkeley, UCB/SEMM-90/20, 1990.
+3. Armen Der Kiureghian and Mario De Stefano, “Efficient algorithm for
    second‐order reliability analysis,” Journal of Engineering Mechanics,
    vol. 117, no. 12, pp. 2904–2923, 1991.
    DOI: 10.1061/(ASCE)0733-9399(1991)117:12(2904)
-3. Vincent Dubourg, “Adaptive surrogate models for reliability analysis
+4. J.-M. Bourinet, F. Deheeger, and M. Lemaire, “Assessing small failure
+   probabilities by combined subset simulation and Support Vector Machines,”
+   Structural Safety, vol. 33, no. 6, pp. 343–353, 2011.
+   DOI: 10.1016/j.strusafe.2011.06.001.
+5. Vincent Dubourg, “Adaptive surrogate models for reliability analysis
    and reliability-based design optimization,”
    Université Blaise Pascal - Clermont II, Clermont-Ferrand, France, 2011.
    URL: https://sites.google.com/site/vincentdubourg/phd-thesis
 """
 import numpy as np
 
 from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
 from .utils import lognorm2norm_mean, lognorm2norm_std
 
-__all__ = ["DampedOscillator"]
+__all__ = ["DampedOscillator", "DampedOscillatorReliability"]
 
 INPUT_MARGINALS_DERKIUREGHIAN1991 = [  # From [2]
     UnivDistSpec(
         name="Mp",
         distribution="lognormal",
         parameters=[
             lognorm2norm_mean(1.5, 0.1 * 1.5),
@@ -100,27 +108,96 @@
             lognorm2norm_mean(100.0, 0.1 * 100.0),
             lognorm2norm_std(100.0, 0.1 * 100.0),
         ],
         description="White noise base acceleration",
     ),
 ]
 
-AVAILABLE_INPUT_SPECS = {
+AVAILABLE_INPUT_SPECS_BASE = {
     "DerKiureghian1991": ProbInputSpecFixDim(
         name="DampedOscillator-DerKiureghian1991",
         description=(
             "Probabilistic input model for the Damped Oscillator model "
             "from Der Kiureghian and De Stefano (1991)."
         ),
         marginals=INPUT_MARGINALS_DERKIUREGHIAN1991,
         copulas=None,
     ),
 }
 
 
+AVAILABLE_INPUT_SPECS_RELIABILITY = {
+    "DerKiureghian1990a": ProbInputSpecFixDim(
+        name="DampedOscillatorReliability-DerKiureghian1990a",
+        description=(
+            "Input model #1 for the damped oscillator reliability "
+            "from Der Kiureghian and De Stefano (1990)"
+        ),
+        marginals=INPUT_MARGINALS_DERKIUREGHIAN1991
+        + [
+            UnivDistSpec(
+                name="Fs",
+                distribution="lognormal",
+                parameters=[
+                    lognorm2norm_mean(15.0, 0.1 * 15.0),
+                    lognorm2norm_std(15.0, 0.1 * 15.0),
+                ],
+                description="Force capacity of the secondary spring",
+            ),
+        ],
+        copulas=None,
+    ),
+    "DerKiureghian1990b": ProbInputSpecFixDim(
+        name="DampedOscillatorReliability-DerKiureghian1990b",
+        description=(
+            "Input model #2 for the damped oscillator reliability "
+            "from Der Kiureghian and De Stefano (1990)"
+        ),
+        marginals=INPUT_MARGINALS_DERKIUREGHIAN1991
+        + [
+            UnivDistSpec(
+                name="Fs",
+                distribution="lognormal",
+                parameters=[
+                    lognorm2norm_mean(21.5, 0.1 * 21.5),
+                    lognorm2norm_std(21.5, 0.1 * 21.5),
+                ],
+                description="Force capacity of the secondary spring",
+            ),
+        ],
+        copulas=None,
+    ),
+    "DerKiureghian1990c": ProbInputSpecFixDim(
+        name="DampedOscillatorReliability-DerKiureghian1990c",
+        description=(
+            "Input model #3 for the damped oscillator reliability "
+            "from Der Kiureghian and De Stefano (1990)"
+        ),
+        marginals=INPUT_MARGINALS_DERKIUREGHIAN1991
+        + [
+            UnivDistSpec(
+                name="Fs",
+                distribution="lognormal",
+                parameters=[
+                    lognorm2norm_mean(27.5, 0.1 * 27.5),
+                    lognorm2norm_std(27.5, 0.1 * 27.5),
+                ],
+                description="Force capacity of the secondary spring",
+            ),
+        ],
+        copulas=None,
+    ),
+}
+
+# peak factor
+AVAILABLE_PARAMETERS_RELIABILITY = {
+    "DerKiureghian1990": 3,
+}
+
+
 def evaluate(xx: np.ndarray) -> np.ndarray:
     """Evaluate the rms displacement of the damped oscillator model.
 
     Parameters
     ----------
     xx : np.ndarray
         A 7-dimensional input values given by an N-by-7 array
@@ -175,12 +252,57 @@
 class DampedOscillator(UQTestFunABC):
     """A concrete implementation of the Damped oscillator test function."""
 
     _tags = ["metamodeling", "sensitivity"]
     _description = (
         "Damped oscillator model from Igusa and Der Kiureghian (1985)"
     )
-    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_inputs = AVAILABLE_INPUT_SPECS_BASE
     _available_parameters = None
     _default_spatial_dimension = 8
 
     eval_ = staticmethod(evaluate)
+
+
+def evaluate_reliability(xx: np.ndarray, parameters: float):
+    """Evaluate the performance function of the system reliability.
+
+    Parameters
+    ----------
+    xx : np.ndarray
+        An 8-dimensional input values given by an N-by-7 array
+        where N is the number of input values.
+    parameters : float
+        The peak factor of the system.
+
+    Returns
+    -------
+    np.ndarray
+        The system's performance evaluation. If less than or equal to zero,
+        the system is in failed state.
+        The output is a 1-dimensional array of length N.
+    """
+    rms_disp = evaluate(xx[:, :-1])  # root-mean-square displacement
+    kk_s = xx[:, 3]  # Secondary spring stiffness
+    ff_s = xx[:, -1]  # Force capacity of the secondary spring
+
+    pf = parameters  # peak factor
+
+    yy = ff_s - pf * kk_s * rms_disp
+
+    return yy
+
+
+class DampedOscillatorReliability(UQTestFunABC):
+    """A concrete implementation of the Damped oscillator reliability func."""
+
+    _tags = ["reliability"]
+    _description = (
+        "Performance function from Der Kiureghian and De Stefano (1990)"
+    )
+    _available_inputs = AVAILABLE_INPUT_SPECS_RELIABILITY
+    _available_parameters = AVAILABLE_PARAMETERS_RELIABILITY
+    _default_spatial_dimension = 8
+    _default_input = "DerKiureghian1990a"
+    _default_parameters = "DerKiureghian1990"
+
+    eval_ = staticmethod(evaluate_reliability)
```

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/flood.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/flood.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/forrester.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/forrester.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/franke.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/franke.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/gramacy2007.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/gramacy2007.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/ishigami.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/ishigami.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/mclain.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/mclain.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/oakley2002.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/oakley2002.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/otl_circuit.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/otl_circuit.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/piston.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/piston.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sobol_g.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sobol_g.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,26 +90,26 @@
             )
         )
 
     return marginals
 
 
 AVAILABLE_INPUT_SPECS = {
-    "Radovic1996": ProbInputSpecVarDim(
-        name="Sobol-G-Radovic-1996",
+    "Saltelli1995": ProbInputSpecVarDim(
+        name="Sobol-G-Saltelli1995",
         description=(
             "Probabilistic input model for the Sobol'-G function "
-            "from Radović et al. (1996)."
+            "from Saltelli and Sobol' (1995)"
         ),
         marginals_generator=_create_sobol_input,
         copulas=None,
     ),
 }
 
-DEFAULT_INPUT_SELECTION = "Radovic1996"
+DEFAULT_INPUT_SELECTION = "Saltelli1995"
 
 
 def _get_params_saltelli_1995_1(spatial_dimension: int) -> np.ndarray:
     """Construct a parameter array for Sobol'-G according to example 1 in [4].
 
     Notes
     -----
```

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sulfur.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/sulfur.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/welch1992.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/welch1992.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/wing_weight.py` & `uqtestfuns-0.3.0/src/uqtestfuns/test_functions/wing_weight.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns/utils.py` & `uqtestfuns-0.3.0/src/uqtestfuns/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns.egg-info/PKG-INFO` & `uqtestfuns-0.3.0/src/uqtestfuns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uqtestfuns
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 Home-page: https://github.com/damar-wicaksono/uqtestfuns
 Author: Damar Wicaksono
 Author-email: damar.wicaksono@outlook.com
 License: MIT
 Platform: ANY
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7703922-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7703922)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.8109901-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.8109901)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
```

### Comparing `uqtestfuns-0.2.0/src/uqtestfuns.egg-info/SOURCES.txt` & `uqtestfuns-0.3.0/src/uqtestfuns.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,23 +37,29 @@
 src/uqtestfuns/meta/basis_functions.py
 src/uqtestfuns/meta/metaspec.py
 src/uqtestfuns/meta/uqmetatestfun.py
 src/uqtestfuns/test_functions/__init__.py
 src/uqtestfuns/test_functions/ackley.py
 src/uqtestfuns/test_functions/borehole.py
 src/uqtestfuns/test_functions/bratley1992.py
+src/uqtestfuns/test_functions/cantilever_beam_2d.py
+src/uqtestfuns/test_functions/circular_pipe_crack.py
 src/uqtestfuns/test_functions/damped_oscillator.py
 src/uqtestfuns/test_functions/flood.py
 src/uqtestfuns/test_functions/forrester.py
+src/uqtestfuns/test_functions/four_branch.py
 src/uqtestfuns/test_functions/franke.py
+src/uqtestfuns/test_functions/gayton_hat.py
 src/uqtestfuns/test_functions/gramacy2007.py
+src/uqtestfuns/test_functions/hyper_sphere.py
 src/uqtestfuns/test_functions/ishigami.py
 src/uqtestfuns/test_functions/mclain.py
 src/uqtestfuns/test_functions/oakley2002.py
 src/uqtestfuns/test_functions/otl_circuit.py
 src/uqtestfuns/test_functions/piston.py
 src/uqtestfuns/test_functions/sobol_g.py
+src/uqtestfuns/test_functions/speed_reducer_shaft.py
 src/uqtestfuns/test_functions/sulfur.py
 src/uqtestfuns/test_functions/utils.py
 src/uqtestfuns/test_functions/welch1992.py
 src/uqtestfuns/test_functions/wing_weight.py
 tests/test_list_functions.py
```

### Comparing `uqtestfuns-0.2.0/tests/test_list_functions.py` & `uqtestfuns-0.3.0/tests/test_list_functions.py`

 * *Files identical despite different names*

