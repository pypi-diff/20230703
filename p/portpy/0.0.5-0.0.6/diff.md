# Comparing `tmp/portpy-0.0.5.tar.gz` & `tmp/portpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\portpy-0.0.5.tar", last modified: Mon Jun 26 20:41:24 2023, max compression
+gzip compressed data, was "dist\portpy-0.0.6.tar", last modified: Mon Jul  3 16:49:37 2023, max compression
```

## Comparing `portpy-0.0.5.tar` & `portpy-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:24.000000 portpy-0.0.5/
--rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8193 2023-06-26 20:41:24.000000 portpy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6587 2023-06-13 18:42:32.000000 portpy-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/images/
--rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.5/images/PortPy_logo.jpg
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/
--rw-rw-rw-   0        0        0       52 2023-06-26 20:40:38.000000 portpy-0.0.5/portpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/
--rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-0.0.5/portpy/config_files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/clinical_criteria/
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/clinical_criteria/Default/
--rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.5/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/optimization_params/
--rw-rw-rw-   0        0        0     2419 2023-06-21 16:45:36.000000 portpy-0.0.5/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/photon/
--rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-0.0.5/portpy/photon/__init__.py
--rw-rw-rw-   0        0        0     8347 2023-06-13 17:33:26.000000 portpy-0.0.5/portpy/photon/beam.py
--rw-rw-rw-   0        0        0     4994 2023-06-13 15:49:21.000000 portpy-0.0.5/portpy/photon/clinical_criteria.py
--rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-0.0.5/portpy/photon/ct.py
--rw-rw-rw-   0        0        0    23325 2023-06-26 14:23:50.000000 portpy-0.0.5/portpy/photon/data_explorer.py
--rw-rw-rw-   0        0        0    15901 2023-06-22 18:40:10.000000 portpy-0.0.5/portpy/photon/evaluation.py
--rw-rw-rw-   0        0        0    48775 2023-06-13 15:28:29.000000 portpy-0.0.5/portpy/photon/influence_matrix.py
--rw-rw-rw-   0        0        0    22066 2023-06-22 20:54:30.000000 portpy-0.0.5/portpy/photon/optimization.py
--rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-0.0.5/portpy/photon/plan.py
--rw-rw-rw-   0        0        0    16378 2023-06-13 17:27:58.000000 portpy-0.0.5/portpy/photon/structures.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/photon/utils/
--rw-rw-rw-   0        0        0      342 2023-06-21 21:52:31.000000 portpy-0.0.5/portpy/photon/utils/__init__.py
--rw-rw-rw-   0        0        0     2931 2023-06-22 16:17:59.000000 portpy-0.0.5/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
--rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.5/portpy/photon/utils/get_eclipse_fluence.py
--rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.5/portpy/photon/utils/save_nrrd.py
--rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.5/portpy/photon/utils/save_or_load_pickle.py
--rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.5/portpy/photon/utils/slicer_script.py
--rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-0.0.5/portpy/photon/utils/view_in_slicer_jupyter.py
--rw-rw-rw-   0        0        0    23970 2023-06-13 17:30:49.000000 portpy-0.0.5/portpy/photon/visualization.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy.egg-info/
--rw-rw-rw-   0        0        0     8193 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      993 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 20:41:24.000000 portpy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:37.000000 portpy-0.0.6/
+-rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     8193 2023-07-03 16:49:37.000000 portpy-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6587 2023-06-13 18:42:32.000000 portpy-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/images/
+-rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.6/images/PortPy_logo.jpg
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy/
+-rw-rw-rw-   0        0        0       52 2023-07-03 16:46:25.000000 portpy-0.0.6/portpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy/config_files/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-0.0.6/portpy/config_files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.6/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2419 2023-06-21 16:45:36.000000 portpy-0.0.6/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy/photon/
+-rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-0.0.6/portpy/photon/__init__.py
+-rw-rw-rw-   0        0        0     8347 2023-06-13 17:33:26.000000 portpy-0.0.6/portpy/photon/beam.py
+-rw-rw-rw-   0        0        0     4994 2023-06-13 15:49:21.000000 portpy-0.0.6/portpy/photon/clinical_criteria.py
+-rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-0.0.6/portpy/photon/ct.py
+-rw-rw-rw-   0        0        0    23555 2023-06-29 15:51:21.000000 portpy-0.0.6/portpy/photon/data_explorer.py
+-rw-rw-rw-   0        0        0    15901 2023-06-22 18:40:10.000000 portpy-0.0.6/portpy/photon/evaluation.py
+-rw-rw-rw-   0        0        0    48833 2023-06-29 15:52:51.000000 portpy-0.0.6/portpy/photon/influence_matrix.py
+-rw-rw-rw-   0        0        0    22066 2023-07-01 16:00:32.000000 portpy-0.0.6/portpy/photon/optimization.py
+-rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-0.0.6/portpy/photon/plan.py
+-rw-rw-rw-   0        0        0    16378 2023-06-13 17:27:58.000000 portpy-0.0.6/portpy/photon/structures.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy/photon/utils/
+-rw-rw-rw-   0        0        0      342 2023-06-21 21:52:31.000000 portpy-0.0.6/portpy/photon/utils/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-07-03 15:57:47.000000 portpy-0.0.6/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
+-rw-rw-rw-   0        0        0     2482 2023-07-01 16:42:21.000000 portpy-0.0.6/portpy/photon/utils/get_eclipse_fluence.py
+-rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.6/portpy/photon/utils/save_nrrd.py
+-rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.6/portpy/photon/utils/save_or_load_pickle.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.6/portpy/photon/utils/slicer_script.py
+-rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-0.0.6/portpy/photon/utils/view_in_slicer_jupyter.py
+-rw-rw-rw-   0        0        0    23970 2023-06-13 17:30:49.000000 portpy-0.0.6/portpy/photon/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:49:35.000000 portpy-0.0.6/portpy.egg-info/
+-rw-rw-rw-   0        0        0     8193 2023-07-03 16:49:33.000000 portpy-0.0.6/portpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      993 2023-07-03 16:49:33.000000 portpy-0.0.6/portpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:49:33.000000 portpy-0.0.6/portpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      367 2023-07-03 16:49:33.000000 portpy-0.0.6/portpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 16:49:33.000000 portpy-0.0.6/portpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 16:49:37.000000 portpy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2529 2023-06-30 17:21:11.000000 portpy-0.0.6/setup.py
```

### Comparing `portpy-0.0.5/PKG-INFO` & `portpy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
```

### Comparing `portpy-0.0.5/README.md` & `portpy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/images/PortPy_logo.jpg` & `portpy-0.0.6/images/PortPy_logo.jpg`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json` & `portpy-0.0.6/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json` & `portpy-0.0.6/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/beam.py` & `portpy-0.0.6/portpy/photon/beam.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/clinical_criteria.py` & `portpy-0.0.6/portpy/photon/clinical_criteria.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/ct.py` & `portpy-0.0.6/portpy/photon/ct.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/data_explorer.py` & `portpy-0.0.6/portpy/photon/data_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,14 +331,18 @@
         e.g. if options['loadInfluenceMatrixFull']=True, it will load full influence matrix
         :return: a dict of data
         """
         if not load_inf_matrix_full:
             if 'influenceMatrixFull_File' in meta_data:
                 meta_data['influenceMatrixFull_File'] = [None] * len(
                     meta_data['influenceMatrixFull_File'])
+        elif load_inf_matrix_full:
+            if 'influenceMatrixSparse_File' in meta_data:
+                meta_data['influenceMatrixSparse_File'] = [None] * len(
+                    meta_data['influenceMatrixSparse_File'])
         meta_data = self.load_file(meta_data=meta_data)  # recursive function to load data from .h5 files
         return meta_data
 
     def load_file(self, meta_data: dict):
         """
         This recursive function loads the data from .h5 files and merge them with the meta_data and returns a dictionary
         including all the data (meta_data+actual numeric data)
```

