# Comparing `tmp/blackboxopt-5.0.0.tar.gz` & `tmp/blackboxopt-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxopt-5.0.0.tar", max compression
+gzip compressed data, was "blackboxopt-5.0.1.tar", max compression
```

## Comparing `blackboxopt-5.0.0.tar` & `blackboxopt-5.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11476 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/LICENSE
--rw-r--r--   0        0        0     4411 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/README.md
--rw-r--r--   0        0        0      410 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/__init__.py
--rw-r--r--   0        0        0     8378 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/base.py
--rw-r--r--   0        0        0     7044 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/evaluation.py
--rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/examples/__init__.py
--rw-r--r--   0        0        0     1408 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/examples/dask_distributed.py
--rw-r--r--   0        0        0     3246 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/examples/multi_objective_multi_param.py
--rw-r--r--   0        0        0     3094 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/io.py
--rw-r--r--   0        0        0      148 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/logger.py
--rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/__init__.py
--rw-r--r--   0        0        0     6094 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/dask_distributed.py
--rw-r--r--   0        0        0     4873 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/sequential.py
--rw-r--r--   0        0        0     2370 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/testing.py
--rw-r--r--   0        0        0     3677 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimization_loops/utils.py
--rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/__init__.py
--rw-r--r--   0        0        0     5209 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/bohb.py
--rw-r--r--   0        0        0    19054 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/botorch_base.py
--rw-r--r--   0        0        0     6286 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/botorch_utils.py
--rw-r--r--   0        0        0     3151 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/hyperband.py
--rw-r--r--   0        0        0     1822 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/random_search.py
--rw-r--r--   0        0        0     1488 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/space_filling.py
--rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/__init__.py
--rw-r--r--   0        0        0    18613 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/bohb.py
--rw-r--r--   0        0        0     1276 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/configuration_sampler.py
--rw-r--r--   0        0        0     2284 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/hyperband.py
--rw-r--r--   0        0        0     6471 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/iteration.py
--rw-r--r--   0        0        0     4572 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/optimizer.py
--rw-r--r--   0        0        0     2636 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/staged/utils.py
--rw-r--r--   0        0        0    16051 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/optimizers/testing.py
--rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/py.typed
--rw-r--r--   0        0        0     4336 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/utils.py
--rw-r--r--   0        0        0        0 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/__init__.py
--rw-r--r--   0        0        0     1869 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/to_html_patch.js
--rw-r--r--   0        0        0     7106 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/utils.py
--rw-r--r--   0        0        0    24900 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/blackboxopt/visualizations/visualizer.py
--rw-r--r--   0        0        0     3274 2023-06-06 07:37:26.000000 blackboxopt-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     6506 1970-01-01 00:00:00.000000 blackboxopt-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11476 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/LICENSE
+-rw-r--r--   0        0        0     4411 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/README.md
+-rw-r--r--   0        0        0      410 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/__init__.py
+-rw-r--r--   0        0        0     8378 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/base.py
+-rw-r--r--   0        0        0     7044 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/evaluation.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/examples/__init__.py
+-rw-r--r--   0        0        0     1408 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/examples/dask_distributed.py
+-rw-r--r--   0        0        0     3246 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/examples/multi_objective_multi_param.py
+-rw-r--r--   0        0        0     3094 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/io.py
+-rw-r--r--   0        0        0      148 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/logger.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimization_loops/__init__.py
+-rw-r--r--   0        0        0     6094 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimization_loops/dask_distributed.py
+-rw-r--r--   0        0        0     5399 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimization_loops/sequential.py
+-rw-r--r--   0        0        0     2370 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimization_loops/testing.py
+-rw-r--r--   0        0        0     3677 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimization_loops/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/__init__.py
+-rw-r--r--   0        0        0     5209 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/bohb.py
+-rw-r--r--   0        0        0    19054 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/botorch_base.py
+-rw-r--r--   0        0        0     6286 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/botorch_utils.py
+-rw-r--r--   0        0        0     3151 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/hyperband.py
+-rw-r--r--   0        0        0     1822 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/random_search.py
+-rw-r--r--   0        0        0     1488 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/space_filling.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/staged/__init__.py
+-rw-r--r--   0        0        0    18613 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/staged/bohb.py
+-rw-r--r--   0        0        0     1276 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/staged/configuration_sampler.py
+-rw-r--r--   0        0        0     2284 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/staged/hyperband.py
+-rw-r--r--   0        0        0     6471 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/staged/iteration.py
+-rw-r--r--   0        0        0     4572 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/staged/optimizer.py
+-rw-r--r--   0        0        0     2636 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/staged/utils.py
+-rw-r--r--   0        0        0    15850 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/optimizers/testing.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/py.typed
+-rw-r--r--   0        0        0     4336 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/visualizations/__init__.py
+-rw-r--r--   0        0        0     1869 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/visualizations/to_html_patch.js
+-rw-r--r--   0        0        0     7106 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/visualizations/utils.py
+-rw-r--r--   0        0        0    24710 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/blackboxopt/visualizations/visualizer.py
+-rw-r--r--   0        0        0     3274 2023-07-03 13:21:28.000000 blackboxopt-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6506 1970-01-01 00:00:00.000000 blackboxopt-5.0.1/PKG-INFO
```

### Comparing `blackboxopt-5.0.0/LICENSE` & `blackboxopt-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/README.md` & `blackboxopt-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/base.py` & `blackboxopt-5.0.1/blackboxopt/base.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/evaluation.py` & `blackboxopt-5.0.1/blackboxopt/evaluation.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/examples/dask_distributed.py` & `blackboxopt-5.0.1/blackboxopt/examples/dask_distributed.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/examples/multi_objective_multi_param.py` & `blackboxopt-5.0.1/blackboxopt/examples/multi_objective_multi_param.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/io.py` & `blackboxopt-5.0.1/blackboxopt/io.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimization_loops/dask_distributed.py` & `blackboxopt-5.0.1/blackboxopt/optimization_loops/dask_distributed.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimization_loops/sequential.py` & `blackboxopt-5.0.1/blackboxopt/optimization_loops/sequential.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) 2020 - for information on the respective copyright owner
 # see the NOTICE file and/or the repository https://github.com/boschresearch/blackboxopt
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import json
 import logging
