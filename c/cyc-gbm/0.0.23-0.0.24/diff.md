# Comparing `tmp/cyc-gbm-0.0.23.tar.gz` & `tmp/cyc-gbm-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyc-gbm-0.0.23.tar", last modified: Fri Jun 30 08:49:36 2023, max compression
+gzip compressed data, was "cyc-gbm-0.0.24.tar", last modified: Mon Jul  3 09:28:40 2023, max compression
```

## Comparing `cyc-gbm-0.0.23.tar` & `cyc-gbm-0.0.24.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.170157 cyc-gbm-0.0.23/
--rw-r--r--   0 Henning    (501) staff       (20)     1073 2023-06-28 08:34:18.000000 cyc-gbm-0.0.23/LICENSE
--rw-r--r--   0 Henning    (501) staff       (20)       24 2023-06-30 07:06:30.000000 cyc-gbm-0.0.23/MANIFEST.in
--rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 08:49:36.169420 cyc-gbm-0.0.23/PKG-INFO
--rw-r--r--   0 Henning    (501) staff       (20)     2399 2023-06-30 07:06:30.000000 cyc-gbm-0.0.23/README.md
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.158284 cyc-gbm-0.0.23/cyc_gbm/
--rw-r--r--   0 Henning    (501) staff       (20)       75 2023-06-12 14:42:41.000000 cyc-gbm-0.0.23/cyc_gbm/__init__.py
--rw-r--r--   0 Henning    (501) staff       (20)     5303 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/baseline_models.py
--rw-r--r--   0 Henning    (501) staff       (20)     7198 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/cyc_gbm.py
--rw-r--r--   0 Henning    (501) staff       (20)    26784 2023-06-30 08:48:10.000000 cyc-gbm-0.0.23/cyc_gbm/distributions.py
--rw-r--r--   0 Henning    (501) staff       (20)     4030 2023-06-28 11:01:36.000000 cyc-gbm-0.0.23/cyc_gbm/gbm_tree.py
--rw-r--r--   0 Henning    (501) staff       (20)     3054 2023-06-12 14:42:41.000000 cyc-gbm-0.0.23/cyc_gbm/logger.py
--rw-r--r--   0 Henning    (501) staff       (20)    12282 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/numerical_illustration.py
--rw-r--r--   0 Henning    (501) staff       (20)     6461 2023-06-28 11:32:48.000000 cyc-gbm-0.0.23/cyc_gbm/tune_kappa.py
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.166387 cyc-gbm-0.0.23/cyc_gbm.egg-info/
--rw-r--r--   0 Henning    (501) staff       (20)     2898 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/PKG-INFO
--rw-r--r--   0 Henning    (501) staff       (20)      431 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/SOURCES.txt
--rw-r--r--   0 Henning    (501) staff       (20)        1 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/dependency_links.txt
--rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/requires.txt
--rw-r--r--   0 Henning    (501) staff       (20)        8 2023-06-30 08:49:36.000000 cyc-gbm-0.0.23/cyc_gbm.egg-info/top_level.txt
--rw-r--r--   0 Henning    (501) staff       (20)      475 2023-06-28 08:34:18.000000 cyc-gbm-0.0.23/pyproject.toml
--rw-r--r--   0 Henning    (501) staff       (20)       62 2023-06-30 07:06:30.000000 cyc-gbm-0.0.23/requirements.txt
--rw-r--r--   0 Henning    (501) staff       (20)       38 2023-06-30 08:49:36.170421 cyc-gbm-0.0.23/setup.cfg
--rw-r--r--   0 Henning    (501) staff       (20)      871 2023-06-30 08:48:27.000000 cyc-gbm-0.0.23/setup.py
-drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-06-30 08:49:36.167394 cyc-gbm-0.0.23/tests/
--rw-r--r--   0 Henning    (501) staff       (20)    17413 2023-06-28 11:49:31.000000 cyc-gbm-0.0.23/tests/test_cyc_gbm.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-07-03 09:28:40.134729 cyc-gbm-0.0.24/
+-rw-r--r--   0 Henning    (501) staff       (20)     1073 2023-06-28 08:34:18.000000 cyc-gbm-0.0.24/LICENSE
+-rw-r--r--   0 Henning    (501) staff       (20)       24 2023-06-30 07:06:30.000000 cyc-gbm-0.0.24/MANIFEST.in
+-rw-r--r--   0 Henning    (501) staff       (20)     3315 2023-07-03 09:28:40.104744 cyc-gbm-0.0.24/PKG-INFO
+-rw-r--r--   0 Henning    (501) staff       (20)     2816 2023-07-03 09:27:48.000000 cyc-gbm-0.0.24/README.md
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-07-03 09:28:40.041504 cyc-gbm-0.0.24/cyc_gbm/
+-rw-r--r--   0 Henning    (501) staff       (20)       45 2023-07-03 09:26:23.000000 cyc-gbm-0.0.24/cyc_gbm/__init__.py
+-rw-r--r--   0 Henning    (501) staff       (20)     4034 2023-07-03 09:26:23.000000 cyc-gbm-0.0.24/cyc_gbm/boosting_tree.py
+-rw-r--r--   0 Henning    (501) staff       (20)     7244 2023-07-03 09:26:23.000000 cyc-gbm-0.0.24/cyc_gbm/cyc_gbm.py
+-rw-r--r--   0 Henning    (501) staff       (20)    26804 2023-06-30 09:14:05.000000 cyc-gbm-0.0.24/cyc_gbm/distributions.py
+-rw-r--r--   0 Henning    (501) staff       (20)     3054 2023-06-12 14:42:41.000000 cyc-gbm-0.0.24/cyc_gbm/logger.py
+-rw-r--r--   0 Henning    (501) staff       (20)     6495 2023-07-03 09:26:23.000000 cyc-gbm-0.0.24/cyc_gbm/tune_kappa.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-07-03 09:28:40.078956 cyc-gbm-0.0.24/cyc_gbm.egg-info/
+-rw-r--r--   0 Henning    (501) staff       (20)     3315 2023-07-03 09:28:39.000000 cyc-gbm-0.0.24/cyc_gbm.egg-info/PKG-INFO
+-rw-r--r--   0 Henning    (501) staff       (20)      375 2023-07-03 09:28:39.000000 cyc-gbm-0.0.24/cyc_gbm.egg-info/SOURCES.txt
+-rw-r--r--   0 Henning    (501) staff       (20)        1 2023-07-03 09:28:39.000000 cyc-gbm-0.0.24/cyc_gbm.egg-info/dependency_links.txt
+-rw-r--r--   0 Henning    (501) staff       (20)       62 2023-07-03 09:28:39.000000 cyc-gbm-0.0.24/cyc_gbm.egg-info/requires.txt
+-rw-r--r--   0 Henning    (501) staff       (20)        8 2023-07-03 09:28:39.000000 cyc-gbm-0.0.24/cyc_gbm.egg-info/top_level.txt
+-rw-r--r--   0 Henning    (501) staff       (20)      475 2023-06-28 08:34:18.000000 cyc-gbm-0.0.24/pyproject.toml
+-rw-r--r--   0 Henning    (501) staff       (20)       62 2023-07-02 18:17:49.000000 cyc-gbm-0.0.24/requirements.txt
+-rw-r--r--   0 Henning    (501) staff       (20)       38 2023-07-03 09:28:40.134953 cyc-gbm-0.0.24/setup.cfg
+-rw-r--r--   0 Henning    (501) staff       (20)      871 2023-07-03 09:26:45.000000 cyc-gbm-0.0.24/setup.py
+drwxr-xr-x   0 Henning    (501) staff       (20)        0 2023-07-03 09:28:40.079444 cyc-gbm-0.0.24/tests/
+-rw-r--r--   0 Henning    (501) staff       (20)    16361 2023-07-03 09:26:23.000000 cyc-gbm-0.0.24/tests/test_cyc_gbm.py
```

### Comparing `cyc-gbm-0.0.23/LICENSE` & `cyc-gbm-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.23/PKG-INFO` & `cyc-gbm-0.0.24/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc-gbm
-Version: 0.0.23
+Version: 0.0.24
 Summary: A python package for the Cyclical Gradient Boosting Machine algorithm
 Home-page: https://github.com/henningzakrisson/cyc-gbm
 Author: Henning Zakrisson
 Author-email: henning.zakrisson@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,16 @@
 A package for the Cyclical Gradient Boosting Machine algorithm. For the (pre-print) paper describing the algorithm, see [here](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4352505).
 
 ## Installation
 You can install the package using pip:
 ```bash
 pip install cyc-gbm
 ```
