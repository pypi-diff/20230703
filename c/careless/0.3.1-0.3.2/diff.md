# Comparing `tmp/careless-0.3.1.tar.gz` & `tmp/careless-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "careless-0.3.1.tar", last modified: Tue Jun 27 21:50:16 2023, max compression
+gzip compressed data, was "careless-0.3.2.tar", last modified: Mon Jul  3 15:35:51 2023, max compression
```

## Comparing `careless-0.3.1.tar` & `careless-0.3.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 21:50:03.000000 careless-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 21:50:03.000000 careless-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-27 21:50:16.425697 careless-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-27 21:50:03.000000 careless-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.417697 careless-0.3.1/careless/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 21:50:03.000000 careless-0.3.1/careless/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 21:50:03.000000 careless-0.3.1/careless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/args/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/filtration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/tf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 21:50:03.000000 careless-0.3.1/careless/callbacks/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4879 2023-06-27 21:50:03.000000 careless-0.3.1/careless/careless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/asu.py
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/xds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/mono.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/merging/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/merging/surrogate_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/merging/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/wilson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-06-27 21:50:03.000000 careless-0.3.1/careless/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/prior_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/rsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/careless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/shame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.417697 careless-0.3.1/careless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-06-27 21:50:03.000000 careless-0.3.1/scripts/make_difference_map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-06-27 21:50:03.000000 careless-0.3.1/scripts/stream2mtz
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-27 21:50:16.425697 careless-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-27 21:50:03.000000 careless-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-27 21:50:03.000000 careless-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-27 21:50:03.000000 careless-0.3.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-03 15:35:37.000000 careless-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 15:35:37.000000 careless-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-03 15:35:51.123209 careless-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-03 15:35:37.000000 careless-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.115202 careless-0.3.2/careless/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 15:35:37.000000 careless-0.3.2/careless/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 15:35:37.000000 careless-0.3.2/careless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/args/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/filtration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 15:35:37.000000 careless-0.3.2/careless/args/tf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 15:35:37.000000 careless-0.3.2/careless/callbacks/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4879 2023-07-03 15:35:37.000000 careless-0.3.2/careless/careless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/asu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-03 15:35:37.000000 careless-0.3.2/careless/io/xds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/likelihoods/mono.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/merging/surrogate_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/merging/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.119205 careless-0.3.2/careless/models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/priors/wilson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/careless/models/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-03 15:35:37.000000 careless-0.3.2/careless/models/scaling/nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-03 15:35:37.000000 careless-0.3.2/careless/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/careless/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/prior_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-03 15:35:37.000000 careless-0.3.2/careless/stats/rsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/careless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-03 15:35:37.000000 careless-0.3.2/careless/utils/shame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.115202 careless-0.3.2/careless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-03 15:35:51.000000 careless-0.3.2/careless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 15:35:50.000000 careless-0.3.2/careless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-03 15:35:37.000000 careless-0.3.2/scripts/make_difference_map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-03 15:35:37.000000 careless-0.3.2/scripts/stream2mtz
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 15:35:51.123209 careless-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-03 15:35:37.000000 careless-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:51.123209 careless-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:35:37.000000 careless-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-03 15:35:37.000000 careless-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-03 15:35:37.000000 careless-0.3.2/tests/test_cli.py
```

### Comparing `careless-0.3.1/LICENSE` & `careless-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/PKG-INFO` & `careless-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.1
+Version: 0.3.2
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.1/README.md` & `careless-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/common.py` & `careless-0.3.2/careless/args/common.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/crossvalidation.py` & `careless-0.3.2/careless/args/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/filtration.py` & `careless-0.3.2/careless/args/filtration.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/interpretation.py` & `careless-0.3.2/careless/args/interpretation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/optimizer.py` & `careless-0.3.2/careless/args/optimizer.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/poly.py` & `careless-0.3.2/careless/args/poly.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/positional_encoding.py` & `careless-0.3.2/careless/args/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/prior.py` & `careless-0.3.2/careless/args/prior.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/required.py` & `careless-0.3.2/careless/args/required.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/scaling.py` & `careless-0.3.2/careless/args/scaling.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/args/tf_options.py` & `careless-0.3.2/careless/args/tf_options.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/callbacks/progress_bar.py` & `careless-0.3.2/careless/callbacks/progress_bar.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/careless.py` & `careless-0.3.2/careless/careless.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/io/asu.py` & `careless-0.3.2/careless/io/asu.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/io/formatter.py` & `careless-0.3.2/careless/io/formatter.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/io/manager.py` & `careless-0.3.2/careless/io/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
         refl_id = BaseModel.get_refl_id(inputs)
         iobs = BaseModel.get_intensities(inputs).flatten()
         sig_iobs = BaseModel.get_uncertainties(inputs).flatten()
         asu_id,H = self.asu_collection.to_asu_id_and_miller_index(refl_id)
         #ipred = model(inputs)
         ipred,sigipred = model.prediction_mean_stddev(inputs)