+import pprint
 import time
 from typing import Any, Callable, List, Optional, Union
 
 from blackboxopt import (
     Evaluation,
     EvaluationSpecification,
     OptimizationComplete,
@@ -22,18 +22,19 @@
 )
 
 
 def run_optimization_loop(
     optimizer: Union[SingleObjectiveOptimizer, MultiObjectiveOptimizer],
     evaluation_function: Callable[[EvaluationSpecification], Evaluation],
     timeout_s: float = float("inf"),
-    max_evaluations: int = None,
+    max_evaluations: Optional[int] = None,
     catch_exceptions_from_evaluation_function: bool = False,
+    pre_evaluation_callback: Optional[Callable[[EvaluationSpecification], Any]] = None,
     post_evaluation_callback: Optional[Callable[[Evaluation], Any]] = None,
-    logger: logging.Logger = None,
+    logger: Optional[logging.Logger] = None,
 ) -> List[Evaluation]:
     """Convenience wrapper for an optimization loop that sequentially fetches evaluation
     specifications until a given timeout or maximum number of evaluations is reached.
 
     This already handles signals from the optimizer in case there is no evaluation
     specification available yet.
 
@@ -49,17 +50,20 @@
             optimization step that exceeded the timeout (in seconds). Defaults to inf.
         max_evaluations: If given, the optimization loop will terminate after the given
             number of steps.
         catch_exceptions_from_evaluation_function: Whether to exit on an unhandled
             exception raised by the evaluation function or instead store their stack
             trace in the evaluation's `stacktrace` attribute. Set to True if there are
             spurious errors due to e.g. numerical instability that should not halt the
-            optimization loop.
+            optimization loop. For more details, see the wrapper that is used internally
+            `blackboxopt.optimization_loops.utils.evaluation_function_wrapper`
+        pre_evaluation_callback: Reference to a callable that is invoked before each
+            evaluation and takes a `blackboxopt.EvaluationSpecification` as an argument.
         post_evaluation_callback: Reference to a callable that is invoked after each
-            evaluation and takes a `blackboxopt.Evaluation` as its argument.
+            evaluation and takes a `blackboxopt.Evaluation` as an argument.
         logger: The logger to use for logging progress. Default: `blackboxopt.logger`
 
     Returns:
         List of evaluation specification and result for all evaluations.
     """
     if logger is None:
         logger = default_logger
@@ -78,36 +82,40 @@
     start = time.time()
     num_evaluations = 0
     while time.time() - start < timeout_s and num_evaluations < _max_evaluations:
         num_evaluations += 1
 
         try:
             evaluation_specification = optimizer.generate_evaluation_specification()
