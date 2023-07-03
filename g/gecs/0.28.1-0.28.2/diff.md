# Comparing `tmp/gecs-0.28.1.tar.gz` & `tmp/gecs-0.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.28.1.tar", max compression
+gzip compressed data, was "gecs-0.28.2.tar", max compression
```

## Comparing `gecs-0.28.1.tar` & `gecs-0.28.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.28.1/LICENSE
--rw-r--r--   0        0        0     2041 2023-07-01 15:06:46.565047 gecs-0.28.1/README.md
--rw-r--r--   0        0        0      697 2023-07-01 15:07:22.368832 gecs-0.28.1/pyproject.toml
--rw-r--r--   0        0        0    43189 2023-07-01 14:46:26.156284 gecs-0.28.1/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.28.1/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 gecs-0.28.1/setup.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 gecs-0.28.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.28.2/LICENSE
+-rw-r--r--   0        0        0     2220 2023-07-03 10:39:36.682086 gecs-0.28.2/README.md
+-rw-r--r--   0        0        0      697 2023-07-03 10:39:36.682086 gecs-0.28.2/pyproject.toml
+-rw-r--r--   0        0        0    44045 2023-07-03 10:39:36.682086 gecs-0.28.2/src/gecs/gec.py
+-rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.28.2/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 gecs-0.28.2/setup.py
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 gecs-0.28.2/PKG-INFO
```

### Comparing `gecs-0.28.1/LICENSE` & `gecs-0.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.28.1/README.md` & `gecs-0.28.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,23 @@
 
     gec.fit(X, y)
 
     gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
 
     gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier
 
+    yhat = gec.predict(X)
+
+    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier
+    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
+
+
+    
+
+
 
 ## Contributing
 
 If you want to contribute, please reach out and I'll design a process around it.
 
 ## License
```

### Comparing `gecs-0.28.1/pyproject.toml` & `gecs-0.28.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.28.1"
+version = "0.28.2"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.28.1/src/gecs/gec.py` & `gecs-0.28.2/src/gecs/gec.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,22 @@
         colsample_bytree: float = 1.0,
         reg_alpha: float = 0.0,
         reg_lambda: float = 0.0,
         random_state: Optional[Union[int, np.random.RandomState]] = None,
         n_jobs: int = -1,
         silent: Union[bool, str] = "warn",
         importance_type: str = "split",
+        frozen: bool = False,
         **kwargs,
     ):
