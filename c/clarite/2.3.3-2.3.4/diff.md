# Comparing `tmp/clarite-2.3.3.tar.gz` & `tmp/clarite-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarite-2.3.3.tar", max compression
+gzip compressed data, was "clarite-2.3.4.tar", max compression
```

## Comparing `clarite-2.3.3.tar` & `clarite-2.3.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1507 2022-12-07 20:13:15.083403 clarite-2.3.3/LICENSE
--rw-r--r--   0        0        0     3031 2022-12-07 20:13:15.083546 clarite-2.3.3/README.rst
--rw-r--r--   0        0        0      321 2022-12-07 20:13:15.083736 clarite-2.3.3/clarite/__init__.py
--rw-r--r--   0        0        0      171 2022-12-07 20:13:15.083929 clarite-2.3.3/clarite/cli/__init__.py
--rw-r--r--   0        0        0      414 2022-12-07 20:13:15.084059 clarite-2.3.3/clarite/cli/cli.py
--rw-r--r--   0        0        0      174 2022-12-07 20:13:15.084255 clarite-2.3.3/clarite/cli/commands/__init__.py
--rw-r--r--   0        0        0     9785 2022-12-07 20:13:15.084437 clarite-2.3.3/clarite/cli/commands/analyze.py
--rw-r--r--   0        0        0     2962 2022-12-07 20:13:15.084616 clarite-2.3.3/clarite/cli/commands/describe.py
--rw-r--r--   0        0        0     2612 2022-12-07 20:13:15.084779 clarite-2.3.3/clarite/cli/commands/load.py
--rw-r--r--   0        0        0    12069 2022-12-07 20:13:15.085003 clarite-2.3.3/clarite/cli/commands/modify.py
--rw-r--r--   0        0        0     8107 2022-12-07 20:13:15.085200 clarite-2.3.3/clarite/cli/commands/plot.py
--rw-r--r--   0        0        0     7323 2022-12-07 20:13:15.085373 clarite-2.3.3/clarite/cli/custom_types.py
--rw-r--r--   0        0        0     2389 2022-12-07 20:13:15.085539 clarite-2.3.3/clarite/cli/parameters.py
--rw-r--r--   0        0        0        0 2022-12-07 20:13:15.085677 clarite-2.3.3/clarite/internal/__init__.py
--rw-r--r--   0        0        0     2430 2022-12-07 20:13:15.085826 clarite-2.3.3/clarite/internal/calculations.py
--rw-r--r--   0        0        0     8113 2023-02-18 00:09:06.995936 clarite-2.3.3/clarite/internal/utilities.py
--rw-r--r--   0        0        0        0 2022-12-07 20:13:15.086112 clarite-2.3.3/clarite/modules/__init__.py
--rw-r--r--   0        0        0      914 2022-12-07 20:13:15.086305 clarite-2.3.3/clarite/modules/analyze/__init__.py
--rw-r--r--   0        0        0     5003 2023-04-03 19:36:52.180718 clarite-2.3.3/clarite/modules/analyze/association_study.py
--rw-r--r--   0        0        0     3801 2022-12-07 20:13:15.086768 clarite-2.3.3/clarite/modules/analyze/ewas.py
--rw-r--r--   0        0        0     5315 2022-12-07 20:13:15.086947 clarite-2.3.3/clarite/modules/analyze/interaction_study.py
--rw-r--r--   0        0        0     1061 2022-12-07 20:13:15.087150 clarite-2.3.3/clarite/modules/analyze/regression/__init__.py
--rw-r--r--   0        0        0     8110 2023-02-16 18:07:16.128065 clarite-2.3.3/clarite/modules/analyze/regression/base.py
--rw-r--r--   0        0        0    22921 2023-02-18 00:10:40.465264 clarite-2.3.3/clarite/modules/analyze/regression/glm_regression.py
--rw-r--r--   0        0        0    16638 2023-02-18 00:11:04.499945 clarite-2.3.3/clarite/modules/analyze/regression/interaction_regression.py
--rw-r--r--   0        0        0        0 2022-12-07 20:13:15.088014 clarite-2.3.3/clarite/modules/analyze/regression/r_code/__init__.py
--rw-r--r--   0        0        0    27736 2022-12-07 20:13:15.088271 clarite-2.3.3/clarite/modules/analyze/regression/r_code/ewas_r.R
--rw-r--r--   0        0        0     1001 2022-12-07 20:13:15.088473 clarite-2.3.3/clarite/modules/analyze/regression/r_code/r_utilities.py
--rw-r--r--   0        0        0    14079 2022-12-07 20:13:15.088656 clarite-2.3.3/clarite/modules/analyze/regression/r_survey_regression.py
--rw-r--r--   0        0        0    19574 2023-02-18 00:11:35.004428 clarite-2.3.3/clarite/modules/analyze/regression/weighted_glm_regression.py
--rw-r--r--   0        0        0     5779 2022-12-07 20:13:15.089060 clarite-2.3.3/clarite/modules/analyze/utils.py
--rw-r--r--   0        0        0     9187 2022-12-07 20:13:15.089239 clarite-2.3.3/clarite/modules/describe.py
--rw-r--r--   0        0        0     2226 2022-12-07 20:13:15.089372 clarite-2.3.3/clarite/modules/load.py
--rw-r--r--   0        0        0    38580 2022-12-07 20:13:15.089700 clarite-2.3.3/clarite/modules/modify.py
--rw-r--r--   0        0        0      594 2022-12-07 20:13:15.089930 clarite-2.3.3/clarite/modules/plot/__init__.py
--rw-r--r--   0        0        0     6660 2022-12-07 20:13:15.090098 clarite-2.3.3/clarite/modules/plot/distributions.py
--rw-r--r--   0        0        0     2051 2023-02-27 17:36:34.504408 clarite-2.3.3/clarite/modules/plot/histogram.py
--rw-r--r--   0        0        0    21329 2022-12-07 20:13:15.090449 clarite-2.3.3/clarite/modules/plot/manhattan.py
--rw-r--r--   0        0        0     5715 2023-02-27 17:42:22.244035 clarite-2.3.3/clarite/modules/plot/top_results.py
--rw-r--r--   0        0        0      443 2022-12-07 20:13:15.090822 clarite-2.3.3/clarite/modules/survey/LICENSE
--rw-r--r--   0        0        0      183 2022-12-07 20:13:15.090951 clarite-2.3.3/clarite/modules/survey/__init__.py
--rw-r--r--   0        0        0    30285 2023-02-07 14:27:01.244472 clarite-2.3.3/clarite/modules/survey/survey_design.py
--rw-r--r--   0        0        0     9975 2023-02-16 18:01:03.446423 clarite-2.3.3/clarite/modules/survey/survey_model.py
--rw-r--r--   0        0        0     1634 2023-04-04 13:33:08.665400 clarite-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 clarite-2.3.3/setup.py
--rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 clarite-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1507 2022-12-07 20:13:15.083403 clarite-2.3.4/LICENSE
+-rw-r--r--   0        0        0     3031 2022-12-07 20:13:15.083546 clarite-2.3.4/README.rst
+-rw-r--r--   0        0        0      321 2022-12-07 20:13:15.083736 clarite-2.3.4/clarite/__init__.py
+-rw-r--r--   0        0        0      171 2022-12-07 20:13:15.083929 clarite-2.3.4/clarite/cli/__init__.py
+-rw-r--r--   0        0        0      414 2022-12-07 20:13:15.084059 clarite-2.3.4/clarite/cli/cli.py
+-rw-r--r--   0        0        0      174 2022-12-07 20:13:15.084255 clarite-2.3.4/clarite/cli/commands/__init__.py
+-rw-r--r--   0        0        0     9785 2022-12-07 20:13:15.084437 clarite-2.3.4/clarite/cli/commands/analyze.py
+-rw-r--r--   0        0        0     2962 2022-12-07 20:13:15.084616 clarite-2.3.4/clarite/cli/commands/describe.py
+-rw-r--r--   0        0        0     2612 2022-12-07 20:13:15.084779 clarite-2.3.4/clarite/cli/commands/load.py
+-rw-r--r--   0        0        0    12069 2022-12-07 20:13:15.085003 clarite-2.3.4/clarite/cli/commands/modify.py
+-rw-r--r--   0        0        0     8107 2022-12-07 20:13:15.085200 clarite-2.3.4/clarite/cli/commands/plot.py
+-rw-r--r--   0        0        0     7323 2022-12-07 20:13:15.085373 clarite-2.3.4/clarite/cli/custom_types.py
+-rw-r--r--   0        0        0     2389 2022-12-07 20:13:15.085539 clarite-2.3.4/clarite/cli/parameters.py
+-rw-r--r--   0        0        0        0 2022-12-07 20:13:15.085677 clarite-2.3.4/clarite/internal/__init__.py
+-rw-r--r--   0        0        0     2430 2022-12-07 20:13:15.085826 clarite-2.3.4/clarite/internal/calculations.py
+-rw-r--r--   0        0        0     8113 2023-02-18 00:09:06.995936 clarite-2.3.4/clarite/internal/utilities.py
+-rw-r--r--   0        0        0        0 2022-12-07 20:13:15.086112 clarite-2.3.4/clarite/modules/__init__.py
+-rw-r--r--   0        0        0      914 2022-12-07 20:13:15.086305 clarite-2.3.4/clarite/modules/analyze/__init__.py
+-rw-r--r--   0        0        0     5003 2023-04-03 19:36:52.180718 clarite-2.3.4/clarite/modules/analyze/association_study.py
+-rw-r--r--   0        0        0     3801 2022-12-07 20:13:15.086768 clarite-2.3.4/clarite/modules/analyze/ewas.py
+-rw-r--r--   0        0        0     5315 2022-12-07 20:13:15.086947 clarite-2.3.4/clarite/modules/analyze/interaction_study.py
+-rw-r--r--   0        0        0     1061 2022-12-07 20:13:15.087150 clarite-2.3.4/clarite/modules/analyze/regression/__init__.py
+-rw-r--r--   0        0        0     8110 2023-02-16 18:07:16.128065 clarite-2.3.4/clarite/modules/analyze/regression/base.py
+-rw-r--r--   0        0        0    23283 2023-06-07 01:46:29.105238 clarite-2.3.4/clarite/modules/analyze/regression/glm_regression.py
+-rw-r--r--   0        0        0    16638 2023-02-18 00:11:04.499945 clarite-2.3.4/clarite/modules/analyze/regression/interaction_regression.py
+-rw-r--r--   0        0        0        0 2022-12-07 20:13:15.088014 clarite-2.3.4/clarite/modules/analyze/regression/r_code/__init__.py
+-rw-r--r--   0        0        0    27736 2022-12-07 20:13:15.088271 clarite-2.3.4/clarite/modules/analyze/regression/r_code/ewas_r.R
+-rw-r--r--   0        0        0     1001 2022-12-07 20:13:15.088473 clarite-2.3.4/clarite/modules/analyze/regression/r_code/r_utilities.py
+-rw-r--r--   0        0        0    14182 2023-06-06 15:25:36.419210 clarite-2.3.4/clarite/modules/analyze/regression/r_survey_regression.py
+-rw-r--r--   0        0        0    19574 2023-02-18 00:11:35.004428 clarite-2.3.4/clarite/modules/analyze/regression/weighted_glm_regression.py
+-rw-r--r--   0        0        0     5779 2022-12-07 20:13:15.089060 clarite-2.3.4/clarite/modules/analyze/utils.py
+-rw-r--r--   0        0        0     9187 2022-12-07 20:13:15.089239 clarite-2.3.4/clarite/modules/describe.py
+-rw-r--r--   0        0        0     2226 2022-12-07 20:13:15.089372 clarite-2.3.4/clarite/modules/load.py
+-rw-r--r--   0        0        0    38580 2022-12-07 20:13:15.089700 clarite-2.3.4/clarite/modules/modify.py
+-rw-r--r--   0        0        0      594 2022-12-07 20:13:15.089930 clarite-2.3.4/clarite/modules/plot/__init__.py
+-rw-r--r--   0        0        0     6660 2022-12-07 20:13:15.090098 clarite-2.3.4/clarite/modules/plot/distributions.py
+-rw-r--r--   0        0        0     2051 2023-02-27 17:36:34.504408 clarite-2.3.4/clarite/modules/plot/histogram.py
+-rw-r--r--   0        0        0    21329 2022-12-07 20:13:15.090449 clarite-2.3.4/clarite/modules/plot/manhattan.py
+-rw-r--r--   0        0        0     5715 2023-02-27 17:42:22.244035 clarite-2.3.4/clarite/modules/plot/top_results.py
+-rw-r--r--   0        0        0      443 2022-12-07 20:13:15.090822 clarite-2.3.4/clarite/modules/survey/LICENSE
+-rw-r--r--   0        0        0      183 2022-12-07 20:13:15.090951 clarite-2.3.4/clarite/modules/survey/__init__.py
+-rw-r--r--   0        0        0    30285 2023-02-07 14:27:01.244472 clarite-2.3.4/clarite/modules/survey/survey_design.py
+-rw-r--r--   0        0        0     9975 2023-02-16 18:01:03.446423 clarite-2.3.4/clarite/modules/survey/survey_model.py
+-rw-r--r--   0        0        0     1634 2023-07-03 17:46:37.784869 clarite-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 clarite-2.3.4/setup.py
+-rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 clarite-2.3.4/PKG-INFO
```

### Comparing `clarite-2.3.3/LICENSE` & `clarite-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/README.rst` & `clarite-2.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/cli/commands/analyze.py` & `clarite-2.3.4/clarite/cli/commands/analyze.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/cli/commands/describe.py` & `clarite-2.3.4/clarite/cli/commands/describe.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/cli/commands/load.py` & `clarite-2.3.4/clarite/cli/commands/load.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/cli/commands/modify.py` & `clarite-2.3.4/clarite/cli/commands/modify.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/cli/commands/plot.py` & `clarite-2.3.4/clarite/cli/commands/plot.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/cli/custom_types.py` & `clarite-2.3.4/clarite/cli/custom_types.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/cli/parameters.py` & `clarite-2.3.4/clarite/cli/parameters.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/internal/calculations.py` & `clarite-2.3.4/clarite/internal/calculations.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/internal/utilities.py` & `clarite-2.3.4/clarite/internal/utilities.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/__init__.py` & `clarite-2.3.4/clarite/modules/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/association_study.py` & `clarite-2.3.4/clarite/modules/analyze/association_study.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/ewas.py` & `clarite-2.3.4/clarite/modules/analyze/ewas.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/interaction_study.py` & `clarite-2.3.4/clarite/modules/analyze/interaction_study.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/__init__.py` & `clarite-2.3.4/clarite/modules/analyze/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/base.py` & `clarite-2.3.4/clarite/modules/analyze/regression/base.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/glm_regression.py` & `clarite-2.3.4/clarite/modules/analyze/regression/glm_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from clarite.internal.utilities import _get_dtypes, _remove_empty_categories
 
 from ..utils import fix_names, statsmodels_var_regex
 from .base import Regression
 
 # GITHUB ISSUE #119: Regressions with Error after Multiprocessing release python > 3.8