-        scale,sigscale = model.prediction_mean_stddev(inputs)
+        scale,sigscale = model.scale_mean_stddev(inputs)
 
         h,k,l = H.T
         results = ()
         for i,asu in enumerate(self.asu_collection):
             idx = asu_id == i
             idx = idx.flatten()
             output = rs.DataSet({
```

### Comparing `careless-0.3.1/careless/io/xds.py` & `careless-0.3.2/careless/io/xds.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/base.py` & `careless-0.3.2/careless/models/base.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/likelihoods/laue.py` & `careless-0.3.2/careless/models/likelihoods/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/likelihoods/mono.py` & `careless-0.3.2/careless/models/likelihoods/mono.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/merging/surrogate_posteriors.py` & `careless-0.3.2/careless/models/merging/surrogate_posteriors.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/merging/variational.py` & `careless-0.3.2/careless/models/merging/variational.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.likelihood = likelihood
         self.scaling_model = scaling_model
         self.mc_sample_size = mc_sample_size
         self.kl_weight = kl_weight
         self.scale_kl_weight = scale_kl_weight
         self.scale_prior = scale_prior
 
-    def scale_mean_sttdev(self, inputs):
+    def scale_mean_stddev(self, inputs):
         """
         Compute the moments of the posterior of reflection observation scale factors. 
 
         Parameters
         ----------
         inputs : data
             inputs is a data structure like [refl_id, image_id, metadata, intensity, uncertainty].
```

### Comparing `careless-0.3.1/careless/models/priors/empirical.py` & `careless-0.3.2/careless/models/priors/empirical.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/priors/wilson.py` & `careless-0.3.2/careless/models/priors/wilson.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/scaling/image.py` & `careless-0.3.2/careless/models/scaling/image.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/models/scaling/nn.py` & `careless-0.3.2/careless/models/scaling/nn.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/parser.py` & `careless-0.3.2/careless/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/ccanom.py` & `careless-0.3.2/careless/stats/ccanom.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/cchalf.py` & `careless-0.3.2/careless/stats/cchalf.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/ccpred.py` & `careless-0.3.2/careless/stats/ccpred.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/completeness.py` & `careless-0.3.2/careless/stats/completeness.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/parser.py` & `careless-0.3.2/careless/stats/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/prior_b.py` & `careless-0.3.2/careless/stats/prior_b.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/rescale.py` & `careless-0.3.2/careless/stats/rescale.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/stats/rsplit.py` & `careless-0.3.2/careless/stats/rsplit.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/utils/distributions.py` & `careless-0.3.2/careless/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/utils/laue.py` & `careless-0.3.2/careless/utils/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless/utils/positional_encoding.py` & `careless-0.3.2/careless/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/careless.egg-info/PKG-INFO` & `careless-0.3.2/careless.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.1
+Version: 0.3.2
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.1/careless.egg-info/SOURCES.txt` & `careless-0.3.2/careless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/scripts/make_difference_map` & `careless-0.3.2/scripts/make_difference_map`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/scripts/stream2mtz` & `careless-0.3.2/scripts/stream2mtz`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/setup.py` & `careless-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/tests/conftest.py` & `careless-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.1/tests/test_cli.py` & `careless-0.3.2/tests/test_cli.py`

 * *Files identical despite different names*