-Alternatively, you can install the package from source by following these steps:
+Alternatively, you can install the package from source.
+This will also include scripts for reproducing the results in the papar. Follow these steps:
 
 1. Clone this repository to your local machine:
     ```bash
     git clone https://github.com/henningzakrisson/c-gbm.git
     ```
 2. Create a virtual environment in the root directory of the repository:
     ```bash
@@ -40,46 +41,50 @@
     pip install -r requirements.txt
     ```
 ## Usage example
 Fitting the mean and (log) sigma parameters of a normal distribution to a simulated dataset:
 
 ```python
 import numpy as np
-from cyc_gbm import CycGBM
+from cyc_gbm import CyclicalGradientBooster
 from sklearn.model_selection import train_test_split
 
 # Simulate data
 X = np.random.normal(size=(1000, 2))
 mu = X[:, 0] + 10 * (X[:, 1] > 0)
 sigma = np.exp(3 - 2 * (X[:, 0] > 0))
 y = np.random.normal(mu, sigma)
 
 # Split data
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 
 # Fit model
-model = CycGBM(
+model = CyclicalGradientBooster(
    distribution='normal',
-   kappa=[26,34],
+   kappa=[26, 34],
    eps=0.1,
    max_depth=2,
    min_samples_leaf=20,
 )
 model.fit(X_train, y_train)
 
 # Evaluate
 loss = model.dist.loss(y=y_test, z=model.predict(X_test)).sum()
 print(f'negative log likelihood: {loss}')
 ```
 
 ## Reproducing the numerical illustrations in the paper
