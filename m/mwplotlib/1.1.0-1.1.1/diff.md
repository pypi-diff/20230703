# Comparing `tmp/mwplotlib-1.1.0.tar.gz` & `tmp/mwplotlib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwplotlib-1.1.0.tar", last modified: Mon Jul  3 04:17:10 2023, max compression
+gzip compressed data, was "mwplotlib-1.1.1.tar", last modified: Mon Jul  3 05:10:24 2023, max compression
```

## Comparing `mwplotlib-1.1.0.tar` & `mwplotlib-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.361210 mwplotlib-1.1.0/
--rw-r--r--   0 wenky      (501) staff       (20)     1066 2023-06-27 18:04:42.000000 mwplotlib-1.1.0/LICENSE
--rw-r--r--   0 wenky      (501) staff       (20)     2644 2023-07-03 04:17:10.361044 mwplotlib-1.1.0/PKG-INFO
--rw-r--r--   0 wenky      (501) staff       (20)     2395 2023-07-03 03:27:51.000000 mwplotlib-1.1.0/README.md
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.359885 mwplotlib-1.1.0/mwplotlib/
--rw-r--r--   0 wenky      (501) staff       (20)       51 2023-06-25 07:35:02.000000 mwplotlib-1.1.0/mwplotlib/__init__.py
--rw-r--r--   0 wenky      (501) staff       (20)     5068 2023-06-27 18:08:59.000000 mwplotlib-1.1.0/mwplotlib/arms_data.py
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.360852 mwplotlib-1.1.0/mwplotlib/data/
--rw-r--r--   0 wenky      (501) staff       (20)    32784 2023-06-25 04:47:07.000000 mwplotlib-1.1.0/mwplotlib/data/apjacc45ct1_mrt.txt
--rw-r--r--   0 wenky      (501) staff       (20)     1306 2023-06-26 11:18:19.000000 mwplotlib-1.1.0/mwplotlib/data/apjacc45ct2_ascii.txt
--rw-r--r--   0 wenky      (501) staff       (20)    12743 2023-07-03 03:24:04.000000 mwplotlib-1.1.0/mwplotlib/spiral_arms.py
--rw-r--r--   0 wenky      (501) staff       (20)     1454 2023-06-27 16:45:14.000000 mwplotlib-1.1.0/mwplotlib/utilities.py
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.360543 mwplotlib-1.1.0/mwplotlib.egg-info/
--rw-r--r--   0 wenky      (501) staff       (20)     2644 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/PKG-INFO
--rw-r--r--   0 wenky      (501) staff       (20)      355 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 wenky      (501) staff       (20)        1 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 wenky      (501) staff       (20)       32 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/requires.txt
--rw-r--r--   0 wenky      (501) staff       (20)       10 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/top_level.txt
--rw-r--r--   0 wenky      (501) staff       (20)       38 2023-07-03 04:17:10.361262 mwplotlib-1.1.0/setup.cfg
--rw-r--r--   0 wenky      (501) staff       (20)      652 2023-07-03 04:16:46.000000 mwplotlib-1.1.0/setup.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:10:24.303449 mwplotlib-1.1.1/
+-rw-r--r--   0 wenky      (501) staff       (20)     1066 2023-06-27 18:04:42.000000 mwplotlib-1.1.1/LICENSE
+-rw-r--r--   0 wenky      (501) staff       (20)     2761 2023-07-03 05:10:24.303250 mwplotlib-1.1.1/PKG-INFO
+-rw-r--r--   0 wenky      (501) staff       (20)     2512 2023-07-03 04:22:21.000000 mwplotlib-1.1.1/README.md
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:10:24.300136 mwplotlib-1.1.1/mwplotlib/
+-rw-r--r--   0 wenky      (501) staff       (20)       51 2023-06-25 07:35:02.000000 mwplotlib-1.1.1/mwplotlib/__init__.py
+-rw-r--r--   0 wenky      (501) staff       (20)     5068 2023-06-27 18:08:59.000000 mwplotlib-1.1.1/mwplotlib/arms_data.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:10:24.302513 mwplotlib-1.1.1/mwplotlib/data/
+-rw-r--r--   0 wenky      (501) staff       (20)    32784 2023-06-25 04:47:07.000000 mwplotlib-1.1.1/mwplotlib/data/apjacc45ct1_mrt.txt
+-rw-r--r--   0 wenky      (501) staff       (20)     1306 2023-06-26 11:18:19.000000 mwplotlib-1.1.1/mwplotlib/data/apjacc45ct2_ascii.txt
+-rw-r--r--   0 wenky      (501) staff       (20)    13059 2023-07-03 04:54:14.000000 mwplotlib-1.1.1/mwplotlib/spiral_arms.py
+-rw-r--r--   0 wenky      (501) staff       (20)     1454 2023-06-27 16:45:14.000000 mwplotlib-1.1.1/mwplotlib/utilities.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:10:24.301484 mwplotlib-1.1.1/mwplotlib.egg-info/
+-rw-r--r--   0 wenky      (501) staff       (20)     2761 2023-07-03 05:10:24.000000 mwplotlib-1.1.1/mwplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 wenky      (501) staff       (20)      355 2023-07-03 05:10:24.000000 mwplotlib-1.1.1/mwplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 wenky      (501) staff       (20)        1 2023-07-03 05:10:24.000000 mwplotlib-1.1.1/mwplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       32 2023-07-03 05:10:24.000000 mwplotlib-1.1.1/mwplotlib.egg-info/requires.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       10 2023-07-03 05:10:24.000000 mwplotlib-1.1.1/mwplotlib.egg-info/top_level.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       38 2023-07-03 05:10:24.303510 mwplotlib-1.1.1/setup.cfg
+-rw-r--r--   0 wenky      (501) staff       (20)      652 2023-07-03 05:09:35.000000 mwplotlib-1.1.1/setup.py
```

### Comparing `mwplotlib-1.1.0/LICENSE` & `mwplotlib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.0/PKG-INFO` & `mwplotlib-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwplotlib
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Milky Way Plotting Library
 Home-page: https://github.com/xiawenke/mwplotlib
 Author: Wenky
 Author-email: wxia1@fandm.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,15 +35,17 @@
 plt.MilkyWay.shape(plot_type="cartesian", style="region")
 
 # Plot the Milky Way in Cartesian coordinates (line-style)
 plt.figure(figsize=(9, 9))
 plt.MilkyWay.shape(plot_type="cartesian", style="line")
 ```
 
-For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on [Google Colab](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing). 
+For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on Google Colab:
+ - [v1.1.0 (Latest)](https://colab.research.google.com/drive/1Jk6WsD9TVHMwbThDjm192cEQLWn4qpbz?usp=sharing)
+ - [v1.0.0](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing)
 
 # Reference
 <!-- Citation Y. Xu et al 2023 ApJ 947 54 -->
 <!-- https://iopscience.iop.org/article/10.3847/1538-4357/acc45c -->
 The galaxy model and data used in this package is based on the following paper:
 ```Latex
 @ARTICLE{2023ApJ...947...54X,
```

### Comparing `mwplotlib-1.1.0/README.md` & `mwplotlib-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 plt.MilkyWay.shape(plot_type="cartesian", style="region")
 
 # Plot the Milky Way in Cartesian coordinates (line-style)
 plt.figure(figsize=(9, 9))
 plt.MilkyWay.shape(plot_type="cartesian", style="line")
 ```
 
-For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on [Google Colab](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing). 
+For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on Google Colab:
+ - [v1.1.0 (Latest)](https://colab.research.google.com/drive/1Jk6WsD9TVHMwbThDjm192cEQLWn4qpbz?usp=sharing)
+ - [v1.0.0](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing)
 
 # Reference
 <!-- Citation Y. Xu et al 2023 ApJ 947 54 -->
 <!-- https://iopscience.iop.org/article/10.3847/1538-4357/acc45c -->
 The galaxy model and data used in this package is based on the following paper:
 ```Latex
 @ARTICLE{2023ApJ...947...54X,
```

### Comparing `mwplotlib-1.1.0/mwplotlib/arms_data.py` & `mwplotlib-1.1.1/mwplotlib/arms_data.py`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.0/mwplotlib/data/apjacc45ct1_mrt.txt` & `mwplotlib-1.1.1/mwplotlib/data/apjacc45ct1_mrt.txt`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.0/mwplotlib/data/apjacc45ct2_ascii.txt` & `mwplotlib-1.1.1/mwplotlib/data/apjacc45ct2_ascii.txt`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.0/mwplotlib/spiral_arms.py` & `mwplotlib-1.1.1/mwplotlib/spiral_arms.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             plotData["color"].append(color_codes[plotData["arm"][i]])
         
         # print(plotData["color"])
         self.plt.scatter(plotData["x"], plotData["y"], s=1, c=plotData["color"])
         # plt.show()
         # input()
 
-    def shape(self, unit="kpc", style="region", step=.001, plot_type="polar", config={}, legend=True, **kwargs):
+    def shape(self, unit="kpc", style="region", step=.001, plot_type="polar", config={}, legend=True, offsets=[0, 0], **kwargs):
         """
         config in the form of:
         {
             "Outer": {
                 "color": "red", 
                 "lw": 1,
                 ... # Matplotlib kwargs
@@ -152,32 +152,32 @@
             
             if(plot_type == "polar"):
                 if(thisRow['Spiral Arm'] != lastArm) :
                     # self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", label=thisRow['Spiral Arm'])
                     # self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", label=thisRow['Spiral Arm'], color=self._get_last_color())
                     # Allow for custom kwargs:
                     if(style == "region"):
-                        self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", **thisKwargs)
-                        self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", color=self._get_last_color(), **self._kwargs_no_color(thisKwargs))
+                        self.plt.plot(thisBetaRange + offsets[0], thisRRange + offsets[1] + thisArmWidth / 2, "--", **thisKwargs)
+                        self.plt.plot(thisBetaRange + offsets[0], thisRRange + offsets[1] - thisArmWidth / 2, "--", color=self._get_last_color(), **self._kwargs_no_color(thisKwargs))
                     elif(style == "line"):
-                        self.plt.plot(thisBetaRange, thisRRange, "--", **thisKwargs)
+                        self.plt.plot(thisBetaRange + offsets[0], thisRRange + offsets[1], "--", **thisKwargs)
                     else:
                         print("Invalid style")
                         return
                 else:
                     # print(thisRow['Spiral Arm'])
                     if(style == "region"):
-                        self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", 
+                        self.plt.plot(thisBetaRange + offsets[0], thisRRange + offsets[1] + thisArmWidth / 2, "--", 
                             color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
-                        self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", 
+                        self.plt.plot(thisBetaRange + offsets[0], thisRRange + offsets[1] - thisArmWidth / 2, "--", 
                             color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     elif(style == "line"):
-                        self.plt.plot(thisBetaRange, thisRRange, "--", 
+                        self.plt.plot(thisBetaRange + offsets[0], thisRRange + offsets[1], "--", 
                             color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     else:
                         print("Invalid style")
                         return
 
                 # self.plt.show()
@@ -190,32 +190,32 @@
                 thisX_regionLower = (thisRRange - thisArmWidth / 2) * np.cos(thisBetaRange)
                 thisY_regionLower = (thisRRange - thisArmWidth / 2) * np.sin(thisBetaRange)
                 if(thisRow['Spiral Arm'] != lastArm) :
                     # self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", label=thisRow['Spiral Arm'])
                     # self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", label=thisRow['Spiral Arm'], color=self._get_last_color())
                     # Allow for custom kwargs:
                     if(style == "region"):
-                        self.plt.plot(thisX_regionUpper, thisY_regionUpper, "--", **thisKwargs)
-                        self.plt.plot(thisX_regionLower, thisY_regionLower, "--", color=self._get_last_color(), **self._kwargs_no_color(thisKwargs))
+                        self.plt.plot(thisX_regionUpper + offsets[0], thisY_regionUpper + offsets[1], "--", **thisKwargs)
+                        self.plt.plot(thisX_regionLower + offsets[0], thisY_regionLower + offsets[1], "--", color=self._get_last_color(), **self._kwargs_no_color(thisKwargs))
                     elif(style == "line"):
-                        self.plt.plot(thisX, thisY, "--", **thisKwargs)
+                        self.plt.plot(thisX + offsets[0], thisY + offsets[1], "--", **thisKwargs)
                     else:
                         print("Invalid style")
                         return
                 else:
                     # print(thisRow['Spiral Arm'])
                     if(style == "region"):
-                        self.plt.plot(thisX_regionUpper, thisY_regionUpper, "--", 
+                        self.plt.plot(thisX_regionUpper + offsets[0], thisY_regionUpper + offsets[1], "--", 
                             color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
-                        self.plt.plot(thisX_regionLower, thisY_regionLower, "--", 
+                        self.plt.plot(thisX_regionLower + offsets[0], thisY_regionLower + offsets[1], "--", 
                             color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     elif(style == "line"):
-                        self.plt.plot(thisX, thisY, "--", 
+                        self.plt.plot(thisX + offsets[0], thisY + offsets[1], "--", 
                             color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     else:
                         print("Invalid style")
                         return
             else:
                 print("Invalid plot type")
@@ -252,14 +252,14 @@
         # Remove color from kwargs
         if('color' in kwargs):
             kwargs.pop('color')
         
         # remove label from kwargs
         if('label' in kwargs):
             kwargs.pop('label')
-            
+
         return kwargs
             
 class MilkyWay():
     def mw_plt(plt):
         plt.MilkyWay = MilkyWayHandler(plt)
         return plt
```

### Comparing `mwplotlib-1.1.0/mwplotlib/utilities.py` & `mwplotlib-1.1.1/mwplotlib/utilities.py`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.0/mwplotlib.egg-info/PKG-INFO` & `mwplotlib-1.1.1/mwplotlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwplotlib
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Milky Way Plotting Library
 Home-page: https://github.com/xiawenke/mwplotlib
 Author: Wenky
 Author-email: wxia1@fandm.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,15 +35,17 @@
 plt.MilkyWay.shape(plot_type="cartesian", style="region")
 
 # Plot the Milky Way in Cartesian coordinates (line-style)
 plt.figure(figsize=(9, 9))
 plt.MilkyWay.shape(plot_type="cartesian", style="line")
 ```
 
-For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on [Google Colab](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing). 
+For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on Google Colab:
+ - [v1.1.0 (Latest)](https://colab.research.google.com/drive/1Jk6WsD9TVHMwbThDjm192cEQLWn4qpbz?usp=sharing)
+ - [v1.0.0](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing)
 
 # Reference
 <!-- Citation Y. Xu et al 2023 ApJ 947 54 -->
 <!-- https://iopscience.iop.org/article/10.3847/1538-4357/acc45c -->
 The galaxy model and data used in this package is based on the following paper:
 ```Latex
 @ARTICLE{2023ApJ...947...54X,
```

### Comparing `mwplotlib-1.1.0/setup.py` & `mwplotlib-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwplotlib",
-    version="1.1.0",
+    version="1.1.1",
     author="Wenky",
     author_email="wxia1@fandm.edu",
     description="The Milky Way Plotting Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xiawenke/mwplotlib",
     packages=setuptools.find_packages(),
```

