# Comparing `tmp/tvdcn-0.3.1.tar.gz` & `tmp/tvdcn-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.3.1.tar", last modified: Sun Jul  2 06:53:12 2023, max compression
+gzip compressed data, was "tvdcn-0.3.2.tar", last modified: Sun Jul  2 23:41:12 2023, max compression
```

## Comparing `tvdcn-0.3.1.tar` & `tvdcn-0.3.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.559211 tvdcn-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 06:51:20.000000 tvdcn-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 06:51:20.000000 tvdcn-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-02 06:53:12.559211 tvdcn-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-02 06:51:20.000000 tvdcn-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-02 06:51:20.000000 tvdcn-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 06:51:20.000000 tvdcn-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-02 06:53:12.559211 tvdcn-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-02 06:51:20.000000 tvdcn-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.547211 tvdcn-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.547211 tvdcn-0.3.1/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.551211 tvdcn-0.3.1/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.551211 tvdcn-0.3.1/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27047 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    30172 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    38630 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30412 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27339 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/utils/tensor_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.559211 tvdcn-0.3.1/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.559211 tvdcn-0.3.1/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    33943 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.551211 tvdcn-0.3.1/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.557254 tvdcn-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 23:39:04.000000 tvdcn-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 23:39:04.000000 tvdcn-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-02 23:41:12.557254 tvdcn-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-02 23:39:04.000000 tvdcn-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-02 23:39:04.000000 tvdcn-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 23:39:04.000000 tvdcn-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-02 23:41:12.557254 tvdcn-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-02 23:39:04.000000 tvdcn-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.541253 tvdcn-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.541253 tvdcn-0.3.2/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.545253 tvdcn-0.3.2/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.549254 tvdcn-0.3.2/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.549254 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27298 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.549254 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    23593 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    38849 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30412 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27339 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.553254 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.553254 tvdcn-0.3.2/tvdcn/csrc/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/utils/tensor_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.553254 tvdcn-0.3.2/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.557254 tvdcn-0.3.2/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.545253 tvdcn-0.3.2/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.3.1/LICENSE.txt` & `tvdcn-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/PKG-INFO` & `tvdcn-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.1
+Version: 0.3.2
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -93,15 +93,16 @@
 | Python version:  |                   3.8-3.11                    |    3.8-3.11    |
 | PyTorch version: |                `torch==2.0.1`                 | `torch==2.0.1` |
 | Cuda version:    |                     11.8                      |       -        |
 | GPU CCs:         | `3.7,5.0,6.0,6.1,7.0,7.5,8.0,8.6,8.9,9.0+PTX` |       -        |
 
 #### From Source:
 
-For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`).
+For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`) with C++17 features
+enabled.
 Clone this repo and execute the following command:
 
 ```terminal
 pip install .
 ```
 
 Or just compile the binary for inplace usage:
@@ -138,31 +139,31 @@
 ```python
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Union[int, Tuple[int, ...]] = 1,
-        padding: Union[int, Tuple[int, ...]] = 0,
-        dilation: Union[int, Tuple[int, ...]] = 1,
+        stride: Union[int, Tuple[int, int]] = 1,
+        padding: Union[int, Tuple[int, int]] = 0,
+        dilation: Union[int, Tuple[int, int]] = 1,
         groups: int = 1) -> Tensor:
     ...
 
 
 def deform_conv_transpose2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Union[int, Tuple[int, ...]] = 1,
-        padding: Union[int, Tuple[int, ...]] = 0,
-        output_padding: Union[int, Tuple[int, ...]] = 0,
-        dilation: Union[int, Tuple[int, ...]] = 1,
+        stride: Union[int, Tuple[int, int]] = 1,
+        padding: Union[int, Tuple[int, int]] = 0,
+        output_padding: Union[int, Tuple[int, int]] = 0,
+        dilation: Union[int, Tuple[int, int]] = 1,
         groups: int = 1) -> Tensor:
     ...
 ```
 
 If `offset=None` and `mask=None`, the executed operations are identical to conventional convolution.
 
 #### Neural Network Layers:
