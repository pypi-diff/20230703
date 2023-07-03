# Comparing `tmp/ml-crafter-0.1.0.tar.gz` & `tmp/ml-crafter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-crafter-0.1.0.tar", last modified: Wed Jun 21 16:10:15 2023, max compression
+gzip compressed data, was "ml-crafter-0.1.1.tar", last modified: Mon Jul  3 08:16:20 2023, max compression
```

## Comparing `ml-crafter-0.1.0.tar` & `ml-crafter-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 16:10:15.146909 ml-crafter-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-01 05:36:24.000000 ml-crafter-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      131 2023-06-21 16:10:15.146909 ml-crafter-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-06-21 08:22:15.000000 ml-crafter-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 16:10:15.126448 ml-crafter-0.1.0/ml_crafter/
--rw-rw-rw-   0        0        0        0 2023-05-22 14:10:41.000000 ml-crafter-0.1.0/ml_crafter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:10:15.143905 ml-crafter-0.1.0/ml_crafter/model_monitoring/
--rw-rw-rw-   0        0        0       39 2023-05-22 14:33:06.000000 ml-crafter-0.1.0/ml_crafter/model_monitoring/__init__.py
--rw-rw-rw-   0        0        0     7081 2023-06-21 05:08:46.000000 ml-crafter-0.1.0/ml_crafter/model_monitoring/_population_drift.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:10:15.145913 ml-crafter-0.1.0/ml_crafter/utils/
--rw-rw-rw-   0        0        0        0 2023-05-22 14:10:41.000000 ml-crafter-0.1.0/ml_crafter/utils/__init__.py
--rw-rw-rw-   0        0        0    13911 2023-06-21 16:08:35.000000 ml-crafter-0.1.0/ml_crafter/utils/compare_dataframes.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:10:15.136260 ml-crafter-0.1.0/ml_crafter.egg-info/
--rw-rw-rw-   0        0        0      131 2023-06-21 16:10:15.000000 ml-crafter-0.1.0/ml_crafter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-21 16:10:15.000000 ml-crafter-0.1.0/ml_crafter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 16:10:15.000000 ml-crafter-0.1.0/ml_crafter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-21 16:10:15.000000 ml-crafter-0.1.0/ml_crafter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 16:10:15.000000 ml-crafter-0.1.0/ml_crafter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 16:10:15.146909 ml-crafter-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-21 05:44:39.000000 ml-crafter-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:16:20.829640 ml-crafter-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-01 05:36:24.000000 ml-crafter-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      131 2023-07-03 08:16:20.828644 ml-crafter-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-06-21 08:22:15.000000 ml-crafter-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 08:16:20.814632 ml-crafter-0.1.1/ml_crafter/
+-rw-rw-rw-   0        0        0        0 2023-05-22 14:10:41.000000 ml-crafter-0.1.1/ml_crafter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:16:20.824668 ml-crafter-0.1.1/ml_crafter/data_preprocessing/
+-rw-rw-rw-   0        0        0       47 2023-07-01 05:00:00.000000 ml-crafter-0.1.1/ml_crafter/data_preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     6775 2023-07-03 07:42:27.000000 ml-crafter-0.1.1/ml_crafter/data_preprocessing/_data_types.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:16:20.825653 ml-crafter-0.1.1/ml_crafter/model_monitoring/
+-rw-rw-rw-   0        0        0       39 2023-05-22 14:33:06.000000 ml-crafter-0.1.1/ml_crafter/model_monitoring/__init__.py
+-rw-rw-rw-   0        0        0     7081 2023-06-21 05:08:46.000000 ml-crafter-0.1.1/ml_crafter/model_monitoring/_population_drift.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:16:20.827647 ml-crafter-0.1.1/ml_crafter/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 14:10:41.000000 ml-crafter-0.1.1/ml_crafter/utils/__init__.py
+-rw-rw-rw-   0        0        0    13911 2023-06-21 16:08:35.000000 ml-crafter-0.1.1/ml_crafter/utils/compare_dataframes.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:16:20.822664 ml-crafter-0.1.1/ml_crafter.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-07-03 08:16:20.000000 ml-crafter-0.1.1/ml_crafter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-07-03 08:16:20.000000 ml-crafter-0.1.1/ml_crafter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:16:20.000000 ml-crafter-0.1.1/ml_crafter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 08:16:20.000000 ml-crafter-0.1.1/ml_crafter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-03 08:16:20.000000 ml-crafter-0.1.1/ml_crafter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:16:20.829640 ml-crafter-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-07-03 08:16:06.000000 ml-crafter-0.1.1/setup.py
```

### Comparing `ml-crafter-0.1.0/LICENSE` & `ml-crafter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-crafter-0.1.0/ml_crafter/model_monitoring/_population_drift.py` & `ml-crafter-0.1.1/ml_crafter/model_monitoring/_population_drift.py`

 * *Files identical despite different names*

### Comparing `ml-crafter-0.1.0/ml_crafter/utils/compare_dataframes.py` & `ml-crafter-0.1.1/ml_crafter/utils/compare_dataframes.py`

 * *Files identical despite different names*