### Comparing `portpy-0.0.5/portpy/photon/evaluation.py` & `portpy-0.0.6/portpy/photon/evaluation.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/influence_matrix.py` & `portpy-0.0.6/portpy/photon/influence_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from shapely.geometry import LinearRing, Polygon, Point
 from scipy import sparse
 from copy import deepcopy
 from scipy.sparse import csr_matrix
-import matplotlib.pyplot as plt
 import itertools
 from patchify import patchify
 from typing import List, Union
 from .ct import CT
 from .beam import Beams
 from .structures import Structures
 
@@ -39,20 +38,22 @@
 
     """
 
     def __init__(self, ct: CT, structs: Structures, beams: Beams,
                  beamlet_width_mm: float = None, beamlet_height_mm: float = None, opt_vox_xyz_res_mm: List[float] = None,
                  is_full: bool = False, target_structure: str = 'PTV', opt_beamlets_PTV_margin_mm: float = 3) -> None:
         """
-        Create a influence matrix object for Influence Matrix class based upon beamlet resolution and down-sampling_xyz ratio
+        Create a influence matrix object for Influence Matrix class based upon beamlet resolution and opt_vox_xyz_res_mm
 
-        :param plan_obj: object of class Plan
+        :param ct: object of class CT
+        :param structs: object of class Structures
+        :param beams: Object of class Beams
         :param beamlet_width_mm: beamlet width in mm. It should be multiple of 2.5, defaults to 2.5
         :param beamlet_height_mm: beamlet height in mm. It should be multiple of 2.5, defaults to 2.5
