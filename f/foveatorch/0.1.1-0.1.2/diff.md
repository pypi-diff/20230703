# Comparing `tmp/foveatorch-0.1.1.tar.gz` & `tmp/foveatorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foveatorch-0.1.1.tar", last modified: Fri Jun  9 00:25:25 2023, max compression
+gzip compressed data, was "foveatorch-0.1.2.tar", last modified: Sun Jul  2 23:09:37 2023, max compression
```

## Comparing `foveatorch-0.1.1.tar` & `foveatorch-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 00:25:25.577038 foveatorch-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-09 00:25:16.000000 foveatorch-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-09 00:25:25.577038 foveatorch-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-09 00:25:16.000000 foveatorch-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 00:25:25.573038 foveatorch-0.1.1/foveatorch/
--rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-06-09 00:25:16.000000 foveatorch-0.1.1/foveatorch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8606 2023-06-09 00:25:16.000000 foveatorch-0.1.1/foveatorch/modfoveate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9216 2023-06-09 00:25:16.000000 foveatorch-0.1.1/foveatorch/neopyramid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 00:25:25.577038 foveatorch-0.1.1/foveatorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-09 00:25:25.000000 foveatorch-0.1.1/foveatorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 00:25:25.000000 foveatorch-0.1.1/foveatorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 00:25:25.000000 foveatorch-0.1.1/foveatorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 00:25:25.000000 foveatorch-0.1.1/foveatorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 00:25:25.000000 foveatorch-0.1.1/foveatorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 00:25:25.577038 foveatorch-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2207 2023-06-09 00:25:16.000000 foveatorch-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:09:37.826476 foveatorch-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-02 23:09:23.000000 foveatorch-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-02 23:09:37.826476 foveatorch-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-02 23:09:23.000000 foveatorch-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:09:37.826476 foveatorch-0.1.2/foveatorch/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-02 23:09:23.000000 foveatorch-0.1.2/foveatorch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8494 2023-07-02 23:09:23.000000 foveatorch-0.1.2/foveatorch/modfoveate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9103 2023-07-02 23:09:23.000000 foveatorch-0.1.2/foveatorch/neopyramid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:09:37.826476 foveatorch-0.1.2/foveatorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 23:09:37.000000 foveatorch-0.1.2/foveatorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 23:09:37.826476 foveatorch-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2207 2023-07-02 23:09:23.000000 foveatorch-0.1.2/setup.py
```

### Comparing `foveatorch-0.1.1/LICENSE` & `foveatorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foveatorch-0.1.1/PKG-INFO` & `foveatorch-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foveatorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Differentiable foveated vision for Deep Learning methods
 Home-page: https://github.com/emaballarin/foveatorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: MIT
 Keywords: Deep Learning,Machine Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foveatorch Version: 0.1.1 Summary: Differentiable
+Metadata-Version: 2.1 Name: foveatorch Version: 0.1.2 Summary: Differentiable
 foveated vision for Deep Learning methods Home-page: https://github.com/
 emaballarin/foveatorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: MIT Keywords: Deep Learning,Machine
 Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
```

### Comparing `foveatorch-0.1.1/README.md` & `foveatorch-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `foveatorch-0.1.1/foveatorch/modfoveate.py` & `foveatorch-0.1.2/foveatorch/modfoveate.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from kornia.core.check import KORNIA_CHECK_SHAPE
 from torch import logical_and
 
 from .neopyramid import retina_pyramid
 
 # ------------------------------------------------------------------------------
 
-__all__ = ["foveate_atomic", "_foveate", "foveate"]
+__all__ = ["foveate_atomic", "foveate", "Foveate2D"]
 
 
 def foveate_atomic(
     xinput: Tensor,
     fixation_pts: Tensor | None = None,
     nlayers: int = 6,
     p: float = 7.5,
@@ -74,16 +74,14 @@
     width: int
     nchannels, height, width = xinput.shape
 
     # Select device
     if device is None:
         device = "cuda" if th.cuda.is_available() else "cpu"
     else:
-        if device not in ["cpu", "cuda"]:
-            raise ValueError("device must be either 'cpu' or 'cuda'.")
         if device == "cuda" and not th.cuda.is_available():
             raise RuntimeError("CUDA is not available.")
 
     # Compute default fixation point
     if fixation_pts is None:
         fixation_pts: Tensor = th.tensor([width / 2, height / 2], device=device)
```

### Comparing `foveatorch-0.1.1/foveatorch/neopyramid.py` & `foveatorch-0.1.2/foveatorch/neopyramid.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,16 +253,14 @@
         f"Invalid kernel size, it must be a positive integer. Got: {kernel_size}",
     )
 
     # Select device
     if device is None:
         device = "cuda" if th.cuda.is_available() else "cpu"
     else:
-        if device not in ["cpu", "cuda"]:
-            raise ValueError("device must be either 'cpu' or 'cuda'.")
         if device == "cuda" and not th.cuda.is_available():
             raise RuntimeError("CUDA is not available.")
 
     # Define the kernel
     kernel: Tensor = get_gaussian_kernel2d(
         (kernel_size, kernel_size), (sigma, sigma), dtype=dtype, device=device
     )
```

### Comparing `foveatorch-0.1.1/foveatorch.egg-info/PKG-INFO` & `foveatorch-0.1.2/foveatorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foveatorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Differentiable foveated vision for Deep Learning methods
 Home-page: https://github.com/emaballarin/foveatorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: MIT
 Keywords: Deep Learning,Machine Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foveatorch Version: 0.1.1 Summary: Differentiable
+Metadata-Version: 2.1 Name: foveatorch Version: 0.1.2 Summary: Differentiable
 foveated vision for Deep Learning methods Home-page: https://github.com/
 emaballarin/foveatorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: MIT Keywords: Deep Learning,Machine
 Learning,Computer Vision,Computational Neuroscience,Differentiable Programming
 Classifier: Development Status :: 4 - Beta Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
```

### Comparing `foveatorch-0.1.1/setup.py` & `foveatorch-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 check_dependencies(DEPENDENCY_PACKAGE_NAMES)
 
 PACKAGENAME: str = "foveatorch"
 
 
 setup(
     name=PACKAGENAME,
-    version="0.1.1",
+    version="0.1.2",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/foveatorch",
     description="Differentiable foveated vision for Deep Learning methods",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=[
```