-The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````src/numerical_illustration.py```` module. 
+The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````numerical_illustration/numerical_illustration.py```` module. 
 The function takes the path to a configuration file as input. 
 The configuration file is a yaml file that specifies the parameters of the numerical illustration.
-An example configuration file can be found in ````config/simulation_config.yaml````.
+An example configuration file can be found in ````numerical_illustration/config/simulation_config.yaml````.
 For running several experiments in one run, I refer to the ````numerical_illustrations```` function in the same module. 
 See the documentation for usage.
-An example configuration file for running several experiments can be found in ````config/simulation_run/master_config.yaml````.
+An example configuration file for running several experiments can be found in ````numerical_illustration/config/simulation_run/master_config.yaml````.
+
+## Not yet implemented
+- [ ] Add support for categorical features (currently the trees are based on ````sklearn.tree.DecisionTreeRegressor```` which does not support categorical features)
+- [ ] Add other tuning methods (such as adaptive shrinkage)
 
 ## Contact
 If you have any questions, feel free to contact me [here](mailto:henning.zakrisson@gmail.com).
```

### Comparing `cyc-gbm-0.0.23/README.md` & `cyc-gbm-0.0.24/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 A package for the Cyclical Gradient Boosting Machine algorithm. For the (pre-print) paper describing the algorithm, see [here](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4352505).
 
 ## Installation
 You can install the package using pip:
 ```bash
 pip install cyc-gbm
 ```
-Alternatively, you can install the package from source by following these steps:
+Alternatively, you can install the package from source.
+This will also include scripts for reproducing the results in the papar. Follow these steps:
 
 1. Clone this repository to your local machine:
     ```bash
     git clone https://github.com/henningzakrisson/c-gbm.git
     ```
 2. Create a virtual environment in the root directory of the repository:
     ```bash
@@ -25,46 +26,50 @@
     pip install -r requirements.txt
     ```
 ## Usage example
 Fitting the mean and (log) sigma parameters of a normal distribution to a simulated dataset:
 
 ```python
 import numpy as np
-from cyc_gbm import CycGBM
+from cyc_gbm import CyclicalGradientBooster
 from sklearn.model_selection import train_test_split
 
 # Simulate data
 X = np.random.normal(size=(1000, 2))
 mu = X[:, 0] + 10 * (X[:, 1] > 0)
 sigma = np.exp(3 - 2 * (X[:, 0] > 0))
 y = np.random.normal(mu, sigma)
 
 # Split data
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 
 # Fit model
-model = CycGBM(
+model = CyclicalGradientBooster(
    distribution='normal',
-   kappa=[26,34],
+   kappa=[26, 34],
    eps=0.1,
    max_depth=2,
    min_samples_leaf=20,
 )
 model.fit(X_train, y_train)
 
 # Evaluate
 loss = model.dist.loss(y=y_test, z=model.predict(X_test)).sum()
 print(f'negative log likelihood: {loss}')
 ```
 
 ## Reproducing the numerical illustrations in the paper
-The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````src/numerical_illustration.py```` module. 
+The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````numerical_illustration/numerical_illustration.py```` module. 
 The function takes the path to a configuration file as input. 
 The configuration file is a yaml file that specifies the parameters of the numerical illustration.
-An example configuration file can be found in ````config/simulation_config.yaml````.
+An example configuration file can be found in ````numerical_illustration/config/simulation_config.yaml````.
 For running several experiments in one run, I refer to the ````numerical_illustrations```` function in the same module. 
 See the documentation for usage.
-An example configuration file for running several experiments can be found in ````config/simulation_run/master_config.yaml````.
+An example configuration file for running several experiments can be found in ````numerical_illustration/config/simulation_run/master_config.yaml````.
+
+## Not yet implemented
+- [ ] Add support for categorical features (currently the trees are based on ````sklearn.tree.DecisionTreeRegressor```` which does not support categorical features)
+- [ ] Add other tuning methods (such as adaptive shrinkage)
 
 ## Contact
 If you have any questions, feel free to contact me [here](mailto:henning.zakrisson@gmail.com).
