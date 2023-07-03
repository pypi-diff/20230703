# Comparing `tmp/numan-1.0.4.tar.gz` & `tmp/numan-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numan-1.0.4.tar", last modified: Tue Jun  6 23:03:01 2023, max compression
+gzip compressed data, was "numan-1.0.6.tar", last modified: Mon Jul  3 20:34:14 2023, max compression
```

## Comparing `numan-1.0.4.tar` & `numan-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.549703 numan-1.0.4/
--rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.4/LICENSE.md
--rw-rw-rw-   0        0        0     2181 2023-06-06 23:03:01.548699 numan-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.4/README.md
--rw-rw-rw-   0        0        0     1314 2023-06-06 20:30:59.000000 numan-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 23:03:01.550700 numan-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.390700 numan-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.487699 numan-1.0.4/src/numan/
--rw-rw-rw-   0        0        0      224 2022-09-25 05:16:00.000000 numan-1.0.4/src/numan/__init__.py
--rw-rw-rw-   0        0        0    30144 2023-06-06 20:27:40.000000 numan-1.0.4/src/numan/analysis.py
--rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.4/src/numan/notifications.py
--rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.4/src/numan/plots.py
--rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.4/src/numan/project.py
--rw-rw-rw-   0        0        0    27170 2023-06-06 23:01:44.000000 numan-1.0.4/src/numan/report.py
--rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.4/src/numan/runner.py
--rw-rw-rw-   0        0        0     5169 2022-09-25 00:13:45.000000 numan-1.0.4/src/numan/utils.py
--rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.4/src/numan/visualization.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.519698 numan-1.0.4/src/numan.egg-info/
--rw-rw-rw-   0        0        0     2181 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 23:03:01.000000 numan-1.0.4/src/numan.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 23:03:01.546699 numan-1.0.4/tests/
--rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.4/tests/test_plots.py
--rw-rw-rw-   0        0        0    15189 2023-06-06 20:27:40.000000 numan-1.0.4/tests/test_plots_cp13.py
--rw-rw-rw-   0        0        0     1469 2022-09-22 06:17:16.000000 numan-1.0.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:14.891616 numan-1.0.6/
+-rw-rw-rw-   0        0        0     1094 2022-05-18 18:25:15.000000 numan-1.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0     2181 2023-07-03 20:34:14.890618 numan-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2022-05-18 18:25:15.000000 numan-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1314 2023-07-03 20:32:40.000000 numan-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:34:14.891616 numan-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0       53 2022-08-16 05:16:10.000000 numan-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:14.793589 numan-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:14.863649 numan-1.0.6/src/numan/
+-rw-rw-rw-   0        0        0      224 2023-07-03 20:32:40.000000 numan-1.0.6/src/numan/__init__.py
+-rw-rw-rw-   0        0        0    44350 2023-07-03 19:08:23.000000 numan-1.0.6/src/numan/analysis.py
+-rw-rw-rw-   0        0        0     1382 2022-08-18 08:58:12.000000 numan-1.0.6/src/numan/notifications.py
+-rw-rw-rw-   0        0        0    32617 2022-09-25 04:39:18.000000 numan-1.0.6/src/numan/plots.py
+-rw-rw-rw-   0        0        0     1097 2022-08-18 04:32:02.000000 numan-1.0.6/src/numan/project.py
+-rw-rw-rw-   0        0        0    27170 2023-06-06 23:01:44.000000 numan-1.0.6/src/numan/report.py
+-rw-rw-rw-   0        0        0     3396 2022-08-21 22:45:27.000000 numan-1.0.6/src/numan/runner.py
+-rw-rw-rw-   0        0        0     6437 2023-07-03 19:08:23.000000 numan-1.0.6/src/numan/utils.py
+-rw-rw-rw-   0        0        0    31015 2023-06-06 20:27:40.000000 numan-1.0.6/src/numan/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:14.885648 numan-1.0.6/src/numan.egg-info/
+-rw-rw-rw-   0        0        0     2181 2023-07-03 20:34:14.000000 numan-1.0.6/src/numan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-03 20:34:14.000000 numan-1.0.6/src/numan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 20:34:14.000000 numan-1.0.6/src/numan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-07-03 20:34:14.000000 numan-1.0.6/src/numan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-03 20:34:14.000000 numan-1.0.6/src/numan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:14.889614 numan-1.0.6/tests/
+-rw-rw-rw-   0        0        0    15043 2022-11-29 19:20:20.000000 numan-1.0.6/tests/test_plots.py
+-rw-rw-rw-   0        0        0    15189 2023-07-03 19:08:29.000000 numan-1.0.6/tests/test_plots_cp13.py
+-rw-rw-rw-   0        0        0     2153 2023-07-03 19:08:23.000000 numan-1.0.6/tests/test_utils.py
```

### Comparing `numan-1.0.4/LICENSE.md` & `numan-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/PKG-INFO` & `numan-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.4
+Version: 1.0.6
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.4/README.md` & `numan-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/pyproject.toml` & `numan-1.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numan"
-version = "1.0.4"
+version = "1.0.6"
 description='numerosity analysis package'
 readme = "README.md"
 authors = [{ name = "Anna Nadtochiy", email = "nadtochi@usc.edu" }]
 license = { file = "LICENSE" }
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Image Processing',
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
 ]
 dependencies = [
-    'vodex >=1.0.18,<2.0.0',
+    'vodex >=1.0.19,<2.0.0',
     'pypdf2',
     'reportlab',
     'scipy',
     'ipykernel',
     'urllib3',
     'nbconvert',
     'scipy',
@@ -34,15 +34,15 @@
 [project.optional-dependencies]
 dev = ["bumpver"]
 
 [project.urls] # Read The Docs will also go in here
 Homepage = "https://github.com/LemonJust/numan"
 
 [tool.bumpver]
-current_version = "1.0.4"
+current_version = "1.0.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `numan-1.0.4/src/numan/analysis.py` & `numan-1.0.6/src/numan/analysis.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """
 Classes for Numerosity analysis.
 """
 from tifffile import TiffFile, imread, imwrite
+from pathlib import Path
 import numpy as np
 import scipy as sp
 import json
 import os
 
 import matplotlib.pyplot as plt
 import warnings
 from tqdm import tqdm
 import pandas as pd
 import PyPDF2
 
+# try:
+import ants
+# except ImportError:
+#     print("ants not installed, some registration will not work")
+
 from .utils import *
 
 
 class Spot:
     """
     This is a class for a n individual segmented spot.
     """
@@ -350,20 +356,20 @@
                 cycled = cycled.reshape(-1, time_shape[1])
 
         mean = np.mean(cycled, axis=0)
 
         if error_type == "prc":
             # error bars : 5 to 95 th percentile around the median
             e = np.r_[np.expand_dims(mean - np.percentile(cycled, 5, axis=0), axis=0),
-                      np.expand_dims(np.percentile(cycled, 95, axis=0) - mean, axis=0)]
+            np.expand_dims(np.percentile(cycled, 95, axis=0) - mean, axis=0)]
         elif error_type == "sem":
             # error bars : sem around hte mean
             sem = np.std(cycled, axis=0, ddof=1) / np.sqrt(cycled.shape[0])
             e = np.r_[np.expand_dims(sem, axis=0),
-                      np.expand_dims(sem, axis=0)]
+            np.expand_dims(sem, axis=0)]
         else:
             e = None
 
         return cycled, mean, e
 
     def to_csv(self, filename):
         """
@@ -675,17 +681,182 @@
     """
     Collection of methods to perform preprocessing of the raw data in experiment.
     """
 
     def __init__(self, experiment):
         self.experiment = experiment
 
-    def batch_dff(self, save_dir, batch_size, window_size, blur_sigma=None, verbose=False):
+    def remove_offset(self, save_dir, batch_size, volumes = None, offset_img=None, offset_file=None, verbose=False):
+        """
+        Denoises the raw movie by subtracting the offset image.
+        The offset image can be prepared using coscmos package.
+        Will only process full volumes.
+        """
+        assert offset_img is not None or offset_file is not None, \
+            "Either offset_img or offset_file should be provided"
+        assert not (offset_img is not None and offset_file is not None), \
+            "Only one of offset_img or offset_file should be provided"
+        if offset_img is None:
+            offset_img = imread(offset_file)
+
+        # Split the volumes into chunks of the defined size that will be loaded into RAM at once
+        # if volumes are not provided, will use all the full volumes
+        # if volumes are provided, will only process the requested volumes
+        chunks = self.experiment.batch_volumes(batch_size, volumes=volumes, full_only=True)
+        
+        if verbose:
+            tot_volumes = 0
+            n_requested_volumes = self.experiment.n_full_volumes
+            if volumes is not None:
+                n_requested_volumes = len(volumes)
+
+        for ichunk, chunk in enumerate(chunks):
+            data = self.experiment.load_volumes(chunk, verbose=False)
+            data = data - offset_img
+            nt, z, y, x = data.shape
+
+            # make sure the output is positive:
+            min_value = data.min()
+            if min_value < 0:
+                warnings.warn(f"Some image values belov zero after subtracting the offset image. "
+                              f"Will be set to zero.")
+                data[data < 0] = 0
+
+            # write image
+            imwrite(f'{save_dir}/removed_offset_movie_{ichunk:04d}.tif',
+                    data.astype(np.int16), shape=(nt, z, y, x),
+                    metadata={'axes': 'TZYX'}, imagej=True)
+
+            if verbose:
+                tot_volumes = tot_volumes + nt
+                print(f"written volumes : {tot_volumes}, out of {n_requested_volumes} full volumes")
+
+    def drift_correct_naive(self, save_dir, batch_size, spacing_xyz, template = 0, 
+                            registration_type = "Rigid", volumes = None, verbose=False, 
+                            ants_kwargs = {}):
+        """
+        Performs drift correction using ANTs library for registration. 
+        template can be an int (a frame to register to), or a 3D numpy array.
+        If template is not provided, the first volume will be used as a template.
+        if volumes is not None, then only the volumes in the list will be registered.
+        For more info, see ANTs documentation: https://antspy.readthedocs.io/en/latest/registration.html
+
+        Args:
+            save_dir (str): directory to save the drift corrected movie.
+            batch_size (int): number of volumes to load at once when processing batches. Each batch is saved as a separate file.
+            spacing_xyz (list): spacing in xyz order
+            template (int or 3D numpy array): template to register to
+            registration_type (str): type of registration to perform, see ANTs documentation for available options.
+            volumes (list): list of volumes to register. If None, all the full volumes will be registered.
+            verbose (bool): whether to print the volumes that have been processed so far on the screen.
+            ants_kwargs (dict): parameters for the registration. If empty, default parameters will be used. See ANTs documentation for available options.
+                mask and moving_mask can be provided as paths to the masks, they will be converted to ants images.
+                Note: (see https://stackoverflow.com/questions/334655/passing-a-dictionary-to-a-function-as-keyword-parameters)
+                 1. ants.registration can have parameters that are not included in the dictionary, just specify what you want, the rest will be default. 
+                 2. You can not override an ants.registration function parameter that is already in the dictionary, 
+                 so don't try to include keywords fixed, moving, type_of_transform, verbose and outprefix in the dictionary.
+                 3. The dictionary can not have values that aren't in the ants.registration function.
+        """
+        def _register(moving_image, fixed_image, spacing, registration_type, outprefix = None):
+
+            # if fixed image in not ants image, convert it
+            if not isinstance(fixed_image, ants.core.ants_image.ANTsImage):
+                print("Converting fixed image to ants image")
+                fixed_image = ants.from_numpy(np.transpose(fixed_image.astype(float), axes=[2,1,0]), 
+                                    spacing=spacing) # spacing in xyz order
+                
+            moving_image = ants.from_numpy(np.transpose(moving_image.astype(float), axes=[2,1,0]), 
+                                spacing=spacing)
+            
+            # run the registration and save verbose to file
+            rr = ants.registration(
+                                    fixed=fixed_image,
+                                    moving=moving_image,
+                                    type_of_transform=registration_type, 
+                                    verbose  = False,
+                                    outprefix = outprefix,
+                                    **ants_kwargs
+                                )
+            return rr['warpedmovout'].numpy().astype(np.int16).transpose((2,1,0))
+        
+        def _register_batch(batch, template, spacing, registration_type, outprefix = None):
+            corrected = []
+            for volume in batch:
+                # load the volume
+                volume_img = self.experiment.load_volumes([volume], verbose=False)[0]
+                # register
+                volume_img = _register(volume_img, template, spacing, registration_type, 
+                                       outprefix = outprefix)
+                corrected.append(volume_img)
+            corrected = np.array(corrected)
+            return corrected
+
+        # prepare list of volumes to register
+        n_full_volumes = self.experiment.n_full_volumes
+        if volumes is not None:
+            volumes = np.array(volumes)
+            assert volumes.max() < n_full_volumes,\
+                  f"Some volumes are outside of the experiment with {n_full_volumes} full volumes" 
+            assert volumes.min() >= 0, "volumes must be positive integers"
+            n_reguested_volumes = len(volumes)
+        else:
+            volumes = np.arange(n_full_volumes)
+            n_reguested_volumes = n_full_volumes
+
+        # if template is not an array, get template volume
+        if isinstance(template, int):
+            assert template < n_full_volumes, f"Template frame {template} is outside of the experiment with {n_full_volumes} full volumes"
+            assert template >= 0, "Template frame must be a positive integer"
+            template = self.experiment.load_volumes([template], verbose=False)[0]
+        # turn template into ants image
+        template = ants.from_numpy(np.transpose(template.astype(float), axes=[2,1,0]), 
+                                    spacing=spacing_xyz) # spacing in xyz order
+        
+        # if mask and moving_mask are in ants_kwargs, convert them to ants images
+        # and if they are string or pthlib.Path, load them as numpy arrays first
+        if 'mask' in ants_kwargs:
+            if isinstance(ants_kwargs['mask'], str) or isinstance(ants_kwargs['mask'], Path):
+                ants_kwargs['mask'] = ants.from_numpy(np.transpose(imread(ants_kwargs['mask']).astype(float), axes=[2,1,0]), 
+                                    spacing=spacing_xyz)
+            elif isinstance(ants_kwargs['mask'], np.ndarray):
+                ants_kwargs['mask'] = ants.from_numpy(np.transpose(ants_kwargs['mask'].astype(float), axes=[2,1,0]), 
+                                    spacing=spacing_xyz)
+
+        if 'moving_mask' in ants_kwargs:
+            if isinstance(ants_kwargs['moving_mask'], str) or isinstance(ants_kwargs['moving_mask'], Path):
+                ants_kwargs['moving_mask'] = ants.from_numpy(np.transpose(imread(ants_kwargs['moving_mask']).astype(float), axes=[2,1,0]), 
+                                    spacing=spacing_xyz)
+            elif isinstance(ants_kwargs['moving_mask'], np.ndarray):
+                ants_kwargs['moving_mask'] = ants.from_numpy(np.transpose(ants_kwargs['moving_mask'].astype(float), axes=[2,1,0]), 
+                                    spacing=spacing_xyz)
+        
+        # load in batches and process volume by volume
+        chunks = self.experiment.batch_volumes(batch_size, volumes= volumes, full_only=True)
+        # create a directory for the transforms
+        os.makedirs(f'{save_dir}/transforms', exist_ok=True)
+
+        tot_volumes = 0
+        for ichunk, chunk in enumerate(chunks):
+            # register the chunk
+            outprefix = f'{save_dir}/transforms/volume_{chunk[0]:04d}'
+            corrected = _register_batch(chunk, template, spacing_xyz, registration_type,
+                                        outprefix = outprefix)
+            # save 
+            nt, z, y, x = corrected.shape
+            imwrite(f'{save_dir}/drift_corrected_movie_{ichunk:04d}.tif',
+                    corrected.astype(np.int16), shape=(nt, z, y, x),
+                    metadata={'axes': 'TZYX'}, imagej=True)
+            if verbose:
+                tot_volumes = tot_volumes + nt
+                print(f"written volumes : {tot_volumes}, out of {n_reguested_volumes} requested volumes")
+
+
+    def batch_dff_sliding_window(self, save_dir, batch_size, window_size, blur_sigma=None, verbose=False):
         """
-        Creates 3D dff movie from raw 3D movie. Will only use full_volumes,
+        Creates 3D dff movie from raw 3D movie using sliding window. Will only use full_volumes,
         so the number of frames in the resulting movie can be smaller than in the original.
 
         :param blur_sigma: If not None, will apply gaussian blur in 3D with sigma = blur_sigma.
                          Can be int - then the same sigma in all 3 directions is applied,
                          or list [sz,sy,sx] for different sigma in ZYX.
         :type blur_sigma: Union(int, list)
         :param save_dir: directory into which to save the dff movie in chunks
@@ -742,10 +913,89 @@
 
             if verbose:
                 print(f"written frames : {chunk[start_tp]} - {chunk[end_tp - 1]}, out of {n_volumes}")
             # exit cycle the first chunk you saw the end of the experiment
             if chunk[-1] == (n_volumes - 1):
                 break
 
+    def calculate_dff(self, save_dir, batch_size, step_size, baseline_volumes,
+                      resolution_xyz = [1, 1, 1], blur_sigma=None, 
+                      verbose=False, save_baseline=False):
+        """
+        Creates 3D dff movie from raw 3D movie by processing movie in steps. Will only use full_volumes,
+        so the number of frames in the resulting movie can be smaller than in the original.
+
+        Args:
+            blur_sigma (Union(int, list)): If not None, will apply gaussian blur in 3D with sigma = blur_sigma.
+                            Can be int - then the same sigma in all 3 directions is applied,
+                            or list [sz,sy,sx] for different sigma in ZYX.
+            save_dir (str): directory into which to save the dff movie in chunks
+            batch_size (int): number of volumes to load at once, must be multiple of step_size
+            step_size (int): the size of the sliding window for the baseline estimation in volumes
+            baseline_volumes (List[int]): volumes inside each step to use for baseline estimation
+            resolution_xyz (List[int]): resolution in xyz order in um
+            verbose (bool): whether to print the volumes that have been processed so far on the screen.
+        """
+        # TODO : make the size & digit estimation
+        # TODO : write resolution into metadata
+
+        assert batch_size % step_size == 0, "batch_size must be multiple of step_size"
+
+        if save_baseline:
+            #create directory for baseline
+            os.makedirs(f'{save_dir}/baseline', exist_ok=True)
+
+        # will only use full volumes
+        volume_list = self.experiment.list_volumes()
+        volume_list = volume_list[volume_list >= 0]
+        n_volumes = len(volume_list)
+
+        # will multiply dff image by this value for better visualisation later
+        SCALE = 1000
+
+        #create chunks
+        chunks = self.experiment.batch_volumes(batch_size, volumes=volume_list, full_only=True)
+
+        for ich, chunk in enumerate(tqdm(chunks, disable=verbose)):
+
+            data = self.experiment.load_volumes(chunk, verbose=False)
+            # add 1 to all pixels to aviod division by zero
+            data = data + 1
+
+            if blur_sigma is not None:
+                data = gaussian_filter(data, blur_sigma)
+            dff_img, baseline_img = get_dff_in_steps(data, step_size, baseline_volumes)
+            t, z, y, x = dff_img.shape
+
+            # special case of the last chunk --> need to output the tail as well, and then break
+            if chunk[-1] == (n_volumes - 1):
+                end_tp = t
+            # special case of the first chunk --> need to output the head as well
+            if ich == 0:
+                start_tp = 0
+
+            # make sure the output fits into the int16 range:
+            min_value = dff_img.min()
+            max_value = dff_img.max()
+            if max_value * SCALE > 32767 or min_value * SCALE < -32768:
+                warnings.warn(f"Scaled DFF values outside the int16 range for scale = {SCALE},"
+                              f" min: {min_value}, max: {max_value}")
+            # write dff image
+            imwrite(f'{save_dir}/dff_movie_{ich:04d}.tif', (dff_img * SCALE).astype(np.int16), shape=(t, z, y, x),
+                    resolution=(1./resolution_xyz[0], 1./resolution_xyz[1]), metadata={'spacing': resolution_xyz[2], 'unit': 'um','axes': 'TZYX'}, 
+                    imagej=True)
+            if save_baseline:
+                # print(f"Baseline shape{baseline_img.shape}")
+                # write baseline image
+                imwrite(f'{save_dir}/baseline/baseline_movie_{ich:04d}.tif', baseline_img.astype(np.int16), shape=(t, z, y, x),
+                        resolution=(1./resolution_xyz[0], 1./resolution_xyz[1]), metadata={'spacing': resolution_xyz[2], 'unit': 'um','axes': 'TZYX'}, 
+                        imagej=True)
+
+            if verbose:
+                print(f"written frames : {chunk[0]} - {chunk[- 1]}, out of {n_volumes}")
+            # exit cycle the first chunk you saw the end of the experiment
+            if chunk[-1] == (n_volumes - 1):
+                break
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `numan-1.0.4/src/numan/notifications.py` & `numan-1.0.6/src/numan/notifications.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/src/numan/plots.py` & `numan-1.0.6/src/numan/plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/src/numan/project.py` & `numan-1.0.6/src/numan/project.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/src/numan/report.py` & `numan-1.0.6/src/numan/report.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/src/numan/runner.py` & `numan-1.0.6/src/numan/runner.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/src/numan/utils.py` & `numan-1.0.6/src/numan/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,35 +51,72 @@
     baseline = np.zeros(array.shape)
     baseline[0:start] = mean_signal[0]
     baseline[start:end] = mean_signal
     baseline[end:] = mean_signal[-1]
 
     return baseline, start, end
 
+def check_baseline_not_zero(baseline):
+    """
+    Checks if baseline is zero, if so, sets it to 10^(-6)
+    """
+    b_zero = baseline == 0
+    if np.sum(b_zero) > 0:
+        warnings.warn(f"{np.sum(b_zero)} baseline values are zero.\n"
+                      f"Setting these values to 10^(-6) to avoid dividing by zero.")
+        baseline[b_zero] = 10 ^ (-6)
+
+    return baseline
+
 
 def get_dff(array, window_size):
     """
-    subtracts average baseline from an ND array along the 0 dimention.
+    subtracts 8th percentile baseline from an ND array along the 0 dimention.
     window_size must be an odd number.
 
     The baseline for the first and the last window//2 elements is the same :
     the first or the last value calculated with the full window
     """
     percentile = 8  # 8th percentile
     baseline, start, end = get_baseline(array, window_size, percentile)
 
     # not to divide by zero:
-    b_zero = baseline == 0
-    if np.sum(b_zero) > 0:
-        warnings.warn(f"{np.sum(b_zero)} baseline values are zero.\n"
-                      f"Setting these values to 10^(-6) to avoid dividing by zero.")
-        baseline[b_zero] = 10 ^ (-6)
+    baseline = check_baseline_not_zero(baseline)
 
     return (array - baseline) / baseline, start, end
 
+def get_dff_in_steps(array, step_size, baseline_volumes):
+    """
+    Subtracts baseline calculated for each step from an ND array along the 0 dimention and divides by baseline.
+
+    Args:
+        array (NumpyArray): 4D array (TZYX) to calculate dff for
+        step_size (int): number of volumes to correct for a single baseline
+        baseline_volumes (List[int]): number of volumes to average for baseline inside each step, 
+            for example [0,1,2] will  average the first 3 volumes inside each step to calculate baseline.
+    """
+    #split array into steps of step_size volumes each
+    n_crops = array.shape[0]//step_size
+
+    #calculate baseline for each step
+    baseline = np.zeros(array.shape)
+    for i in range(n_crops):
+        from_idx = i*step_size
+        to_idx = (i+1)*step_size
+        baseline[from_idx:to_idx] = np.mean(array[from_idx:to_idx][baseline_volumes], axis=0)
+    # not to divide by zero:
+    baseline = check_baseline_not_zero(baseline)
+
+    return (array - baseline) / baseline, baseline
+
+
+
+    
+
+
 
 def get_t_score(movie1, movie2, absolute=True):
     """
     Returns absolute t-score image ( 2D or 3D, depending on input),
     for t-score calculations see for example :
     https://www.jmp.com/en_us/statistics-knowledge-portal/t-test/two-sample-t-test.html
     """
```

### Comparing `numan-1.0.4/src/numan/visualization.py` & `numan-1.0.6/src/numan/visualization.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/src/numan.egg-info/PKG-INFO` & `numan-1.0.6/src/numan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numan
-Version: 1.0.4
+Version: 1.0.6
 Summary: numerosity analysis package
 Author-email: Anna Nadtochiy <nadtochi@usc.edu>
 Project-URL: Homepage, https://github.com/LemonJust/numan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numan-1.0.4/tests/test_plots.py` & `numan-1.0.6/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/tests/test_plots_cp13.py` & `numan-1.0.6/tests/test_plots_cp13.py`

 * *Files identical despite different names*

### Comparing `numan-1.0.4/tests/test_utils.py` & `numan-1.0.6/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,7 +32,28 @@
 
         sigma = 1
         three_first_volumes = gaussian_filter(three_first_volumes, sigma)
         # write blurred image
         imwrite(f'{self.save_dir}/three_volumes_blurred.tif',
                 three_first_volumes.astype(np.uint16), shape=(3, 52, 468, 500),
                 metadata={'axes': 'TZYX'}, imagej=True)
+
+class TestGetDffInSteps(unittest.TestCase):
+    array = np.ones((10, 2, 2))
+    array[:, 0, 0] = [2, 2, 4, 2, 2, 3, 3, 6, 3, 3]
+    step_size = 5
+    baseline_volumes = [0, 1]
+
+    def test_get_dff_in_steps(self):
+        dff, baseline = get_dff_in_steps(self.array, self.step_size, self.baseline_volumes)
+
+        true_baseline = np.ones((10, 2, 2))
+        true_baseline[:, 0, 0] = [2, 2, 2, 2, 2, 3, 3, 3, 3, 3]
+
+        true_dff = np.zeros((10, 2, 2))
+        true_dff[:, 0, 0] = [0, 0, 1, 0, 0, 0, 0, 1, 0, 0]
+
+        assert np.array_equal(baseline, true_baseline)
+        assert np.array_equal(dff, true_dff)
+
+if __name__ == '__main__':
+    unittest.main()
```

