# Comparing `tmp/mwplotlib-1.0.0.tar.gz` & `tmp/mwplotlib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwplotlib-1.0.0.tar", last modified: Tue Jun 27 18:19:00 2023, max compression
+gzip compressed data, was "mwplotlib-1.1.0.tar", last modified: Mon Jul  3 04:17:10 2023, max compression
```

## Comparing `mwplotlib-1.0.0.tar` & `mwplotlib-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-06-27 18:19:00.516916 mwplotlib-1.0.0/
--rw-r--r--   0 wenky      (501) staff       (20)     1066 2023-06-27 18:04:42.000000 mwplotlib-1.0.0/LICENSE
--rw-r--r--   0 wenky      (501) staff       (20)     2471 2023-06-27 18:19:00.516759 mwplotlib-1.0.0/PKG-INFO
--rw-r--r--   0 wenky      (501) staff       (20)     2221 2023-06-27 18:12:59.000000 mwplotlib-1.0.0/README.md
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-06-27 18:19:00.514642 mwplotlib-1.0.0/mwplotlib/
--rw-r--r--   0 wenky      (501) staff       (20)       51 2023-06-25 07:35:02.000000 mwplotlib-1.0.0/mwplotlib/__init__.py
--rw-r--r--   0 wenky      (501) staff       (20)     5068 2023-06-27 18:08:59.000000 mwplotlib-1.0.0/mwplotlib/arms_data.py
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-06-27 18:19:00.516338 mwplotlib-1.0.0/mwplotlib/data/
--rw-r--r--   0 wenky      (501) staff       (20)    32784 2023-06-25 04:47:07.000000 mwplotlib-1.0.0/mwplotlib/data/apjacc45ct1_mrt.txt
--rw-r--r--   0 wenky      (501) staff       (20)     1306 2023-06-26 11:18:19.000000 mwplotlib-1.0.0/mwplotlib/data/apjacc45ct2_ascii.txt
--rw-r--r--   0 wenky      (501) staff       (20)    11377 2023-06-27 18:10:55.000000 mwplotlib-1.0.0/mwplotlib/spiral_arms.py
--rw-r--r--   0 wenky      (501) staff       (20)     1454 2023-06-27 16:45:14.000000 mwplotlib-1.0.0/mwplotlib/utilities.py
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-06-27 18:19:00.515524 mwplotlib-1.0.0/mwplotlib.egg-info/
--rw-r--r--   0 wenky      (501) staff       (20)     2471 2023-06-27 18:19:00.000000 mwplotlib-1.0.0/mwplotlib.egg-info/PKG-INFO
--rw-r--r--   0 wenky      (501) staff       (20)      355 2023-06-27 18:19:00.000000 mwplotlib-1.0.0/mwplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 wenky      (501) staff       (20)        1 2023-06-27 18:19:00.000000 mwplotlib-1.0.0/mwplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 wenky      (501) staff       (20)       32 2023-06-27 18:19:00.000000 mwplotlib-1.0.0/mwplotlib.egg-info/requires.txt
--rw-r--r--   0 wenky      (501) staff       (20)       10 2023-06-27 18:19:00.000000 mwplotlib-1.0.0/mwplotlib.egg-info/top_level.txt
--rw-r--r--   0 wenky      (501) staff       (20)       38 2023-06-27 18:19:00.516970 mwplotlib-1.0.0/setup.cfg
--rw-r--r--   0 wenky      (501) staff       (20)      652 2023-06-27 17:51:36.000000 mwplotlib-1.0.0/setup.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.361210 mwplotlib-1.1.0/
+-rw-r--r--   0 wenky      (501) staff       (20)     1066 2023-06-27 18:04:42.000000 mwplotlib-1.1.0/LICENSE
+-rw-r--r--   0 wenky      (501) staff       (20)     2644 2023-07-03 04:17:10.361044 mwplotlib-1.1.0/PKG-INFO
+-rw-r--r--   0 wenky      (501) staff       (20)     2395 2023-07-03 03:27:51.000000 mwplotlib-1.1.0/README.md
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.359885 mwplotlib-1.1.0/mwplotlib/
+-rw-r--r--   0 wenky      (501) staff       (20)       51 2023-06-25 07:35:02.000000 mwplotlib-1.1.0/mwplotlib/__init__.py
+-rw-r--r--   0 wenky      (501) staff       (20)     5068 2023-06-27 18:08:59.000000 mwplotlib-1.1.0/mwplotlib/arms_data.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.360852 mwplotlib-1.1.0/mwplotlib/data/
+-rw-r--r--   0 wenky      (501) staff       (20)    32784 2023-06-25 04:47:07.000000 mwplotlib-1.1.0/mwplotlib/data/apjacc45ct1_mrt.txt
+-rw-r--r--   0 wenky      (501) staff       (20)     1306 2023-06-26 11:18:19.000000 mwplotlib-1.1.0/mwplotlib/data/apjacc45ct2_ascii.txt
+-rw-r--r--   0 wenky      (501) staff       (20)    12743 2023-07-03 03:24:04.000000 mwplotlib-1.1.0/mwplotlib/spiral_arms.py
+-rw-r--r--   0 wenky      (501) staff       (20)     1454 2023-06-27 16:45:14.000000 mwplotlib-1.1.0/mwplotlib/utilities.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 04:17:10.360543 mwplotlib-1.1.0/mwplotlib.egg-info/
+-rw-r--r--   0 wenky      (501) staff       (20)     2644 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 wenky      (501) staff       (20)      355 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 wenky      (501) staff       (20)        1 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       32 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/requires.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       10 2023-07-03 04:17:10.000000 mwplotlib-1.1.0/mwplotlib.egg-info/top_level.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       38 2023-07-03 04:17:10.361262 mwplotlib-1.1.0/setup.cfg
+-rw-r--r--   0 wenky      (501) staff       (20)      652 2023-07-03 04:16:46.000000 mwplotlib-1.1.0/setup.py
```

### Comparing `mwplotlib-1.0.0/LICENSE` & `mwplotlib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.0.0/PKG-INFO` & `mwplotlib-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwplotlib
-Version: 1.0.0
+Version: 1.1.0
 Summary: The Milky Way Plotting Library
 Home-page: https://github.com/xiawenke/mwplotlib
 Author: Wenky
 Author-email: wxia1@fandm.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,20 +35,20 @@
 plt.MilkyWay.shape(plot_type="cartesian", style="region")
 
 # Plot the Milky Way in Cartesian coordinates (line-style)
 plt.figure(figsize=(9, 9))
 plt.MilkyWay.shape(plot_type="cartesian", style="line")
 ```
 
-For more examples, see the [examples](./example.ipynb) notebook.
+For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on [Google Colab](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing). 
 
 # Reference
 <!-- Citation Y. Xu et al 2023 ApJ 947 54 -->
 <!-- https://iopscience.iop.org/article/10.3847/1538-4357/acc45c -->
-The galaxy model used in this package is based on the following paper:
+The galaxy model and data used in this package is based on the following paper:
 ```Latex
 @ARTICLE{2023ApJ...947...54X,
        author = {{Xu}, Y. and {Hao}, C.~J. and {Liu}, D.~J. and {Lin}, Z.~H. and {Bian}, S.~B. and {Hou}, L.~G. and {Li}, J.~J. and {Li}, Y.~J.},
         title = "{What Does the Milky Way Look Like?}",
       journal = {\apj},
      keywords = {Galaxy structure, Milky Way Galaxy, Trigonometric parallax, 622, 1054, 1713},
          year = 2023,
@@ -58,14 +58,14 @@
           eid = {54},
         pages = {54},
           doi = {10.3847/1538-4357/acc45c},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2023ApJ...947...54X},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
