# Comparing `tmp/msgram_core-1.3.1.tar.gz` & `tmp/msgram_core-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram_core-1.3.1.tar", last modified: Sat Jun 24 19:59:32 2023, max compression
+gzip compressed data, was "msgram_core-1.3.2.tar", last modified: Mon Jul  3 01:03:15 2023, max compression
```

## Comparing `msgram_core-1.3.1.tar` & `msgram_core-1.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-06-24 19:59:13.000000 msgram_core-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-24 19:59:32.770504 msgram_core-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-24 19:59:13.000000 msgram_core-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-24 19:59:13.000000 msgram_core-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:59:32.770504 msgram_core-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/aggregated_normalized_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/measures_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/core/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/msgram_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 19:59:32.000000 msgram_core-1.3.1/src/msgram_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.766504 msgram_core-1.3.1/src/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/parsers/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/src/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/resources/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/src/staticfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/default_pre_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/sonarqube_available_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/staticfiles/sonarqube_supported_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-24 19:59:13.000000 msgram_core-1.3.1/src/util/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:59:32.770504 msgram_core-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-24 19:59:13.000000 msgram_core-1.3.1/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-07-03 01:02:54.000000 msgram_core-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-07-03 01:03:15.515213 msgram_core-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-03 01:02:54.000000 msgram_core-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 01:02:54.000000 msgram_core-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:03:15.515213 msgram_core-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.511213 msgram_core-1.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.511213 msgram_core-1.3.2/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/aggregated_normalized_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/measures_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/core/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.511213 msgram_core-1.3.2/src/msgram_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 01:03:15.000000 msgram_core-1.3.2/src/msgram_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/parsers/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/resources/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/default_pre_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/sonarqube_available_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/staticfiles/sonarqube_supported_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 01:02:54.000000 msgram_core-1.3.2/src/util/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:03:15.515213 msgram_core-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-03 01:02:54.000000 msgram_core-1.3.2/tests/test_helpers.py
```

### Comparing `msgram_core-1.3.1/LICENSE` & `msgram_core-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/PKG-INFO` & `msgram_core-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram_core
-Version: 1.3.1
+Version: 1.3.2
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.3.1/README.md` & `msgram_core-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/pyproject.toml` & `msgram_core-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram_core"
-version = "1.3.1"
+version = "1.3.2"
 description = "The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `msgram_core-1.3.1/src/core/aggregated_normalized_measures.py` & `msgram_core-1.3.2/src/core/aggregated_normalized_measures.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import core.measures_functions as ems_functions
 import core.transformations as transformations
 from util.check import Checker
 
 
 def non_complex_files_density(
     data_frame,
-    min_complex_files_density: float = 0,
-    max_complex_files_density: float = 10,
+    min_threshold: float = 0,
+    max_threshold: float = 10,
 ):
     """
     Calculates non-complex files density.
     This function calculates non-complex files density measure
     used to assess the changeability quality subcharacteristic.
 
     This function gets the dataframe metrics
@@ -24,222 +24,206 @@
     Checker.check_metric_values(files_complexity, "complexity")
     Checker.check_metric_values(files_functions, "functions")
 
     if len(files_complexity) == len(files_functions) == 0:
         return 0.0
 
     Checker.check_threshold(
-        min_complex_files_density,
-        max_complex_files_density,
+        min_threshold,
+        max_threshold,
         "non_complex_files_density",
     )
 
     (
         complex_files_density,
         number_of_files,
     ) = ems_functions.get_non_complex_files_density(
         data={
             "complexity": files_complexity,
             "functions": files_functions,
         }
     )
 
-    files_in_thresholds_bool_index = complex_files_density <= max_complex_files_density
+    files_in_thresholds_bool_index = complex_files_density <= max_threshold
     files_functions_gt_zero_bool_index = files_functions > 0
-    x = complex_files_density[
-        files_in_thresholds_bool_index * files_functions_gt_zero_bool_index
-    ]
+    x = complex_files_density[files_in_thresholds_bool_index * files_functions_gt_zero_bool_index]
 
     interpretation_function_value = transformations.interpretation_function(
         x=x,
-        min_threshold=min_complex_files_density,
-        max_threshold=max_complex_files_density,
+        min_threshold=min_threshold,
+        max_threshold=max_threshold,
         gain_interpretation=-1,
     )
 
     aggregated_and_normalized_measure = transformations.calculate_measure(
         interpretation_function_value, number_of_files
     )
     return aggregated_and_normalized_measure
 
 
-def commented_files_density(
-    data_frame, min_comment_density: float = 10, max_comment_density: float = 30
-):
+def commented_files_density(data_frame, min_threshold: float = 10, max_threshold: float = 30):
     """
     Calculates commented files density.
 
     This function gets the dataframe metrics
     and returns the commented files density measure.
     """
     files_comment_lines_density = data_frame["comment_lines_density"]
 
     Checker.check_metric_values(files_comment_lines_density, "comment_lines_density")
 
     if len(files_comment_lines_density) == 0:
         return 0.0
 
-    Checker.check_threshold(
-        min_comment_density, max_comment_density, "comment_files_density"
-    )
+    Checker.check_threshold(min_threshold, max_threshold, "comment_files_density")
 
     (
         files_comment_lines_density,
         number_of_files,
     ) = ems_functions.get_commented_files_density(
         data={
             "comment_lines_density": files_comment_lines_density,
         }
     )
 
     x = files_comment_lines_density[
         files_comment_lines_density.between(
-            min_comment_density,
-            max_comment_density,
+            min_threshold,
+            max_threshold,
             inclusive="both",
         )
     ]
     interpretation_function_value = transformations.interpretation_function(
         x=x,
-        min_threshold=min_comment_density,
-        max_threshold=max_comment_density,
+        min_threshold=min_threshold,
+        max_threshold=max_threshold,
         gain_interpretation=-1,
     )
     aggregated_and_normalized_measure = transformations.calculate_measure(
         interpretation_function_value, number_of_files
     )
     return aggregated_and_normalized_measure
 
 
-def absence_of_duplications(
-    data_frame, min_duplicated_lines: float = 0, max_duplicated_lines: float = 5.0
-):
+def absence_of_duplications(data_frame, min_threshold: float = 0, max_threshold: float = 5.0):
     """
     Calculates duplicated files absence (em3).
 
     This function gets the dataframe metrics
     and returns the duplicated files absence measure (em3).
     """
     files_duplicated_lines_density = data_frame["duplicated_lines_density"]  # m5 metric
 
-    Checker.check_metric_values(
-        files_duplicated_lines_density, "duplicated_lines_density"
-    )
+    Checker.check_metric_values(files_duplicated_lines_density, "duplicated_lines_density")
 
     if len(files_duplicated_lines_density) == 0:
         return 0.0
 
-    Checker.check_threshold(
-        min_duplicated_lines, max_duplicated_lines, "absence_of_duplications"
-    )
+    Checker.check_threshold(min_threshold, max_threshold, "absence_of_duplications")
 
     (
         files_duplicated_lines_density,
         number_of_files,
     ) = ems_functions.get_absence_of_duplications(
         data={"duplicated_lines_density": files_duplicated_lines_density},
     )
 
-    x = files_duplicated_lines_density[
-        files_duplicated_lines_density <= max_duplicated_lines
-    ]
+    x = files_duplicated_lines_density[files_duplicated_lines_density <= max_threshold]
 
     interpretation_function_value = transformations.interpretation_function(
         x=x,
-        min_threshold=min_duplicated_lines,
-        max_threshold=max_duplicated_lines,
+        min_threshold=min_threshold,
+        max_threshold=max_threshold,
         gain_interpretation=-1,
     )
     aggregated_and_normalized_measure = transformations.calculate_measure(
         interpretation_function_value, number_of_files
     )
     return aggregated_and_normalized_measure
 
 
 def test_coverage(
     data_frame,
-    min_coverage: float = 60,
-    max_coverage: float = 100,
+    min_threshold: float = 60,
+    max_threshold: float = 100,
 ):
     """
     Calculates test coverage (em6).
 
     This function gets the dataframe metrics
     and returns the test coverage measure (em6).
     """
     coverage = data_frame["coverage"]  # m6 metric
 
     Checker.check_metric_values(coverage, "coverage")
 
     if len(coverage) == 0:
         return 0.0
 
-    Checker.check_threshold(min_coverage, max_coverage, "test_coverage")
+    Checker.check_threshold(min_threshold, max_threshold, "test_coverage")
 
     coverage, number_of_files = ems_functions.get_test_coverage(
         data={"coverage": coverage},
     )
-    x = coverage[coverage >= min_coverage]
+    x = coverage[coverage >= min_threshold]
     interpretation_function_value = transformations.interpretation_function(
         x=x,
-        min_threshold=min_coverage,
-        max_threshold=max_coverage,
+        min_threshold=min_threshold,
+        max_threshold=max_threshold,
         gain_interpretation=1,
     )
     aggregated_and_normalized_measure = transformations.calculate_measure(
         interpretation_function_value, number_of_files
     )
     return aggregated_and_normalized_measure
 
 
-def fast_test_builds(
-    data_frame, min_fast_test_time: float = 0, max_fast_test_time: float = 300000
-):
+def fast_test_builds(data_frame, min_threshold: float = 0, max_threshold: float = 300000):
     """
     Calculates fast test builds (em5)
     This function gets the dataframe metrics
     and returns the fast test builds measure (em5).
     """
     test_execution_time = data_frame["test_execution_time"]
     tests = data_frame["tests"]
 
     Checker.check_metric_values(test_execution_time, "test_execution_time")
     Checker.check_metric_values(tests, "tests")
 
     if len(test_execution_time) == len(tests) == 0:
         return 0.0
 
-    Checker.check_threshold(min_fast_test_time, max_fast_test_time, "fast_test_builds")
+    Checker.check_threshold(min_threshold, max_threshold, "fast_test_builds")
 
     (
         execution_time,
         number_of_files,
         number_of_tests,
     ) = ems_functions.get_fast_test_builds(
         data={"test_execution_time": test_execution_time, "tests": tests},
     )
 
-    execution_between_thresholds = execution_time[execution_time <= max_fast_test_time]
+    execution_between_thresholds = execution_time[execution_time <= max_threshold]
     x = np.divide(execution_between_thresholds, number_of_tests)
 
     interpretation_function_value = transformations.interpretation_function(
         x=x,
-        min_threshold=min_fast_test_time,
-        max_threshold=max_fast_test_time,
+        min_threshold=min_threshold,
+        max_threshold=max_threshold,
         gain_interpretation=-1,
     )
 
     aggregated_and_normalized_measure = transformations.calculate_measure(
         interpretation_function_value, number_of_files
     )
 
     return aggregated_and_normalized_measure
 
 
-def passed_tests(data_frame, min_passed_tests: float = 0, max_passed_tests: float = 1):
+def passed_tests(data_frame, min_threshold: float = 0, max_threshold: float = 1):
     """
     Calculates passed tests (em4)
 
     This function gets the dataframe metrics
     and returns the passed tests measure (em4).
     """
 
@@ -249,31 +233,29 @@
 
     Checker.check_metric_values(tests, "tests")
     if len(tests) == 0:
         return 0.0
     Checker.check_metric_value(test_failures, "test_failures")
     Checker.check_metric_value(test_errors, "test_errors")
 
-    Checker.check_threshold(min_passed_tests, max_passed_tests, "passed_tests")
+    Checker.check_threshold(min_threshold, max_threshold, "passed_tests")
 
     number_of_tests, number_of_fail_tests = ems_functions.get_passed_tests(
         data={
             "tests": tests,
             "test_errors": float(test_errors),
             "test_failures": float(test_failures),
         }
     )
 
     x = np.divide((number_of_tests - number_of_fail_tests), number_of_tests)
 
     interpretation_function_value = transformations.interpretation_function(
         x=x,
-        min_threshold=min_passed_tests,
-        max_threshold=max_passed_tests,
+        min_threshold=min_threshold,
+        max_threshold=max_threshold,
         gain_interpretation=1,
     )
 
-    aggregated_and_normalized_measure = transformations.calculate_measure(
-        interpretation_function_value
-    )
+    aggregated_and_normalized_measure = transformations.calculate_measure(interpretation_function_value)
 
     return aggregated_and_normalized_measure
```

### Comparing `msgram_core-1.3.1/src/core/measures_functions.py` & `msgram_core-1.3.2/src/core/measures_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/src/core/schemas.py` & `msgram_core-1.3.2/src/core/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,24 +71,20 @@
                 ]
             },
             ...
         ]
     }
     """
 