```

### Comparing `tvdcn-0.3.1/README.md` & `tvdcn-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 | Python version:  |                   3.8-3.11                    |    3.8-3.11    |
 | PyTorch version: |                `torch==2.0.1`                 | `torch==2.0.1` |
 | Cuda version:    |                     11.8                      |       -        |
 | GPU CCs:         | `3.7,5.0,6.0,6.1,7.0,7.5,8.0,8.6,8.9,9.0+PTX` |       -        |
 
 #### From Source:
 
-For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`).
+For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`) with C++17 features
+enabled.
 Clone this repo and execute the following command:
 
 ```terminal
 pip install .
 ```
 
 Or just compile the binary for inplace usage:
@@ -106,31 +107,31 @@
 ```python
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Union[int, Tuple[int, ...]] = 1,
-        padding: Union[int, Tuple[int, ...]] = 0,
-        dilation: Union[int, Tuple[int, ...]] = 1,
+        stride: Union[int, Tuple[int, int]] = 1,
+        padding: Union[int, Tuple[int, int]] = 0,
+        dilation: Union[int, Tuple[int, int]] = 1,
         groups: int = 1) -> Tensor:
     ...
 
 
 def deform_conv_transpose2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Union[int, Tuple[int, ...]] = 1,
-        padding: Union[int, Tuple[int, ...]] = 0,
-        output_padding: Union[int, Tuple[int, ...]] = 0,
-        dilation: Union[int, Tuple[int, ...]] = 1,
+        stride: Union[int, Tuple[int, int]] = 1,
+        padding: Union[int, Tuple[int, int]] = 0,
+        output_padding: Union[int, Tuple[int, int]] = 0,
+        dilation: Union[int, Tuple[int, int]] = 1,
         groups: int = 1) -> Tensor:
     ...
 ```
 
 If `offset=None` and `mask=None`, the executed operations are identical to conventional convolution.
 
 #### Neural Network Layers:
```

### Comparing `tvdcn-0.3.1/pyproject.toml` & `tvdcn-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/setup.cfg` & `tvdcn-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/setup.py` & `tvdcn-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
     source_cuda = glob.glob(os.path.join(extensions_dir, 'ops', 'cuda', '*.cu'))
     source_cuda += glob.glob(os.path.join(extensions_dir, 'ops', 'autocast', '*.cpp'))
 
     sources = main_file + source_cpu
     extension = CppExtension
     extra_compile_args = {'cxx': []}
+    extra_compile_args['cxx'].append('/std:c++17' if sys.platform == 'win32' else '-std=c++17')
     define_macros = []
 
     print('Compiling extensions with following flags:')
     force_cuda = os.getenv('FORCE_CUDA', '0') == '1'
     print(f'  FORCE_CUDA: {force_cuda}')
     debug_mode = os.getenv('DEBUG', '0') == '1'
     print(f'  DEBUG: {debug_mode}')
@@ -58,14 +59,15 @@
         extension = CUDAExtension
         sources += source_cuda
         define_macros += [('WITH_CUDA', None)]
         if nvcc_flags == '':
             nvcc_flags = []
         else:
             nvcc_flags = nvcc_flags.split(' ')
+        nvcc_flags.append('-std=c++17')
         extra_compile_args['nvcc'] = nvcc_flags
 
     if sys.platform == 'win32':
         define_macros += [(f'{PACKAGE_ROOT}_EXPORTS', None)]
         define_macros += [('USE_PYTHON', None)]
         extra_compile_args['cxx'].append('/MP')