-multiprocessing.get_start_method("fork")
+# multiprocessing.get_start_method("fork")
 
 
 class GLMRegression(Regression):
     """
     Statsmodels GLM Regression.
     This class handles running a regression for each variable of interest and collecting results.
 
@@ -125,23 +125,33 @@
             )
             self.family = sm.families.Gaussian(link=sm.families.links.identity())
             self.use_t = True
         elif self.outcome_dtype == "binary":
             # Use the order according to the categorical
             counts = self.data[self.outcome_variable].value_counts().to_dict()
 
-            categories = self.data[self.outcome_variable].cat.categories
+            # Add sorted
+            categories = sorted(self.data[self.outcome_variable].cat.categories)
+
             # GITHUB ISSUES #115: Keep control as 0 and case as 1
             if categories[0] == "Case" and categories[1] == "Control":
                 categories = sorted(categories, reverse=True)
 
             # TODO: Allow only 0/1 or Control/Case entries | Other entries generate a warning
 
             codes, categories = zip(*enumerate(categories))
             self.data[self.outcome_variable].replace(categories, codes, inplace=True)
+
+            # After upgrade to Pandas >= 1.5 the replace stop to covert as float
+            # if stay as category, when create y will create to columns and will invert the
+            # beta signal.
+            self.data[self.outcome_variable] = self.data[self.outcome_variable].astype(
+                float
+            )
+
             self.description += (
                 f"Binary Outcome (family = Binomial): '{self.outcome_variable}'\n"
                 f"\t{counts[categories[0]]:,} occurrences of '{categories[0]}' coded as 0\n"
                 f"\t{counts[categories[1]]:,} occurrences of '{categories[1]}' coded as 1"
             )
             self.family = sm.families.Binomial(link=sm.families.links.logit())
             self.use_t = False
```

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/interaction_regression.py` & `clarite-2.3.4/clarite/modules/analyze/regression/interaction_regression.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/r_code/ewas_r.R` & `clarite-2.3.4/clarite/modules/analyze/regression/r_code/ewas_r.R`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/r_code/r_utilities.py` & `clarite-2.3.4/clarite/modules/analyze/regression/r_code/r_utilities.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/r_survey_regression.py` & `clarite-2.3.4/clarite/modules/analyze/regression/r_survey_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import List, Optional
 
 import pandas as pd
 
-from clarite.internal.utilities import requires, _get_dtypes
+from clarite.internal.utilities import _get_dtypes, requires
 
-from .base import Regression
 from ...survey import SurveyDesignSpec
+from .base import Regression
 
 
 class RSurveyRegression(Regression):
     """
     Run regressions by calling R from Python
     When a SurveyDesignSpec is provided, the R *survey* library is used.
     Results should match those run with either GLMRegression or WeightedGLMRegression.