+
             logger.info(
-                "The optimizer proposed a specification for evaluation:\n"
-                + f"{json.dumps(evaluation_specification.to_dict(), indent=2)}"
+                "The optimizer proposed the following evaluation specification:\n%s",
+                pprint.pformat(evaluation_specification.to_dict(), compact=True),
             )
+            if pre_evaluation_callback:
+                pre_evaluation_callback(evaluation_specification)
 
             evaluation = evaluation_function_wrapper(
                 evaluation_function=evaluation_function,
                 evaluation_specification=evaluation_specification,
                 logger=logger,
                 objectives=objectives,
                 catch_exceptions_from_evaluation_function=catch_exceptions_from_evaluation_function,
             )
+
             logger.info(
-                "Reporting the result from the evaluation function to the optimizer:\n"
-                + f"{json.dumps(evaluation.to_dict(), indent=2)}"
+                "Reporting the following evaluation result to the optimizer:\n%s",
+                pprint.pformat(evaluation.to_dict(), compact=True),
             )
+            if post_evaluation_callback:
+                post_evaluation_callback(evaluation)
+
             optimizer.report(evaluation)
             evaluations.append(evaluation)
 
-            if post_evaluation_callback is not None:
-                post_evaluation_callback(evaluation)
-
         except OptimizerNotReady:
             logger.info("Optimizer is not ready yet, retrying in two seconds")
             time.sleep(2)
             continue
 
         except OptimizationComplete:
             logger.info("Optimization is complete")
```

### Comparing `blackboxopt-5.0.0/blackboxopt/optimization_loops/testing.py` & `blackboxopt-5.0.1/blackboxopt/optimization_loops/testing.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimization_loops/utils.py` & `blackboxopt-5.0.1/blackboxopt/optimization_loops/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/bohb.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/bohb.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/botorch_base.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/botorch_base.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/botorch_utils.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/botorch_utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/hyperband.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/hyperband.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/random_search.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/random_search.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/space_filling.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/space_filling.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/staged/bohb.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/staged/bohb.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/staged/configuration_sampler.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/staged/configuration_sampler.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/staged/hyperband.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/staged/hyperband.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/staged/iteration.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/staged/iteration.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/staged/optimizer.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/staged/optimizer.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/staged/utils.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/staged/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/optimizers/testing.py` & `blackboxopt-5.0.1/blackboxopt/optimizers/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,14 @@
 
     Args:
         optimizer_class: Optimizer to test.
         optimizer_kwargs: Expected to contain additional arguments for initializing
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
-
-    Returns:
-        `True` if the test is passed.
     """
     if seed is None:
         seed = 42
 
     n_evaluations = 5
     losses = [0.1, 0.2, 0.3, 0.4, 0.5]
 
@@ -186,17 +183,14 @@
 
     Args:
         optimizer_class: Optimizer to test.
         optimizer_kwargs: Expected to contain additional arguments for initializing
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
-
-    Returns:
-        `True` if the test is passed.
     """
     if seed is None:
         seed = 0
 
     space = ps.ParameterSpace()
     space.add(ps.ContinuousParameter("p1", (0, 1)))
     space.seed(seed)
@@ -274,17 +268,14 @@
 
     Args:
         optimizer_class: Optimizer to test.
         optimizer_kwargs: Expected to contain additional arguments for initializing
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
-
-    Returns:
-        `True` if the test is passed.
     """
     opt = _initialize_optimizer(optimizer_class, optimizer_kwargs, seed=seed)
     evaluations = []
     for i in range(3):
         es = opt.generate_evaluation_specification()
 
         objectives = {"loss": 0.42 * i}
@@ -313,17 +304,14 @@
 
     Args:
         optimizer_class: Optimizer to test.
         optimizer_kwargs: Expected to contain additional arguments for initializing
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
-
-    Returns:
-        `True` if the test is passed.
     """
     opt = _initialize_optimizer(optimizer_class, optimizer_kwargs, seed=seed)
     es_1 = opt.generate_evaluation_specification()
     es_2 = opt.generate_evaluation_specification()
     es_3 = opt.generate_evaluation_specification()
 
     # NOTE: The following is not using pytest.raises because this would add pytest as