-        assert str(inspect.signature(LGBMClassifier.__init__)) == str(
-            inspect.signature(GEC.__init__)
-        )
+        adapted_lgbm_params = str(inspect.signature(LGBMClassifier.__init__)).replace(
+            "importance_type: str = 'split'", "importance_type: str = 'split', frozen: bool = False"
+        ) 
+        gec_params = str( inspect.signature(GEC.__init__))
+        assert adapted_lgbm_params == gec_params, gec_params
 
         r"""Construct a gradient boosting model.
 
         Parameters
         ----------
         boosting_type : str, optional (default='gbdt')
             'gbdt', traditional Gradient Boosting Decision Tree.
@@ -203,14 +206,15 @@
         self.set_params(**kwargs)
 
         self._init_kwargs = {
             k: v for k, v in kwargs.items()
             if k not in ["bagging_freq", "bagging_fraction"]
         }
 
+        self.frozen = frozen
         non_optimized_init_args = [
             "max_depth",
             "subsample_for_bin",
             "objective",
             "class_weight",
             "min_split_gain", 
             "subsample",
@@ -228,15 +232,15 @@
             "l": 1.0,
             "l_bagging": 0.1,
             "hyperparams_acquisition_percentile": 0.7,
             "bagging_acquisition_percentile": 0.7,
             "bandit_greediness": 1.0,
             "n_random_exploration": 10,
             "n_sample": 1000,
-            "n_sample_initial": 10000,
+            "n_sample_initial": 1000,
             "best_share": 0.2,
             "hyperparameters": [
                 "learning_rate",
                 "n_estimators",
                 "num_leaves",
                 "reg_alpha",
                 "reg_lambda",
@@ -248,15 +252,15 @@
         }
         self._set_gec_attributes()
         self._set_gec_fields()
 
 
     def _set_gec_attributes(self):
         self.categorical_hyperparameters = [
-            ("boosting", ["gbdt", "dart", "rf"]),
+            ("boosting_type", ["gbdt", "dart", "rf"]),
             ("bagging", ["yes_bagging", "no_bagging"]),
         ]
 
         self._categorical_hyperparameter_names, _ = zip(
             *self.categorical_hyperparameters
         )
 
@@ -351,14 +355,15 @@
 
         self._rescale_bagging_combination = lambda freq, frac: (((freq/5)-1), ((frac*4)-3))
         self._invert_rescaled_bagging_combination =  lambda freq, frac: (((freq+1)*5), ((frac+3)/4))
         self._bagging_combinations_rescaled = [self._rescale_bagging_combination(freq, frac) for freq, frac in self._bagging_combinations]
 
         self.best_score = None
         self.best_params_ = None
+        self.fit_params = None
         self.n_iterations = 0
 
         # parameters for bandit
         self.rewards = {
             c: {"a": 1, "b": 1} for c in self._categorical_hyperparameter_combinations
         }
         self.selected_arms = []
@@ -379,15 +384,15 @@
     @kernel_bagging.setter
     def kernel_bagging(self, value):
         self._kernel_bagging = value
         self.gaussian_bagging = GaussianProcessRegressor(kernel=value)
 
     @property
     def gec_iter(self):
-        return len(self.hyperparameter_scores)
+        return len(self.hyperparameter_scores["output"])
 
     @classmethod
     def _cast_to_type(cls, value, type_):
         if type_ == np.float64:
             return float(value)
         elif type_ == np.int64:
             return int(value)
@@ -427,14 +432,15 @@
         gec.bagging_scores = gec._convert_gaussian_process_data_from_deserialisation(
             representation["bagging_scores"]
         )
         gec.best_params_ = representation["best_params_"]
         gec.best_score = float(representation["best_score"])
         gec.best_params_gec = representation["best_params_gec"]
         gec.best_scores_gec = representation["best_scores_gec"]
+        gec.fit_params = representation["fit_params"]
 
         if X is not None and y is not None:
             gec._fit_best_params(X, y)
         else:
             warnings.warn(
                 "If X and y are not provided, the GEC model is not fitted for inference"
             )
@@ -485,15 +491,16 @@
             "selected_arms": self.selected_arms,
             "hyperparameter_scores": hyperparameter_scores,
             "bagging_scores": bagging_scores,
             "best_params_": self.best_params_,
             "best_score": self.best_score,
             "best_params_gec": self.best_params_gec,
             "best_scores_gec": self.best_scores_gec,
-            "gec_iter": self.gec_iter
+            "gec_iter": self.gec_iter,
+            "fit_params": self.fit_params
         }
         return representation
 
 
     def _validate_parameter_maps(self):
         real_to_linear_to_real = [
             self._real_hyperparameters_map[hp][self._real_hyperparameters_map_reverse[hp][v]] == v
@@ -519,14 +526,40 @@
         assert np.all(
             np.array([hp in self.gec_hyperparameters for hp in gec_hyperparameters.keys()])
         )
         self.gec_hyperparameters.update(gec_hyperparameters)
         self._set_gec_attributes()
 
 
+    def freeze(self):
+        self.frozen = True
+        return(self)
+
+    def unfreeze(self):
+        self.frozen = False
+        return(self)
+    
+    def get_params(self, deep=True):
+        if hasattr(self, "best_params_") and self.best_params_ is not None:
+            params = copy.deepcopy(self.best_params_)
+        else:
+            params = super().get_params(deep)
+        params["frozen"] = self.frozen
+        
+        return(params)
+
+    def __sklearn_clone__(self):
+        gec = GEC()
+
+        for k, v in self.__dict__.items():
+            gec.__dict__[k] = copy.deepcopy(v)
+
+        return(gec)
+
+
     def fit(
             self,
             X,
             y,
             n_iter=50,
             fixed_hyperparameters=["n_estimators", "num_leaves"],
             sample_weight=None,
@@ -550,74 +583,67 @@
         ----------
             n_iter : int
                 number of optimization steps
             fixed_hyperparameters : list[str]
                 list of hyperparameters that should not be optimised
         """
 
