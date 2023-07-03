# Comparing `tmp/gecs-0.28.2.tar.gz` & `tmp/gecs-0.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.28.2.tar", max compression
+gzip compressed data, was "gecs-0.28.3.tar", max compression
```

## Comparing `gecs-0.28.2.tar` & `gecs-0.28.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.28.2/LICENSE
--rw-r--r--   0        0        0     2220 2023-07-03 10:39:36.682086 gecs-0.28.2/README.md
--rw-r--r--   0        0        0      697 2023-07-03 10:39:36.682086 gecs-0.28.2/pyproject.toml
--rw-r--r--   0        0        0    44045 2023-07-03 10:39:36.682086 gecs-0.28.2/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.28.2/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 gecs-0.28.2/setup.py
--rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 gecs-0.28.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.28.3/LICENSE
+-rw-r--r--   0        0        0     2220 2023-07-03 10:39:36.682086 gecs-0.28.3/README.md
+-rw-r--r--   0        0        0      697 2023-07-03 17:47:08.299609 gecs-0.28.3/pyproject.toml
+-rw-r--r--   0        0        0    44198 2023-07-03 17:47:08.299609 gecs-0.28.3/src/gecs/gec.py
+-rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.28.3/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 gecs-0.28.3/setup.py
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 gecs-0.28.3/PKG-INFO
```

### Comparing `gecs-0.28.2/LICENSE` & `gecs-0.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.28.2/README.md` & `gecs-0.28.3/README.md`

 * *Files identical despite different names*

### Comparing `gecs-0.28.2/pyproject.toml` & `gecs-0.28.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.28.2"
+version = "0.28.3"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.28.2/src/gecs/gec.py` & `gecs-0.28.3/src/gecs/gec.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,14 +534,21 @@
         self.frozen = True
         return(self)
 
     def unfreeze(self):
         self.frozen = False
         return(self)
     
+
+    def set_params(self, **kwargs):
+        if "frozen" in kwargs:
+            self["frozen"] = kwargs.pop("frozen")
+        super().set_params(**kwargs)
+
+
     def get_params(self, deep=True):
         if hasattr(self, "best_params_") and self.best_params_ is not None:
             params = copy.deepcopy(self.best_params_)
         else:
             params = super().get_params(deep)
         params["frozen"] = self.frozen
         
@@ -868,15 +875,15 @@
         return {**arguments, **self.fixed_params,  **self._init_args, **self._init_kwargs}
 
     def _fit_best_params(self, X, y):
 
         if hasattr(self, "best_params_") and self.best_params_ is not None:
             for k, v in self.best_params_.items():
                 setattr(self, k, v)
-                setattr(self, "random_state", 101)
+            setattr(self, "random_state", 101)
 
         super().fit(X, y, **self.fit_params)
 
     def _fit_gaussian(self):
         self.gaussian.fit(
             np.array(self.hyperparameter_scores["inputs"]),
             np.array(self.hyperparameter_scores["output"]) - np.mean(self.hyperparameter_scores["output"]),
```

### Comparing `gecs-0.28.2/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.28.3/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.28.2/setup.py` & `gecs-0.28.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.28.2',
+    'version': '0.28.3',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
     'long_description': "![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Project Overview\n\nThe package `gecs` provides the class `GEC`, which is a child class of the class `LGBMClassifier` from the package `lightgbm`. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API. The difference to `LGBMClassifier` lies in the fact that `GEC`automatically does bayesian hyperparameter optimization of the parameters `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree` and optionally also of `num_leaves` and `n_estimators`.\n\nThe fit method has two new parameters: `n_iter`, which sets the number of hyperparameter combinations that will be tried (the higher `n_iter` the higher the expected accuracy, but at a cost of compute) and `fixed_hyperparameters`, which determines which hyperparameters of the LGBM classifier won't get optimized. By default, these are `n_estimators` and `num_leaves`, as the highest possible value for these hyperparameters is almost always optimal. The idea then is to set these as high as makes sense in a specific context and then optimize the other hyperparameters.\n\n\n## Installation\n\n    pip install gecs\n\n## Usage\n\n    from gecs.gec import GEC\n\n    gec.fit(X, y)\n\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n\n    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier\n\n    yhat = gec.predict(X)\n\n    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier\n    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation\n\n\n    \n\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I'll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)",
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
```

### Comparing `gecs-0.28.2/PKG-INFO` & `gecs-0.28.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.28.2
+Version: 0.28.3
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
```

