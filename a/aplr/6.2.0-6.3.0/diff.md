# Comparing `tmp/aplr-6.2.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-6.3.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 357900 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   403968 b- defN 23-Jul-01 12:10 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   426496 b- defN 23-Jul-01 12:14 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jul-01 12:04 aplr/__init__.py
--rw-rw-rw-  2.0 fat    11238 b- defN 23-Jul-01 12:04 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-Jul-01 12:14 aplr-6.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      655 b- defN 23-Jul-01 12:14 aplr-6.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-01 12:14 aplr-6.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-01 12:14 aplr-6.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      691 b- defN 23-Jul-01 12:14 aplr-6.2.0.dist-info/RECORD
-9 files, 844322 bytes uncompressed, 356728 bytes compressed:  57.7%
+Zip file size: 366312 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   417280 b- defN 23-Jul-03 16:48 aplr_cpp.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   442368 b- defN 23-Jul-03 16:52 aplr_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jul-03 16:42 aplr/__init__.py
+-rw-rw-rw-  2.0 fat    12116 b- defN 23-Jul-03 16:42 aplr/aplr.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-Jul-03 16:52 aplr-6.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      655 b- defN 23-Jul-03 16:52 aplr-6.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-03 16:52 aplr-6.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-03 16:52 aplr-6.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      691 b- defN 23-Jul-03 16:52 aplr-6.3.0.dist-info/RECORD
+9 files, 874384 bytes uncompressed, 365140 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: aplr/__init__.py
 Comment: 
 
 Filename: aplr/aplr.py
 Comment: 
 
-Filename: aplr-6.2.0.dist-info/LICENSE
+Filename: aplr-6.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-6.2.0.dist-info/METADATA
+Filename: aplr-6.3.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-6.2.0.dist-info/WHEEL
+Filename: aplr-6.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-6.2.0.dist-info/top_level.txt
+Filename: aplr-6.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-6.2.0.dist-info/RECORD
+Filename: aplr-6.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aplr/aplr.py

```diff
@@ -5,15 +5,17 @@
 
 
 class APLRRegressor():
     def __init__(self, m:int=1000, v:float=0.1, random_state:int=0, loss_function:str="mse", link_function:str="identity", n_jobs:int=0, 
                  validation_ratio:float=0.2, bins:int=300, max_interaction_level:int=1, max_interactions:int=100000, 
                  min_observations_in_split:int=20, ineligible_boosting_steps_added:int=10, max_eligible_terms:int=5, verbosity:int=0, 
                  dispersion_parameter:float=1.5, validation_tuning_metric:str="default", quantile:float=0.5,
-                 calculate_custom_validation_error_function:Optional[Callable[[npt.ArrayLike, npt.ArrayLike, npt.ArrayLike, npt.ArrayLike], float]]=None):
+                 calculate_custom_validation_error_function:Optional[Callable[[npt.ArrayLike, npt.ArrayLike, npt.ArrayLike, npt.ArrayLike], float]]=None,
+                 calculate_custom_loss_function:Optional[Callable[[npt.ArrayLike, npt.ArrayLike, npt.ArrayLike, npt.ArrayLike], float]]=None,
+                 calculate_custom_negative_gradient_function:Optional[Callable[[npt.ArrayLike, npt.ArrayLike, npt.ArrayLike], npt.ArrayLike]]=None):
         self.m=m
         self.v=v
         self.random_state=random_state
         self.loss_function=loss_function
         self.link_function=link_function
         self.n_jobs=n_jobs
         self.validation_ratio=validation_ratio
@@ -24,14 +26,16 @@
         self.ineligible_boosting_steps_added=ineligible_boosting_steps_added
         self.max_eligible_terms=max_eligible_terms
         self.verbosity=verbosity
         self.dispersion_parameter=dispersion_parameter
         self.validation_tuning_metric=validation_tuning_metric
         self.quantile=quantile
         self.calculate_custom_validation_error_function=calculate_custom_validation_error_function
+        self.calculate_custom_loss_function=calculate_custom_loss_function
+        self.calculate_custom_negative_gradient_function=calculate_custom_negative_gradient_function
 
         #Creating aplr_cpp and setting parameters
         self.APLRRegressor=aplr_cpp.APLRRegressor()
         self.__set_params_cpp()
 
     #Sets parameters for aplr_cpp.APLRRegressor cpp object
     def __set_params_cpp(self):
@@ -49,14 +53,16 @@
         self.APLRRegressor.ineligible_boosting_steps_added=self.ineligible_boosting_steps_added
         self.APLRRegressor.max_eligible_terms=self.max_eligible_terms
         self.APLRRegressor.verbosity=self.verbosity
         self.APLRRegressor.dispersion_parameter=self.dispersion_parameter
         self.APLRRegressor.validation_tuning_metric=self.validation_tuning_metric
         self.APLRRegressor.quantile=self.quantile
         self.APLRRegressor.calculate_custom_validation_error_function=self.calculate_custom_validation_error_function
+        self.APLRRegressor.calculate_custom_loss_function=self.calculate_custom_loss_function
+        self.APLRRegressor.calculate_custom_negative_gradient_function=self.calculate_custom_negative_gradient_function
 
     def fit(self, X:npt.ArrayLike, y:npt.ArrayLike, sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[], group:npt.ArrayLike = np.empty(0), interaction_constraints:List[int]=[]):
         self.__set_params_cpp()
         self.APLRRegressor.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints,group,interaction_constraints)
 
     def predict(self, X:npt.ArrayLike, cap_predictions_to_minmax_in_training:bool=True)->npt.ArrayLike:
         return self.APLRRegressor.predict(X, cap_predictions_to_minmax_in_training)
@@ -119,15 +125,17 @@
             "verbosity":self.verbosity,
             "min_observations_in_split":self.min_observations_in_split,
             "ineligible_boosting_steps_added":self.ineligible_boosting_steps_added,
             "max_eligible_terms":self.max_eligible_terms,
             "dispersion_parameter":self.dispersion_parameter,
             "validation_tuning_metric":self.validation_tuning_metric,
             "quantile":self.quantile,
-            "calculate_custom_validation_error_function":self.calculate_custom_validation_error_function
+            "calculate_custom_validation_error_function":self.calculate_custom_validation_error_function,
+            "calculate_custom_loss_function":self.calculate_custom_loss_function,
+            "calculate_custom_negative_gradient_function":self.calculate_custom_negative_gradient_function
         }
 
     #For sklearn
     def set_params(self, **parameters):
         for parameter, value in parameters.items():
             setattr(self, parameter, value)
         self.__set_params_cpp()
```

## Comparing `aplr-6.2.0.dist-info/LICENSE` & `aplr-6.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aplr-6.2.0.dist-info/METADATA` & `aplr-6.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 6.2.0
+Version: 6.3.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
```