@@ -46,14 +46,16 @@
         outcome_variable: str,
         regression_variables: List[str],
         covariates: Optional[List[str]],
         survey_design_spec: Optional[SurveyDesignSpec] = None,
         min_n: int = 200,
         report_categorical_betas: bool = False,
         standardize_data: bool = False,
+        encoding=None,  # TODO: Error on call
+        edge_encoding_info=None,  # TODO: Error on call
     ):
         # base class init
         # This takes in minimal regression params (data, outcome_variable, covariates) and
         # initializes additional parameters (outcome dtype, regression variables, error, and warnings)
         super().__init__(
             data=data,
             outcome_variable=outcome_variable,
@@ -171,15 +173,16 @@
     def run(self):
         """
         Run the regression using R
         """
         # Source R script to define the function
         import rpy2.robjects as ro
         from rpy2.robjects import pandas2ri
-        from .r_code.r_utilities import ewasresult2py, df_pandas2r
+
+        from .r_code.r_utilities import df_pandas2r, ewasresult2py
 
         r_code_folder = Path(__file__).parent / "r_code"
         filename = str(r_code_folder / "ewas_r.R")
         ro.r.source(filename)
 
         # Print warnings as they occur
         ro.r("options(warn=1)")
```

### Comparing `clarite-2.3.3/clarite/modules/analyze/regression/weighted_glm_regression.py` & `clarite-2.3.4/clarite/modules/analyze/regression/weighted_glm_regression.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/analyze/utils.py` & `clarite-2.3.4/clarite/modules/analyze/utils.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/describe.py` & `clarite-2.3.4/clarite/modules/describe.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/load.py` & `clarite-2.3.4/clarite/modules/load.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/modify.py` & `clarite-2.3.4/clarite/modules/modify.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/plot/__init__.py` & `clarite-2.3.4/clarite/modules/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/plot/distributions.py` & `clarite-2.3.4/clarite/modules/plot/distributions.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/plot/histogram.py` & `clarite-2.3.4/clarite/modules/plot/histogram.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/plot/manhattan.py` & `clarite-2.3.4/clarite/modules/plot/manhattan.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/plot/top_results.py` & `clarite-2.3.4/clarite/modules/plot/top_results.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/survey/survey_design.py` & `clarite-2.3.4/clarite/modules/survey/survey_design.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/clarite/modules/survey/survey_model.py` & `clarite-2.3.4/clarite/modules/survey/survey_model.py`

 * *Files identical despite different names*

### Comparing `clarite-2.3.3/pyproject.toml` & `clarite-2.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clarite"
-version = "2.3.3"
+version = "2.3.4"
 description = "CLeaning to Analysis: Reproducibility-based Interface for Traits and Exposures"
 authors = ["Andre Rico <alr6366@psu.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 repository = "https://github.com/HallLab/clarite-python/"
 documentation = "https://clarite-python.readthedocs.io/en/latest/"
 classifiers=[
```

### Comparing `clarite-2.3.3/setup.py` & `clarite-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
           'sphinx-click>=4,<5']}
 
 entry_points = \
 {'console_scripts': ['clarite-cli = clarite.cli:entry_point']}
 
 setup_kwargs = {
     'name': 'clarite',
-    'version': '2.3.3',
+    'version': '2.3.4',
     'description': 'CLeaning to Analysis: Reproducibility-based Interface for Traits and Exposures',
     'long_description': '.. image:: https://raw.githubusercontent.com/HallLab/clarite-python/master/docs/source/_static/clarite_logo.png\n   :target: https://clarite-python.readthedocs.io/en/stable/\n   :align: center\n   :alt: CLARITE Logo\n\n------------\n\n.. image:: https://img.shields.io/badge/python-3.7+-blue.svg?style=flat-square\n   :target: https://pypi.python.org/pypi/clarite\n   :alt: Python version\n\n.. image:: https://img.shields.io/pypi/v/clarite.svg?style=flat-square\n   :target: https://pypi.org/project/clarite/\n   :alt: PyPI\n\n.. image:: https://img.shields.io/github/workflow/status/HallLab/clarite-python/CI?style=flat-square\n   :target: https://github.com/HallLab/clarite-python/actions?query=workflow%3ACI\n   :alt: Build status\n\n.. image:: https://img.shields.io/readthedocs/clarite-python?style=flat-square\n   :target: https://clarite-python.readthedocs.io/en/latest/\n   :alt: Docs\n\n.. image:: https://img.shields.io/codecov/c/gh/HallLab/clarite-python.svg?style=flat-square\n   :target: https://codecov.io/gh/HallLab/clarite-python/\n   :alt: Test coverage\n\n.. image:: https://img.shields.io/pypi/l/clarite?style=flat-square\n   :target: https://opensource.org/licenses/BSD-3-Clause\n   :alt: License\n\n.. image:: https://img.shields.io/badge/code%20style-Black-black?style=flat-square\n   :target: https://github.com/psf/black\n   :alt: Black\n\n------------\n\nCLeaning to Analysis: Reproducibility-based Interface for Traits and Exposures\n==============================================================================\n\n* Free software: 3-clause BSD license\n* Documentation: https://www.hall-lab.org/clarite-python/.\n\nExamples\n--------\n\n**Run an EWAS in a few lines of code**\n\n.. image:: docs/source/_static/code/quick_ewas.png\n\n|\n\n**More realistically, perform some QC first:**\n\n.. image:: docs/source/_static/code/filters.png\n\n|\n\n**Genotype data is supported via Pandas-Genomics**\n\n.. image:: docs/source/_static/code/gwas.png\n\nInstallation\n------------\n\nIn order to use the *r_survey* regression_kind in the *ewas* function, R must be installed along with the *survey* library.\n\n1. Install R and ensure it is accessible from the command line.  You may need to add its location to the PATH environmental variable.\n2. Use *install.packages* in R to install the *survey* library.\n\nQuestions\n---------\nIf you have any questions not answered by the `documentation <https://clarite-python.readthedocs.io/en/latest/>`_,\nfeel free to open an `Issue <https://github.com/HallLab/clarite-python/issues>`_.\n\nCiting CLARITE\n--------------\n\n1.\nLucas AM, et al (2019)\n`CLARITE facilitates the quality control and analysis process for EWAS of metabolic-related traits. <https://www.frontiersin.org/article/10.3389/fgene.2019.01240>`_\n*Frontiers in Genetics*: 10, 1240\n\n2.\nPassero K, et al (2020)\n`Phenome-wide association studies on cardiovascular health and fatty acids considering phenotype quality control practices for epidemiological data. <https://www.worldscientific.com/doi/abs/10.1142/9789811215636_0058>`_\n*Pacific Symposium on Biocomputing*: 25, 659\n',
     'author': 'Andre Rico',
     'author_email': 'alr6366@psu.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/HallLab/clarite-python/',
```

### Comparing `clarite-2.3.3/PKG-INFO` & `clarite-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarite
-Version: 2.3.3
+Version: 2.3.4
 Summary: CLeaning to Analysis: Reproducibility-based Interface for Traits and Exposures
 Home-page: https://github.com/HallLab/clarite-python/
 License: BSD-3-Clause
 Author: Andre Rico
 Author-email: alr6366@psu.edu
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 4 - Beta
```