-Please BOTH cite the above paper AND acknowledge this package if you use it in your research.
+Please BOTH cite the above paper AND acknowledge this package if you are using it in your research.
 
 # License
 This package is licensed under the MIT license. See [LICENSE](./LICENSE) for details.
 
 # Acknowledgement
-We would like to thank the authors of the above paper for making their data publicly available, which made this package possible. We would also like to credit Prof. Ryan Trainor of Franklin and Marshall College for his guidance and support.
+We would like to thank the authors of the above paper for making their data publicly available, which made this package possible. We would also like to credit Prof. Ryan Trainor at Franklin and Marshall College for his guidance and support.
```

### Comparing `mwplotlib-1.0.0/README.md` & `mwplotlib-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 plt.MilkyWay.shape(plot_type="cartesian", style="region")
 
 # Plot the Milky Way in Cartesian coordinates (line-style)
 plt.figure(figsize=(9, 9))
 plt.MilkyWay.shape(plot_type="cartesian", style="line")
 ```
 
-For more examples, see the [examples](./example.ipynb) notebook.
+For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on [Google Colab](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing). 
 
 # Reference
 <!-- Citation Y. Xu et al 2023 ApJ 947 54 -->
 <!-- https://iopscience.iop.org/article/10.3847/1538-4357/acc45c -->
-The galaxy model used in this package is based on the following paper:
+The galaxy model and data used in this package is based on the following paper:
 ```Latex
 @ARTICLE{2023ApJ...947...54X,
        author = {{Xu}, Y. and {Hao}, C.~J. and {Liu}, D.~J. and {Lin}, Z.~H. and {Bian}, S.~B. and {Hou}, L.~G. and {Li}, J.~J. and {Li}, Y.~J.},
         title = "{What Does the Milky Way Look Like?}",
       journal = {\apj},
      keywords = {Galaxy structure, Milky Way Galaxy, Trigonometric parallax, 622, 1054, 1713},
          year = 2023,
@@ -48,14 +48,14 @@
           eid = {54},
         pages = {54},
           doi = {10.3847/1538-4357/acc45c},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2023ApJ...947...54X},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