```

### Comparing `tvdcn-0.3.1/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.3.2/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tests/test_grad.py` & `tvdcn-0.3.2/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,26 @@
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 for (index_t i = 0; i < weight_w; ++i) {
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, width,
-                                    x + offset[b][offset_group_idx][i][0][w])
-                                       : sample(input, b, c, width, x);
-
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                    scalar_t val, mask_val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, width,
+                                x + offset[b][offset_group_idx][i][0][w]);
+                    else
+                        val = sample(input, b, c, width, x);
+
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     columns[c][i][b][w] = val * mask_val;
                 }
             }
         }
 
         void arr2col_cpu(
@@ -208,20 +211,23 @@
                 const index_t b = (index / (weight_w * out_w * in_channels));
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                const scalar_t mask_val =
-                        modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                scalar_t mask_val;
+                if constexpr (modulated)
+                    mask_val = mask[b][mask_group_idx][i][w];
+                else
+                    mask_val = static_cast<scalar_t>(1);
 
-                const scalar_t val = columns[c][i][b][w] * mask_val;
+                scalar_t val = columns[c][i][b][w] * mask_val;
 
-                if (deformable)
+                if constexpr (deformable)
                     interpolate_insert(
                             grad_input, b, c, width,
                             x + offset[b][offset_group_idx][i][0][w],
                             val);
                 else
                     insert(grad_input, b, c, width, x, val);
             }
@@ -302,20 +308,23 @@
                 const index_t c_start = g * c_per_offset_group;
                 const index_t c_end = c_start + c_per_offset_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    const scalar_t weight = coordinate_weight(
+                    scalar_t weight = coordinate_weight(
                             input, b, c, width,
                             x + offset[b][g][i][0][w]);
 
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                    scalar_t mask_val;
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     grad_offset_val += columns[c][i][b][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][0][w] = grad_offset_val;
             }
         }
@@ -397,20 +406,21 @@
                 const index_t c_start = g * c_per_mask_group;
                 const index_t c_end = c_start + c_per_mask_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t offset_group_idx = c / c_per_offset_group;
 
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, width,
-                                    x + offset[b][offset_group_idx][i][0][w])
-                                       : sample(input, b, c, width, x);
+                    scalar_t val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, width,
+                                x + offset[b][offset_group_idx][i][0][w]);
+                    else
+                        val = sample(input, b, c, width, x);
 
                     grad_mask_val += columns[c][i][b][w] * val;
                 }
 
                 grad_mask[b][g][i][w] = grad_mask_val;
             }
         }
```

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -163,24 +163,27 @@
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 for (index_t i = 0; i < weight_h; ++i) {
                     for (index_t j = 0; j < weight_w; ++j) {
                         const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                         const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                        const scalar_t val =
-                                deformable ?
-                                interpolate_sample(
-                                        input, b, c, height, width,
-                                        y + offset[b][offset_group_idx][i][j][0][h][w],
-                                        x + offset[b][offset_group_idx][i][j][1][h][w])
-                                           : sample(input, b, c, height, width, y, x);
-
-                        const scalar_t mask_val =
-                                modulated ? mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                        scalar_t val, mask_val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, height, width,
+                                    y + offset[b][offset_group_idx][i][j][0][h][w],
+                                    x + offset[b][offset_group_idx][i][j][1][h][w]);
+                        else
+                            val = sample(input, b, c, height, width, y, x);
+
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][j][h][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
 
                         columns[c][i][j][b][h][w] = val * mask_val;
                     }
                 }
             }
         }
 
@@ -275,20 +278,23 @@
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                 const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                const scalar_t mask_val =
-                        modulated ? mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                scalar_t mask_val;
+                if constexpr (modulated)
+                    mask_val = mask[b][mask_group_idx][i][j][h][w];
+                else
+                    mask_val = static_cast<scalar_t>(1);
 
-                const scalar_t val = columns[c][i][j][b][h][w] * mask_val;
+                scalar_t val = columns[c][i][j][b][h][w] * mask_val;
 
-                if (deformable)
+                if constexpr (deformable)
                     interpolate_insert(
                             grad_input, b, c, height, width,
                             y + offset[b][offset_group_idx][i][j][0][h][w],
                             x + offset[b][offset_group_idx][i][j][1][h][w],
                             val);
                 else
                     insert(grad_input, b, c, height, width, y, x, val);
@@ -392,22 +398,25 @@
                 const index_t c_end = c_start + c_per_offset_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    const scalar_t weight = coordinate_weight(
+                    scalar_t weight = coordinate_weight(
                             input, b, c, height, width,
                             y + offset[b][g][i][j][0][h][w],
                             x + offset[b][g][i][j][1][h][w],
                             o);
 
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                    scalar_t mask_val;
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][j][h][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
             }
         }
@@ -510,21 +519,22 @@
                 const index_t c_end = c_start + c_per_mask_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t offset_group_idx = c / c_per_offset_group;
 
                     const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, height, width,
-                                    y + offset[b][offset_group_idx][i][j][0][h][w],
-                                    x + offset[b][offset_group_idx][i][j][1][h][w])
-                                       : sample(input, b, c, height, width, y, x);
+                    scalar_t val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, height, width,
+                                y + offset[b][offset_group_idx][i][j][0][h][w],
+                                x + offset[b][offset_group_idx][i][j][1][h][w]);
+                    else
+                        val = sample(input, b, c, height, width, y, x);
 
                     grad_mask_val += columns[c][i][j][b][h][w] * val;
                 }
 
                 grad_mask[b][g][i][j][h][w] = grad_mask_val;
             }
         }
```

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -237,26 +237,28 @@
                 for (index_t i = 0; i < weight_d; ++i) {
                     for (index_t j = 0; j < weight_h; ++j) {
                         for (index_t k = 0; k < weight_w; ++k) {
                             const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                             const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                             const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                            const scalar_t val =
-                                    deformable ?
-                                    interpolate_sample(
-                                            input, b, c, depth, height, width,
-                                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w])
-                                               : sample(input, b, c, depth, height, width, z, y, x);
-
-                            const scalar_t mask_val =
-                                    modulated ?
-                                    mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
+                            scalar_t val, mask_val;
+                            if constexpr (deformable)
+                                val = interpolate_sample(
+                                        input, b, c, depth, height, width,
+                                        z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                        y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                        x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                            else
+                                val = sample(input, b, c, depth, height, width, z, y, x);
+
+                            if constexpr (modulated)
+                                mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                            else
+                                mask_val = static_cast<scalar_t>(1);
 
                             columns[c][i][j][k][b][d][h][w] = val * mask_val;
                         }
                     }
                 }
             }
         }