-    subcharacteristics = fields.List(
-        fields.Nested(SubCharacteristicSchema), required=True
-    )
+    subcharacteristics = fields.List(fields.Nested(SubCharacteristicSchema), required=True)
 
 
 class CharacteristicSchema(Schema):
     key = fields.Str(required=True)
-    subcharacteristics = fields.List(
-        fields.Nested(CalculatedSubEntitySchema), required=True
-    )
+    subcharacteristics = fields.List(fields.Nested(CalculatedSubEntitySchema), required=True)
 
 
 class CalculateCharacteristicSchema(Schema):
     """
     {
         "characteristics": [
             {
@@ -108,17 +104,15 @@
     """
 
     characteristics = fields.List(fields.Nested(CharacteristicSchema), required=True)
 
 
 class TSQMISchema(Schema):
     key = fields.Str(required=True)
-    characteristics = fields.List(
-        fields.Nested(CalculatedSubEntitySchema), required=True
-    )
+    characteristics = fields.List(fields.Nested(CalculatedSubEntitySchema), required=True)
 
 
 class CalculateTSQMISchema(Schema):
     """
     {
         "tsqmi": {
             "key": "tsqmi",
@@ -197,13 +191,9 @@
 
 class TeamThroughputSchema(Schema):
     """
     "key": "team_throughput",
     "function": calculate_em7
     """
 
-    number_of_resolved_issues_with_US_label_in_the_last_x_days = fields.Integer(
-        required=True
-    )
-    total_number_of_issues_with_US_label_in_the_last_x_days = fields.Integer(
-        required=True
-    )
+    number_of_resolved_issues_with_US_label_in_the_last_x_days = fields.Integer(required=True)
+    total_number_of_issues_with_US_label_in_the_last_x_days = fields.Integer(required=True)
```

### Comparing `msgram_core-1.3.1/src/core/transformations.py` & `msgram_core-1.3.2/src/core/transformations.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/src/msgram_core.egg-info/PKG-INFO` & `msgram_core-1.3.2/src/msgram_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-core
-Version: 1.3.1
+Version: 1.3.2
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram_core-1.3.1/src/msgram_core.egg-info/SOURCES.txt` & `msgram_core-1.3.2/src/msgram_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/src/parsers/sonarqube.py` & `msgram_core-1.3.2/src/parsers/sonarqube.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/src/resources/analysis.py` & `msgram_core-1.3.2/src/resources/analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,25 +10,21 @@
 from core.transformations import calculate_aggregated_weighted_value
 from util.constants import AGGREGATED_NORMALIZED_MEASURES_MAPPING
 from util.exceptions import MeasureKeyNotSupported
 
 
 def calculate_measures(
     extracted_measures: CalculateMeasureSchema,
-    config: dict = {
-        "characteristics": [{"subcharacteristics": [{"measures": [{"key": ""}]}]}]
-    },
+    config: dict = {"characteristics": [{"subcharacteristics": [{"measures": [{"key": ""}]}]}]},
 ):
     # Validate if outter keys is valid
     try:
         data = CalculateMeasureSchema().load(extracted_measures)
     except ValidationError as error:
-        raise ValidationError(
-            f"error: Failed to validate input.\nschema_errors: {error.messages}"
-        )
+        raise ValidationError(f"error: Failed to validate input.\nschema_errors: {error.messages}")
 
     # Objeto retornado em caso de sucesso
     result_data = {"measures": []}
 
     valid_measures = AGGREGATED_NORMALIZED_MEASURES_MAPPING.keys()
 
     for measure in data["measures"]:
@@ -43,33 +39,31 @@
         try:
             validated_params = schema().load(measure_params)
         except ValidationError as exc:
             raise ValidationError(
                 f"error: Metric parameters {measure_key} are not valid.\nschema_errors: {exc.messages}"
             )
 
-        aggregated_normalized_measure = AGGREGATED_NORMALIZED_MEASURES_MAPPING[
-            measure_key
-        ]["aggregated_normalized_measure"]
+        aggregated_normalized_measure = AGGREGATED_NORMALIZED_MEASURES_MAPPING[measure_key][
+            "aggregated_normalized_measure"
+        ]
 
         measures = [
             measure
             for characteristic in config["characteristics"]
             for subcharacteristic in characteristic["subcharacteristics"]
             for measure in subcharacteristic["measures"]
         ]
 
         threshold_config = {
             key: value
             for measure in measures
             for key, value in measure.items()
-            if measure["key"] == measure_key
-            and key in AGGREGATED_NORMALIZED_MEASURES_MAPPING[measure_key]["thresholds"]
+            if measure["key"] == measure_key and ("min_threshold" == key or "max_threshold" == key)
         }
-
         result = aggregated_normalized_measure(validated_params, **threshold_config)
 
         result_data["measures"].append(
             {
                 "key": measure_key,
                 "value": result,
             }
@@ -78,30 +72,26 @@
     return result_data
 
 
 def calculate_subcharacteristics(extracted_subcharacteristics):
     try:
         data = CalculateSubCharacteristicSchema().load(extracted_subcharacteristics)
     except ValidationError as error:
-        raise ValidationError(
-            f"error: Failed to validate input.\nschema_errors: {error.messages}"
-        )
+        raise ValidationError(f"error: Failed to validate input.\nschema_errors: {error.messages}")
 
     result_data = {"subcharacteristics": []}
 
     for subcharacteristic in data["subcharacteristics"]:
         subcharacteristic_key: str = subcharacteristic["key"]
 
         vector_aggregated_normalized_measure = np.array([])
         vector_weight_aggregated_normalized_measure = np.array([])
 
         for measure in subcharacteristic["measures"]:
-            vector_aggregated_normalized_measure = np.append(
-                vector_aggregated_normalized_measure, measure["value"]
-            )
+            vector_aggregated_normalized_measure = np.append(vector_aggregated_normalized_measure, measure["value"])
             vector_weight_aggregated_normalized_measure = np.append(
                 vector_weight_aggregated_normalized_measure, measure["weight"]
             )
         aggregated_value = calculate_aggregated_weighted_value(
             vector_aggregated_normalized_measure,
             vector_weight_aggregated_normalized_measure,
         )
@@ -116,17 +106,15 @@
     return result_data
 
 
 def calculate_characteristics(extracted_characteristics):
     try:
         data = CalculateCharacteristicSchema().load(extracted_characteristics)
     except ValidationError as error:
-        raise ValidationError(
-            f"error: Failed to validate input.\nschema_errors: {error.messages}"
-        )
+        raise ValidationError(f"error: Failed to validate input.\nschema_errors: {error.messages}")
 
     result_data = {"characteristics": []}
 
     for characteristic in data["characteristics"]:
         characteristic_key: str = characteristic["key"]
 
         vector_aggregated_normalized_subcharacteristics = np.array([])
@@ -156,17 +144,15 @@
     return result_data
 
 
 def calculate_tsqmi(extracted_tsqmi):
     try:
         data = CalculateTSQMISchema().load(extracted_tsqmi)
     except ValidationError as error:
-        raise ValidationError(
-            f"error: Failed to validate input.\nschema_errors: {error.messages}"
-        )
+        raise ValidationError(f"error: Failed to validate input.\nschema_errors: {error.messages}")
 
     result_data = {"tsqmi": []}
 
     tsqmi = data["tsqmi"]
     tsqmi_key: str = tsqmi["key"]
 
     vector_aggregated_normalized_characteristics = np.array([])
```

### Comparing `msgram_core-1.3.1/src/staticfiles/default_pre_config.py` & `msgram_core-1.3.2/src/staticfiles/default_pre_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,28 +9,28 @@
                 {
                     "key": "testing_status",
                     "weight": 100,
                     "measures": [
                         {
                             "key": "passed_tests",
                             "weight": 33,
-                            "min_passed_tests": 0,
-                            "max_passed_tests": 1,
+                            "min_threshold": 0,
+                            "max_threshold": 1,
                         },
                         {
                             "key": "test_builds",
                             "weight": 33,
-                            "min_fast_test_time": 0,
-                            "max_fast_test_time": 300000,
+                            "min_threshold": 0,
+                            "max_threshold": 300000,
                         },
                         {
                             "key": "test_coverage",
                             "weight": 34,
-                            "min_coverage": 60,
-                            "max_coverage": 100,
+                            "min_threshold": 60,
+                            "max_threshold": 100,
                         },
                     ],
                 }
             ],
         },
         {
             "key": "maintainability",
@@ -39,28 +39,28 @@
                 {
                     "key": "modifiability",
                     "weight": 100,
                     "measures": [
                         {
                             "key": "non_complex_file_density",
                             "weight": 33,
-                            "min_complex_files_density": 0,
-                            "max_complex_files_density": 10,
+                            "min_threshold": 0,
+                            "max_threshold": 10,
                         },
                         {
                             "key": "commented_file_density",
                             "weight": 33,
-                            "min_comment_density": 10,
-                            "max_comment_density": 30,
+                            "min_threshold": 10,
+                            "max_threshold": 30,
                         },
                         {
                             "key": "duplication_absense",
                             "weight": 34,
-                            "min_duplicated_lines": 0,
-                            "max_duplicated_lines": 5,
+                            "min_threshold": 0,
+                            "max_threshold": 5,
                         },
                     ],
                 }
             ],
         },
         # {
         #   "key": "functional_suitability",
```

### Comparing `msgram_core-1.3.1/src/staticfiles/sonarqube_available_metrics.py` & `msgram_core-1.3.2/src/staticfiles/sonarqube_available_metrics.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/src/staticfiles/sonarqube_supported_metrics.py` & `msgram_core-1.3.2/src/staticfiles/sonarqube_supported_metrics.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/src/util/constants.py` & `msgram_core-1.3.2/src/util/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -97,40 +97,33 @@
     },
 }
 
 AGGREGATED_NORMALIZED_MEASURES_MAPPING = {
     "non_complex_file_density": {
         "aggregated_normalized_measure": non_complex_files_density,
         "schema": schemas.NonComplexFileDensitySchema,
-        "thresholds": ["min_complex_files_density", "max_complex_files_density"],
     },
     "commented_file_density": {
         "aggregated_normalized_measure": commented_files_density,
         "schema": schemas.CommentedFileDensitySchema,
-        "thresholds": ["min_comment_density", "max_comment_density"],
     },
     "duplication_absense": {
         "aggregated_normalized_measure": absence_of_duplications,
         "schema": schemas.DuplicationAbsenceSchema,
-        "thresholds": ["min_duplicated_lines", "max_duplicated_lines"],
     },
     "passed_tests": {
         "aggregated_normalized_measure": passed_tests,
         "schema": schemas.PassedTestsSchema,
-        "thresholds": ["min_passed_tests", "max_passed_tests"],
     },
     "test_builds": {
         "aggregated_normalized_measure": fast_test_builds,
         "schema": schemas.TestBuildsSchema,
-        "thresholds": ["min_fast_test_time", "max_fast_test_time"],
     },
     "test_coverage": {
         "aggregated_normalized_measure": test_coverage,
         "schema": schemas.TestCoverageSchema,
-        "thresholds": ["min_coverage", "max_coverage"],
     },
     "team_throughput": {
         "aggregated_normalized_measure": ...,
         "schema": schemas.TeamThroughputSchema,
-        "thresholds": [],
     },
 }
```

### Comparing `msgram_core-1.3.1/src/util/exceptions.py` & `msgram_core-1.3.2/src/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.3.1/tests/test_helpers.py` & `msgram_core-1.3.2/tests/test_helpers.py`

 * *Files identical despite different names*

