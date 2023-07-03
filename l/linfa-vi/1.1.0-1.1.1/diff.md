# Comparing `tmp/linfa_vi-1.1.0.tar.gz` & `tmp/linfa_vi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.1.0.tar", last modified: Mon Jul  3 16:17:20 2023, max compression
+gzip compressed data, was "linfa_vi-1.1.1.tar", last modified: Mon Jul  3 17:25:48 2023, max compression
```

## Comparing `linfa_vi-1.1.0.tar` & `linfa_vi-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:20.894684 linfa_vi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-03 16:17:20.890684 linfa_vi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:20.890684 linfa_vi-1.1.0/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/plot_res.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:20.890684 linfa_vi-1.1.0/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:17:20.894684 linfa_vi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:25:48.362683 linfa_vi-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 17:25:48.362683 linfa_vi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:25:48.358683 linfa_vi-1.1.1/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:25:48.362683 linfa_vi-1.1.1/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 17:25:48.000000 linfa_vi-1.1.1/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-03 17:25:48.000000 linfa_vi-1.1.1/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:25:48.000000 linfa_vi-1.1.1/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-03 17:25:48.000000 linfa_vi-1.1.1/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 17:25:48.000000 linfa_vi-1.1.1/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:25:48.362683 linfa_vi-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:25:34.000000 linfa_vi-1.1.1/setup.py
```

### Comparing `linfa_vi-1.1.0/LICENSE` & `linfa_vi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.0/PKG-INFO` & `linfa_vi-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -49,14 +49,15 @@
 - Y. Wang, F. Liu and D.E. Schiavazzi, *[Variational Inference with NoFAS: Normalizing Flow with Adaptive Surrogate for Computationally Expensive Models](https://www.sciencedirect.com/science/article/abs/pii/S0021999122005162)*
 - E.R. Cobian, J.D. Hauenstein, F. Liu and D.E. Schiavazzi, *[AdaAnn: Adaptive Annealing Scheduler for Probability Density Approximation](https://www.dl.begellhouse.com/journals/52034eb04b657aea,796f39cb1acf1296,6f85fe1149ff41d9.html?sgstd=1)*
 
 ### Requirements
 
 * PyTorch 1.13.1
 * Numpy 1.22
+* Matplotlib 3.6 (only plot functionalities `linfa.plot_res`)
 
 ### Numerical Benchmarks
 
 LINFA includes five numerical benchmarks:
 
 * Trivial example.
 * High dimensional example (Sobol' function).
@@ -64,16 +65,15 @@
 * Three-element Windkessel model (a.k.a. RCR model).
 * Friedman 1 dataset example.
 
 The implementation of the lumped parameter network models (RC and RCR models) follows closely from the code developed by [the Schiavazzi Lab at the University of Notre Dame](https://github.com/desResLab/supplMatHarrod20).
 
 To run the tests type
 ```sh
-cd tests
-python -m unittest test_linfa.py linfa_test_suite.NAME_example
+python -m unittest linfa.tests.test_linfa.linfa_test_suite.NAME_example
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
@@ -90,16 +90,15 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-cd tests
-python plot_test_res.py -n NAME -i IT
+python linfa.plot_res -n NAME -i IT
 ```
 where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest. 
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
```

### Comparing `linfa_vi-1.1.0/README.md` & `linfa_vi-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 - Y. Wang, F. Liu and D.E. Schiavazzi, *[Variational Inference with NoFAS: Normalizing Flow with Adaptive Surrogate for Computationally Expensive Models](https://www.sciencedirect.com/science/article/abs/pii/S0021999122005162)*
 - E.R. Cobian, J.D. Hauenstein, F. Liu and D.E. Schiavazzi, *[AdaAnn: Adaptive Annealing Scheduler for Probability Density Approximation](https://www.dl.begellhouse.com/journals/52034eb04b657aea,796f39cb1acf1296,6f85fe1149ff41d9.html?sgstd=1)*
 
 ### Requirements
 
 * PyTorch 1.13.1
 * Numpy 1.22
+* Matplotlib 3.6 (only plot functionalities `linfa.plot_res`)
 
 ### Numerical Benchmarks
 
 LINFA includes five numerical benchmarks:
 
 * Trivial example.
 * High dimensional example (Sobol' function).
@@ -42,16 +43,15 @@
 * Three-element Windkessel model (a.k.a. RCR model).
 * Friedman 1 dataset example.
 
 The implementation of the lumped parameter network models (RC and RCR models) follows closely from the code developed by [the Schiavazzi Lab at the University of Notre Dame](https://github.com/desResLab/supplMatHarrod20).
 
 To run the tests type
 ```sh
-cd tests
-python -m unittest test_linfa.py linfa_test_suite.NAME_example
+python -m unittest linfa.tests.test_linfa.linfa_test_suite.NAME_example
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
@@ -68,16 +68,15 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-cd tests
-python plot_test_res.py -n NAME -i IT
+python linfa.plot_res -n NAME -i IT
 ```
 where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest. 
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
```

### Comparing `linfa_vi-1.1.0/linfa/maf.py` & `linfa_vi-1.1.1/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.0/linfa/nofas.py` & `linfa_vi-1.1.1/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.0/linfa/plot_res.py` & `linfa_vi-1.1.1/linfa/plot_res.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.0/linfa/run_experiment.py` & `linfa_vi-1.1.1/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.0/linfa/transform.py` & `linfa_vi-1.1.1/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.0/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.1.1/linfa_vi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -49,14 +49,15 @@
 - Y. Wang, F. Liu and D.E. Schiavazzi, *[Variational Inference with NoFAS: Normalizing Flow with Adaptive Surrogate for Computationally Expensive Models](https://www.sciencedirect.com/science/article/abs/pii/S0021999122005162)*
 - E.R. Cobian, J.D. Hauenstein, F. Liu and D.E. Schiavazzi, *[AdaAnn: Adaptive Annealing Scheduler for Probability Density Approximation](https://www.dl.begellhouse.com/journals/52034eb04b657aea,796f39cb1acf1296,6f85fe1149ff41d9.html?sgstd=1)*
 
 ### Requirements
 
 * PyTorch 1.13.1
 * Numpy 1.22
+* Matplotlib 3.6 (only plot functionalities `linfa.plot_res`)
 
 ### Numerical Benchmarks
 
 LINFA includes five numerical benchmarks:
 
 * Trivial example.
 * High dimensional example (Sobol' function).
@@ -64,16 +65,15 @@
 * Three-element Windkessel model (a.k.a. RCR model).
 * Friedman 1 dataset example.
 
 The implementation of the lumped parameter network models (RC and RCR models) follows closely from the code developed by [the Schiavazzi Lab at the University of Notre Dame](https://github.com/desResLab/supplMatHarrod20).
 
 To run the tests type
 ```sh
-cd tests
-python -m unittest test_linfa.py linfa_test_suite.NAME_example
+python -m unittest linfa.tests.test_linfa.linfa_test_suite.NAME_example
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
@@ -90,16 +90,15 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-cd tests
-python plot_test_res.py -n NAME -i IT
+python linfa.plot_res -n NAME -i IT
 ```
 where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest. 
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
```

### Comparing `linfa_vi-1.1.0/pyproject.toml` & `linfa_vi-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["variational inference", "normalizig flow", "adaptive annealing", "physics-based modeling"]
 dependencies = [
     "torch==1.13.1",
     "numpy==1.19.5",
+    "matplotlib==3.6",
     'tomli; python_version < "3.11"',    
 ]
 requires-python = ">=3.7"
 
 [tool.setuptools]
 packages = ["linfa"]
```