@@ -373,20 +375,23 @@
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                 const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                 const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                const scalar_t mask_val =
-                        modulated ? mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
+                scalar_t mask_val;
+                if constexpr (modulated)
+                    mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                else
+                    mask_val = static_cast<scalar_t>(1);
 
-                const scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
+                scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
 
-                if (deformable)
+                if constexpr (deformable)
                     interpolate_insert(
                             grad_input, b, c, depth, height, width,
                             z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
                             y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
                             x + offset[b][offset_group_idx][i][j][k][2][d][h][w],
                             val);
                 else
@@ -514,24 +519,27 @@
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                     const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    const scalar_t weight =
+                    scalar_t weight =
                             coordinate_weight(
                                     input, b, c, depth, height, width,
                                     z + offset[b][g][i][j][k][0][d][h][w],
                                     y + offset[b][g][i][j][k][1][d][h][w],
                                     x + offset[b][g][i][j][k][2][d][h][w],
                                     o);
 
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
+                    scalar_t mask_val;
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     grad_offset_val += columns[c][i][j][k][b][d][h][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][j][k][o][d][h][w] = grad_offset_val;
             }
         }
@@ -656,22 +664,23 @@
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t offset_group_idx = c / c_per_offset_group;
 
                     const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                     const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, depth, height, width,
-                                    z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                    y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                    x + offset[b][offset_group_idx][i][j][k][2][d][h][w])
-                                       : sample(input, b, c, depth, height, width, z, y, x);
+                    scalar_t val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, depth, height, width,
+                                z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                    else
+                        val = sample(input, b, c, depth, height, width, z, y, x);
 
                     grad_mask_val += columns[c][i][j][k][b][d][h][w] * val;
                 }
 
                 grad_mask[b][g][i][j][k][d][h][w] = grad_mask_val;
             }
         }
```

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu` & `tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu`

 * *Files 1% similar despite different names*