-        :param structure: target struct_name for creating BEV beamlets, defaults to 'PTV'
+        :param target_structure: target struct_name for creating BEV beamlets, defaults to 'PTV'
         :param opt_vox_xyz_res_mm: It down-samples optimization voxels as factor of ct resolution
                 e.g. opt_vox_xyz_res = [5*ct.res.x,5*ct.res.y,1*ct.res.z]. It will down-sample optimization voxels with 5 * ct res. in x direction, 5 * ct res. in y direction and 1*ct res. in z direction.
                 defaults to None. When None it will use the original optimization voxel resolution.
         :param is_full: Load full or sparse matrix. defaults to False. If True, will load full matrix
 
         """
         if beamlet_width_mm is None and beamlet_height_mm is None:
@@ -73,15 +74,15 @@
             down_sample_xyz = [round(i / j) for i, j in zip(opt_vox_xyz_res_mm, ct.get_ct_res_xyz_mm())]
             if np.all(np.array(down_sample_xyz) == 1):  # if all are 1 then no down sample
                 down_sample_xyz = None
 
         self._down_sample_xyz = down_sample_xyz
         self.is_full = is_full
 
-        # create deepcopy of the object or else it will modify the my_plan object
+        # create deepcopy of the object or else it will modify the structs object
         if hasattr(structs, 'opt_voxels_dict'):
             self.opt_voxels_dict = deepcopy(structs.opt_voxels_dict)
             # del structs.opt_voxels_dict  # remove opt_voxels_dict from structures
         else:
             self.opt_voxels_dict = deepcopy(self.opt_voxels_dict)
 
         # creating deepcopy so that it doesnt modify beams object
```

### Comparing `portpy-0.0.5/portpy/photon/optimization.py` & `portpy-0.0.6/portpy/photon/optimization.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/plan.py` & `portpy-0.0.6/portpy/photon/plan.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/structures.py` & `portpy-0.0.6/portpy/photon/structures.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py` & `portpy-0.0.6/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     rt_dose = arr_dose * dose_img.DoseGridScaling
     rt_dose_itk = sitk.GetImageFromArray(rt_dose)
     if 'Phantom' in dose_file_name:
         # There is issue for phantom patient. CT and dose dicom images have different origin w.r.t eclipse.
         # Eclipse have different origin
         dose_img.ImagePositionPatient[0] = dose_img.ImagePositionPatient[0] - 65.63
     rt_dose_itk.SetOrigin(dose_img.ImagePositionPatient)
-    rt_dose_itk.SetSpacing([np.float(dose_img.PixelSpacing[0]), np.float(dose_img.PixelSpacing[1]),
+    rt_dose_itk.SetSpacing([float(dose_img.PixelSpacing[0]), float(dose_img.PixelSpacing[1]),
                             dose_img.GridFrameOffsetVector[1] - dose_img.GridFrameOffsetVector[0]])
     # return dose_img
     return rt_dose_itk
 
 
 def read_dicom(in_dir):
     dicom_names = os.listdir(in_dir)
```

### Comparing `portpy-0.0.5/portpy/photon/utils/get_eclipse_fluence.py` & `portpy-0.0.6/portpy/photon/utils/get_eclipse_fluence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+from __future__ import annotations
 import os
 import numpy as np
 from typing import List
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from portpy.photon.plan import Plan
 
 
-def get_eclipse_fluence(sol: dict, path: str = None, beam_ids: List[str] = None) -> None:
+def get_eclipse_fluence(my_plan: Plan, sol: dict, path: str = None, beam_ids: List[str] = None) -> None:
     """
     save eclipse fluence in the path directory
