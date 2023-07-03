# Comparing `tmp/bootstrapping_tools-1.0.0.tar.gz` & `tmp/bootstrapping_tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrapping_tools-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bootstrapping_tools-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bootstrapping_tools-1.0.0.tar` & `bootstrapping_tools-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      200 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/README.md
--rw-r--r--   0        0        0      137 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/bootstrapping_tools/__init__.py
--rw-r--r--   0        0        0    10923 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/bootstrapping_tools/bootstrapping.py
--rw-r--r--   0        0        0      871 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/bootstrapping_tools/resample_by_blocks.py
--rw-r--r--   0        0        0      516 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/README.md
+-rw-r--r--   0        0        0      137 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/bootstrapping_tools/__init__.py
+-rw-r--r--   0        0        0    11784 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/bootstrapping_tools/bootstrapping.py
+-rw-r--r--   0        0        0      859 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/bootstrapping_tools/resample_by_blocks.py
+-rw-r--r--   0        0        0      516 2023-07-03 18:18:07.786256 bootstrapping_tools-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-1.1.0/PKG-INFO
```

### Comparing `bootstrapping_tools-1.0.0/bootstrapping_tools/bootstrapping.py` & `bootstrapping_tools-1.1.0/bootstrapping_tools/bootstrapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,40 @@
         lambda_upper_bound (int, optional):  Max lambda coefficient. Defaults to 50.
 
     Returns:
         [ndarray]: The coefficients array for power_law (N0,lamda).
     """
     temporadas = np.array(temporadas)
     numero_agno = temporadas - temporadas[0]
+    popt = fit_power_law_parameters(
+        maximo_nidos, max_iter, lower_bounds, lambda_upper_bound, numero_agno
+    )
+    return popt
+
+
+def lambda_calculator_from_resampled_data(
+    temporadas, maximo_nidos, max_iter=10000, lower_bounds=0, lambda_upper_bound=50
+):
+    temporadas = np.array(temporadas)
+    popt = fit_power_law_parameters(
+        maximo_nidos, max_iter, lower_bounds, lambda_upper_bound, temporadas
+    )
+    return popt
+
+
+def fit_power_law_parameters(maximo_nidos, max_iter, lower_bounds, lambda_upper_bound, numero_agno):
     maximo_nidos = np.array(maximo_nidos)
     popt, _ = curve_fit(
         power_law,
         numero_agno,
         maximo_nidos,
         maxfev=max_iter,
         bounds=((lower_bounds, lower_bounds), (lambda_upper_bound, np.inf)),
     )
+
     return popt
 
 
 def seasons_from_date(data):
     """Extract years from string date format: dd/mm/aaaa.
 
     Args:
@@ -168,17 +186,17 @@
         If `return_distribution` is True, returns the distribution too.
     """
     lambdas_bootstraps = []
     cont = 0
     rand = 0
     print("Calculating bootstrap growth rates distribution:")
     while cont < N:
-        resampled_data = resample_data(dataframe, rand, blocks_length)
+        resampled_data = resample_and_shift_data(dataframe, rand, blocks_length)
         try:
-            fitting_result = lambda_calculator(
+            fitting_result = lambda_calculator_from_resampled_data(
                 resampled_data["Temporada"], resampled_data[column_name]
             )
         except RuntimeError:
             rand += 1
             continue
         lambdas_bootstraps.append(fitting_result[0])
         cont += 1
@@ -190,16 +208,23 @@
 
 
 def _calculate_intevals(lambdas_distribution, limits):
     return np.percentile(lambdas_distribution, limits)
 
 
 def resample_data(dataframe, seed, blocks_length):
-    random.seed(seed)
-    return random_resample_data_by_blocks(dataframe, blocks_length)
+    rng = random.Random(seed)
+    return random_resample_data_by_blocks(dataframe, blocks_length, rng)
+
+
+def resample_and_shift_data(dataframe, seed, blocks_length):
+    resampled_data = resample_data(dataframe, seed, blocks_length)
+    min_season = dataframe.iloc[:, 0].min()
+    resampled_data.iloc[:, 0] = resampled_data.iloc[:, 0] - min_season
+    return resampled_data
 
 
 def calculate_intervals_from_p_values_and_alpha(distribution, p_values, alpha):
     limits = calculate_limits_from_p_values_and_alpha(p_values, alpha)
     return _calculate_intevals(distribution, limits)
```

### Comparing `bootstrapping_tools-1.0.0/bootstrapping_tools/resample_by_blocks.py` & `bootstrapping_tools-1.1.0/bootstrapping_tools/resample_by_blocks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
-import random
 
 
-def random_resample_data_by_blocks(original_sample, blocks_length):
+def random_resample_data_by_blocks(original_sample, blocks_length, rng):
     n_rows_original = len(original_sample)
     block_labels = _get_labels(n_rows_original, blocks_length)
     length_block_labels = len(block_labels)
-    block_labels = random.choices(block_labels, k=length_block_labels)
+    block_labels = rng.choices(block_labels, k=length_block_labels)
     rows = _get_rows(block_labels, n_rows_original, blocks_length)
     resample = original_sample.iloc[rows, :].reset_index(drop=True)
     return resample
 
 
 def _get_labels(n_rows_original, blocks_length):
     blocks_number = np.ceil(n_rows_original / blocks_length)
```

### Comparing `bootstrapping_tools-1.0.0/pyproject.toml` & `bootstrapping_tools-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-1.0.0/PKG-INFO` & `bootstrapping_tools-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrapping_tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: GECI Tools for bootstrapping
 Home-page: https://github.com/IslasGECI/bootstrapping_tools
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bootstrapping_tools Version: 1.0.0 Summary: GECI
+Metadata-Version: 2.1 Name: bootstrapping_tools Version: 1.1.0 Summary: GECI
 Tools for bootstrapping Home-page: https://github.com/IslasGECI/
 bootstrapping_tools Author: Ciencia de Datos â¢ GECI Author-email:
 ciencia.datos@islas.org.mx Requires-Python: >=3 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: GNU General Public License v3
 or later (GPLv3+) Requires-Dist: numpy Requires-Dist: pandas-stubs Requires-
 Dist: pandas Requires-Dist: scipy Requires-Dist: tqdm [https://
 www.islas.org.mx/img/logo.svg] # Bootstrapping tools GECI tools to perform
```