```diff
@@ -121,23 +121,26 @@
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 for (index_t i = 0; i < weight_w; ++i) {
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, width,
-                                    x + offset[b][offset_group_idx][i][0][w])
-                                       : sample(input, b, c, width, x);
-
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                    scalar_t val, mask_val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, width,
+                                x + offset[b][offset_group_idx][i][0][w]);
+                    else
+                        val = sample(input, b, c, width, x);
+
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     columns[c][i][b][w] = val * mask_val;
                 }
             }
         }
 
         void arr2col_cuda(
@@ -215,20 +218,23 @@
                 const index_t b = (index / (weight_w * out_w * in_channels));
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                const scalar_t mask_val =
-                        modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                scalar_t mask_val;
+                if constexpr (modulated)
+                    mask_val = mask[b][mask_group_idx][i][w];
+                else
+                    mask_val = static_cast<scalar_t>(1);
 
-                const scalar_t val = columns[c][i][b][w] * mask_val;
+                scalar_t val = columns[c][i][b][w] * mask_val;
 
-                if (deformable)
+                if constexpr (deformable)
                     interpolate_insert(
                             grad_input, b, c, width,
                             x + offset[b][offset_group_idx][i][0][w],
                             val);
                 else
                     insert(grad_input, b, c, width, x, val);
             }
@@ -314,20 +320,23 @@
                 const index_t c_start = g * c_per_offset_group;
                 const index_t c_end = c_start + c_per_offset_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    const scalar_t weight = coordinate_weight(
+                    scalar_t weight = coordinate_weight(
                             input, b, c, width,
                             x + offset[b][g][i][0][w]);
 
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][w] : static_cast<scalar_t>(1);
+                    scalar_t mask_val;
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     grad_offset_val += columns[c][i][b][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][0][w] = grad_offset_val;
             }
         }
@@ -414,20 +423,21 @@
                 const index_t c_start = g * c_per_mask_group;
                 const index_t c_end = c_start + c_per_mask_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t offset_group_idx = c / c_per_offset_group;
 
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, width,
-                                    x + offset[b][offset_group_idx][i][0][w])
-                                       : sample(input, b, c, width, x);
+                    scalar_t val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, width,
+                                x + offset[b][offset_group_idx][i][0][w]);
+                    else
+                        val = sample(input, b, c, width, x);
 
                     grad_mask_val += columns[c][i][b][w] * val;
                 }
 
                 grad_mask[b][g][i][w] = grad_mask_val;
             }
         }
```

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu` & `tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu`

 * *Files 2% similar despite different names*

```diff
@@ -165,24 +165,27 @@
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 for (index_t i = 0; i < weight_h; ++i) {
                     for (index_t j = 0; j < weight_w; ++j) {
                         const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                         const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                        const scalar_t val =
-                                deformable ?
-                                interpolate_sample(
-                                        input, b, c, height, width,
-                                        y + offset[b][offset_group_idx][i][j][0][h][w],
-                                        x + offset[b][offset_group_idx][i][j][1][h][w])
-                                           : sample(input, b, c, height, width, y, x);
-
-                        const scalar_t mask_val =
-                                modulated ? mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                        scalar_t val, mask_val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, height, width,
+                                    y + offset[b][offset_group_idx][i][j][0][h][w],
+                                    x + offset[b][offset_group_idx][i][j][1][h][w]);
+                        else
+                            val = sample(input, b, c, height, width, y, x);
+
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][j][h][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
 
                         columns[c][i][j][b][h][w] = val * mask_val;
                     }
                 }
             }
         }
 
@@ -282,20 +285,23 @@
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                 const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                const scalar_t mask_val =
-                        modulated ? mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                scalar_t mask_val;
+                if constexpr (modulated)
+                    mask_val = mask[b][mask_group_idx][i][j][h][w];
+                else
+                    mask_val = static_cast<scalar_t>(1);
 
-                const scalar_t val = columns[c][i][j][b][h][w] * mask_val;
+                scalar_t val = columns[c][i][j][b][h][w] * mask_val;
 
-                if (deformable)
+                if constexpr (deformable)
                     interpolate_insert(
                             grad_input, b, c, height, width,
                             y + offset[b][offset_group_idx][i][j][0][h][w],
                             x + offset[b][offset_group_idx][i][j][1][h][w],
                             val);
                 else
                     insert(grad_input, b, c, height, width, y, x, val);