+
+    :param my_plan: object of class Plan
+    :param sol: dictionary containing optimal intensity
+    :param path: directory for saving the optimal fluence
+    :param beam_ids: list of string containing beam ids
+
     """
     if path is None:
         path = os.getcwd()
     tol = 1e-06
     inf_matrix = sol['inf_matrix']
     optimal_fluence_2d = inf_matrix.fluence_1d_to_2d(sol=sol)
     for i in range(len(optimal_fluence_2d)):
         if beam_ids is not None:
             beam_id = beam_ids[i]
         else:
             beam_id = str(inf_matrix.beamlets_dict[i]['beam_id'])
         file_name = 'ID' + beam_id + '.optimal_fluence'
         filepath = os.path.join(path, file_name)
         f = open(filepath, 'w')
-        fluence_2d = optimal_fluence_2d[i]
+        fluence_2d = optimal_fluence_2d[i]/(my_plan.get_prescription()/my_plan.get_num_of_fractions())
         f.write('optimalfluence\n')
         f.write('SizeX      {}\n'.format(fluence_2d.shape[1]))
         f.write('SizeY      {}\n'.format(fluence_2d.shape[0]))
         f.write('SpacingX   {}\n'.format(2.5))
         f.write('SpacingY   {}\n'.format(2.5))
         beamlets = inf_matrix._beams.beams_dict['beamlets'][i]
         x_positions = beamlets['position_x_mm'][0] - beamlets['width_mm'][
```

### Comparing `portpy-0.0.5/portpy/photon/utils/save_nrrd.py` & `portpy-0.0.6/portpy/photon/utils/save_nrrd.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/utils/save_or_load_pickle.py` & `portpy-0.0.6/portpy/photon/utils/save_or_load_pickle.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/utils/slicer_script.py` & `portpy-0.0.6/portpy/photon/utils/slicer_script.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/utils/view_in_slicer_jupyter.py` & `portpy-0.0.6/portpy/photon/utils/view_in_slicer_jupyter.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy/photon/visualization.py` & `portpy-0.0.6/portpy/photon/visualization.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/portpy.egg-info/PKG-INFO` & `portpy-0.0.6/portpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
```

### Comparing `portpy-0.0.5/portpy.egg-info/SOURCES.txt` & `portpy-0.0.6/portpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portpy-0.0.5/setup.py` & `portpy-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,10 +66,11 @@
         "SimpleITK>=2.0.2",
         "tabulate>=0.9.0",
         "typing>=3.7.4.3",
         "jinja2>=3.0.1",
         "typing-extensions>=3.10.0.0",
         "scikit-image>=0.17.2",
         "patchify>=0.2.3",
+        "pydicom>=2.2.0",
     ],
 
 )
```