-
-        self._fit_params = {
+        self.fit_params = {
             "sample_weight": sample_weight,
             "init_score": init_score,
             "eval_set": eval_set,
             "eval_names": eval_names,
             "eval_sample_weight": eval_sample_weight,
             "eval_class_weight": eval_class_weight,
             "eval_init_score": eval_init_score,
             "eval_metric": eval_metric,
             "feature_name": feature_name,
             "categorical_feature": categorical_feature,
             "callbacks": callbacks,
             "init_model": init_model
         }
+        if not self.frozen:
+            filtered_hyperparameters = list(set(self.gec_hyperparameters["hyperparameters"]).difference(set(fixed_hyperparameters)))
+            self.set_gec_hyperparameters({"hyperparameters": filtered_hyperparameters })
+
+            self.best_scores_gec = {}
+            self.best_params_gec = {}
+            (
+                self.best_params_gec["search"],
+                self.best_scores_gec["search"],
+            ) = self._optimise_hyperparameters(
+                n_iter, X, y, self.best_score, self.best_params_
+            )
+            self.best_params_gec["grid"] = self._find_best_parameters()
+            self.best_scores_gec["grid"] = self._calculate_cv_score(
+                X, y, self.best_params_gec["grid"]
+            )
+            best_params_prep = copy.deepcopy(self.best_params_gec["search"])
+            self.best_params_gec[
+                "grid_from_search"
+            ] = self._find_best_parameters_from_search(best_params_prep)
 
-        filtered_hyperparameters = list(set(self.gec_hyperparameters["hyperparameters"]).difference(set(fixed_hyperparameters)))
-        self.set_gec_hyperparameters({"hyperparameters": filtered_hyperparameters })
-
-        self.best_scores_gec = {}
-        self.best_params_gec = {}
-        (
-            self.best_params_gec["search"],
-            self.best_scores_gec["search"],
-        ) = self._optimise_hyperparameters(
-            n_iter, X, y, self.best_score, self.best_params_
-        )
-        self.best_params_gec["grid"] = self._find_best_parameters()
-        self.best_scores_gec["grid"] = self._calculate_cv_score(
-            X, y, self.best_params_gec["grid"]
-        )
-        best_params_prep = copy.deepcopy(self.best_params_gec["search"])
-        self.best_params_gec[
-            "grid_from_search"
-        ] = self._find_best_parameters_from_search(best_params_prep)
-
-        self.best_scores_gec["grid_from_search"] = self._calculate_cv_score(
-            X, y, self.best_params_gec["grid_from_search"]
-        )
-
-        for source, score in self.best_scores_gec.items():
-            if self.best_score is None or score > self.best_score:
-                self.best_score = score
-                self.best_params_ = self.best_params_gec[source]
+            self.best_scores_gec["grid_from_search"] = self._calculate_cv_score(
+                X, y, self.best_params_gec["grid_from_search"]
+            )
 
-        # hyperparameter_scores, rewards = copy.deepcopy(self.hyperparameter_scores), copy.deepcopy(self.rewards)
-        # selected_arms = copy.deepcopy(self.selected_arms)
+            for source, score in self.best_scores_gec.items():
+                if self.best_score is None or score > self.best_score:
+                    self.best_score = score
+                    self.best_params_ = self.best_params_gec[source]
 
         self._fit_best_params(X, y)
 
-        # self.hyperparameter_scores, self.rewards = hyperparameter_scores, rewards
-        # self.selected_arms = selected_arms
-
         return self
 
     def _calculate_cv_score(self, X, y, params):
         clf = LGBMClassifier(**params)
         try:
             with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
-                cross_val_scores = cross_val_score(clf, X, y, cv=5, fit_params=self._fit_params)
+                cross_val_scores = cross_val_score(clf, X, y, cv=5, fit_params=self.fit_params)
                 score = np.mean(cross_val_scores)
         except:
             warnings.warn(f"Could not calculate cross val scores for parameters: {params}")
             score = 0.0
         return score
 
 
@@ -839,21 +865,20 @@
                 hyperparameter_values,
             )
         )
         return {**arguments, **self.fixed_params,  **self._init_args, **self._init_kwargs}
 
     def _fit_best_params(self, X, y):
 
