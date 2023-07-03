# Comparing `tmp/linfa_vi-1.1.2.tar.gz` & `tmp/linfa_vi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.1.2.tar", last modified: Mon Jul  3 17:45:34 2023, max compression
+gzip compressed data, was "linfa_vi-1.1.3.tar", last modified: Mon Jul  3 19:13:43 2023, max compression
```

## Comparing `linfa_vi-1.1.2.tar` & `linfa_vi-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:45:34.094138 linfa_vi-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 17:45:34.094138 linfa_vi-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:45:34.094138 linfa_vi-1.1.2/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/linfa/plot_res.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:45:34.094138 linfa_vi-1.1.2/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 17:45:34.000000 linfa_vi-1.1.2/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-03 17:45:34.000000 linfa_vi-1.1.2/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:45:34.000000 linfa_vi-1.1.2/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-03 17:45:34.000000 linfa_vi-1.1.2/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 17:45:34.000000 linfa_vi-1.1.2/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:45:34.094138 linfa_vi-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:45:19.000000 linfa_vi-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:43.548683 linfa_vi-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 19:13:43.544683 linfa_vi-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:43.544683 linfa_vi-1.1.3/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:43.544683 linfa_vi-1.1.3/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:13:43.548683 linfa_vi-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/setup.py
```

### Comparing `linfa_vi-1.1.2/LICENSE` & `linfa_vi-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.2/PKG-INFO` & `linfa_vi-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.1.2/README.md` & `linfa_vi-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.2/linfa/maf.py` & `linfa_vi-1.1.3/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.2/linfa/nofas.py` & `linfa_vi-1.1.3/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.2/linfa/plot_res.py` & `linfa_vi-1.1.3/linfa/plot_res.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.2/linfa/run_experiment.py` & `linfa_vi-1.1.3/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.2/linfa/transform.py` & `linfa_vi-1.1.3/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.2/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.1.3/linfa_vi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.1.2/pyproject.toml` & `linfa_vi-1.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.1.2"
+version = "1.1.3"
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
-    "matplotlib==3.6",
+    "matplotlib==3.5.3",
     'tomli; python_version < "3.11"',    
 ]
 requires-python = ">=3.7"
 
 [tool.setuptools]
 packages = ["linfa"]
```

