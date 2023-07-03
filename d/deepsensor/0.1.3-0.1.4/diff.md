# Comparing `tmp/deepsensor-0.1.3.tar.gz` & `tmp/deepsensor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsensor-0.1.3.tar", last modified: Tue Jun 13 14:45:52 2023, max compression
+gzip compressed data, was "deepsensor-0.1.4.tar", last modified: Mon Jul  3 12:19:26 2023, max compression
```

## Comparing `deepsensor-0.1.3.tar` & `deepsensor-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-13 14:45:52.329380 deepsensor-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-13 14:45:41.000000 deepsensor-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.325380 deepsensor-0.1.3/deepsensor/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/nps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/train/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-13 14:45:41.000000 deepsensor-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-13 14:45:52.329380 deepsensor-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 14:45:41.000000 deepsensor-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/test_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/test_task_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-03 12:19:26.801427 deepsensor-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-03 12:19:18.000000 deepsensor-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/active_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/active_learning/acquisition_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/active_learning/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24110 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20840 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/convnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/model/nps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/deepsensor/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-03 12:19:18.000000 deepsensor-0.1.4/deepsensor/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.797426 deepsensor-0.1.4/deepsensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 12:19:26.000000 deepsensor-0.1.4/deepsensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 12:19:18.000000 deepsensor-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-03 12:19:26.801427 deepsensor-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 12:19:18.000000 deepsensor-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:26.801427 deepsensor-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_task_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 12:19:18.000000 deepsensor-0.1.4/tests/utils.py
```

### Comparing `deepsensor-0.1.3/PKG-INFO` & `deepsensor-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,78 @@
-Metadata-Version: 2.1
-Name: deepsensor
-Version: 0.1.3
-Summary: A Python package for modelling xarray and pandas data with neural processes.
-Home-page: https://github.com/tom-andersson/deepsensor
-Author: Tom R. Andersson
-Author-email: tomand@bas.ac.uk
-License: MIT
-Platform: unix
-Platform: linux
-Platform: osx
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
+[//]: # (![]&#40;figs/DeepSensorLogo.png&#41;)
+<ul style="text-align: center;">
+<img src="figs/DeepSensorLogo.png" width="700"/>
+</ul>
 
-# DeepSensor: A Python package for modelling environmental data with neural processes
+<ul style="margin-top:0px;">
 
+
+<p style="text-align: center; font-size: 15px">A Python package and open-source project for modelling environmental
+data with neural processes</p>
+
+-----------
+
+[![release](https://img.shields.io/badge/release-v0.1.3-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
-**DeepSensor** is an open source project and Python package
-for modelling xarray and pandas data with neural processes (NPs).
-
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
 Why neural processes?
 -----------
 NPs are a highly flexible class of probabilistic models that can:
 - ingest multiple context sets (i.e. data streams) containing gridded or pointwise observations
 - handle multiple gridded resolutions
 - predict at arbitrary target locations
 - quantify prediction uncertainty
 
 These capabilities make NPs well suited to modelling spatio-temporal data, such as
 satellite observations, climate model output, and in-situ measurements.
 NPs have been used for range of environmental applications, including:
-- spatial interpolation (sensor placement)
 - downscaling (i.e. super-resolution)
 - forecasting
+- infilling missing satellite data
+- sensor placement
 
 Why DeepSensor?
 -----------
 DeepSensor aims to faithfully match the flexibility of NPs with a simple and intuitive
 interface.
 DeepSensor wraps around the powerful [neuralprocessess](https://github.com/wesselb/neuralprocesses)
 package for the core modelling functionality, while allowing users to stay in
 the familiar [xarray](https://xarray.pydata.org) and [pandas](https://pandas.pydata.org) world
 and avoid the murky depths of tensors!
 
-Backend agnosticism
+Deep learning library agnosticism
 -----------
 DeepSensor leverages the [backends](https://github.com/wesselb/lab) package to be compatible with
-either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.tensorflow.org/)
-deep learning libraries.
-Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose your backend!
+either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.tensorflow.org/).
+Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose between them!
 
 Quick start
 ----------
 
 Here we will demonstrate a simple example of training a convolutional conditional neural process
 (ConvCNP) to spatially interpolate ERA5 data.
 First, pip install the package. In this case we will use the TensorFlow backend.
 ```bash
 pip install deepsensor
 pip install tensorflow
 pip install tensorflow-probability
 ```
 
 We can go from imports to predictions with a trained model in <30 lines of code!
+
 ```python
 import deepsensor.tensorflow
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
-from deepsensor.model.models import ConvNP
+from deepsensor.model.convnp import ConvNP
 from deepsensor.train.train import train_epoch
 
 import xarray as xr
 import pandas as pd
 import numpy as np
 
 # Load raw data
@@ -96,19 +90,19 @@
 
 # Generate training tasks with up to 10% of grid cells passed as context and all grid cells
 # passed as targets
 train_tasks = []
 for date in pd.date_range("2013-01-01", "2014-11-30"):
     task = task_loader(date, context_sampling=np.random.uniform(0.0, 0.1), target_sampling="all")
     train_tasks.append(task)
-    
+
 # Train model
 for epoch in range(100):
     train_epoch(model, train_tasks, progress_bar=True)
-    
+
 # Predict on new task with 10% of context data
 test_task = task_loader("2014-12-31", 0.1)
 mean_ds, std_ds = model.predict(test_task, X_t=ds_raw)
 ```
 
 After training, the model can predict directly to `xarray` in your data's original units and coordinate system:
 ```python
@@ -119,18 +113,43 @@
   * time     (time) datetime64[ns] 2014-12-31
   * lat      (lat) float32 75.0 72.5 70.0 67.5 65.0 ... 25.0 22.5 20.0 17.5 15.0
   * lon      (lon) float32 200.0 202.5 205.0 207.5 ... 322.5 325.0 327.5 330.0
 Data variables:
     air      (time, lat, lon) float32 246.7 244.4 245.5 ... 290.2 289.8 289.4
 ```
 
+Extending DeepSensor with new models
+----------
+To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
+and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
+such as `.mean` and `.stddev`.
+```python
+class NewModel(DeepSensorModel):
+    """A very naive model that predicts the mean of the first context set with a fixed stddev"""
+    def __init__(self, data_processor: DataProcessor, task_loader: TaskLoader):
+        super().__init__(data_processor, task_loader)
+        
+    def mean(self, task: Task):
+        """Compute mean at target locations"""
+        return np.mean(task["Y_c"][0])
+    
+    def stddev(self, task: Task):
+        """Compute stddev at target locations"""
+        return 0.1
+    
+    ...
+```
+`NewModel` can then be used in the same way as the built-in `ConvNP` model.
+See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/extending_models.ipynb)
+for more details.
+
 Learn more
 ----------
 - Documentation: TODO
 - Issue tracker: https://github.com/tom-andersson/deepsensor/issues
 - Source code: https://github.com/tom-andersson/deepsensor
 
 **Talks**
 - Environmental Sensor Placement with ConvGNPs: https://youtu.be/v0pmqh09u1Y
 
 **Papers**
-- TODO
+- TODO
```

### Comparing `deepsensor-0.1.3/README.md` & `deepsensor-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,93 @@
-# DeepSensor: A Python package for modelling environmental data with neural processes
+Metadata-Version: 2.1
+Name: deepsensor
+Version: 0.1.4
+Summary: A Python package for modelling xarray and pandas data with neural processes.
+Home-page: https://github.com/tom-andersson/deepsensor
+Author: Tom R. Andersson
+Author-email: tomand@bas.ac.uk
+License: MIT
+Platform: unix
+Platform: linux
+Platform: osx
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+
+[//]: # (![]&#40;figs/DeepSensorLogo.png&#41;)
+<ul style="text-align: center;">
+<img src="figs/DeepSensorLogo.png" width="700"/>
+</ul>
 
+<ul style="margin-top:0px;">
+
+
+<p style="text-align: center; font-size: 15px">A Python package and open-source project for modelling environmental
+data with neural processes</p>
+
+-----------
+
+[![release](https://img.shields.io/badge/release-v0.1.3-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
-**DeepSensor** is an open source project and Python package
-for modelling xarray and pandas data with neural processes (NPs).
-
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
 Why neural processes?
 -----------
 NPs are a highly flexible class of probabilistic models that can:
 - ingest multiple context sets (i.e. data streams) containing gridded or pointwise observations
 - handle multiple gridded resolutions
 - predict at arbitrary target locations
 - quantify prediction uncertainty
 
 These capabilities make NPs well suited to modelling spatio-temporal data, such as
 satellite observations, climate model output, and in-situ measurements.
 NPs have been used for range of environmental applications, including:
-- spatial interpolation (sensor placement)
 - downscaling (i.e. super-resolution)
 - forecasting
+- infilling missing satellite data
+- sensor placement
 
 Why DeepSensor?
 -----------
 DeepSensor aims to faithfully match the flexibility of NPs with a simple and intuitive
 interface.
 DeepSensor wraps around the powerful [neuralprocessess](https://github.com/wesselb/neuralprocesses)
 package for the core modelling functionality, while allowing users to stay in
 the familiar [xarray](https://xarray.pydata.org) and [pandas](https://pandas.pydata.org) world
 and avoid the murky depths of tensors!
 
-Backend agnosticism
+Deep learning library agnosticism
 -----------
 DeepSensor leverages the [backends](https://github.com/wesselb/lab) package to be compatible with
-either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.tensorflow.org/)
-deep learning libraries.
-Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose your backend!
+either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.tensorflow.org/).
+Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose between them!
 
 Quick start
 ----------
 
 Here we will demonstrate a simple example of training a convolutional conditional neural process
 (ConvCNP) to spatially interpolate ERA5 data.
 First, pip install the package. In this case we will use the TensorFlow backend.
 ```bash
 pip install deepsensor
 pip install tensorflow
 pip install tensorflow-probability
 ```
 
 We can go from imports to predictions with a trained model in <30 lines of code!
+
 ```python
 import deepsensor.tensorflow
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
-from deepsensor.model.models import ConvNP
+from deepsensor.model.convnp import ConvNP
 from deepsensor.train.train import train_epoch
 
 import xarray as xr
 import pandas as pd
 import numpy as np
 
 # Load raw data
@@ -81,19 +105,19 @@
 
 # Generate training tasks with up to 10% of grid cells passed as context and all grid cells
 # passed as targets
 train_tasks = []
 for date in pd.date_range("2013-01-01", "2014-11-30"):
     task = task_loader(date, context_sampling=np.random.uniform(0.0, 0.1), target_sampling="all")
     train_tasks.append(task)
-    
+
 # Train model
 for epoch in range(100):
     train_epoch(model, train_tasks, progress_bar=True)
-    
+
 # Predict on new task with 10% of context data
 test_task = task_loader("2014-12-31", 0.1)
 mean_ds, std_ds = model.predict(test_task, X_t=ds_raw)
 ```
 
 After training, the model can predict directly to `xarray` in your data's original units and coordinate system:
 ```python
@@ -104,14 +128,39 @@
   * time     (time) datetime64[ns] 2014-12-31
   * lat      (lat) float32 75.0 72.5 70.0 67.5 65.0 ... 25.0 22.5 20.0 17.5 15.0
   * lon      (lon) float32 200.0 202.5 205.0 207.5 ... 322.5 325.0 327.5 330.0
 Data variables:
     air      (time, lat, lon) float32 246.7 244.4 245.5 ... 290.2 289.8 289.4
 ```
 
+Extending DeepSensor with new models
+----------
+To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
+and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
+such as `.mean` and `.stddev`.
+```python
+class NewModel(DeepSensorModel):
+    """A very naive model that predicts the mean of the first context set with a fixed stddev"""
+    def __init__(self, data_processor: DataProcessor, task_loader: TaskLoader):
+        super().__init__(data_processor, task_loader)
+        
+    def mean(self, task: Task):
+        """Compute mean at target locations"""
+        return np.mean(task["Y_c"][0])
+    
+    def stddev(self, task: Task):
+        """Compute stddev at target locations"""
+        return 0.1
+    
+    ...
+```
+`NewModel` can then be used in the same way as the built-in `ConvNP` model.
+See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/extending_models.ipynb)
+for more details.
+
 Learn more
 ----------
 - Documentation: TODO
 - Issue tracker: https://github.com/tom-andersson/deepsensor/issues
 - Source code: https://github.com/tom-andersson/deepsensor
 
 **Talks**
```

### Comparing `deepsensor-0.1.3/deepsensor/data/loader.py` & `deepsensor-0.1.4/deepsensor/data/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             pd.DataFrame,
             List[Union[xr.DataArray, xr.Dataset, pd.DataFrame]],
         ],
         links: Union[Tuple, List[Tuple[int, int]], None] = None,
         context_delta_t: Union[int, List[int]] = 0,
         target_delta_t: Union[int, List[int]] = 0,
         time_freq: str = "D",
+        xarray_interp_method: str = "linear",
         dtype: object = "float32",
     ) -> None:
         """Initialise a TaskLoader object
 
         :param context: Context data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
             or a list/tuple of these.
         :param target: Target data. Can be a single xr.DataArray, xr.Dataset or pd.DataFrame,
@@ -39,18 +40,20 @@
             integer is the index of the target data. Can be a single tuple in the case of a single
             link. If None, no links are specified. Default: None.
         :param context_delta_t: Time difference between context data and t=0 (task init time).
             Can be a single int (same for all context data) or a list/tuple of ints.
         :param target_delta_t: Time difference between target data and t=0 (task init time).
             Can be a single int (same for all target data) or a list/tuple of ints.
         :param time_freq: Time frequency of the data. Default: 'D' (daily).
+        :param xarray_interp_method: Interpolation method to use when interpolating xr.DataArray
         :param dtype: Data type of the data. Used to cast the data to the specified dtype.
             Default: 'float32'.
         """
         self.time_freq = time_freq
+        self.xarray_interp_method = xarray_interp_method
         self.dtype = dtype
 
         if isinstance(context, (xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series)):
             context = (context,)
         if isinstance(target, (xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series)):
             target = (target,)
         context, target = self.cast_context_and_target_to_dtype(context, target)
@@ -264,15 +267,15 @@
         s += f"\nContext variable IDs: {self.context_var_IDs}"
         s += f"\nTarget variable IDs: {self.target_var_IDs}"
         return s
 
     def sample_da(
         self,
         da: Union[xr.DataArray, xr.Dataset],
-        sampling_strat: Union[str, int, float],
+        sampling_strat: Union[str, int, float, np.ndarray],
         seed: int = None,
     ) -> (np.ndarray, np.ndarray):
         """Sample a DataArray according to a given strategy
 
         :param da: DataArray to sample, assumed to be sliced for the task already
         :param sampling_strat: Sampling strategy, either "all" or an integer for random grid cell sampling
         :param seed: Seed for random sampling
@@ -281,24 +284,40 @@
         da = da.load()  # Converts dask -> numpy if not already loaded
         if isinstance(da, xr.Dataset):
             da = da.to_array()
 
         if isinstance(sampling_strat, float):
             sampling_strat = int(sampling_strat * da.size)
 
-        if isinstance(sampling_strat, int):
+        if isinstance(sampling_strat, (int, np.integer)):
             N = sampling_strat
             rng = np.random.default_rng(seed)
             x1 = rng.choice(da.coords["x1"].values, N, replace=True)
             x2 = rng.choice(da.coords["x2"].values, N, replace=True)
             X_c = np.array([x1, x2])
             Y_c = da.sel(x1=xr.DataArray(x1), x2=xr.DataArray(x2)).data
             if Y_c.ndim == 1:
                 # returned a 1D array, but we need a 2D array of shape (variable, N)
                 Y_c = Y_c.reshape(1, *Y_c.shape)
+
+        elif isinstance(sampling_strat, np.ndarray):
+            X_c = sampling_strat.astype(self.dtype)
+            Y_c = np.array(
+                da.interp(
+                    x1=xr.DataArray(X_c[0]),
+                    x2=xr.DataArray(X_c[1]),
+                    method=self.xarray_interp_method,
+                    kwargs=dict(fill_value=None, bounds_error=False),
+                ),
+                dtype=self.dtype,
+            )
+            if Y_c.ndim == 1:
+                # returned a 1D array, but we need a 2D array of shape (variable, N)
+                Y_c = Y_c.reshape(1, *Y_c.shape)
+
         elif sampling_strat == "all":
             X_c = (
                 da.coords["x1"].values[np.newaxis],
                 da.coords["x2"].values[np.newaxis],
             )
             Y_c = da.data
             if Y_c.ndim == 2:
@@ -323,15 +342,15 @@
         :return: Sampled DataArray
         """
         df = df.dropna(how="any")  # If any obs are NaN, drop them
 
         if isinstance(sampling_strat, float):
             sampling_strat = int(sampling_strat * df.shape[0])
 
-        if isinstance(sampling_strat, int):
+        if isinstance(sampling_strat, (int, np.integer)):
             N = sampling_strat
             rng = np.random.default_rng(seed)
             idx = rng.choice(df.index, N)
             X_c = df.loc[idx].reset_index()[["x1", "x2"]].values.T.astype(self.dtype)
             Y_c = df.loc[idx].values.T
         elif sampling_strat in ["all", "split"]:
             # NOTE if "split", we assume that the context-target split has already been applied to the df
@@ -342,25 +361,31 @@
             raise ValueError(f"Unknown sampling strategy {sampling_strat}")
 
         return X_c, Y_c
 
     def task_generation(
         self,
         date: pd.Timestamp,
-        context_sampling: Union[str, int, float, List[Union[str, int]]] = "all",
-        target_sampling: Union[str, int, float, List[Union[str, int]]] = "all",
+        context_sampling: Union[
+            str, int, float, np.ndarray, List[Union[str, int, float, np.ndarray]]
+        ] = "all",
+        target_sampling: Union[
+            str, int, float, np.ndarray, List[Union[str, int, float, np.ndarray]]
+        ] = "all",
         split_frac: float = 0.5,
         deterministic: bool = False,
     ) -> Task:
         """Generate a task for a given date
 
         There are several sampling strategies available for the context and target data:
         - "all": Sample all observations.
         - int: Sample N observations uniformly at random.
         - float: Sample a fraction of observations uniformly at random.
+        - np.ndarray, shape (2, N): Sample N observations at the given x1, x2 coordinates.
+            Coords are assumed to be unnormalised.
 
         :param date: Date for which to generate the task
         :param context_sampling: Sampling strategy for the context data, either a list of
             sampling strategies for each context set, or a single strategy applied to all context sets
         :param target_sampling: Sampling strategy for the target data, either a list of
             sampling strategies for each target set, or a single strategy applied to all target sets
         :param split_frac: The fraction of observations to use for the context set with the "split"
@@ -382,16 +407,33 @@
             elif isinstance(sampling_strat, (list, tuple)) and len(
                 sampling_strat
             ) != len(set):
                 raise ValueError(
                     f"Length of sampling_strat ({len(sampling_strat)}) must match number of"
                     f"context sets ({len(set)})"
                 )
-            elif isinstance(sampling_strat, (str, int)):
-                sampling_strat = tuple([sampling_strat] * len(set))
+
+            for strat in sampling_strat:
+                if not isinstance(strat, (str, int, np.integer, float, np.ndarray)):
+                    raise ValueError(
+                        f"Unknown sampling strategy {strat} of type {type(strat)}"
+                    )
+                if isinstance(strat, str) and strat not in ["all", "split"]:
+                    raise ValueError(f"Unknown sampling strategy {strat} for type str")
+                if isinstance(strat, float) and not 0 <= strat <= 1:
+                    raise ValueError(
+                        f"If sampling strategy is a float, must be fraction must be in [0, 1], got {strat}"
+                    )
+                if isinstance(strat, int) and strat <= 0:
+                    raise ValueError(f"Sampling N must be positive, got {strat}")
+                if isinstance(strat, np.ndarray) and strat.shape[0] != 2:
+                    raise ValueError(
+                        f"Sampling coordinates must be of shape (2, N), got {strat.shape}"
+                    )
+
             return sampling_strat
 
         def time_slice_variable(var, delta_t):
             """Slice a variable by a given time delta"""
             # TODO: Does this work with instantaneous time?
             delta_t = pd.Timedelta(delta_t, unit=self.time_freq)
             if isinstance(var, (xr.Dataset, xr.DataArray)):
```

### Comparing `deepsensor-0.1.3/deepsensor/data/processor.py` & `deepsensor-0.1.4/deepsensor/data/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import numpy
 import numpy as np
+import xarray
 
 import xarray as xr
 import pandas as pd
 
 import pprint
 
 from copy import deepcopy
@@ -98,23 +100,23 @@
     def _validate_pandas(self, df: Union[pd.DataFrame, pd.Series]):
         coord_names = [
             self.norm_params["coords"][coord]["name"] for coord in ["time", "x1", "x2"]
         ]
 
         if coord_names[0] not in df.index.names:
             # We don't have a time dimension.
-            if list(df.index.names)[-2:] != coord_names[1:]:
+            if list(df.index.names)[:2] != coord_names[1:]:
                 raise ValueError(
-                    f"Indexes need to end with {coord_names} or {coord_names[1:]} but are {df.index.names}."
+                    f"Indexes need to start with {coord_names} or {coord_names[1:]} but are {df.index.names}."
                 )
         else:
             # We have a time dimension.
-            if list(df.index.names)[-3:] != coord_names:
+            if list(df.index.names)[:3] != coord_names:
                 raise ValueError(
-                    f"Indexes need to end with {coord_names} or {coord_names[1:]} but are {df.index.names}."
+                    f"Indexes need to start with {coord_names} or {coord_names[1:]} but are {df.index.names}."
                 )
 
     def __str__(self):
         s = "DataProcessor with normalisation params:\n"
         s += pprint.pformat(self.norm_params)
         return s
 
@@ -191,14 +193,25 @@
                 )
             self.add_to_norm_params(var_ID, **{param1_ID: param1, param2_ID: param2})
         else:
             param1 = self.norm_params[var_ID][param1_ID]
             param2 = self.norm_params[var_ID][param2_ID]
         return param1, param2
 
+    def map_coord_array(self, coord_array: np.ndarray, unnorm: bool = False):
+        """Normalise or unnormalise a coordinate array
+
+        Args:
+            coord_array (np.ndarray): Array of shape (2, N) containing coords
+            unnorm (bool, optional): Whether to unnormalise. Defaults to False.
+        """
+        x1, x2 = self.map_x1_and_x2(coord_array[0], coord_array[1], unnorm=unnorm)
+        new_coords = np.stack([x1, x2], axis=0)
+        return new_coords
+
     def map_x1_and_x2(self, x1: np.ndarray, x2: np.ndarray, unnorm: bool = False):
         """Normalise or unnormalise spatial coords in a array
 
         Args:
             x1 (np.ndarray): Array of shape (N_x1,) containing spatial coords of x1
             unnorm (bool, optional): Whether to unnormalise. Defaults to False.
         """
@@ -210,15 +223,19 @@
             new_coords_x2 = (x2 - x21) / (x22 - x21)
         else:
             new_coords_x1 = x1 * (x12 - x11) + x11
             new_coords_x2 = x2 * (x22 - x21) + x21
 
         return new_coords_x1, new_coords_x2
 
-    def map_coords(self, data, unnorm=False):
+    def map_coords(
+        self,
+        data: Union[xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series],
+        unnorm=False,
+    ):
         """Normalise spatial coords in a pandas or xarray object"""
         if isinstance(data, (pd.DataFrame, pd.Series)):
             # Reset index to get coords as columns
             indexes = list(data.index.names)
             data = data.reset_index()
 
         if not unnorm:
@@ -270,15 +287,15 @@
                 old: new for old, new in zip(old_coord_IDs, new_coord_IDs) if old != new
             }
             data = data.rename(rename)
 
         if isinstance(data, (pd.DataFrame, pd.Series)):
             # Set index back to original
             [indexes.remove(old_coord_ID) for old_coord_ID in old_coord_IDs]
-            indexes.extend(new_coord_IDs)
+            indexes = new_coord_IDs + indexes  # Put dims first
             data = data.set_index(indexes)
         return data
 
     def map(
         self,
         data: Union[xr.DataArray, xr.Dataset, pd.DataFrame, pd.Series],
         method: str = "mean_std",
@@ -365,7 +382,27 @@
             add_offset (bool, optional): Whether to add the offset to the data when unnormalising.
                 Set to False to unnormalise uncertainty values (e.g. std dev). Defaults to True.
         """
         if isinstance(data, list):
             return [self.map(d, method, add_offset, unnorm=True) for d in data]
         else:
             return self.map(data, method, add_offset, unnorm=True)
+
+
+def xarray_to_coord_array_normalised(da: Union[xr.Dataset, xr.DataArray]):
+    x1, x2 = da["x1"].values, da["x2"].values
+    X1, X2 = np.meshgrid(x1, x2, indexing="ij")
+    return np.stack([X1.ravel(), X2.ravel()], axis=0)
+
+
+def mask_coord_array_normalised(coord_arr, mask_da):
+    if mask_da is None:
+        return coord_arr
+    mask_da = mask_da.astype(float)  # Temporarily convert to float for interpolation
+    mask_da = mask_da.interp(
+        {"x1": xr.DataArray(coord_arr[0]), "x2": xr.DataArray(coord_arr[1])},
+        method="nearest",
+        kwargs=dict(fill_value=None, bounds_error=False),
+    ).data.astype(
+        bool
+    )  # Shape `coord_arr.shape[1]`, False if point is outside mask
+    return coord_arr[:, mask_da]
```

### Comparing `deepsensor-0.1.3/deepsensor/model/defaults.py` & `deepsensor-0.1.4/deepsensor/model/defaults.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,23 @@
             max_ppu = 300
         else:
             raise ValueError(f"Unknown context input type: {type(var)}")
 
     return int(max_ppu)
 
 
+def gen_decoder_scale(model_ppu: int) -> float:
+    """Computes informed setting for the decoder SetConv scale
+
+    The decoder scale should be as small as possible given the model's internal discretisation.
+    The value chosen is 1 / model_ppu.
+    """
+    return 1 / model_ppu
+
+
 def gen_encoder_scales(model_ppu: int, task_loader: TaskLoader) -> list:
     """Computes data-informed settings for the encoder SetConv scale for each context set
 
     For off-grid station data, the scale should be as small as possible given the model's
     internal discretisation density (ppu, points per unit). The value chosen is 0.5 / model_ppu.
 
     For gridded data, the scale should be such that the functional representation smoothly
```

### Comparing `deepsensor-0.1.3/deepsensor/model/models.py` & `deepsensor-0.1.4/deepsensor/model/convnp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,360 +1,31 @@
+import copy
+from typing import Union, List
+
+import lab as B
+import numpy as np
+from matrix import Diagonal
+from plum import ModuleType, dispatch
+
 from deepsensor import backend
-from deepsensor.model.defaults import gen_encoder_scales, gen_ppu
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
 from deepsensor.data.task import Task
+from deepsensor.model.defaults import gen_ppu, gen_encoder_scales, gen_decoder_scale
+from deepsensor.model.model import DeepSensorModel
 from deepsensor.model.nps import (
-    convert_task_to_nps_args,
-    run_nps_model,
     construct_neural_process,
+    run_nps_model,
+    convert_task_to_nps_args,
 )
 
-import copy
-
-from typing import List, Union
-
-import time
-from tqdm import tqdm
-
-import numpy as np
-import pandas as pd
-import xarray as xr
-import lab as B
-from matrix import Diagonal
-from plum import dispatch
-
-# For dispatching with TF and PyTorch model types when they have not yet been loaded.
-# See https://beartype.github.io/plum/types.html#moduletype
-from plum import ModuleType
-
 TFModel = ModuleType("tensorflow.keras", "Model")
 TorchModel = ModuleType("torch.nn", "Module")
 
 
-def create_empty_prediction_array(
-    dates,
-    resolution_factor,
-    X_t,
-    coord_names={"x1": "x1", "x2": "x2"},
-    data_vars=["mean", "std"],
-):
-    # Check for any repeated data_vars
-    if len(data_vars) != len(set(data_vars)):
-        raise ValueError(
-            f"Duplicate data_vars found in data_vars: {data_vars}. "
-            "This woudld cause the xarray.Dataset to have fewer variables than expected."
-        )
-
-    x1_lowres = X_t.coords[coord_names["x1"]]
-    x2_lowres = X_t.coords[coord_names["x2"]]
-
-    x1_hires = np.linspace(
-        x1_lowres[0],
-        x1_lowres[-1],
-        int(x1_lowres.size * resolution_factor),
-        dtype="float32",
-    )
-    x2_hires = np.linspace(
-        x2_lowres[0],
-        x2_lowres[-1],
-        int(x2_lowres.size * resolution_factor),
-        dtype="float32",
-    )
-
-    dims = ["time", coord_names["x1"], coord_names["x2"]]
-    coords = {
-        "time": pd.to_datetime(dates),
-        coord_names["x1"]: x1_hires,
-        coord_names["x2"]: x2_hires,
-    }
-
-    pred_ds = xr.Dataset(
-        {data_var: xr.DataArray(dims=dims, coords=coords) for data_var in data_vars}
-    ).astype("float32")
-
-    # Convert time coord to pandas timestamps
-    pred_ds = pred_ds.assign_coords(time=pd.to_datetime(pred_ds.time.values))
-
-    # TODO: Convert init time to forecast time?
-    # pred_ds = pred_ds.assign_coords(
-    #     time=pred_ds['time'] + pd.Timedelta(days=task_loader.target_delta_t[0]))
-
-    return pred_ds
-
-
-class ProbabilisticModel:
-
-    """
-    Base class for probabilistic model used for DeepSensor.
-    Ensures a set of methods required for DeepSensor
-    are implemented by specific model classes that inherit from it.
-    """
-
-    def __init__(self):
-        pass
-
-    def mean(self, dataset, *args, **kwargs):
-        """
-        Computes the model mean prediction over target points based on given context
-        data.
-        """
-        raise NotImplementedError()
-
-    def covariance(self, dataset, *args, **kwargs):
-        """
-        Computes the model covariance matrix over target points based on given context
-        data. Shape (N, N).
-        """
-        raise NotImplementedError()
-
-    def variance(self, dataset, *args, **kwargs):
-        """
-        Model marginal variance over target points given context points.
-        Shape (N,).
-        """
-        raise NotImplementedError()
-
-    def stddev(self, dataset):
-        """
-        Model marginal standard deviation over target points given context points.
-        Shape (N,).
-        """
-        var = self.variance(dataset)
-        return var**0.5
-
-    def entropy(self, dataset, *args, **kwargs):
-        """
-        Computes the model entropy over target points based on given context
-        data.
-        """
-        raise NotImplementedError()
-
-    def logpdf(self, dataset, *args, **kwargs):
-        """
-        Computes the joint model logpdf over target points based on given context
-        data.
-        """
-        raise NotImplementedError()
-
-    def loss(self, dataset, *args, **kwargs):
-        """
-        Computes the model loss over target points based on given context data.
-        """
-        raise NotImplementedError()
-
-    def sample(self, dataset, n_samples=1, *args, **kwargs):
-        """
-        Draws `n_samples` joint samples over target points based on given context
-        data.
-        returned shape is (n_samples, n_target).
-        """
-        raise NotImplementedError()
-
-    def mutual_information(
-        self, dataset, X_new, Y_new, *args, context_set_idx=0, **kwargs
-    ):
-        """
-        WIP: Old code not using new dataset data structure.
-
-        Computes the mutual information over target set T given context set C and
-        the new (proposed) context set N:
-            I(T|C;N) = H(T|C) - H(T|C,N)
-
-        Uses the subclassed `entropy` method.
-        """
-
-        dataset_with_new = concat_obs_to_dataset(dataset, X_new, Y_new, context_set_idx)
-
-        entropy_before = self.entropy(dataset)
-
-        entropy_after = self.entropy(dataset_with_new)
-
-        return entropy_before - entropy_after
-
-
-class DeepSensorModel(ProbabilisticModel):
-
-    """
-    Implements DeepSensor prediction functionality of a ProbabilisticModel.
-    Allows for outputting an xarray object containing on-grid predictions or a pandas
-    object containing off-grid predictions.
-    """
-
-    def __init__(
-        self, data_processor: DataProcessor = None, task_loader: TaskLoader = None
-    ):
-        """Initialise DeepSensorModel
-
-        :param task_loader: TaskLoader object, used to determine target variables for unnormalising
-        :param data_processor: DataProcessor object, used to unnormalise predictions
-        """
-        self.task_loader = task_loader
-        self.data_processor = data_processor
-
-    def predict(
-        self,
-        tasks: Union[List[Task], Task],
-        X_t: Union[xr.Dataset, xr.DataArray, pd.DataFrame, pd.Series, pd.Index],
-        X_t_normalised: bool = False,
-        resolution_factor=1,
-        n_samples=0,
-        unnormalise=True,
-        noiseless_samples=True,
-        seed=0,
-        progress_bar=0,
-        verbose=False,
-    ):
-        """Predict on a regular grid or at off-grid locations.
-
-        TODO:
-        - Test with multiple targets model
-
-        :param tasks: List of tasks containing context data.
-        :param X_t: Target locations to predict at. Can be an xarray object containing
-            on-grid locations or a pandas object containing off-grid locations.
-        :param X_t_normalised: Whether the `X_t` coords are normalised.
-            If False, will normalise the coords before passing to model. Default False.
-        :param resolution_factor: Optional factor to increase the resolution of the
-            target grid by. E.g. 2 will double the target resolution, 0.5 will halve it.
-            Applies to on-grid predictions only. Default 1.
-        :param n_samples: Number of joint samples to draw from the model.
-            If 0, will not draw samples. Default 0.
-        :param unnormalise: Whether to unnormalise the predictions. Only works if
-            `self` has a `data_processor` and `task_loader` attribute. Default True.
-        :param noiseless_samples: Whether to draw noiseless samples from the model. Default True.
-        :param seed: Random seed for deterministic sampling. Default 0.
-        :param progress_bar: Whether to display a progress bar over tasks. Default 0.
-        :param verbose: Whether to print time taken for prediction. Default False.
-
-        Returns:
-            - If X_t is a pandas object, returns pandas objects containing off-grid predictions.
-            - If X_t is an xarray object, returns xarray object containing on-grid predictions.
-            - If n_samples == 0, returns only mean and std predictions.
-            - If n_samples > 0, returns mean, std and samples predictions.
-        """
-        tic = time.time()
-
-        if type(tasks) is Task:
-            tasks = [tasks]
-
-        if n_samples >= 1:
-            B.set_random_seed(seed)
-            np.random.seed(seed)
-
-        dates = [task["time"] for task in tasks]
-
-        # Flatten tuple of tups to single list
-        target_var_IDs = [
-            var_ID for set in self.task_loader.target_var_IDs for var_ID in set
-        ]
-
-        if isinstance(X_t, pd.Index):
-            X_t = pd.DataFrame(index=X_t)
-
-        if not X_t_normalised:
-            X_t = self.data_processor.map_coords(X_t)
-
-        if isinstance(X_t, (xr.DataArray, xr.Dataset)):
-            mode = "on-grid"
-        elif isinstance(X_t, (pd.DataFrame, pd.Series, pd.Index)):
-            mode = "off-grid"
-
-        if mode == "on-grid":
-            mean = create_empty_prediction_array(
-                dates, resolution_factor, X_t, data_vars=target_var_IDs
-            ).to_array(dim="data_var")
-            std = create_empty_prediction_array(
-                dates, resolution_factor, X_t, data_vars=target_var_IDs
-            ).to_array(dim="data_var")
-            if n_samples >= 1:
-                samples = create_empty_prediction_array(
-                    dates, resolution_factor, X_t, data_vars=target_var_IDs
-                ).to_array(dim="data_var")
-                samples = samples.expand_dims(
-                    dim=dict(sample=np.arange(n_samples))
-                ).copy()
-
-            X_t_arr = (mean["x1"].values, mean["x2"].values)
-
-        elif mode == "off-grid":
-            # Repeat target locs for each date to create multiindex
-            idxs = [(date, *idxs) for date in dates for idxs in X_t.index]
-            index = pd.MultiIndex.from_tuples(idxs, names=["time", *X_t.index.names])
-            mean = pd.DataFrame(index=index, columns=target_var_IDs)
-            std = pd.DataFrame(index=index, columns=target_var_IDs)
-            if n_samples >= 1:
-                idxs_samples = [
-                    (sample, date, *idxs)
-                    for sample in range(n_samples)
-                    for date in dates
-                    for idxs in X_t.index
-                ]
-                index_samples = pd.MultiIndex.from_tuples(
-                    idxs_samples, names=["sample", "time", *X_t.index.names]
-                )
-                samples = pd.DataFrame(index=index_samples, columns=target_var_IDs)
-
-            X_t_arr = X_t.reset_index()[["x1", "x2"]].values.T
-
-        for task in tqdm(tasks, position=0, disable=progress_bar < 1, leave=True):
-            # TODO - repeat based on number of targets?
-            task["X_t"] = [X_t_arr]
-
-            # Run model forwards once to generate output distribution
-            dist = self(task, n_samples=n_samples)
-
-            if mode == "on-grid":
-                mean.loc[:, task["time"], :, :] = self.mean(dist)
-                std.loc[:, task["time"], :, :] = self.stddev(dist)
-                if n_samples >= 1:
-                    B.set_random_seed(seed)
-                    np.random.seed(seed)
-                    samples.loc[:, :, task["time"], :, :] = self.sample(
-                        dist, n_samples=n_samples, noiseless=noiseless_samples
-                    )
-            elif mode == "off-grid":
-                # TODO multi-target case
-                mean.loc[task["time"]] = self.mean(dist).T
-                std.loc[task["time"]] = self.stddev(dist).T
-                if n_samples >= 1:
-                    B.set_random_seed(seed)
-                    np.random.seed(seed)
-                    samples_arr = self.sample(
-                        dist, n_samples=n_samples, noiseless=noiseless_samples
-                    )
-                    for sample_i in range(n_samples):
-                        samples.loc[sample_i, task["time"]] = samples_arr[sample_i].T
-
-        if mode == "on-grid":
-            mean = mean.to_dataset(dim="data_var")
-            std = std.to_dataset(dim="data_var")
-            if n_samples >= 1:
-                samples = samples.to_dataset(dim="data_var")
-
-        if (
-            self.task_loader is not None
-            and self.data_processor is not None
-            and unnormalise == True
-        ):
-            mean = self.data_processor.unnormalise(mean)
-            std = self.data_processor.unnormalise(std, add_offset=False)
-            if n_samples >= 1:
-                samples = self.data_processor.unnormalise(samples)
-
-        if verbose:
-            dur = time.time() - tic
-            print(f"Done in {np.floor(dur / 60)}m:{dur % 60:.0f}s.\n")
-
-        if n_samples >= 1:
-            return mean, std, samples
-        else:
-            return mean, std
-
-
 class ConvNP(DeepSensorModel):
 
     """A ConvNP regression probabilistic model.
 
     Wraps around the `neuralprocesses` package to construct a ConvNP model.
     See: https://github.com/wesselb/neuralprocesses/blob/main/neuralprocesses/architectures/convgnp.py
 
@@ -467,16 +138,21 @@
                 print(f"points_per_unit inferred from TaskLoader: {ppu}")
             kwargs["points_per_unit"] = ppu
         if "encoder_scales" not in kwargs:
             encoder_scales = gen_encoder_scales(kwargs["points_per_unit"], task_loader)
             if verbose:
                 print(f"encoder_scales inferred from TaskLoader: {encoder_scales}")
             kwargs["encoder_scales"] = encoder_scales
+        if "decoder_scale" not in kwargs:
+            decoder_scale = gen_decoder_scale(kwargs["points_per_unit"])
+            if verbose:
+                print(f"decoder_scale inferred from TaskLoader: {decoder_scale}")
+            kwargs["decoder_scale"] = decoder_scale
 
-        self.model = construct_neural_process(dim_x=2, *args, **kwargs)
+        self.model = construct_neural_process(*args, dim_x=2, **kwargs)
 
     @dispatch
     def __init__(
         self,
         data_processor: DataProcessor,
         task_loader: TaskLoader,
         neural_process: Union[TFModel, TorchModel],
@@ -492,17 +168,17 @@
 
         def array_modify_fn(arr):
             arr = arr[np.newaxis, ...]  # Add batch dim
 
             arr = arr.astype(np.float32)  # Cast to float32
 
             # Find NaNs and keep size-1 variable dim
-            mask = np.any(np.isnan(arr), axis=1, keepdims=False)
+            mask = np.any(np.isnan(arr), axis=1, keepdims=True)
             if np.any(mask):
-                # Set NaNs to zero - necessary for `neural_process`
+                # Set NaNs to zero - necessary for `neuralprocesses` (can't have NaNs)
                 arr[mask] = 0.0
 
             # Convert to tensor object based on deep learning backend
             arr = backend.convert_to_tensor(arr)
 
             # Convert to `nps.Masked` object if there are NaNs
             if B.any(mask):
@@ -526,62 +202,136 @@
         """Compute ConvNP distribution."""
         task = ConvNP.check_task(task)
         dist = run_nps_model(self.model, task, n_samples, requires_grad)
         return dist
 
     @dispatch
     def mean(self, dist: backend.nps.AbstractMultiOutputDistribution):
-        return B.to_numpy(dist.mean)[0, 0]
+        mean = dist.mean
+        if isinstance(mean, backend.nps.Aggregate):
+            return [B.to_numpy(m)[0, 0] for m in mean]
+        else:
+            return B.to_numpy(mean)[0, 0]
 
     @dispatch
     def mean(self, task: Task):
-        return B.to_numpy(self(task).mean)[0, 0]
+        dist = self(task)
+        return self.mean(dist)
 
     @dispatch
-    def entropy(self, dist: backend.nps.AbstractMultiOutputDistribution):
-        """Model entropy over target points given context points."""
-        return B.to_numpy(dist.entropy())[0, 0]
+    def variance(self, dist: backend.nps.AbstractMultiOutputDistribution):
+        variance = dist.var
+        if isinstance(variance, backend.nps.Aggregate):
+            return [B.to_numpy(v)[0, 0] for v in variance]
+        else:
+            return B.to_numpy(variance)[0, 0]
 
     @dispatch
-    def entropy(self, task: Task):
-        return B.to_numpy(self(task).entropy())[0, 0]
+    def variance(self, task: Task):
+        dist = self(task)
+        return self.variance(dist)
+
+    @dispatch
+    def stddev(self, dist: backend.nps.AbstractMultiOutputDistribution):
+        variance = self.variance(dist)
+        if isinstance(variance, (list, tuple)):
+            return [np.sqrt(v) for v in variance]
+        else:
+            return np.sqrt(variance)
+
+    @dispatch
+    def stddev(self, task: Task):
+        dist = self(task)
+        return self.stddev(dist)
 
     @dispatch
     def covariance(self, dist: backend.nps.AbstractMultiOutputDistribution):
         return B.to_numpy(B.dense(dist.vectorised_normal.var))[0, 0]
 
     @dispatch
     def covariance(self, task: Task):
-        return B.to_numpy(B.dense(self(task).vectorised_normal.var))[0, 0]
+        dist = self(task)
+        return self.covariance(dist)
 
     @dispatch
-    def variance(self, dist: backend.nps.AbstractMultiOutputDistribution):
-        return B.to_numpy(dist.var)[0, 0]
+    def sample(
+        self,
+        dist: backend.nps.AbstractMultiOutputDistribution,
+        n_samples=1,
+        noiseless=True,
+    ):
+        if noiseless:
+            samples = dist.noiseless.sample(n_samples)
+        else:
+            samples = dist.sample(n_samples)
+
+        if isinstance(samples, backend.nps.Aggregate):
+            return [B.to_numpy(s)[:, 0, 0] for s in samples]
+        else:
+            return B.to_numpy(samples)[:, 0, 0]
 
     @dispatch
-    def variance(self, task: Task):
-        return B.to_numpy(self(task).var)[0, 0]
+    def sample(self, task: Task, n_samples=1, noiseless=True):
+        dist = self(task)
+        return self.sample(dist, n_samples, noiseless)
 
     @dispatch
-    def logpdf(self, dist: backend.nps.AbstractMultiOutputDistribution, task: Task):
-        # Need Y_target to be the right shape for model in the event that task is from the
-        # default DataLoader... is this the best way to do this?
-        task = ConvNP.check_task(task)
+    def slice_diag(self, task: Task):
+        """Slice out the ConvCNP part of the ConvNP distribution."""
+        dist = self(task)
+        dist_diag = backend.nps.MultiOutputNormal(
+            dist._mean,
+            B.zeros(dist._var),
+            Diagonal(B.diag(dist._noise + dist._var)),
+            dist.shape,
+        )
+        return dist_diag
 
-        Y_target = B.concat(*task["Y_t"], axis=1)
-        return B.to_numpy(dist.logpdf(Y_target)).mean()
+    @dispatch
+    def slice_diag(self, dist: backend.nps.AbstractMultiOutputDistribution):
+        """Slice out the ConvCNP part of the ConvNP distribution."""
+        dist_diag = backend.nps.MultiOutputNormal(
+            dist._mean,
+            B.zeros(dist._var),
+            Diagonal(B.diag(dist._noise + dist._var)),
+            dist.shape,
+        )
+        return dist_diag
 
     @dispatch
-    def logpdf(self, task: Task):
-        # Need Y_target to be the right shape for model in the event that task is from the
-        # default DataLoader... is this the best way to do this?
-        task = ConvNP.check_task(task)
+    def mean_marginal_entropy(self, dist: backend.nps.AbstractMultiOutputDistribution):
+        """Mean marginal entropy over target points given context points."""
+        dist_diag = self.slice_diag(dist)
+        return B.mean(B.to_numpy(dist_diag.entropy())[0, 0])
+
+    @dispatch
+    def mean_marginal_entropy(self, task: Task):
+        """Mean marginal entropy over target points given context points."""
+        dist_diag = self.slice_diag(task)
+        return B.mean(B.to_numpy(dist_diag.entropy())[0, 0])
+
+    @dispatch
+    def joint_entropy(self, dist: backend.nps.AbstractMultiOutputDistribution):
+        """Model entropy over target points given context points."""
+        return B.to_numpy(dist.entropy())[0, 0]
+
+    @dispatch
+    def joint_entropy(self, task: Task):
+        return B.to_numpy(self(task).entropy())[0, 0]
+
+    @dispatch
+    def logpdf(self, dist: backend.nps.AbstractMultiOutputDistribution, task: Task):
+        # Model outputs joint distribution over all targets: Concat targets along observation dimension
+        Y_t = B.concat(*task["Y_t"], axis=-1)
+        return B.to_numpy(dist.logpdf(Y_t)).mean()
 
-        Y_target = B.concat(*task["Y_t"], axis=1)
-        return B.to_numpy(self(task).logpdf(Y_target)).mean()
+    @dispatch
+    def logpdf(self, task: Task):
+        dist = self(task)
+        return self.logpdf(dist, task)
 
     def loss_fn(self, task: Task, fix_noise=None, num_lv_samples=8, normalise=False):
         """
 
         Parameters
         ----------
         model_config
@@ -608,58 +358,14 @@
             normalise=normalise,
         )
 
         loss = -B.mean(logpdfs)
 
         return loss
 
-    @dispatch
-    def sample(
-        self,
-        dist: backend.nps.AbstractMultiOutputDistribution,
-        n_samples=1,
-        noiseless=True,
-    ):
-        if noiseless:
-            return B.to_numpy(dist.noiseless.sample(n_samples))[:, 0, 0]  # first batch
-        else:
-            return B.to_numpy(dist.sample(n_samples))[:, 0, 0]
-
-    @dispatch
-    def sample(self, task: Task, n_samples=1, noiseless=True):
-        if noiseless:
-            return B.to_numpy(self(task).noiseless.sample(n_samples))[
-                :, 0, 0
-            ]  # first batch
-        else:
-            return B.to_numpy(self(task).sample(n_samples))[:, 0, 0]
-
-    @dispatch
-    def slice_diag(self, task: Task):
-        """Slice out the ConvCNP part of the ConvNP distribution."""
-        dist = self(task)
-        dist_diag = backend.nps.MultiOutputNormal(
-            dist._mean,
-            B.zeros(dist._var),
-            Diagonal(B.diag(dist._noise + dist._var)),
-            dist.shape,
-        )
-        return dist_diag
-
-    @dispatch
-    def slice_diag(self, dist: backend.nps.AbstractMultiOutputDistribution):
-        """Slice out the ConvCNP part of the ConvNP distribution."""
-        dist_diag = backend.nps.MultiOutputNormal(
-            dist._mean,
-            B.zeros(dist._var),
-            Diagonal(B.diag(dist._noise + dist._var)),
-            dist.shape,
-        )
-        return dist_diag
-
     def ar_sample(
         self, task: Task, n_samples=1, X_target_AR=None, ar_subsample_factor=1
     ):
         """AR sampling with optional functionality to only draw AR samples over a subset of the
         target set and then infull the rest of the sample with the model mean conditioned on the
         AR samples."""
         if X_target_AR is not None:
@@ -719,7 +425,91 @@
 
                 full_samples.append(pred)
             full_samples = np.stack(full_samples, axis=0)
 
             return full_samples
         else:
             return noiseless_samples[:, 0]  # Slice out batch dim
+
+
+def concat_tasks(tasks: List[Task], multiple: int = 1) -> Task:
+    """Concatenate a list of tasks into a single task containing multiple batches.
+
+    TODO:
+    - Consider moving to `nps.py` as this leverages `neuralprocesses` functionality.
+    - Raise error if aux_t values passed (not supported I don't think)
+
+    Parameters
+    ----------
+    tasks : list of Task. List of tasks to concatenate into a single task.
+    multiple : int. Contexts are padded to the smallest multiple of this number that is greater
+        than the number of contexts in each task. Defaults to 1 (padded to the largest number of
+        contexts in the tasks). Setting to a larger number will increase the amount of padding
+        but decrease the range of tensor shapes presented to the model, which simplifies
+        the computational graph in graph mode.
+
+    Returns
+    -------
+    merged_task : Task. Task containing multiple batches.
+    """
+    if len(tasks) == 1:
+        return tasks[0]
+
+    # Assert number of target sets equal
+    n_targets = [len(task["Y_t"]) for task in tasks]
+    if not all([n == n_targets[0] for n in n_targets]):
+        raise ValueError(
+            f"All tasks must have the same number of target sets to concatenate: got {n_targets}. "
+        )
+
+    # For each target set, determine number of targets in each task and raise error if not all equal
+    for target_set_i in range(len(tasks[0]["Y_t"])):
+        n_target_obs = [task["Y_t"][target_set_i].shape[-1] for task in tasks]
+        if not all([n == n_target_obs[0] for n in n_target_obs]):
+            raise ValueError(
+                f"All tasks must have the same number of targets to concatenate: got {n_targets}. "
+                "If you want to train using batches containing tasks with differing numbers of targets, "
+                "you can run the model individually over each task and average the losses."
+            )
+
+    contexts = []
+    for i, task in enumerate(tasks):
+        # Ensure converted to tensors with batch dims
+        task = ConvNP.modify_task(task)
+        tasks[i] = task
+
+        # List of tuples of (x_c, y_c)
+        context_i = list(zip(task["X_c"], task["Y_c"]))
+        contexts.append(context_i)
+
+    # List of tuples of merged (x_c, y_c) along batch dim with padding (w/ multiple=1000)
+    merged_context = [
+        backend.nps.merge_contexts(*[ci for ci in c], multiple=multiple)
+        for c in zip(*contexts)
+    ]
+
+    merged_task = copy.deepcopy(tasks[0])
+
+    # Convert list of tuples of (x_c, y_c) to list of x_c and list of y_c
+    merged_task["X_c"] = [c[0] for c in merged_context]
+    merged_task["Y_c"] = [c[1] for c in merged_context]
+
+    # This assumes that all tasks have the same number of targets
+    merged_task["X_t"] = [
+        B.concat(*[t["X_t"][i] for t in tasks], axis=0)
+        for i in range(len(tasks[0]["X_t"]))
+    ]
+    merged_task["Y_t"] = [
+        B.concat(*[t["Y_t"][i] for t in tasks], axis=0)
+        for i in range(len(tasks[0]["Y_t"]))
+    ]
+    # # Multiple target sets, different target locations
+    # xts = [task["X_t"] for task in tasks]
+    # yts = [task["Y_t"] for task in tasks]
+    # merged_task["X_t"] = backend.nps.AggregateInput(*[(xt, i) for i, xt in enumerate(xts)])
+    # merged_task["Y_t"] = backend.nps.Aggregate(*yts)
+
+    merged_task["time"] = [t["time"] for t in tasks]
+
+    merged_task = Task(merged_task)
+
+    return merged_task
```

### Comparing `deepsensor-0.1.3/deepsensor/model/nps.py` & `deepsensor-0.1.4/deepsensor/model/nps.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,33 @@
     context_data = list(zip(task["X_c"], task["Y_c"]))
 
     # context_data = [nps.mask.merge_contexts(ctx, multiple=5000) for ctx in context_data]
     # context_data[0] = nps.mask.merge_contexts(context_data[0], multiple=5000)  # TEMP not converting gridded
 
     # TEMP: assume target sets all on same spatial locations
     #   just use the first entry from the lists of target data
-    xt = task["X_t"][0]
-    yt = B.concat(*task["Y_t"], axis=1)
+    # xt = task["X_t"][0]
+    # yt = B.concat(*task["Y_t"], axis=1)
 
-    # TODO: allow for varying target set locations
-    # xt = backend.nps.AggregateInput(*[(xt, i) for i, xt in enumerate(task['X_t'])])
-    # yt = backend.nps.Aggregate(*[yt for yt in enumerate(task['Y_t'])])
+    if len(task["X_t"]) == 1 and len(task["Y_t"]) == 1:
+        # Single target set
+        xt = task["X_t"][0]
+        yt = task["Y_t"][0]
+    elif len(task["X_t"]) > 1 and len(task["Y_t"]) > 1:
+        # Multiple target sets, different target locations
+        xt = backend.nps.AggregateInput(*[(xt, i) for i, xt in enumerate(task["X_t"])])
+        yt = backend.nps.Aggregate(*[yt for yt in enumerate(task["Y_t"])])
+    elif len(task["X_t"]) == 1 and len(task["Y_t"]) > 1:
+        # Multiple target sets, same target locations
+        xt = task["X_t"][0]
+        yt = B.concat(*task["Y_t"], axis=1)
+    else:
+        raise ValueError(
+            f"Incorrect target locations and target observations (got {len(task['X_t'])} and {len(task['Y_t'])})"
+        )
 
     # Assume one target set, convert to tf.Tensor and AggregateInput for AR
     #   sampling
     # xt = tf.cast(tf.convert_to_tensor(xt), tf.float32)
     # xt = nps.aggregate.AggregateInput(
     #     (xt, 0),
     # )
```

### Comparing `deepsensor-0.1.3/deepsensor/tensorflow/__init__.py` & `deepsensor-0.1.4/deepsensor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.3/deepsensor/torch/__init__.py` & `deepsensor-0.1.4/deepsensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.3/deepsensor/train/train.py` & `deepsensor-0.1.4/deepsensor/train/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import deepsensor
 from deepsensor.data.task import Task
-from deepsensor.data.utils import concat_tasks
-from deepsensor.model.models import ConvNP
+from deepsensor.model.convnp import ConvNP, concat_tasks
 
 import numpy as np
 
 import lab as B
 
 from typing import List
 
@@ -15,26 +14,28 @@
         # Run on GPU if available
         import torch
 
         if torch.cuda.is_available():
             # Set default GPU device
             torch.set_default_device("cuda")
             B.set_global_device("cuda:0")
+        else:
+            raise RuntimeError("No GPU available: torch.cuda.is_available() == False")
     elif deepsensor.backend.str == "tf":
         # Run on GPU if available
         import tensorflow as tf
 
         if tf.test.is_gpu_available():
             # Set default GPU device
             tf.config.set_visible_devices(
                 tf.config.list_physical_devices("GPU")[0], "GPU"
             )
             B.set_global_device("GPU:0")
-        # Check GPU visible to tf
-        # print("Num GPUs Available: ", len(tf.config.list_physical_devices('GPU')))
+        else:
+            raise RuntimeError("No GPU available: tf.test.is_gpu_available() == False")
 
     else:
         raise NotImplementedError(f"Backend {deepsensor.backend.str} not implemented")
 
 
 def train_epoch(
     model: ConvNP,
```

### Comparing `deepsensor-0.1.3/deepsensor.egg-info/PKG-INFO` & `deepsensor-0.1.4/deepsensor.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,93 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
-# DeepSensor: A Python package for modelling environmental data with neural processes
+[//]: # (![]&#40;figs/DeepSensorLogo.png&#41;)
+<ul style="text-align: center;">
+<img src="figs/DeepSensorLogo.png" width="700"/>
+</ul>
 
+<ul style="margin-top:0px;">
+
+
+<p style="text-align: center; font-size: 15px">A Python package and open-source project for modelling environmental
+data with neural processes</p>
+
+-----------
+
+[![release](https://img.shields.io/badge/release-v0.1.3-green?logo=github)](https://github.com/tom-andersson/deepsensor/releases)
 ![Tests](https://github.com/tom-andersson/deepsensor/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/tom-andersson/deepsensor/badge.svg?branch=main)](https://coveralls.io/github/tom-andersson/deepsensor?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
-**DeepSensor** is an open source project and Python package
-for modelling xarray and pandas data with neural processes (NPs).
-
 **NOTE**: This package is currently undergoing very active development. If you are interested in using
 DeepSensor, please get in touch first (tomand@bas.ac.uk).
 
 Why neural processes?
 -----------
 NPs are a highly flexible class of probabilistic models that can:
 - ingest multiple context sets (i.e. data streams) containing gridded or pointwise observations
 - handle multiple gridded resolutions
 - predict at arbitrary target locations
 - quantify prediction uncertainty
 
 These capabilities make NPs well suited to modelling spatio-temporal data, such as
 satellite observations, climate model output, and in-situ measurements.
 NPs have been used for range of environmental applications, including:
-- spatial interpolation (sensor placement)
 - downscaling (i.e. super-resolution)
 - forecasting
+- infilling missing satellite data
+- sensor placement
 
 Why DeepSensor?
 -----------
 DeepSensor aims to faithfully match the flexibility of NPs with a simple and intuitive
 interface.
 DeepSensor wraps around the powerful [neuralprocessess](https://github.com/wesselb/neuralprocesses)
 package for the core modelling functionality, while allowing users to stay in
 the familiar [xarray](https://xarray.pydata.org) and [pandas](https://pandas.pydata.org) world
 and avoid the murky depths of tensors!
 
-Backend agnosticism
+Deep learning library agnosticism
 -----------
 DeepSensor leverages the [backends](https://github.com/wesselb/lab) package to be compatible with
-either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.tensorflow.org/)
-deep learning libraries.
-Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose your backend!
+either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.tensorflow.org/).
+Simply `import deepsensor.torch` or `import deepsensor.tensorflow` to choose between them!
 
 Quick start
 ----------
 
 Here we will demonstrate a simple example of training a convolutional conditional neural process
 (ConvCNP) to spatially interpolate ERA5 data.
 First, pip install the package. In this case we will use the TensorFlow backend.
 ```bash
 pip install deepsensor
 pip install tensorflow
 pip install tensorflow-probability
 ```
 
 We can go from imports to predictions with a trained model in <30 lines of code!
+
 ```python
 import deepsensor.tensorflow
 from deepsensor.data.loader import TaskLoader
 from deepsensor.data.processor import DataProcessor
-from deepsensor.model.models import ConvNP
+from deepsensor.model.convnp import ConvNP
 from deepsensor.train.train import train_epoch
 
 import xarray as xr
 import pandas as pd
 import numpy as np
 
 # Load raw data
@@ -96,19 +105,19 @@
 
 # Generate training tasks with up to 10% of grid cells passed as context and all grid cells
 # passed as targets
 train_tasks = []
 for date in pd.date_range("2013-01-01", "2014-11-30"):
     task = task_loader(date, context_sampling=np.random.uniform(0.0, 0.1), target_sampling="all")
     train_tasks.append(task)
-    
+
 # Train model
 for epoch in range(100):
     train_epoch(model, train_tasks, progress_bar=True)
-    
+
 # Predict on new task with 10% of context data
 test_task = task_loader("2014-12-31", 0.1)
 mean_ds, std_ds = model.predict(test_task, X_t=ds_raw)
 ```
 
 After training, the model can predict directly to `xarray` in your data's original units and coordinate system:
 ```python
@@ -119,14 +128,39 @@
   * time     (time) datetime64[ns] 2014-12-31
   * lat      (lat) float32 75.0 72.5 70.0 67.5 65.0 ... 25.0 22.5 20.0 17.5 15.0
   * lon      (lon) float32 200.0 202.5 205.0 207.5 ... 322.5 325.0 327.5 330.0
 Data variables:
     air      (time, lat, lon) float32 246.7 244.4 245.5 ... 290.2 289.8 289.4
 ```
 
+Extending DeepSensor with new models
+----------
+To extend DeepSensor with a new model, simply create a new class that inherits from `deepsensor.model.DeepSensorModel`
+and implement the low-level prediction methods defined in `deepsensor.model.ProbabilisticModel`,
+such as `.mean` and `.stddev`.
+```python
+class NewModel(DeepSensorModel):
+    """A very naive model that predicts the mean of the first context set with a fixed stddev"""
+    def __init__(self, data_processor: DataProcessor, task_loader: TaskLoader):
+        super().__init__(data_processor, task_loader)
+        
+    def mean(self, task: Task):
+        """Compute mean at target locations"""
+        return np.mean(task["Y_c"][0])
+    
+    def stddev(self, task: Task):
+        """Compute stddev at target locations"""
+        return 0.1
+    
+    ...
+```
+`NewModel` can then be used in the same way as the built-in `ConvNP` model.
+See [this Jupyter notebook](https://github.com/tom-andersson/deepsensor/blob/main/notebooks/extending_models.ipynb)
+for more details.
+
 Learn more
 ----------
 - Documentation: TODO
 - Issue tracker: https://github.com/tom-andersson/deepsensor/issues
 - Source code: https://github.com/tom-andersson/deepsensor
 
 **Talks**
```

### Comparing `deepsensor-0.1.3/deepsensor.egg-info/SOURCES.txt` & `deepsensor-0.1.4/deepsensor.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 deepsensor/__init__.py
 deepsensor/config.py
+deepsensor/errors.py
 deepsensor/plot.py
 deepsensor/py.typed
 deepsensor.egg-info/PKG-INFO
 deepsensor.egg-info/SOURCES.txt
 deepsensor.egg-info/dependency_links.txt
 deepsensor.egg-info/not-zip-safe
 deepsensor.egg-info/requires.txt
 deepsensor.egg-info/top_level.txt
+deepsensor/active_learning/__init__.py
+deepsensor/active_learning/acquisition_fns.py
+deepsensor/active_learning/algorithms.py
 deepsensor/data/__init__.py
 deepsensor/data/loader.py
 deepsensor/data/processor.py
 deepsensor/data/task.py
 deepsensor/data/utils.py
 deepsensor/model/__init__.py
+deepsensor/model/convnp.py
 deepsensor/model/defaults.py
-deepsensor/model/models.py
+deepsensor/model/model.py
 deepsensor/model/nps.py
 deepsensor/tensorflow/__init__.py
 deepsensor/torch/__init__.py
 deepsensor/train/__init__.py
 deepsensor/train/train.py
 tests/__init__.py
+tests/test_active_learning.py
 tests/test_data_processor.py
 tests/test_model.py
+tests/test_plotting.py
 tests/test_task_loader.py
+tests/test_training.py
 tests/utils.py
```

### Comparing `deepsensor-0.1.3/setup.cfg` & `deepsensor-0.1.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepsensor
-version = 0.1.3
+version = 0.1.4
 author = Tom R. Andersson
 author_email = tomand@bas.ac.uk
 description = A Python package for modelling xarray and pandas data with neural processes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tom-andersson/deepsensor
 license = MIT
```

### Comparing `deepsensor-0.1.3/tests/test_data_processor.py` & `deepsensor-0.1.4/tests/test_data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,22 +202,22 @@
         )
 
         with self.assertRaises(ValueError):
             dp(df_raw)
 
     def test_extra_indexes_preserved_pandas(self):
         """
-        Other metadata indexes are allowed (only *before* the default dimension indexes of
+        Other metadata indexes are allowed (only *after* the default dimension indexes of
         [time, x1, x2] or just [x1, x2]), and these should be preserved during normalisation.
         """
         coords = dict(
-            station=["A", "B"],
             time=pd.date_range("2020-01-01", "2020-01-31", freq="D"),
             lat=np.linspace(20, 40, 30),
             lon=np.linspace(40, 60, 20),
+            station=["A", "B"],
         )
         df_raw = _gen_data_pandas(coords=coords)
 
         dp = DataProcessor(
             x1_map=(20, 40),
             x2_map=(40, 60),
             time_name="time",
@@ -232,22 +232,22 @@
         self.assertTrue(
             self.assert_allclose_pd(df_unnorm, df_raw),
             f"Original {type(df_raw).__name__} not restored.",
         )
 
     def test_wrong_extra_indexes_pandas(self):
         """
-        Other metadata indexes are allowed but if they are not *before* the default dimension
+        Other metadata indexes are allowed but if they are not *after* the default dimension
         indexes of [time, x1, x2] or just [x1, x2], then an error should be raised.
         """
         coords = dict(
+            station=["A", "B"],
             time=pd.date_range("2020-01-01", "2020-01-31", freq="D"),
             lat=np.linspace(20, 40, 30),
             lon=np.linspace(40, 60, 20),
-            station=["A", "B"],
         )
         df_raw = _gen_data_pandas(coords=coords)
 
         dp = DataProcessor(
             x1_map=(20, 40),
             x2_map=(40, 60),
             time_name="time",
```

### Comparing `deepsensor-0.1.3/tests/test_model.py` & `deepsensor-0.1.4/tests/test_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import lab as B
 
 import deepsensor.tensorflow as deepsensor
 
 from deepsensor.data.processor import DataProcessor
 from deepsensor.data.loader import TaskLoader
-from deepsensor.model.models import ConvNP
+from deepsensor.model.convnp import ConvNP
 
 from tests.utils import gen_random_data_xr, gen_random_data_pandas
 
 
 def _gen_data_xr(coords=None, dims=None, data_vars=None):
     """Gen random normalised data"""
     if coords is None:
@@ -118,70 +118,91 @@
             ):
                 task = tl("2020-01-01", context_sampling, target_sampling)
                 dist = model(task)
 
         return None
 
     @parameterized.expand(range(1, 4))
-    def test_prediction_shapes_lowlevel(self, target_dim):
-        """Test low-level model prediction interface"""
+    def test_prediction_shapes_lowlevel(self, n_target_sets):
+        """Test low-level model prediction interface over a range of number of target sets"""
         tl = TaskLoader(
             context=self.da,
-            target=[self.da] * target_dim,
+            target=[self.da] * n_target_sets,
         )
 
+        context_sampling = 10
+
         model = ConvNP(self.dp, tl, unet_channels=(5, 5, 5), verbose=False)
 
-        context_sampling = 10
-        for expected_shape, target_sampling in (
-            ((10,), 10),
-            (self.da.shape[-2:], "all"),
+        for target_sampling, expected_obs_shape in (
+            (10, (10,)),  # expected shape is (10,) when target_sampling is 10
+            (
+                "all",
+                self.da.shape[-2:],
+            ),  # expected shape is da.shape[-2:] when target_sampling is "all"
         ):
             task = tl("2020-01-01", context_sampling, target_sampling)
 
-            dist = model(task)
-
-            n_targets = np.product(expected_shape)
+            n_targets = np.product(expected_obs_shape)
 
             # Tensors
-            assert_shape(model.mean(dist), (target_dim, *expected_shape))
-            assert_shape(model.mean(task), (target_dim, *expected_shape))
-            assert_shape(model.variance(dist), (target_dim, *expected_shape))
-            assert_shape(model.variance(task), (target_dim, *expected_shape))
-            assert_shape(model.stddev(dist), (target_dim, *expected_shape))
-            assert_shape(model.stddev(task), (target_dim, *expected_shape))
-            assert_shape(
-                model.covariance(dist), (n_targets * target_dim, n_targets * target_dim)
-            )
-            assert_shape(
-                model.covariance(task), (n_targets * target_dim, n_targets * target_dim)
-            )
+            mean = model.mean(task)
+            # TODO avoid repeated code
+            if isinstance(mean, (list, tuple)):
+                for m, dim_y in zip(mean, tl.target_dims):
+                    assert_shape(m, (dim_y, *expected_obs_shape))
+            else:
+                assert_shape(mean, (n_target_sets, *expected_obs_shape))
+
+            variance = model.variance(task)
+            if isinstance(variance, (list, tuple)):
+                for v, dim_y in zip(variance, tl.target_dims):
+                    assert_shape(v, (dim_y, *expected_obs_shape))
+            else:
+                assert_shape(variance, (n_target_sets, *expected_obs_shape))
+
+            stddev = model.stddev(task)
+            if isinstance(stddev, (list, tuple)):
+                for s, dim_y in zip(stddev, tl.target_dims):
+                    assert_shape(s, (dim_y, *expected_obs_shape))
+            else:
+                assert_shape(stddev, (n_target_sets, *expected_obs_shape))
+
             n_samples = 5
+            samples = model.sample(task, n_samples)
+            if isinstance(samples, (list, tuple)):
+                for s, dim_y in zip(samples, tl.target_dims):
+                    assert_shape(s, (n_samples, dim_y, *expected_obs_shape))
+            else:
+                assert_shape(samples, (n_samples, n_target_sets, *expected_obs_shape))
+
+            n_target_dims = np.product(tl.target_dims)
             assert_shape(
-                model.sample(dist, n_samples), (n_samples, target_dim, *expected_shape)
-            )
-            assert_shape(
-                model.sample(task, n_samples), (n_samples, target_dim, *expected_shape)
+                model.covariance(task),
+                (
+                    n_targets * n_target_sets * n_target_dims,
+                    n_targets * n_target_sets * n_target_dims,
+                ),
             )
 
             # Scalars
-            x = model.logpdf(dist, task)
-            assert x.size == 1 and x.shape == ()
             x = model.logpdf(task)
             assert x.size == 1 and x.shape == ()
-            x = model.entropy(dist)
+            x = model.joint_entropy(task)
             assert x.size == 1 and x.shape == ()
-            x = model.entropy(task)
+            x = model.mean_marginal_entropy(task)
             assert x.size == 1 and x.shape == ()
-            x = B.to_numpy(model.loss_fn(task))
+            if n_target_sets == 1:
+                # TEMP loss function for multiple non-overlapping target sets is not yet implemented
+                x = B.to_numpy(model.loss_fn(task))
             assert x.size == 1 and x.shape == ()
 
     @parameterized.expand(range(1, 4))
     def test_prediction_shapes_highlevel(self, target_dim):
-        """Test high-level `.predict` interface"""
+        """Test high-level `.predict` interface over a range of number of target sets"""
 
         if target_dim > 1:
             # Avoid data var name clash in `predict`
             target_names = [f"target_{i}" for i in range(target_dim)]
             target = [self.da] * target_dim
             for i, name in enumerate(target_names):
                 target[i] = copy.deepcopy(target[i])
@@ -231,14 +252,27 @@
         )
         assert [isinstance(df, pd.DataFrame) for df in [mean_df, std_df, samples_df]]
         n_preds = len(dates) * len(X_t)
         assert_shape(mean_df, (n_preds, target_dim))
         assert_shape(std_df, (n_preds, target_dim))
         assert_shape(samples_df, (n_samples * n_preds, target_dim))
 
+    def test_nans_in_context(self):
+        """Test nothing breaks when NaNs present in context"""
+        tl = TaskLoader(context=self.da, target=self.da)
+        task = tl("2020-01-01", context_sampling=10, target_sampling=10)
+
+        # Convert first observation of context to NaN
+        task["Y_c"][0][0] = np.nan
+
+        model = ConvNP(self.dp, tl, unet_channels=(5, 5, 5), verbose=False)
+
+        # Check that nothing breaks
+        model(task)
+
 
 def assert_shape(x, shape: tuple):
     """ex: assert_shape(conv_input_array, [8, 3, None, None])"""
     # TODO put this in a utils module?
     assert len(x.shape) == len(shape), (x.shape, shape)
     for _a, _b in zip(x.shape, shape):
         if isinstance(_b, int):
```

### Comparing `deepsensor-0.1.3/tests/test_task_loader.py` & `deepsensor-0.1.4/tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.3/tests/utils.py` & `deepsensor-0.1.4/tests/utils.py`

 * *Files identical despite different names*