-        gec = GEC(**{**self.best_params_, "random_state": 101})
-
-        for k, v in gec.__dict__.items():
-            if k not in self.__dict__ or self.__dict__[k] is None:
-                self.__dict__[k] = v
+        if hasattr(self, "best_params_") and self.best_params_ is not None:
+            for k, v in self.best_params_.items():
+                setattr(self, k, v)
+                setattr(self, "random_state", 101)
 
-        super().fit(X, y)
+        super().fit(X, y, **self.fit_params)
 
     def _fit_gaussian(self):
         self.gaussian.fit(
             np.array(self.hyperparameter_scores["inputs"]),
             np.array(self.hyperparameter_scores["output"]) - np.mean(self.hyperparameter_scores["output"]),
         )
 
@@ -898,15 +923,15 @@
 
         if "bagging_freq" in params:
             del params["bagging_freq"]
             del params["bagging_fraction"]
             bagging = "yes_bagging"
         else:
             bagging = "no_bagging"
-        boosting = params.pop("boosting")
+        boosting = params.pop("boosting_type")
         best_arm = f"{boosting}-{bagging}"
 
         best_params_linear_values = [
             self._real_hyperparameters_map_reverse[name][params[name]]
             for name in self._real_hyperparameter_names
         ]
         best_params = self._find_best_parameters_from_initial_parameters(
```

### Comparing `gecs-0.28.1/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.28.2/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.28.1/setup.py` & `gecs-0.28.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.28.1',
+    'version': '0.28.2',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
-    'long_description': "![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Project Overview\n\nThe package `gecs` provides the class `GEC`, which is a child class of the class `LGBMClassifier` from the package `lightgbm`. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API. The difference to `LGBMClassifier` lies in the fact that `GEC`automatically does bayesian hyperparameter optimization of the parameters `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree` and optionally also of `num_leaves` and `n_estimators`.\n\nThe fit method has two new parameters: `n_iter`, which sets the number of hyperparameter combinations that will be tried (the higher `n_iter` the higher the expected accuracy, but at a cost of compute) and `fixed_hyperparameters`, which determines which hyperparameters of the LGBM classifier won't get optimized. By default, these are `n_estimators` and `num_leaves`, as the highest possible value for these hyperparameters is almost always optimal. The idea then is to set these as high as makes sense in a specific context and then optimize the other hyperparameters.\n\n\n## Installation\n\n    pip install gecs\n\n## Usage\n\n    from gecs.gec import GEC\n\n    gec.fit(X, y)\n\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n\n    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I'll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)",
+    'long_description': "![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Project Overview\n\nThe package `gecs` provides the class `GEC`, which is a child class of the class `LGBMClassifier` from the package `lightgbm`. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API. The difference to `LGBMClassifier` lies in the fact that `GEC`automatically does bayesian hyperparameter optimization of the parameters `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree` and optionally also of `num_leaves` and `n_estimators`.\n\nThe fit method has two new parameters: `n_iter`, which sets the number of hyperparameter combinations that will be tried (the higher `n_iter` the higher the expected accuracy, but at a cost of compute) and `fixed_hyperparameters`, which determines which hyperparameters of the LGBM classifier won't get optimized. By default, these are `n_estimators` and `num_leaves`, as the highest possible value for these hyperparameters is almost always optimal. The idea then is to set these as high as makes sense in a specific context and then optimize the other hyperparameters.\n\n\n## Installation\n\n    pip install gecs\n\n## Usage\n\n    from gecs.gec import GEC\n\n    gec.fit(X, y)\n\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n\n    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier\n\n    yhat = gec.predict(X)\n\n    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier\n    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation\n\n\n    \n\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I'll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)",
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `gecs-0.28.1/PKG-INFO` & `gecs-0.28.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.28.1
+Version: 0.28.2
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
@@ -56,14 +56,23 @@
 
     gec.fit(X, y)
 
     gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
 
     gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier
 
+    yhat = gec.predict(X)
+
+    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier
+    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
+
+
+    
+
+
 
 ## Contributing
 
 If you want to contribute, please reach out and I'll design a process around it.
 
 ## License
```

