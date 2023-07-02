# Comparing `tmp/torchshow-0.5.0.tar.gz` & `tmp/torchshow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchshow-0.5.0.tar", last modified: Mon Nov  7 23:30:05 2022, max compression
+gzip compressed data, was "torchshow-0.5.1.tar", last modified: Sun Jul  2 22:13:18 2023, max compression
```

## Comparing `torchshow-0.5.0.tar` & `torchshow-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 xiaowen    (501) staff       (20)        0 2022-11-07 23:30:05.710003 torchshow-0.5.0/
--rw-r--r--   0 xiaowen    (501) staff       (20)     1072 2022-11-06 04:28:03.000000 torchshow-0.5.0/LICENSE
--rw-r--r--   0 xiaowen    (501) staff       (20)     9643 2022-11-07 23:30:05.709825 torchshow-0.5.0/PKG-INFO
--rw-r--r--   0 xiaowen    (501) staff       (20)     9184 2022-11-07 23:16:16.000000 torchshow-0.5.0/README.md
--rw-r--r--   0 xiaowen    (501) staff       (20)       38 2022-11-07 23:30:05.710052 torchshow-0.5.0/setup.cfg
--rw-r--r--   0 xiaowen    (501) staff       (20)      787 2022-11-07 23:28:36.000000 torchshow-0.5.0/setup.py
-drwxr-xr-x   0 xiaowen    (501) staff       (20)        0 2022-11-07 23:30:05.708929 torchshow-0.5.0/torchshow/
--rw-r--r--   0 xiaowen    (501) staff       (20)      136 2022-11-07 23:12:41.000000 torchshow-0.5.0/torchshow/__init__.py
--rw-r--r--   0 xiaowen    (501) staff       (20)     1023 2022-11-06 04:28:03.000000 torchshow-0.5.0/torchshow/config.py
--rw-r--r--   0 xiaowen    (501) staff       (20)     4219 2022-11-06 04:28:03.000000 torchshow-0.5.0/torchshow/flow.py
--rw-r--r--   0 xiaowen    (501) staff       (20)     7830 2022-11-07 23:12:41.000000 torchshow-0.5.0/torchshow/torchshow.py
--rw-r--r--   0 xiaowen    (501) staff       (20)     5539 2022-11-07 23:12:41.000000 torchshow-0.5.0/torchshow/utils.py
--rw-r--r--   0 xiaowen    (501) staff       (20)    14171 2022-11-07 23:12:41.000000 torchshow-0.5.0/torchshow/visualization.py
-drwxr-xr-x   0 xiaowen    (501) staff       (20)        0 2022-11-07 23:30:05.709684 torchshow-0.5.0/torchshow.egg-info/
--rw-r--r--   0 xiaowen    (501) staff       (20)     9643 2022-11-07 23:30:05.000000 torchshow-0.5.0/torchshow.egg-info/PKG-INFO
--rw-r--r--   0 xiaowen    (501) staff       (20)      319 2022-11-07 23:30:05.000000 torchshow-0.5.0/torchshow.egg-info/SOURCES.txt
--rw-r--r--   0 xiaowen    (501) staff       (20)        1 2022-11-07 23:30:05.000000 torchshow-0.5.0/torchshow.egg-info/dependency_links.txt
--rw-r--r--   0 xiaowen    (501) staff       (20)       17 2022-11-07 23:30:05.000000 torchshow-0.5.0/torchshow.egg-info/requires.txt
--rw-r--r--   0 xiaowen    (501) staff       (20)       10 2022-11-07 23:30:05.000000 torchshow-0.5.0/torchshow.egg-info/top_level.txt
+drwxr-xr-x   0 xiaowen    (501) staff       (20)        0 2023-07-02 22:13:18.509564 torchshow-0.5.1/
+-rw-r--r--   0 xiaowen    (501) staff       (20)     1072 2022-11-06 04:28:03.000000 torchshow-0.5.1/LICENSE
+-rw-r--r--   0 xiaowen    (501) staff       (20)     9524 2023-07-02 22:13:18.509373 torchshow-0.5.1/PKG-INFO
+-rw-r--r--   0 xiaowen    (501) staff       (20)     9065 2023-07-02 22:12:09.000000 torchshow-0.5.1/README.md
+-rw-r--r--   0 xiaowen    (501) staff       (20)       38 2023-07-02 22:13:18.509604 torchshow-0.5.1/setup.cfg
+-rw-r--r--   0 xiaowen    (501) staff       (20)      787 2023-07-02 19:14:17.000000 torchshow-0.5.1/setup.py
+drwxr-xr-x   0 xiaowen    (501) staff       (20)        0 2023-07-02 22:13:18.506841 torchshow-0.5.1/tests/
+-rw-r--r--   0 xiaowen    (501) staff       (20)    10253 2023-07-02 06:10:51.000000 torchshow-0.5.1/tests/tests.py
+drwxr-xr-x   0 xiaowen    (501) staff       (20)        0 2023-07-02 22:13:18.508379 torchshow-0.5.1/torchshow/
+-rw-r--r--   0 xiaowen    (501) staff       (20)      136 2022-11-07 23:12:41.000000 torchshow-0.5.1/torchshow/__init__.py
+-rw-r--r--   0 xiaowen    (501) staff       (20)     1023 2022-11-06 04:28:03.000000 torchshow-0.5.1/torchshow/config.py
+-rw-r--r--   0 xiaowen    (501) staff       (20)     4219 2022-11-06 04:28:03.000000 torchshow-0.5.1/torchshow/flow.py
+-rw-r--r--   0 xiaowen    (501) staff       (20)     9100 2023-06-06 06:33:43.000000 torchshow-0.5.1/torchshow/torchshow.py
+-rw-r--r--   0 xiaowen    (501) staff       (20)     5616 2023-06-06 06:33:43.000000 torchshow-0.5.1/torchshow/utils.py
+-rw-r--r--   0 xiaowen    (501) staff       (20)    14411 2023-07-02 06:26:02.000000 torchshow-0.5.1/torchshow/visualization.py
+drwxr-xr-x   0 xiaowen    (501) staff       (20)        0 2023-07-02 22:13:18.509212 torchshow-0.5.1/torchshow.egg-info/
+-rw-r--r--   0 xiaowen    (501) staff       (20)     9524 2023-07-02 22:13:18.000000 torchshow-0.5.1/torchshow.egg-info/PKG-INFO
+-rw-r--r--   0 xiaowen    (501) staff       (20)      334 2023-07-02 22:13:18.000000 torchshow-0.5.1/torchshow.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaowen    (501) staff       (20)        1 2023-07-02 22:13:18.000000 torchshow-0.5.1/torchshow.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaowen    (501) staff       (20)       17 2023-07-02 22:13:18.000000 torchshow-0.5.1/torchshow.egg-info/requires.txt
+-rw-r--r--   0 xiaowen    (501) staff       (20)       10 2023-07-02 22:13:18.000000 torchshow-0.5.1/torchshow.egg-info/top_level.txt
```

### Comparing `torchshow-0.5.0/LICENSE` & `torchshow-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchshow-0.5.0/PKG-INFO` & `torchshow-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchshow
-Version: 0.5.0
+Version: 0.5.1
 Summary: Visualizing PyTorch tensors with a single line of code.
 Home-page: https://github.com/xwying/torchshow
 Author: Xiaowen Ying
 Author-email: shawnying.inbox@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,20 +37,18 @@
 - [x] Multiple Images
 - [x] Videos
 - [x] Multiple Videos
 - [x] Optical Flows (powered by [flow_vis](https://github.com/tomrunia/OpticalFlow_Visualization))
 
 
 
-## What's New in v0.5.0
-- Support specifying the color map for grayscale image. 
-- Support PIL Image.
-- Support filenames as input.
-- Addinng `ts.overlay()` API which can be used to blend multiple plots. See [examples](#12-overlay-visualizations).
-- Fix bugs when unnormalize with customize mean and std.
+## What's New in v0.5.1
+- Fix `np.int` depreciation issues.
+- Allow specifying `nrows` and `ncols` when visualizing a list of tensors.
+- Fix unexpected white spaces when saving figures.
 
 See the complete [changelogs](changelogs.md).
 
 
 ## Installation
 Install from [PyPI](https://pypi.org/project/torchshow/):
```

### Comparing `torchshow-0.5.0/README.md` & `torchshow-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,18 @@
 - [x] Multiple Images
 - [x] Videos
 - [x] Multiple Videos
 - [x] Optical Flows (powered by [flow_vis](https://github.com/tomrunia/OpticalFlow_Visualization))
 
 
 
-## What's New in v0.5.0
-- Support specifying the color map for grayscale image. 
-- Support PIL Image.
-- Support filenames as input.
-- Addinng `ts.overlay()` API which can be used to blend multiple plots. See [examples](#12-overlay-visualizations).
-- Fix bugs when unnormalize with customize mean and std.
+## What's New in v0.5.1
+- Fix `np.int` depreciation issues.
+- Allow specifying `nrows` and `ncols` when visualizing a list of tensors.
+- Fix unexpected white spaces when saving figures.
 
 See the complete [changelogs](changelogs.md).
 
 
 ## Installation
 Install from [PyPI](https://pypi.org/project/torchshow/):
```

### Comparing `torchshow-0.5.0/setup.py` & `torchshow-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="torchshow", # Replace with your own username
-    version="0.5.0",
+    version="0.5.1",
     author="Xiaowen Ying",
     author_email="shawnying.inbox@gmail.com",
     description="Visualizing PyTorch tensors with a single line of code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xwying/torchshow",
     packages=setuptools.find_packages(),
```

### Comparing `torchshow-0.5.0/torchshow/config.py` & `torchshow-0.5.1/torchshow/config.py`

 * *Files identical despite different names*

### Comparing `torchshow-0.5.0/torchshow/flow.py` & `torchshow-0.5.1/torchshow/flow.py`

 * *Files identical despite different names*

### Comparing `torchshow-0.5.0/torchshow/torchshow.py` & `torchshow-0.5.1/torchshow/torchshow.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,16 +64,25 @@
         elif x.ndim == 2: # (H, W)
             vis_list = [[x]]
             
         else:
             raise TypeError("Unsupported shape of numpy array {} .".format(x.shape))
         
     elif isinstance(x, list):
-        if isinstance(x[0], np.ndarray): # if the input is list of images [img1, img2], make it [[img1, img2]]
-            vis_list = [x]
+        if isinstance(x[0], np.ndarray): # if the input is list of images [img1, img2, ....]
+            nrows = kwargs.get('nrows', None)
+            ncols = kwargs.get('ncols', None)
+            if (nrows is not None) or (ncols is not None): # If user specified the grid layout
+                N = len(x)
+                # Here we assume either `nrows` or `ncols` must given so we do not have to specify H, W
+                nrows, ncols = calculate_grid_layout(N, None, None, nrows, ncols)
+                assert (nrows * ncols >= N)
+                vis_list = [list(x[i:i + ncols]) for i in range(0, N, ncols)] # vis_list is now a list of list
+            else:    
+                vis_list = [x] # Make it [[img1, img2, ...]] if `nrows` or `ncols` are not specified
         else:
             vis_list = x
 
     else:
         raise NotImplementedError("Does not support input type \"{}\"".format(type(x)))
 
 
@@ -107,16 +116,25 @@
     if isinstance(x, (np.ndarray)):
         x = x.copy()
         assert x.ndim in [3,4], "only support 3D array (N, H, W) or 4D array (N, C, H, W) in video mode"
         print(x.shape)
         video_list = [[x]] # for a single video, make it [[vid]]
         
     elif isinstance(x, list):
-        if isinstance(x[0], np.ndarray): # if the input is list of array [vid1, vid2], make it [[vid1, vid2]]
-            video_list = [x]
+        if isinstance(x[0], np.ndarray): # if the input is list of array [vid1, vid2, ...]
+            nrows = kwargs.get('nrows', None)
+            ncols = kwargs.get('ncols', None)
+            if (nrows is not None) or (ncols is not None): # If user specified the grid layout
+                N = len(x)
+                # Here we assume either `nrows` or `ncols` must given so we do not have to specify H, W.
+                nrows, ncols = calculate_grid_layout(N, None, None, nrows, ncols)
+                assert (nrows * ncols >= N)
+                video_list = [list(x[i:i + ncols]) for i in range(0, N, ncols)] # video_list is now a list of list
+            else:    
+                video_list = [x] # Make it [[vid1, vid2, ...]] if `nrows` or `ncols` are not specified
         else:
             video_list = x
             
     else:
         raise NotImplementedError("Does not support input type \"{}\"".format(type(x)))
```

### Comparing `torchshow-0.5.0/torchshow/utils.py` & `torchshow-0.5.1/torchshow/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     return (x.min() >= 0) and (x.max() <= 255)
 
 
 def calculate_grid_layout(N, img_H, img_W, nrow=None, ncol=None):
     """
     Function to calculate grid_layout
     """
-    if (nrow != None and ncol == None):
+    if (nrow != None): # `nrow` has higher priority than `ncol`.
         ncol = int(np.ceil(N / nrow))
-    elif (nrow == None and ncol != None):
+    elif (ncol != None):
         nrow = int(np.ceil(N / ncol))
-    else:
+    else: # If both nrow and ncols are not set, perform automatic calculation.
         N_sqrt = np.sqrt(N)
         if img_H >= img_W:
             nrow = int(np.floor(N_sqrt))
             ncol = int(np.ceil(N/nrow))
         else:
             ncol = int(np.floor(N_sqrt))
             nrow = int(np.ceil(N/ncol))
```

### Comparing `torchshow-0.5.0/torchshow/visualization.py` & `torchshow-0.5.1/torchshow/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,19 @@
             imshow(axes[i,j], vis, show_rich_info=show_rich_info)
             title_namespace["img_id"] = i*ncols+j
             title_namespace["img_id_from_1"] = title_namespace["img_id"] + 1
             title_namespace["row"] = i
             title_namespace["column"] = j
             if axes_title is not None:
                 axes[i, j].set_title(axes_title.format(**title_namespace))
+    
+    # Delete empty axes            
+    for ax in axes.ravel():
+        if not ax.has_data():
+            fig.delaxes(ax)
            
     if not show_axis:
         for ax in axes.ravel():
             ax.axis('off')
             
     if tight_layout:
         fig.tight_layout()
@@ -230,14 +235,19 @@
         for j, vis in enumerate(plots_per_row):
             if vis is not None:
                 plot = axes[i, j].imshow(vis['disp'], **vis['plot_cfg'])
                 plots.append(plot)
             else:
                 plots.append(None)
     
+    # Delete empty axes
+    for ax in axes.ravel():
+        if not ax.has_data():
+            fig.delaxes(ax)
+    
     if not show_axis:
         for ax in axes.ravel():
             ax.axis('off')
             
     if tight_layout:
         fig.tight_layout()            
     
@@ -412,19 +422,19 @@
         warnings.warn('Input has negative value when trying to visualize as categorical mask, which will all be converted to -1 and displayed in white.')
         x[x<0] = -1 # Map all negative value to -1
         color_list = np.concatenate([np.ones((1,4)).astype(np.float32), color_list], axis=0) # appending an extra value.
         N = N + 1
     
     cmap = colors.ListedColormap(color_list, N=N)
     
-    x = cmap(x.astype(np.int), alpha=None, bytes=True)[:,:,:3]
+    x = cmap(x.astype(int), alpha=None, bytes=True)[:,:,:3]
     # print(x.shape)
     plot_cfg = dict( interpolation="nearest")
     
     vis['disp'] = x
     vis['plot_cfg'] = plot_cfg
     vis['mode'] = 'Categorical'
     return vis
 
 
 if __name__ == "__main__":
-    print(create_color_map())
+    print(create_color_map())
```

### Comparing `torchshow-0.5.0/torchshow.egg-info/PKG-INFO` & `torchshow-0.5.1/torchshow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchshow
-Version: 0.5.0
+Version: 0.5.1
 Summary: Visualizing PyTorch tensors with a single line of code.
 Home-page: https://github.com/xwying/torchshow
 Author: Xiaowen Ying
 Author-email: shawnying.inbox@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,20 +37,18 @@
 - [x] Multiple Images
 - [x] Videos
 - [x] Multiple Videos
 - [x] Optical Flows (powered by [flow_vis](https://github.com/tomrunia/OpticalFlow_Visualization))
 
 
 
-## What's New in v0.5.0
-- Support specifying the color map for grayscale image. 
-- Support PIL Image.
-- Support filenames as input.
-- Addinng `ts.overlay()` API which can be used to blend multiple plots. See [examples](#12-overlay-visualizations).
-- Fix bugs when unnormalize with customize mean and std.
+## What's New in v0.5.1
+- Fix `np.int` depreciation issues.
+- Allow specifying `nrows` and `ncols` when visualizing a list of tensors.
+- Fix unexpected white spaces when saving figures.
 
 See the complete [changelogs](changelogs.md).
 
 
 ## Installation
 Install from [PyPI](https://pypi.org/project/torchshow/):
```

