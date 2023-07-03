# Comparing `tmp/cjm-yolox-pytorch-0.0.7.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.7.tar", last modified: Mon Jul  3 19:10:22 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.8.tar", last modified: Mon Jul  3 19:12:06 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.7.tar` & `cjm-yolox-pytorch-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:10:22.533817 cjm-yolox-pytorch-0.0.7/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.7/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.7/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:10:22.533657 cjm-yolox-pytorch-0.0.7/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-03 18:20:50.000000 cjm-yolox-pytorch-0.0.7/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:10:22.531100 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-03 19:09:50.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-03 19:09:50.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    21383 2023-07-03 19:09:50.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-03 19:09:50.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15405 2023-07-03 19:09:50.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-03 19:09:50.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:10:22.533320 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:10:22.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-03 19:10:22.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-03 19:10:22.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-03 19:10:22.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-03 19:10:22.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-03 19:10:22.000000 cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-03 19:09:02.000000 cjm-yolox-pytorch-0.0.7/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-03 19:10:22.533867 cjm-yolox-pytorch-0.0.7/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.7/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:12:06.956851 cjm-yolox-pytorch-0.0.8/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.8/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.8/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:12:06.956696 cjm-yolox-pytorch-0.0.8/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-03 18:20:50.000000 cjm-yolox-pytorch-0.0.8/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:12:06.954098 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    21379 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15405 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-03 19:11:47.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-03 19:12:06.956349 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-03 19:12:06.000000 cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-03 19:11:35.000000 cjm-yolox-pytorch-0.0.8/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-03 19:12:06.956927 cjm-yolox-pytorch-0.0.8/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.8/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.7/LICENSE` & `cjm-yolox-pytorch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.7/PKG-INFO` & `cjm-yolox-pytorch-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.7/README.md` & `cjm-yolox-pytorch-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         stride = self.strides[level_idx]
         shift_x = (torch.arange(0., feat_w, device=device) + self.offset) * stride
         shift_y = (torch.arange(0., feat_h, device=device) + self.offset) * stride
         shift_xx, shift_yy = torch.meshgrid(shift_x, shift_y, indexing='xy')
         shift_xx, shift_yy = shift_xx.flatten(), shift_yy.flatten()
 
         if with_stride:
-            shifts = torch.stack([shift_xx, shift_yy, torch.full_like(shift_xx, stride_w), torch.full_like(shift_yy, stride_h)], dim=-1)
+            shifts = torch.stack([shift_xx, shift_yy, torch.full_like(shift_xx, stride), torch.full_like(shift_yy, stride)], dim=-1)
         else:
             shifts = torch.stack([shift_xx, shift_yy], dim=-1)
         
         return shifts.to(device)
 
 # %% ../nbs/02_loss.ipynb 10
 class SamplingResult:
```

### Comparing `cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.7/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.8/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.7/settings.ini` & `cjm-yolox-pytorch-0.0.8/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.7
+version = 0.0.8
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.7/setup.py` & `cjm-yolox-pytorch-0.0.8/setup.py`

 * *Files identical despite different names*