@@ -404,22 +410,25 @@
                 const index_t c_end = c_start + c_per_offset_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    const scalar_t weight = coordinate_weight(
+                    scalar_t weight = coordinate_weight(
                             input, b, c, height, width,
                             y + offset[b][g][i][j][0][h][w],
                             x + offset[b][g][i][j][1][h][w],
                             o);
 
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][j][h][w] : static_cast<scalar_t>(1);
+                    scalar_t mask_val;
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][j][h][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
             }
         }
@@ -527,21 +536,22 @@
                 const index_t c_end = c_start + c_per_mask_group;
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t offset_group_idx = c / c_per_offset_group;
 
                     const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, height, width,
-                                    y + offset[b][offset_group_idx][i][j][0][h][w],
-                                    x + offset[b][offset_group_idx][i][j][1][h][w])
-                                       : sample(input, b, c, height, width, y, x);
+                    scalar_t val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, height, width,
+                                y + offset[b][offset_group_idx][i][j][0][h][w],
+                                x + offset[b][offset_group_idx][i][j][1][h][w]);
+                    else
+                        val = sample(input, b, c, height, width, y, x);
 
                     grad_mask_val += columns[c][i][j][b][h][w] * val;
                 }
 
                 grad_mask[b][g][i][j][h][w] = grad_mask_val;
             }
         }
```

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu` & `tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu`

 * *Files 2% similar despite different names*

```diff
@@ -239,26 +239,28 @@
                 for (index_t i = 0; i < weight_d; ++i) {
                     for (index_t j = 0; j < weight_h; ++j) {
                         for (index_t k = 0; k < weight_w; ++k) {
                             const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                             const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                             const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                            const scalar_t val =
-                                    deformable ?
-                                    interpolate_sample(
-                                            input, b, c, depth, height, width,
-                                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w])
-                                               : sample(input, b, c, depth, height, width, z, y, x);
-
-                            const scalar_t mask_val =
-                                    modulated ?
-                                    mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
+                            scalar_t val, mask_val;
+                            if constexpr (deformable)
+                                val = interpolate_sample(
+                                        input, b, c, depth, height, width,
+                                        z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                        y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                        x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                            else
+                                val = sample(input, b, c, depth, height, width, z, y, x);
+
+                            if constexpr (modulated)
+                                mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                            else
+                                mask_val = static_cast<scalar_t>(1);
 
                             columns[c][i][j][k][b][d][h][w] = val * mask_val;
                         }
                     }
                 }
             }
         }
@@ -380,20 +382,23 @@
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
 
                 const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                 const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                 const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                const scalar_t mask_val =
-                        modulated ? mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
+                scalar_t mask_val;
+                if constexpr (modulated)
+                    mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                else
+                    mask_val = static_cast<scalar_t>(1);
 
-                const scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
+                scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
 
-                if (deformable)
+                if constexpr (deformable)
                     interpolate_insert(
                             grad_input, b, c, depth, height, width,
                             z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
                             y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
                             x + offset[b][offset_group_idx][i][j][k][2][d][h][w],
                             val);
                 else
@@ -526,24 +531,27 @@
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                     const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    const scalar_t weight =
+                    scalar_t weight =
                             coordinate_weight(
                                     input, b, c, depth, height, width,
                                     z + offset[b][g][i][j][k][0][d][h][w],
                                     y + offset[b][g][i][j][k][1][d][h][w],
                                     x + offset[b][g][i][j][k][2][d][h][w],
                                     o);
 
-                    const scalar_t mask_val =
-                            modulated ? mask[b][mask_group_idx][i][j][k][d][h][w] : static_cast<scalar_t>(1);
+                    scalar_t mask_val;
+                    if constexpr (modulated)
+                        mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                    else
+                        mask_val = static_cast<scalar_t>(1);
 
                     grad_offset_val += columns[c][i][j][k][b][d][h][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][j][k][o][d][h][w] = grad_offset_val;
             }
         }
@@ -673,22 +681,23 @@
                 for (index_t c = c_start; c < c_end; ++c) {
                     const index_t offset_group_idx = c / c_per_offset_group;
 
                     const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                     const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    const scalar_t val =
-                            deformable ?
-                            interpolate_sample(
-                                    input, b, c, depth, height, width,
-                                    z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                    y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                    x + offset[b][offset_group_idx][i][j][k][2][d][h][w])
-                                       : sample(input, b, c, depth, height, width, z, y, x);
+                    scalar_t val;
+                    if constexpr (deformable)
+                        val = interpolate_sample(
+                                input, b, c, depth, height, width,
+                                z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                    else
+                        val = sample(input, b, c, depth, height, width, z, y, x);
 
                     grad_mask_val += columns[c][i][j][k][b][d][h][w] * val;
                 }
 
                 grad_mask[b][g][i][j][k][d][h][w] = grad_mask_val;
             }
         }
```

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/ops/utils/tensor_utils.cpp` & `tvdcn-0.3.2/tvdcn/csrc/ops/utils/tensor_utils.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.3.2/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/extension.py` & `tvdcn-0.3.2/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.3.2/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.3.2/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/ops/deform_conv.py` & `tvdcn-0.3.2/tvdcn/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.3.2/tvdcn/ops/deform_conv_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import torch
 from torch import nn, Tensor
 from torch.nn import init
 from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.utils import _single, _pair, _triple
 