-Please BOTH cite the above paper AND acknowledge this package if you use it in your research.
+Please BOTH cite the above paper AND acknowledge this package if you are using it in your research.
 
 # License
 This package is licensed under the MIT license. See [LICENSE](./LICENSE) for details.
 
 # Acknowledgement
-We would like to thank the authors of the above paper for making their data publicly available, which made this package possible. We would also like to credit Prof. Ryan Trainor of Franklin and Marshall College for his guidance and support.
+We would like to thank the authors of the above paper for making their data publicly available, which made this package possible. We would also like to credit Prof. Ryan Trainor at Franklin and Marshall College for his guidance and support.
```

### Comparing `mwplotlib-1.0.0/mwplotlib/arms_data.py` & `mwplotlib-1.1.0/mwplotlib/arms_data.py`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.0.0/mwplotlib/data/apjacc45ct1_mrt.txt` & `mwplotlib-1.1.0/mwplotlib/data/apjacc45ct1_mrt.txt`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.0.0/mwplotlib/data/apjacc45ct2_ascii.txt` & `mwplotlib-1.1.0/mwplotlib/data/apjacc45ct2_ascii.txt`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.0.0/mwplotlib/spiral_arms.py` & `mwplotlib-1.1.0/mwplotlib/spiral_arms.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,17 @@
         self.plt = plt
         self.arms = ArmsData()
         self.utilities = utilities()
         self.plt_colors = self._get_plt_colorcodes()
         
     def scatter(self, unit="pc"):
 
+        if(type(unit) != str):
+            unit = unit.to_string()
+
         # Name Alias RAh RAm      RAs DE- DEd DEm     DEs    plx   _plx    pmE  _pmE    pmN  _pmN VLSR _VLSR  Arm    Ref
         # G305.20+  G305.20+00.01   NaN  13  11  16.8912   -  62  45  55.008  0.250  0.050  -6.90  0.33  -0.52  0.33  -38     5  Nor     61
         # G339.88-  G339.88-01.25   NaN  16  52  04.6776   -  46  08  34.404  0.480  0.080  -1.60  0.52  -1.90  0.52  -34     3  Nor     37
         # G348.70-  G348.70-01.04   NaN  17  20  04.0360   -  38  58  30.920  0.296  0.026  -0.73  0.31  -2.83  0.59   -9     5  Nor      1
         # G359.61-  G359.61-00.24   NaN  17  45  39.0697   -  29  23  30.265  0.375  0.021   1.00  0.40  -1.50  0.50   21     5  Nor   1 52
         # G000.31-  G000.31-00.20   NaN  17  47  09.1092   -  28  46  16.278  0.342  0.042   0.21  0.39  -1.76  0.64   18     3  Nor     53
         # ...                 ...   ...  ..  ..      ...  ..  ..  ..     ...    ...    ...    ...   ...    ...   ...  ...   ...  ...    ...
@@ -61,28 +64,59 @@
             plotData["color"].append(color_codes[plotData["arm"][i]])
         
         # print(plotData["color"])
         self.plt.scatter(plotData["x"], plotData["y"], s=1, c=plotData["color"])
         # plt.show()
         # input()
 
-    def shape(self, unit="kpc", style="region", step=.001, plot_type="polar", **kwargs):
+    def shape(self, unit="kpc", style="region", step=.001, plot_type="polar", config={}, legend=True, **kwargs):
+        """
+        config in the form of:
+        {
+            "Outer": {
+                "color": "red", 
+                "lw": 1,
+                ... # Matplotlib kwargs
+            }, 
+            "Norma": {
+                "color": "blue",
+                "lw": 1,
+                ... # Matplotlib kwargs
+            }, 
+            ...
+        """
         plotData = []
 
+        if(type(unit) != str):
+            unit = unit.to_string()
+
         if(plot_type == "polar"):
             # set plot type to polar
             if(hasattr(self.plt, "polar")):
                 self.plt.polar([], [])
             else:
                 # Show warning
                 print("Warning: polar plot not automatically set. If you are using ax, please add subplot_kw=dict(projection='polar') argument to your plt.subplots() call.")
                 print("You may ignore this warning if the argument is already present.")
 
         lastArm = ""
         for thisRow in self.arms("shape", 'dict'):
+            thisKwargs = {}
+            if(thisRow['Spiral Arm'] in config):
+                thisKwargs = config[thisRow['Spiral Arm']]
+                for key in kwargs:
+                    if(key not in thisKwargs):
+                        thisKwargs[key] = kwargs[key]
+            else: 
+                thisKwargs = kwargs.copy()
+            
+            if(legend):
+                thisKwargs["label"] = thisRow['Spiral Arm']
+                    
+
             # print(thisRow)
             # betaRange_0 = int(thisRow['beta Range'].split('rarr')[0].strip()) / 180 * np.pi
             # betaRange_1 = int(thisRow['beta Range'].split('rarr')[1].strip()) / 180 * np.pi
             betaRange_0 = int(thisRow['beta Range'].split('rarr')[0].strip())
             betaRange_1 = int(thisRow['beta Range'].split('rarr')[1].strip())
 
             thisBetaRange = np.linspace(
@@ -118,33 +152,33 @@
             
             if(plot_type == "polar"):
                 if(thisRow['Spiral Arm'] != lastArm) :
                     # self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", label=thisRow['Spiral Arm'])
                     # self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", label=thisRow['Spiral Arm'], color=self._get_last_color())
                     # Allow for custom kwargs:
                     if(style == "region"):
-                        self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", label=thisRow['Spiral Arm'], **kwargs)
-                        self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", color=self._get_last_color(), **kwargs)
+                        self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", **thisKwargs)
+                        self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", color=self._get_last_color(), **self._kwargs_no_color(thisKwargs))
                     elif(style == "line"):
-                        self.plt.plot(thisBetaRange, thisRRange, "--", label=thisRow['Spiral Arm'], **kwargs)
+                        self.plt.plot(thisBetaRange, thisRRange, "--", **thisKwargs)
                     else:
                         print("Invalid style")
                         return
                 else:
                     # print(thisRow['Spiral Arm'])
                     if(style == "region"):
                         self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", 
-                            color=self._get_last_color(), **kwargs
+                            color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                         self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", 
-                            color=self._get_last_color(), **kwargs
+                            color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     elif(style == "line"):
                         self.plt.plot(thisBetaRange, thisRRange, "--", 
-                            color=self._get_last_color(), **kwargs
+                            color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     else:
                         print("Invalid style")
                         return
 
                 # self.plt.show()
                 # input()
@@ -156,46 +190,46 @@
                 thisX_regionLower = (thisRRange - thisArmWidth / 2) * np.cos(thisBetaRange)
                 thisY_regionLower = (thisRRange - thisArmWidth / 2) * np.sin(thisBetaRange)
                 if(thisRow['Spiral Arm'] != lastArm) :
                     # self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", label=thisRow['Spiral Arm'])
                     # self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", label=thisRow['Spiral Arm'], color=self._get_last_color())
                     # Allow for custom kwargs:
                     if(style == "region"):
-                        self.plt.plot(thisX_regionUpper, thisY_regionUpper, "--", label=thisRow['Spiral Arm'], **kwargs)
-                        self.plt.plot(thisX_regionLower, thisY_regionLower, "--", color=self._get_last_color(), **kwargs)
+                        self.plt.plot(thisX_regionUpper, thisY_regionUpper, "--", **thisKwargs)
+                        self.plt.plot(thisX_regionLower, thisY_regionLower, "--", color=self._get_last_color(), **self._kwargs_no_color(thisKwargs))
                     elif(style == "line"):
-                        self.plt.plot(thisX, thisY, "--", label=thisRow['Spiral Arm'], **kwargs)
+                        self.plt.plot(thisX, thisY, "--", **thisKwargs)
                     else:
                         print("Invalid style")
                         return
                 else:
                     # print(thisRow['Spiral Arm'])
                     if(style == "region"):
                         self.plt.plot(thisX_regionUpper, thisY_regionUpper, "--", 
-                            color=self._get_last_color(), **kwargs
+                            color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                         self.plt.plot(thisX_regionLower, thisY_regionLower, "--", 
-                            color=self._get_last_color(), **kwargs
+                            color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     elif(style == "line"):
                         self.plt.plot(thisX, thisY, "--", 
-                            color=self._get_last_color(), **kwargs
+                            color=self._get_last_color(), **self._kwargs_no_color(thisKwargs)
                         )
                     else:
                         print("Invalid style")
                         return
             else:
                 print("Invalid plot type")
                 return    
 
             lastArm = thisRow['Spiral Arm']
                     
             # plt.show()
             # input()
-        self.plt.legend()
+        # self.plt.legend()
         # self.plt.show()
         
     def _get_last_color(self):
         # return self.plt.gca().lines[-1].get_color()
         # It is possible that the user is using ax instead of plt
         if(hasattr(self.plt, "gca")):
             return self.plt.gca().lines[-1].get_color()
@@ -210,12 +244,22 @@
         # It is possible that the user is using ax instead of plt
         if(hasattr(self.plt, "rcParams")):
             return self.plt.rcParams['axes.prop_cycle'].by_key()['color']
         else:
             import matplotlib.pyplot as plt
             return plt.rcParams['axes.prop_cycle'].by_key()['color']
 
+    def _kwargs_no_color(self, kwargs):
+        # Remove color from kwargs
+        if('color' in kwargs):
+            kwargs.pop('color')
+        
+        # remove label from kwargs
+        if('label' in kwargs):
+            kwargs.pop('label')
+            
+        return kwargs
             
 class MilkyWay():
     def mw_plt(plt):
         plt.MilkyWay = MilkyWayHandler(plt)
         return plt
```