@@ -367,17 +355,14 @@
 
     Args:
         optimizer_class: Optimizer to test.
         optimizer_kwargs: Expected to contain additional arguments for initializing
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
-
-    Returns:
-        `True` if the test is passed.
     """
     space = ps.ParameterSpace()
     space.add(ps.ContinuousParameter("my_fixed_param", (-10.0, 200.0)))
     space.add(ps.ContinuousParameter("x", (-2.0, 2.0)))
     space.seed(seed)
 
     fixed_value = 1.0
@@ -403,41 +388,40 @@
 
 def handles_conditional_space(
     optimizer_class: Union[
         Type[SingleObjectiveOptimizer], Type[MultiObjectiveOptimizer]
     ],
     optimizer_kwargs: dict,
     seed: Optional[int] = None,
+    n_max_evaluations: int = 10,
 ):
     """Check if optimizer handles conditional i.e. hierarchical search spaces.
 
     Args:
         optimizer_class: Optimizer to test.
         optimizer_kwargs: Expected to contain additional arguments for initializing
             the optimizer. (`search_space` and `objective(s)` are set automatically
             by the test.)
         seed: (optional) custom seed
-
-    Returns:
-        `True` if the test is passed.
+        n_max_evaluations: Maximum number of evaluation to try
     """
     space = ps.ParameterSpace()
     space.add(ps.CategoricalParameter("optimizer", ("adam", "sgd")))
     space.add(ps.ContinuousParameter("lr", (0.0001, 0.1), transformation="log"))
     space.add(
         ps.ContinuousParameter("momentum", (0.0, 1.0)),
         lambda optimizer: optimizer == "sgd",
     )
     space.seed(seed)
 
     opt = _initialize_optimizer(
         optimizer_class, optimizer_kwargs, space=space, seed=seed
     )
 
-    for _ in range(10):
+    for _ in range(n_max_evaluations):
         es = opt.generate_evaluation_specification()
         objectives = {
             "loss": es.configuration.get("momentum", 1.0) * es.configuration["lr"] ** 2
         }
         if isinstance(opt, MultiObjectiveOptimizer):
             objectives["score"] = -1.0 * es.configuration["lr"] ** 2
         opt.report(
```

### Comparing `blackboxopt-5.0.0/blackboxopt/utils.py` & `blackboxopt-5.0.1/blackboxopt/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/visualizations/to_html_patch.js` & `blackboxopt-5.0.1/blackboxopt/visualizations/to_html_patch.js`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/visualizations/utils.py` & `blackboxopt-5.0.1/blackboxopt/visualizations/utils.py`

 * *Files identical despite different names*

### Comparing `blackboxopt-5.0.0/blackboxopt/visualizations/visualizer.py` & `blackboxopt-5.0.1/blackboxopt/visualizations/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import plotly.io._html
 import scipy.stats as sps
 from pymoo.indicators.hv import HV
-from pymoo.util.nds.efficient_non_dominated_sort import efficient_non_dominated_sort
 
 from blackboxopt import Evaluation, Objective
 from blackboxopt.utils import get_loss_vector
 from blackboxopt.visualizations import utils
 
 QUALITATIVE_COLORS = px.colors.qualitative.G10
 
@@ -206,28 +205,24 @@
 
 
 def compute_hypervolume(
     evaluations: List[Evaluation],
     objectives: Sequence[Objective],
     reference_point: List[float],
 ) -> float:
+    hv = HV(reference_point, nds=True)
     losses = np.array(
         [
             get_loss_vector(
                 known_objectives=objectives, reported_objectives=e.objectives
             )
             for e in evaluations
         ]
     )
-    pareto_front_idx = efficient_non_dominated_sort(losses)[0]
-    pareto_front = losses[pareto_front_idx]
-
-    hv = HV(reference_point)
-
-    return hv(pareto_front)
+    return hv(losses)
 
 
 def hypervolume_over_iterations(
     evaluations_per_optimizer: Dict[str, List[List[Evaluation]]],
     objectives: Sequence[Objective],
     reference_point: List[float],
     percentiles: Optional[Tuple[float, float, float]] = None,
```

### Comparing `blackboxopt-5.0.0/pyproject.toml` & `blackboxopt-5.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackboxopt"
-version = "5.0.0"
+version = "5.0.1"
 description = "A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts."
 readme = "README.md"
 repository = "https://github.com/boschresearch/blackboxopt"
 authors = ["Bosch Center for AI, Robert Bosch GmbH"]
 license = "Apache-2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `blackboxopt-5.0.0/PKG-INFO` & `blackboxopt-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxopt
-Version: 5.0.0
+Version: 5.0.1
 Summary: A common interface for blackbox optimization algorithms along with useful helpers like parallel optimization loops, analysis and visualization scripts.
 Home-page: https://github.com/boschresearch/blackboxopt
 License: Apache-2.0
 Author: Bosch Center for AI, Robert Bosch GmbH
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