```

### Comparing `cyc-gbm-0.0.23/cyc_gbm/cyc_gbm.py` & `cyc-gbm-0.0.24/cyc_gbm/cyc_gbm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Union, Optional
 
 import numpy as np
 
 from cyc_gbm.distributions import Distribution, initiate_distribution
 from cyc_gbm.logger import CycGBMLogger
-from cyc_gbm.gbm_tree import GBMTree
+from cyc_gbm.boosting_tree import BoostingTree
 
 
-class CycGBM:
+class CyclicalGradientBooster:
     """
-    Class for cyclical gradient boosting machine regressors
+    Class for cyclical gradient boosting regressors
     """
 
     def __init__(
         self,
         kappa: Union[int, List[int]] = 100,
         eps: Union[float, List[float]] = 0.1,
         max_depth: Union[int, List[int]] = 2,
@@ -85,15 +85,15 @@
             w = np.ones(len(y)) * w
         self.z0 = self.dist.mle(y=y, w=w)[:, None]
         z = np.tile(self.z0, (1, len(y)))
         for k in range(0, max(self.kappa)):
             for j in range(self.d):
                 if k >= self.kappa[j]:
                     continue
-                tree = GBMTree(
+                tree = BoostingTree(
                     max_depth=self.max_depth[j],
                     min_samples_leaf=self.min_samples_leaf[j],
                     distribution=self.dist,
                 )
                 tree.fit_gradients(X=X, y=y, z=z, w=w, j=j)
                 z[j] += self.eps[j] * tree.predict(X)
                 self.trees[j][k] = tree
@@ -115,15 +115,15 @@
         :param y: The target values for the training data.
         :param j: Parameter dimension to update
         :param w: Weights for the training data, of shape (n_samples,). Default is 1 for all samples.
         """
         if isinstance(w, float):
             w = np.ones(len(y)) * w
         z = self.predict(X)
-        tree = GBMTree(
+        tree = BoostingTree(
             max_depth=self.max_depth[j],
             min_samples_leaf=self.min_samples_leaf[j],
             distribution=self.dist,
         )
         tree.fit_gradients(X=X, y=y, z=z, w=w, j=j)
         self.trees[j] += [tree]
         self.kappa[j] += 1
@@ -184,9 +184,9 @@
     z2 = 0.2 * X[:, 3] + 0.03 * X[:, 2] ** 2
     z = np.stack([z0, z1, z2])
     distribution = initiate_distribution(distribution="multivariate_normal")
     y = distribution.simulate(z=z, random_state=5)
 
     kappa = [23, 17, 79]
     eps = [0.5, 0.25, 0.1]
-    gbm = CycGBM(distribution="multivariate_normal", kappa=kappa, eps=eps)
+    gbm = CyclicalGradientBooster(distribution="multivariate_normal", kappa=kappa, eps=eps)
     gbm.fit(X, y)
```

### Comparing `cyc-gbm-0.0.23/cyc_gbm/distributions.py` & `cyc-gbm-0.0.24/cyc_gbm/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,16 +157,16 @@
         self,
     ):
         """Initialize a multivariate normal distribution object with equal means and variances and
         correlation
 
         Parameterization: z[0] = mu, z[1] = 2*log(sigma), z[2] = inv_sigm(rho)
         where
-        E[X] = [w*mu,w*mu]
-        Cov(X) = w*[sigma^2, rho*sigma^2; rho*sigma^2, sigma^2]
+        E[Y] = [w*mu,w*mu]
+        Cov(Y) = w*[sigma^2, rho*sigma^2; rho*sigma^2, sigma^2]
         """
         super().__init__(d=3)
 
     def loss(
         self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         if np.any(w != 1):
@@ -283,15 +283,15 @@
 @inherit_docstrings
 class NormalDistribution(Distribution):
     def __init__(
         self,
     ):
         """Initialize a normal distribution object.
 
-        Parameterization: z[0] = mu, z[1] = log(sigma), where E[X] = w*mu, Var(X) = w*sigma^2
+        Parameterization: z[0] = mu, z[1] = log(sigma), where E[Y] = w*mu, Var(Y) = w*sigma^2
         """
         super().__init__(d=2)
 
     def loss(
         self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         return (
@@ -330,21 +330,22 @@
         self, z: np.ndarray, k: int, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         if k == 1:
             return w * z[0]
         elif k == 2:
             return w * np.exp(2 * z[1])
 
+@inherit_docstrings
 class NormalDistributionUni(Distribution):
     def __init__(
         self,
     ):
         """Initialize a normal distribution object with only the mu parameter.
 
-        Parameterization: z[0] = mu, where E[X] = mu, Var(X) = 1
+        Parameterization: z[0] = mu, where E[Y] = mu, Var(Y) = 1
         """
         super().__init__(d=1)
 
     def loss(
         self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         if np.any(w != 1):
@@ -380,15 +381,15 @@
 @inherit_docstrings
 class NegativeBinomialDistribution(Distribution):
     def __init__(
         self,
     ):
         """Initialize a negative binomial distribution object.
 
-        Parameterization: z[0] = np.log(mu), z[1] = log(theta), where E[X] = w*mu, Var(X) = w*mu*(1+mu/theta)
+        Parameterization: z[0] = np.log(mu), z[1] = log(theta), where E[Y] = w*mu, Var(Y) = w*mu*(1+mu/theta)
         """
         super().__init__(d=2)
 
     def loss(
         self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         return (
@@ -454,15 +455,15 @@
 @inherit_docstrings
 class InverseGaussianDistribution(Distribution):
     def __init__(
         self,
     ):
         """Initialize a inverse Gaussian distribution object.
 
-        Parameterization: z[0] = log(mu), z[1] = log(lambda), where E[X] = w*mu, Var(X) =w*mu^3 / lambda
+        Parameterization: z[0] = log(mu), z[1] = log(lambda), where E[Y] = w*mu, Var(Y) =w*mu^3 / lambda
         """
         super().__init__(d=2)
 
     def loss(
         self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         if np.any(w != 1):
@@ -532,15 +533,15 @@
 class GammaDistribution(Distribution):
     def __init__(
         self,
     ):
         """
         Initialize a gamma distribution object.
 
-        Parameterization: z[0] = log(mu), z[1] = log(phi), where E[X] = w*mu, Var(X) =w*phi * mu^2
+        Parameterization: z[0] = log(mu), z[1] = log(phi), where E[Y] = w*mu, Var(Y) =w*phi * mu^2
         """
         super().__init__(d=2)
 
     def loss(
         self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         return (
@@ -604,15 +605,15 @@
 class BetaPrimeDistribution(Distribution):
     def __init__(
         self,
     ):
         """
         Initialize a beta prime distribution object.
 
-        Parameterization: z[0] = log(mu), z[1] = log(v), where E[X] = w*mu, Var(X) =w*mu*(1+mu)/v
+        Parameterization: z[0] = log(mu), z[1] = log(v), where E[Y] = w*mu, Var(Y) =w*mu*(1+mu)/v
         """
         super().__init__(d=2)
 
     def loss(
         self, y: np.ndarray, z: np.ndarray, w: Union[np.ndarray, float] = 1.0
     ) -> np.ndarray:
         if np.any(np.any(w != 1)):
```

### Comparing `cyc-gbm-0.0.23/cyc_gbm/gbm_tree.py` & `cyc-gbm-0.0.24/cyc_gbm/boosting_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from sklearn.tree import DecisionTreeRegressor
 
 from .distributions import Distribution
 
 
-class GBMTree(DecisionTreeRegressor):
+class BoostingTree(DecisionTreeRegressor):
     """
     A Gradient Boosting Machine tree.
 
     :param max_depth: The maximum depth of the tree.
     :param min_samples_leaf: The minimum number of samples required to be at a leaf node.
     :param distribution: The distribution function used for calculating the gradients.
 
@@ -98,15 +98,15 @@
         """
         Fits the GBMTree to the negative gradients and adjusts node values to minimize loss.
 
         :param X: The training input samples.
         :param y: The target values.
         :param z: The predicted parameter values from the previous iteration.
         :param w: Weights for the training data, of shape (n_samples,).
-        :param j: The index of the current iteration.
+        :param j: The parameter dimension to update.
         """
         g = self.distribution.grad(y=y, z=z, w=w, j=j)
         self.fit(X, -g)
         self._adjust_node_values(X=X, y=y, z=z, w=w, j=j)
 
     def feature_importances(self) -> np.ndarray:
         """
```

### Comparing `cyc-gbm-0.0.23/cyc_gbm/logger.py` & `cyc-gbm-0.0.24/cyc_gbm/logger.py`

 * *Files identical despite different names*

### Comparing `cyc-gbm-0.0.23/cyc_gbm/tune_kappa.py` & `cyc-gbm-0.0.24/cyc_gbm/tune_kappa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union, List, Dict, Tuple, Optional
 import logging
 
 import numpy as np
 
-from cyc_gbm import CycGBM
+from cyc_gbm import CyclicalGradientBooster
 from cyc_gbm.distributions import initiate_distribution, Distribution
 from cyc_gbm.logger import CycGBMLogger
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 logger.addHandler(logging.StreamHandler())
 formatter = logging.Formatter("[%(asctime)s][%(message)s]", datefmt="%Y-%m-%d %H:%M")
@@ -88,15 +88,15 @@
     for i, idx in enumerate(folds):
         logger.append_format_level(f"fold {i+1}/{n_splits}")
         logger.log("tuning", verbose=1)
         idx_train, idx_valid = idx
         X_train, y_train, w_train = X[idx_train], y[idx_train], w[idx_train]
         X_valid, y_valid, w_valid = X[idx_valid], y[idx_valid], w[idx_valid]
 
-        gbm = CycGBM(
+        gbm = CyclicalGradientBooster(
             kappa=0,
             eps=eps,
             max_depth=max_depth,
             min_samples_leaf=min_samples_leaf,
             distribution=distribution,
         )
         gbm.fit(X_train, y_train, w_train)
```

### Comparing `cyc-gbm-0.0.23/cyc_gbm.egg-info/PKG-INFO` & `cyc-gbm-0.0.24/cyc_gbm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyc-gbm
-Version: 0.0.23
+Version: 0.0.24
 Summary: A python package for the Cyclical Gradient Boosting Machine algorithm
 Home-page: https://github.com/henningzakrisson/cyc-gbm
 Author: Henning Zakrisson
 Author-email: henning.zakrisson@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,16 @@
 A package for the Cyclical Gradient Boosting Machine algorithm. For the (pre-print) paper describing the algorithm, see [here](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4352505).
 
 ## Installation
 You can install the package using pip:
 ```bash
 pip install cyc-gbm
 ```
-Alternatively, you can install the package from source by following these steps:
+Alternatively, you can install the package from source.
+This will also include scripts for reproducing the results in the papar. Follow these steps:
 
 1. Clone this repository to your local machine:
     ```bash
     git clone https://github.com/henningzakrisson/c-gbm.git
     ```
 2. Create a virtual environment in the root directory of the repository:
     ```bash
@@ -40,46 +41,50 @@
     pip install -r requirements.txt
     ```
 ## Usage example
 Fitting the mean and (log) sigma parameters of a normal distribution to a simulated dataset:
 
 ```python
 import numpy as np
-from cyc_gbm import CycGBM
+from cyc_gbm import CyclicalGradientBooster
 from sklearn.model_selection import train_test_split
 
 # Simulate data
 X = np.random.normal(size=(1000, 2))
 mu = X[:, 0] + 10 * (X[:, 1] > 0)
 sigma = np.exp(3 - 2 * (X[:, 0] > 0))
 y = np.random.normal(mu, sigma)
 
 # Split data
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 
 # Fit model
-model = CycGBM(
+model = CyclicalGradientBooster(
    distribution='normal',
-   kappa=[26,34],
+   kappa=[26, 34],
    eps=0.1,
    max_depth=2,
    min_samples_leaf=20,
 )
 model.fit(X_train, y_train)
 
 # Evaluate
 loss = model.dist.loss(y=y_test, z=model.predict(X_test)).sum()
 print(f'negative log likelihood: {loss}')
 ```
 
 ## Reproducing the numerical illustrations in the paper
-The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````src/numerical_illustration.py```` module. 
+The numerical illustrations in the paper can be reproduced by running the ````numerical_illustration```` function in the ````numerical_illustration/numerical_illustration.py```` module. 
 The function takes the path to a configuration file as input. 
 The configuration file is a yaml file that specifies the parameters of the numerical illustration.
-An example configuration file can be found in ````config/simulation_config.yaml````.
+An example configuration file can be found in ````numerical_illustration/config/simulation_config.yaml````.
 For running several experiments in one run, I refer to the ````numerical_illustrations```` function in the same module. 
 See the documentation for usage.
-An example configuration file for running several experiments can be found in ````config/simulation_run/master_config.yaml````.
+An example configuration file for running several experiments can be found in ````numerical_illustration/config/simulation_run/master_config.yaml````.
+
+## Not yet implemented
+- [ ] Add support for categorical features (currently the trees are based on ````sklearn.tree.DecisionTreeRegressor```` which does not support categorical features)
+- [ ] Add other tuning methods (such as adaptive shrinkage)
 
 ## Contact
 If you have any questions, feel free to contact me [here](mailto:henning.zakrisson@gmail.com).
```

### Comparing `cyc-gbm-0.0.23/setup.py` & `cyc-gbm-0.0.24/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="cyc-gbm",
-    version="0.0.23",
+    version="0.0.24",
     author="Henning Zakrisson",
     author_email="henning.zakrisson@gmail.com",
     description="A python package for the Cyclical Gradient Boosting Machine algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/henningzakrisson/cyc-gbm",
     packages=find_packages(),
```

### Comparing `cyc-gbm-0.0.23/tests/test_cyc_gbm.py` & `cyc-gbm-0.0.24/tests/test_cyc_gbm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import numpy as np
 
-from cyc_gbm import CycGBM, CycGLM
+from cyc_gbm import CyclicalGradientBooster
 from cyc_gbm.tune_kappa import tune_kappa
 from cyc_gbm.distributions import initiate_distribution
 
 
 class GBMTests(unittest.TestCase):
     """
     A class that defines unit tests for the `GBM` classes.
@@ -26,15 +26,15 @@
         z_0 = 10 * (X[:, 0] > 0.3 * n) + 5 * (X[:, 1] > 0.5 * n)
         z_1 = np.ones(n) * np.log(1.5)
         z = np.stack([z_0, z_1])
         dist = initiate_distribution(distribution="normal")
         y = dist.simulate(z, random_state=10)
 
         kappa = [100, 0]
-        gbm = CycGBM(distribution="normal", kappa=kappa)
+        gbm = CyclicalGradientBooster(distribution="normal", kappa=kappa)
         gbm.fit(X, y)
         loss = gbm.dist.loss(y=y, z=gbm.predict(X)).sum()
 
         self.assertAlmostEqual(
             first=51.017764411696184,
             second=loss,
             places=5,
@@ -56,15 +56,15 @@
         z_1 = np.ones(n) * np.log(1)
         z = np.stack([z_0, z_1])
         dist = initiate_distribution(distribution="gamma")
         y = dist.simulate(z, random_state=10)
 
         kappa = [100, 0]
         eps = 0.1
-        gbm = CycGBM(distribution="gamma", kappa=kappa, eps=eps)
+        gbm = CyclicalGradientBooster(distribution="gamma", kappa=kappa, eps=eps)
         gbm.fit(X, y)
         loss = gbm.dist.loss(y=y, z=gbm.predict(X)).sum()
 
         self.assertAlmostEqual(
             first=130.9327996047943,
             second=loss,
             places=5,
@@ -114,15 +114,15 @@
         X = np.stack([X0, X1]).T
         y = rng.normal(mu, sigma)
 
         kappas = [100, 10]
         eps = 0.1
         max_depth = 2
         min_samples_leaf = 20
-        gbm = CycGBM(
+        gbm = CyclicalGradientBooster(
             kappa=kappas,
             eps=eps,
             min_samples_leaf=min_samples_leaf,
             max_depth=max_depth,
         )
         gbm.fit(X, y)
         z_hat = gbm.predict(X)
@@ -154,15 +154,15 @@
         phi = np.exp(1 + 1 * (X0 < 0.4 * n))
 
         X = np.stack([X0, X1]).T
         y = rng.gamma(1 / phi, mu * phi)
 
         kappas = [15, 30]
         eps = 0.1
-        gbm = CycGBM(kappa=kappas, eps=eps, distribution="gamma")
+        gbm = CyclicalGradientBooster(kappa=kappas, eps=eps, distribution="gamma")
         gbm.fit(X, y)
         z_hat = gbm.predict(X)
 
         loss = gbm.dist.loss(y=y, z=z_hat).sum()
 
         self.assertAlmostEqual(
             first=expected_loss,
@@ -235,15 +235,15 @@
         y = y0 / (1 - y0)
 
         max_depth = 2
         min_samples_leaf = 20
         eps = [0.1, 0.1]
         kappa = [20, 100]
 
-        gbm = CycGBM(
+        gbm = CyclicalGradientBooster(
             kappa=kappa,
             eps=eps,
             max_depth=max_depth,
             min_samples_leaf=min_samples_leaf,
             distribution="beta_prime",
         )
         gbm.fit(X, y)
@@ -275,15 +275,15 @@
         l = np.exp(-1 + 0.1 * X0 - 0.002 * X1**2)
 
         X = np.stack([X0, X1]).T
         y = rng.wald(mu, l)
 
         kappa = 100
         eps = 0.001
-        gbm = CycGBM(distribution="inv_gauss", kappa=kappa)
+        gbm = CyclicalGradientBooster(distribution="inv_gauss", kappa=kappa)
         gbm.fit(X, y)
         z_hat = gbm.predict(X)
         loss = gbm.dist.loss(y=y, z=z_hat).sum()
 
         self.assertAlmostEqual(
             first=expected_loss,
             second=loss,
@@ -307,15 +307,15 @@
         z1 = -2 + 0.3 * (X[:, 1] > 0) + 0.2 * np.abs(X[:, 1]) * (X[:, 0] > 0)
         z = np.stack([z0, z1])
         distribution = initiate_distribution(distribution="neg_bin")
         y = distribution.simulate(z=z, random_state=5)
 
         kappa = 100
         eps = 0.01
-        gbm = CycGBM(distribution="neg_bin", kappa=kappa)
+        gbm = CyclicalGradientBooster(distribution="neg_bin", kappa=kappa)
         gbm.fit(X, y)
         z_hat = gbm.predict(X)
         loss = gbm.dist.loss(y=y, z=z_hat).sum()
 
         # The tolerance is set to 1 decimal place because the negative binomial
         # loss is not convex in two dimensions
         self.assertAlmostEqual(
@@ -348,15 +348,15 @@
         z2 = 0.2 * X[:, 3] + 0.03 * X[:, 2] ** 2
         z = np.stack([z0, z1, z2])
         distribution = initiate_distribution(distribution="multivariate_normal")
         y = distribution.simulate(z=z, random_state=5)
 
         kappa = [23, 17, 79]
         eps = [0.5, 0.25, 0.1]
-        gbm = CycGBM(distribution="multivariate_normal", kappa=kappa, eps=eps)
+        gbm = CyclicalGradientBooster(distribution="multivariate_normal", kappa=kappa, eps=eps)
         gbm.fit(X, y)
         z_hat = gbm.predict(X)
         loss = gbm.dist.loss(y=y, z=z_hat).sum()
 
         self.assertAlmostEqual(
             first=expected_loss,
             second=loss,
@@ -375,15 +375,15 @@
         z = np.stack([z0, z1])
         distribution = initiate_distribution(distribution="normal")
         y = distribution.simulate(z=z, random_state=5)
 
         kappa = 100
         eps = 0.1
         max_depth = 2
-        gbm = CycGBM(distribution="normal", kappa=kappa, eps=eps, max_depth=max_depth)
+        gbm = CyclicalGradientBooster(distribution="normal", kappa=kappa, eps=eps, max_depth=max_depth)
         gbm.fit(X, y)
 
         feature_importances = {j: gbm.feature_importances(j=j) for j in [0, 1, "all"]}
         expected_feature_importances = {
             0: [0, 0.27203, 0.72798, 0, 0],
             1: [0, 0.94076, 0.05484, 0.00224, 0.00217],
             "all": [0, 0.64087, 0.3567, 0.00123, 0.0012],
@@ -393,49 +393,14 @@
                 self.assertAlmostEqual(
                     first=expected_feature_importances[j][feature],
                     second=feature_importances[j][feature],
                     places=5,
                     msg=f"CycGBM feature importance not as expected for feature {feature}, parameter {j}",
                 )
 
-    def test_cyc_glm(self):
-        """
-        Test method for the `CycGLM` class on a dataset where the target variable
-        follows a normal distribution.
-        :raises AssertionError: If the estimated parameters do not match the true ones
-        """
-        rng = np.random.default_rng(seed=11)
-        n = 10000
-        p = 3
-        X = rng.normal(0, 1, (n, p))
-        beta_0 = np.array([0, 1, 2]) / 10
-        beta_1 = np.array([0, 2, 1]) / 10
-
-        z0 = beta_0 @ X.T
-        z1 = beta_1 @ X.T
-        z = np.stack([z0, z1])
-        distribution = initiate_distribution(distribution="normal")
-        y = distribution.simulate(z=z, random_state=5)
-
-        max_iter = 10000
-        eps = 1e-7
-        tol = 1e-6
-        cyc_glm = CycGLM(distribution="normal", max_iter=max_iter, eps=eps, tol=tol)
-        cyc_glm.fit(X, y)
-        beta_hat = cyc_glm.beta
-
-        for j in range(2):
-            for k in range(p):
-                self.assertAlmostEqual(
-                    first=beta_hat[j, k],
-                    second=beta_0[k] if j == 0 else beta_1[k],
-                    places=1,
-                    msg=f"CycGLM parameter estimate not as expected for parameter dimension {j}, covariate parameter {k}",
-                )
-
     def test_gamma_with_weights(self):
         """
         Test method for the `CycGBM` class on a dataset where the target variable
         follows a gamma distribution with weights.
         :raises AssertionError: If the calculated loss does not match the expected loss
             to within a tolerance.
         """
@@ -453,15 +418,15 @@
         X = np.stack([X0, X1]).T
         z = np.stack([z0, z1])
         distribution = initiate_distribution(distribution="gamma")
         y = distribution.simulate(z=z, w=w, random_state=5)
 
         kappas = [15, 30]
         eps = 0.1
-        gbm = CycGBM(kappa=kappas, eps=eps, distribution="gamma")
+        gbm = CyclicalGradientBooster(kappa=kappas, eps=eps, distribution="gamma")
         gbm.fit(X, y)
         z_hat = gbm.predict(X)
 
         loss = gbm.dist.loss(y=y, z=z_hat).sum()
 
         self.assertAlmostEqual(
             first=expected_loss,
@@ -491,15 +456,15 @@
         X = np.stack([X0, X1]).T
         z = np.stack([z0, z1])
         distribution = initiate_distribution(distribution="normal")
         y = distribution.simulate(z=z, w=w, random_state=5)
 
         kappas = [15, 30]
         eps = 0.1
-        gbm = CycGBM(kappa=kappas, eps=eps, distribution="normal")
+        gbm = CyclicalGradientBooster(kappa=kappas, eps=eps, distribution="normal")
         gbm.fit(X, y)
         z_hat = gbm.predict(X)
 
         loss = gbm.dist.loss(y=y, z=z_hat).sum()
 
         self.assertAlmostEqual(
             first=expected_loss,
```