### Comparing `mwplotlib-1.0.0/mwplotlib/utilities.py` & `mwplotlib-1.1.0/mwplotlib/utilities.py`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.0.0/mwplotlib.egg-info/PKG-INFO` & `mwplotlib-1.1.0/mwplotlib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwplotlib
-Version: 1.0.0
+Version: 1.1.0
 Summary: The Milky Way Plotting Library
 Home-page: https://github.com/xiawenke/mwplotlib
 Author: Wenky
 Author-email: wxia1@fandm.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,20 +35,20 @@
 plt.MilkyWay.shape(plot_type="cartesian", style="region")
 
 # Plot the Milky Way in Cartesian coordinates (line-style)
 plt.figure(figsize=(9, 9))
 plt.MilkyWay.shape(plot_type="cartesian", style="line")
 ```
 
-For more examples, see the [examples](./example.ipynb) notebook.
+For more examples of usage, please refer to [examples](./example.ipynb) notebook. Those examples are also available on [Google Colab](https://colab.research.google.com/drive/1M9IawDSco0dbIZz5crcxTUm4NkWu43fq?usp=sharing). 
 
 # Reference
 <!-- Citation Y. Xu et al 2023 ApJ 947 54 -->
 <!-- https://iopscience.iop.org/article/10.3847/1538-4357/acc45c -->
-The galaxy model used in this package is based on the following paper:
+The galaxy model and data used in this package is based on the following paper:
 ```Latex
 @ARTICLE{2023ApJ...947...54X,
        author = {{Xu}, Y. and {Hao}, C.~J. and {Liu}, D.~J. and {Lin}, Z.~H. and {Bian}, S.~B. and {Hou}, L.~G. and {Li}, J.~J. and {Li}, Y.~J.},
         title = "{What Does the Milky Way Look Like?}",
       journal = {\apj},
      keywords = {Galaxy structure, Milky Way Galaxy, Trigonometric parallax, 622, 1054, 1713},
          year = 2023,
@@ -58,14 +58,14 @@
           eid = {54},
         pages = {54},
           doi = {10.3847/1538-4357/acc45c},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2023ApJ...947...54X},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
-Please BOTH cite the above paper AND acknowledge this package if you use it in your research.
+Please BOTH cite the above paper AND acknowledge this package if you are using it in your research.
 
 # License
 This package is licensed under the MIT license. See [LICENSE](./LICENSE) for details.
 
 # Acknowledgement
-We would like to thank the authors of the above paper for making their data publicly available, which made this package possible. We would also like to credit Prof. Ryan Trainor of Franklin and Marshall College for his guidance and support.
+We would like to thank the authors of the above paper for making their data publicly available, which made this package possible. We would also like to credit Prof. Ryan Trainor at Franklin and Marshall College for his guidance and support.
```

### Comparing `mwplotlib-1.0.0/setup.py` & `mwplotlib-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwplotlib",
-    version="1.0.0",
+    version="1.1.0",
     author="Wenky",
     author_email="wxia1@fandm.edu",
     description="The Milky Way Plotting Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xiawenke/mwplotlib",
     packages=setuptools.find_packages(),
```