-# noinspection PyUnresolvedReferences
 from .activations import (
     MaskSigmoid, MaskSoftmax1d, MaskSoftmax2d, MaskSoftmax3d,
 )
 from .deform_conv import _DeformConvNd
 from .._types import _IntTuple, _Activation
 from ..extension import _assert_has_ops
 from ..utils import _log_api_usage_once
```

### Comparing `tvdcn-0.3.1/tvdcn/utils.py` & `tvdcn-0.3.2/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.1/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.3.2/tvdcn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.1
+Version: 0.3.2
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -93,15 +93,16 @@
 | Python version:  |                   3.8-3.11                    |    3.8-3.11    |
 | PyTorch version: |                `torch==2.0.1`                 | `torch==2.0.1` |
 | Cuda version:    |                     11.8                      |       -        |
 | GPU CCs:         | `3.7,5.0,6.0,6.1,7.0,7.5,8.0,8.6,8.9,9.0+PTX` |       -        |
 
 #### From Source:
 
-For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`).
+For installing from source, you need a C++ compiler (`gcc`/`msvc`) and a Cuda compiler (`nvcc`) with C++17 features
+enabled.
 Clone this repo and execute the following command:
 
 ```terminal
 pip install .
 ```
 
 Or just compile the binary for inplace usage:
@@ -138,31 +139,31 @@
 ```python
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Union[int, Tuple[int, ...]] = 1,
-        padding: Union[int, Tuple[int, ...]] = 0,
-        dilation: Union[int, Tuple[int, ...]] = 1,
+        stride: Union[int, Tuple[int, int]] = 1,
+        padding: Union[int, Tuple[int, int]] = 0,
+        dilation: Union[int, Tuple[int, int]] = 1,
         groups: int = 1) -> Tensor:
     ...
 
 
 def deform_conv_transpose2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Union[int, Tuple[int, ...]] = 1,
-        padding: Union[int, Tuple[int, ...]] = 0,
-        output_padding: Union[int, Tuple[int, ...]] = 0,
-        dilation: Union[int, Tuple[int, ...]] = 1,
+        stride: Union[int, Tuple[int, int]] = 1,
+        padding: Union[int, Tuple[int, int]] = 0,
+        output_padding: Union[int, Tuple[int, int]] = 0,
+        dilation: Union[int, Tuple[int, int]] = 1,
         groups: int = 1) -> Tensor:
     ...
 ```
 
 If `offset=None` and `mask=None`, the executed operations are identical to conventional convolution.
 
 #### Neural Network Layers:
```

### Comparing `tvdcn-0.3.1/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.3.2/tvdcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

