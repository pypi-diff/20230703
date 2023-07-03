# Comparing `tmp/straw_machine-0.0.2.tar.gz` & `tmp/straw_machine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "straw_machine-0.0.2.tar", last modified: Mon Feb 20 07:39:04 2023, max compression
+gzip compressed data, was "straw_machine-0.0.3.tar", last modified: Mon Jul  3 02:30:57 2023, max compression
```

## Comparing `straw_machine-0.0.2.tar` & `straw_machine-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:39:04.989709 straw_machine-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-20 07:38:45.000000 straw_machine-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-20 07:38:45.000000 straw_machine-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-20 07:39:04.989709 straw_machine-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-02-20 07:38:45.000000 straw_machine-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 07:38:45.000000 straw_machine-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 07:39:04.989709 straw_machine-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-20 07:38:45.000000 straw_machine-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:39:04.989709 straw_machine-0.0.2/straw_machine/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-20 07:38:45.000000 straw_machine-0.0.2/straw_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:39:04.989709 straw_machine-0.0.2/straw_machine/dataclass/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-20 07:38:45.000000 straw_machine-0.0.2/straw_machine/dataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-20 07:38:45.000000 straw_machine-0.0.2/straw_machine/dataclass/_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-02-20 07:38:45.000000 straw_machine-0.0.2/straw_machine/dataclass/_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:39:04.989709 straw_machine-0.0.2/straw_machine/util/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-20 07:38:45.000000 straw_machine-0.0.2/straw_machine/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-20 07:38:45.000000 straw_machine-0.0.2/straw_machine/util/_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:39:04.989709 straw_machine-0.0.2/straw_machine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-20 07:39:04.000000 straw_machine-0.0.2/straw_machine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-20 07:39:04.000000 straw_machine-0.0.2/straw_machine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 07:39:04.000000 straw_machine-0.0.2/straw_machine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-20 07:39:04.000000 straw_machine-0.0.2/straw_machine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 07:39:04.000000 straw_machine-0.0.2/straw_machine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:30:57.835942 straw_machine-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 02:30:42.000000 straw_machine-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-03 02:30:42.000000 straw_machine-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-03 02:30:57.835942 straw_machine-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-03 02:30:42.000000 straw_machine-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:30:42.000000 straw_machine-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:30:57.835942 straw_machine-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-03 02:30:42.000000 straw_machine-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:30:57.831941 straw_machine-0.0.3/straw_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:30:57.831941 straw_machine-0.0.3/straw_machine/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/dataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/dataclass/_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/dataclass/_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:30:57.831941 straw_machine-0.0.3/straw_machine/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/gallery/date.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:30:57.835942 straw_machine-0.0.3/straw_machine/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 02:30:42.000000 straw_machine-0.0.3/straw_machine/util/_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:30:57.831941 straw_machine-0.0.3/straw_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-03 02:30:57.000000 straw_machine-0.0.3/straw_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-03 02:30:57.000000 straw_machine-0.0.3/straw_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:30:57.000000 straw_machine-0.0.3/straw_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 02:30:57.000000 straw_machine-0.0.3/straw_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 02:30:57.000000 straw_machine-0.0.3/straw_machine.egg-info/top_level.txt
```

### Comparing `straw_machine-0.0.2/LICENSE` & `straw_machine-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `straw_machine-0.0.2/PKG-INFO` & `straw_machine-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straw_machine
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python making machine of sklearn pipeline
 Home-page: https://github.com/blizhan/straw-machine
 Author: blizhan
 Author-email: blizhan@icloud.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 ![](./static/straw_machine.jpg)
 
 
 ### Install
 
 ```shell
-pip install straw_machine==0.0.1
+pip install straw_machine==0.0.2
 ```
 
 ### [Usage](example/example.ipynb)
 ```python
 from straw_machine.util import (
     generate_estimator, 
     generate_transformer,
```

### Comparing `straw_machine-0.0.2/README.md` & `straw_machine-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ![](./static/straw_machine.jpg)
 
 
 ### Install
 
 ```shell
-pip install straw_machine==0.0.1
+pip install straw_machine==0.0.2
 ```
 
 ### [Usage](example/example.ipynb)
 ```python
 from straw_machine.util import (
     generate_estimator, 
     generate_transformer,
```

### Comparing `straw_machine-0.0.2/setup.py` & `straw_machine-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `straw_machine-0.0.2/straw_machine/dataclass/_estimator.py` & `straw_machine-0.0.3/straw_machine/dataclass/_estimator.py`

 * *Files identical despite different names*

### Comparing `straw_machine-0.0.2/straw_machine/dataclass/_transformer.py` & `straw_machine-0.0.3/straw_machine/dataclass/_transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import List
 import os
 
 @dataclass
 class step:
     name: str
     estimators: List[estimator]
+    remain_other: bool
 
 class pipeline(Pipeline):
     def __init__(self, steps, *, memory=None, verbose=False):
         super().__init__(steps, memory=memory, verbose=verbose)
 
     def __add__(self, pl) -> Pipeline:
         steps = self.steps.copy()
@@ -31,21 +32,27 @@
             os.makedirs(dir, exist_ok=True)
         with open(savepath, 'wb') as f:
             cloudpickle.dump(self, f, **kwargs)
 
 
 class transformer(ColumnTransformer):
     def __init__(self, transform_step:step, **kwargs):
+        """transformer 
+
+        Args:
+            transform_step (step): single transform step that contains multi estimators
+            remain_other (bool, optional): remain other columns or not. Defaults to True.
+        """
         self.name = transform_step.name
-        self.transform_step = step
+        self.transform_step = transform_step
         self.cols_tranform_list = [(e.name, e, e.inputs) for e in transform_step.estimators]
 
         super().__init__(
             transformers=self.cols_tranform_list,
-            remainder='passthrough',
+            remainder= 'passthrough' if transform_step.remain_other else 'drop',
             verbose_feature_names_out=False,
             # **kwargs
         )
         super().set_output(transform='pandas')
 
     def save(self, savepath, **kwargs):
         dir = os.path.dirname(savepath)
```

### Comparing `straw_machine-0.0.2/straw_machine/util/_generate.py` & `straw_machine-0.0.3/straw_machine/util/_generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,20 +21,22 @@
     )
     e = estimator(oper)
     return e
 
 def generate_transformer(
     name:str,
     estimators: List[estimator],
+    remain_other: bool=True,
     **kwargs,
 ) -> transformer:
 
     s = step(
         name=name,
-        estimators=estimators
+        estimators=estimators,
+        remain_other=remain_other,
     )
     return transformer(s, **kwargs)
 
 
 def generate_pipeline(
     transformers: List[transformer],
     **kwargs
```

### Comparing `straw_machine-0.0.2/straw_machine.egg-info/PKG-INFO` & `straw_machine-0.0.3/straw_machine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straw-machine
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python making machine of sklearn pipeline
 Home-page: https://github.com/blizhan/straw-machine
 Author: blizhan
 Author-email: blizhan@icloud.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 ![](./static/straw_machine.jpg)
 
 
 ### Install
 
 ```shell
-pip install straw_machine==0.0.1
+pip install straw_machine==0.0.2
 ```
 
 ### [Usage](example/example.ipynb)
 ```python
 from straw_machine.util import (
     generate_estimator, 
     generate_transformer,
```

