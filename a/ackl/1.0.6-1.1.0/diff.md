# Comparing `tmp/ackl-1.0.6.tar.gz` & `tmp/ackl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ackl-1.0.6.tar", last modified: Thu Jun 29 08:04:07 2023, max compression
+gzip compressed data, was "ackl-1.1.0.tar", last modified: Mon Jul  3 01:26:03 2023, max compression
```

## Comparing `ackl-1.0.6.tar` & `ackl-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.627028 ackl-1.0.6/
--rw-rw-rw-   0        0        0     1087 2022-09-05 02:47:29.000000 ackl-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     1679 2023-06-29 08:04:07.627028 ackl-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1088 2023-06-23 01:41:47.000000 ackl-1.0.6/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 ackl-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      900 2023-06-29 08:04:07.627028 ackl-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.330206 ackl-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.595767 ackl-1.0.6/src/ackl/
--rw-rw-rw-   0        0        0       75 2022-09-28 13:06:58.000000 ackl-1.0.6/src/ackl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.627028 ackl-1.0.6/src/ackl/gui/
--rw-rw-rw-   0        0        0        0 2023-01-31 05:39:02.000000 ackl-1.0.6/src/ackl/gui/__init__.py
--rw-rw-rw-   0        0        0     2564 2023-03-31 07:47:59.000000 ackl-1.0.6/src/ackl/gui/run.py
--rw-rw-rw-   0        0        0    38910 2023-06-29 04:12:06.000000 ackl-1.0.6/src/ackl/kernels.py
--rw-rw-rw-   0        0        0    24988 2023-06-29 05:36:46.000000 ackl-1.0.6/src/ackl/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-29 08:04:07.627028 ackl-1.0.6/src/ackl.egg-info/
--rw-rw-rw-   0        0        0     1679 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-29 08:04:07.000000 ackl-1.0.6/src/ackl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.403746 ackl-1.1.0/
+-rw-rw-rw-   0        0        0     1087 2022-09-05 02:47:29.000000 ackl-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-07-01 14:25:20.000000 ackl-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1691 2023-07-03 01:26:03.403746 ackl-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1100 2023-07-01 14:02:39.000000 ackl-1.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 ackl-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      900 2023-07-03 01:26:03.406744 ackl-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.336745 ackl-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.353742 ackl-1.1.0/src/ackl/
+-rw-rw-rw-   0        0        0      160 2023-06-30 14:07:27.000000 ackl-1.1.0/src/ackl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.383741 ackl-1.1.0/src/ackl/gui/
+-rw-rw-rw-   0        0        0        0 2023-01-31 05:39:02.000000 ackl-1.1.0/src/ackl/gui/__init__.py
+-rw-rw-rw-   0        0        0     2637 2023-07-01 14:04:30.000000 ackl-1.1.0/src/ackl/gui/run.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.396748 ackl-1.1.0/src/ackl/gui/static/
+-rw-rw-rw-   0        0        0   202389 2023-01-16 12:00:51.000000 ackl-1.1.0/src/ackl/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   136072 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    86929 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0    24228 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17131 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0  1477676 2022-12-23 14:00:42.000000 ackl-1.1.0/src/ackl/gui/static/sample.csv
+drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.401747 ackl-1.1.0/src/ackl/gui/templates/
+-rw-rw-rw-   0        0        0    13445 2023-03-31 05:31:00.000000 ackl-1.1.0/src/ackl/gui/templates/home.html
+-rw-rw-rw-   0        0        0    38912 2023-07-01 02:44:57.000000 ackl-1.1.0/src/ackl/kernels.py
+-rw-rw-rw-   0        0        0    29083 2023-07-03 00:51:01.000000 ackl-1.1.0/src/ackl/metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.379738 ackl-1.1.0/src/ackl.egg-info/
+-rw-rw-rw-   0        0        0     1691 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/top_level.txt
```

### Comparing `ackl-1.0.6/LICENSE` & `ackl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ackl-1.0.6/PKG-INFO` & `ackl-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ackl
-Version: 1.0.6
+Version: 1.1.0
 Summary: A Python library for kernels used in analytical chemistry
 Home-page: https://github.com/zhangys11/ack
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/ack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,15 +56,15 @@
 import ackl.metrics
 ackl.metrics.linear_response_pattern(20)
 ```
 
 ### Run Kernels on Target Dataset
 
 ```
-dics = ackl.metrics.preview_kernels(X, y,embed_title = False)
+_, dics, _ = ackl.metrics.classify_with_kernels(X, y,embed_title = False)
 ```
 
 Show the result as HTML table and bar charts: 
 
 ```
 html_str = ackl.metrics.visualize_metric_dicts(dics, plot = True)
 display(HTML( html_str ))
```

### Comparing `ackl-1.0.6/README.md` & `ackl-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 import ackl.metrics
 ackl.metrics.linear_response_pattern(20)
 ```
 
 ### Run Kernels on Target Dataset
 
 ```
-dics = ackl.metrics.preview_kernels(X, y,embed_title = False)
+_, dics, _ = ackl.metrics.classify_with_kernels(X, y,embed_title = False)
 ```
 
 Show the result as HTML table and bar charts: 
 
 ```
 html_str = ackl.metrics.visualize_metric_dicts(dics, plot = True)
 display(HTML( html_str ))
```

### Comparing `ackl-1.0.6/setup.cfg` & `ackl-1.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 636b 6c0d 0a76 6572 7369 6f6e   = ackl..version
-00000020: 203d 2031 2e30 2e36 0d0a 6175 7468 6f72   = 1.0.6..author
+00000020: 203d 2031 2e31 2e30 0d0a 6175 7468 6f72   = 1.1.0..author
 00000030: 203d 2059 696e 7368 656e 6720 5a68 616e   = Yinsheng Zhan
 00000040: 6720 2850 682e 442e 290d 0a61 7574 686f  g (Ph.D.)..autho
 00000050: 725f 656d 6169 6c20 3d20 6f6f 407a 6a75  r_email = oo@zju
 00000060: 2e65 6475 2e63 6e0d 0a64 6573 6372 6970  .edu.cn..descrip
 00000070: 7469 6f6e 203d 2041 2050 7974 686f 6e20  tion = A Python 
 00000080: 6c69 6272 6172 7920 666f 7220 6b65 726e  library for kern
 00000090: 656c 7320 7573 6564 2069 6e20 616e 616c  els used in anal
```

### Comparing `ackl-1.0.6/src/ackl/gui/run.py` & `ackl-1.1.0/src/ackl/gui/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,18 @@
                 r += io.draw_class_average(X, y, X_names, labels, output_html=True)
 
             r += io.scatter_plot(X, y, labels=labels, output_html=True)
 
         r += '<p>' + desc + '</p><hr/>'
         r += '<h6>Kernel Transformation</h6>'
 
-        dic, s = metrics.preview_kernels(X, y, scale = True,
-                                        metrics=True,
-                                        scatterplot=True,
+        _, dic_test_accs, dic, s = metrics.classify_with_kernels(X, y, scale = True,
+                                        do_cla=True,
+                                        run_clfs=True,
+                                        plots=True,
                                         logplot=True,
                                         output_html= True,
                                         selected_kernel_names = kernel_type)
 
         r += s
         r += metrics.visualize_metric_dicts(dic, plot=False)
```

### Comparing `ackl-1.0.6/src/ackl/kernels.py` & `ackl-1.1.0/src/ackl/kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,16 +410,16 @@
 }
 
 
 # Stores the hyper parameter search range for each kernel.
 # Some hparams are dynamic (based on data dim).
 # Not all kernels have tunable hyper-parameters.
 kernel_hparams = {
-    "poly": [1, 2, 3, 4],  # when d = 1, becomes a linear kernel
-    "gaussian": [0.1, 1, 3.33, 10, 60, 100, 300, 400],
+    "poly": [2, 3, 4],  # skip d = 1, as it degrades to a linear kernel
+    "gaussian": [0.1, 1, 3.33, 10, 60, 100, 300],
     "sigmoid": [0.01, 0.1, 1, 10],
     "laplace": [0.001, 0.01, 0.1, 1, 10, 30, 50],
     # "exp": alias of laplace
     "chi2":  [0.00001, 0.0001, 0.001, 0.01, 0.1, 1.0, 10, 100],
     "anova": [0.000001, 0.00001, 0.001, 0.1, 1, 10, 1000, 100000],
     "cauchy": [0.01, 0.1, 1, 10, 100, 1000, 10000],
     "power": [.00001, .0001, .001, .01, .1, 1],
```

### Comparing `ackl-1.0.6/src/ackl/metrics.py` & `ackl-1.1.0/src/ackl/metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import sys
 import math
 import timeit
+from itertools import combinations
 import numpy as np
+import pickle
 import matplotlib.pyplot as plt
 import IPython.display
 
 from sklearn.decomposition import PCA
 from sklearn.cross_decomposition import PLSRegression
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
 from sklearn.linear_model import LogisticRegressionCV
-from sklearn.metrics import classification_report, confusion_matrix
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.decomposition import PCA
+from sklearn.model_selection import train_test_split
 from cla.metrics import get_metrics, metric_polarity_dict, es_max, run_multiclass_clfs
 from cla.vis.plt2base64 import plt2html
 
 if __package__:
     from .kernels import kernel_names, kernel_hparams, kernel_formulas, \
     kernel_fullnames, kernel_dict, kernel_hparas_divide_n, \
     cosine_kernel
@@ -166,16 +168,16 @@
     1  k(1,0) k(1,1)
 
     Parameter
     ---------
     cmap : color map scheme
     '''
     X = np.array([0, 1]).reshape(-1, 1)
-    _ = preview_kernels(X, np.array(
-        [0, 1]), cmap, None, True, False, False, False, False)
+    _ = classify_with_kernels(X, np.array(
+        [0, 1]), cmap, None, scale=True, run_clfs=False, do_cla=False)
 
 
 def linear_response_pattern(n=10, dim=1, cmap='gray'):
     '''
     Generates a response pattern of pairwise-point-distances.
     See how each kernel responds to / varies with linearly arranged points.
 
@@ -193,26 +195,27 @@
     y = [0]*round(n/2) + [1]*(n-round(n/2))
 
     if dim == 2:
         zeros = np.array([0] * n).reshape(-1, 1)
         X = np.vstack((np.hstack((X, zeros)), np.hstack((zeros, X))))
         y = [0] * n + [1] * n
 
-    _ = preview_kernels(X, np.array(y), cmap, hyper_param_optimizer = None,
-                        scale = True, calc_metrics = False,
-                        scatterplot = False, embed_title = False, verbose = False)
+    _ = classify_with_kernels(X, np.array(y), cmap, hyper_param_optimizer = None,
+                        scale = True, run_clfs = False, do_cla = False,
+                        plots = True, embed_title = False, verbose = False)
 
 
-def preview_kernels(X, y, cmap=None, hyper_param_optimizer=kes,
-                    scale=False, calc_metrics=True, logplot=False, 
-                    scatterplot=True, embed_title=True,
+def classify_with_kernels(X, y, cmap=None, hyper_param_optimizer=kes,
+                    scale=False, run_clfs=True, do_cla = False,
+                    multi_kernels=[1], multi_kernel_topk=-1,
+                    logplot=False, plots=True, embed_title=False,
                     output_html=False,
                     selected_kernel_names=None, verbose = True):
     '''
-    Try various kernel types to evaluate the pattern after kernel-ops.  
+    Try various kernel types for classification task.  
     Each kernel uses their own default/empirical paramters.    
     In binary classification, because the first and last half samples belong to two classes respectively. 
     We want to get a contrasive pattern, i.e., (LT、RB) and （LB、RT）have blocks of different colors. 
 
     Parameters
     ----------
     X : an m-by-n data matrix. 
@@ -221,47 +224,56 @@
     y : class labels
     cmap : color map scheme to use. set None to use default, or set another scheme, e.g., 'gray', 'viridis', 'jet', 'rainbow', etc.
         For small dataset, we recommend 'gray'. For complex dataset, we recommend 'viridis'.
     hyper_param_optimizer : which optimizer to optimize the hyper parameters for each kernel. 
         For real-world dataset, use kes by default. For toy dataset, set None to disable optimizer.
         For multi-class dataset (y has more than 5 classes), use acc.
     scale : whether do feature scaling
-    calc_metrics : whether calculate classifiability metrics.
+    run_clfs : whether run multiple classfiers and show confusion matrices
+    multi_kernels : how many kernels to use. Default is [1].
+    multi_kernel_topk : the k best single kernels to use in multi-kernel combinations. Default is 5.
     logplot : whether to output the log-scale plot in parallel.
-    scatterplot : whether to ouptut the kernel heatmaps and the scatter plots after PCA / PLS, to check classifiability.
+    plots : whether to ouptut the kernel heatmaps and the scatter plots after PCA / PLS, to check classifiability.
         The PLS tries to maximize the covariance between X and Y.
     embed_title : whether embed the title in the plots. If not, will generate the title in HTML.
+    do_cla : whether to do classifiability analysis using the cla package.
     selected_kernel_names : a list of kernel names to be process. 
         If None or 'all', will use all kernels.
     '''
 
+    dic_test_accs = {}
     all_dic_metrics = {}
     html_str = ''
 
     if scale:
         X = MinMaxScaler().fit_transform(X)
+        print('perform min-max scaling')
 
-    if calc_metrics:
+    if run_clfs:
         result_html = '<h3>0. no kernel</h3><p>Classification on original dataset</p>'
-        result_html += run_multiclass_clfs(X, y, show = False)
+        dic, mc_html = run_multiclass_clfs(X, y, clfs=['LinearDiscriminantAnalysis()'], show = False)
+        dic_test_accs['no kernel'] = dic
+        result_html += mc_html
         if output_html:
             html_str += result_html
-        else:
+        if plots:
             IPython.display.display(IPython.display.HTML(result_html))
 
     # to be safe, perform a re-order
     if (y is not None and len(set(y)) == 2):
         labels = list(set(y))  # re-order X by y
         X = np.vstack((X[y == labels[0]], X[y == labels[1]]))
         y = [labels[0]] * np.sum(y == labels[0]) + \
             [labels[1]] * np.sum(y == labels[1])
 
     if selected_kernel_names is None or selected_kernel_names == 'all':
         selected_kernel_names = kernel_names
 
+    KX = {} # store the data matrix after each kernel
+
     for i, key in enumerate(selected_kernel_names):
         best_hparam = None
         best_metric = -np.inf
         title = str(i+1) + '. ' + \
             (kernel_fullnames[key] if key in kernel_fullnames else key)
 
         if hyper_param_optimizer is not None and key in kernel_hparams:
@@ -281,32 +293,36 @@
             kns = kernel_dict[key](X, X)
             # metric_nmd = nmd(X, y, lambda x, y: kernel_dict[key](x, y), verbose = verbose)
         else:
             kns = kernel_dict[key](X, X, best_hparam)
             # metric_nmd = nmd(X, y, lambda x, y: kernel_dict[key](x, y, param), verbose = verbose)
 
         kns = np.nan_to_num(kns)
+        KX[key] = kns
 
         ######## plot after kernel transforms ########
         
-        if scatterplot or output_html:
+        if plots or output_html:
             _, ax = plt.subplots(1, 2, figsize=(round(len(set(y))/2.0) + 6, round(len(set(y))/4.0) + 3)) # figsize = (round(len(labels)/4.0) + 4, round(len(labels)/4.0) + 3)
             ax[0].imshow(kns, cmap=cmap)
             ax[0].set_axis_off()
             if logplot:
                 ax[1].imshow(1+np.log(kns), cmap=cmap)
                 ax[1].set_axis_off()
 
             plt.axis('off')
             if embed_title:
                 plt.title(title + '\n' + kernel_formulas[key] + '\n') # + "NMD = %.3g" % metric_nmd)
             else:
                 # print(title)
-                IPython.display.display(IPython.display.HTML('<h3>' + title + '</h3>' + '<p>' + kernel_formulas[key].replace('<', '&lt;')
-                                                            .replace('>', '&gt;') + '</p>')) # <p>' + "NMD = %.3g" % metric_nmd + '</p>'
+                kernel_title = '<h3>' + title + '</h3>' + '<p>' + kernel_formulas[key].replace('<', '&lt;').replace('>', '&gt;') + '</p>'
+                if output_html:
+                    html_str += kernel_title
+                else:
+                    IPython.display.display(IPython.display.HTML(kernel_title)) # <p>' + "NMD = %.3g" % metric_nmd + '</p>'
             if output_html:
                 html_str += plt2html(plt)
                 plt.close()
             else:
                 plt.show()
 
             ######## scatter plot after PCA ########            
@@ -317,29 +333,32 @@
             plt.title('PCA')
 
             if output_html:
                 html_str += plt2html(plt)
                 plt.close()
             else:
                 plt.show()
-
+           
             ######## scatter plot after LDA ########
 
+            k_train, k_test, y_train, y_test = train_test_split(
+                    kns, y, test_size=0.3, random_state = 2, stratify=y)
+
             try:
                 lda = LinearDiscriminantAnalysis()
-                X_lda = lda.fit(kns, y).transform(kns)
+                X_lda = lda.fit(k_train, y_train).transform(k_test)
                 X_lda = np.nan_to_num(X_lda)
 
-                lda.score(kns, y)
+                lda.score(k_test, y_test)
                 if (X_lda.shape[1] == 1):
                     X_lda = np.hstack((X_lda, np.zeros((X_lda.shape[0], 1))))
-                plot_components_2d(X_lda, y)
+                plot_components_2d(X_lda, y_test)
                 # the coefficient of determination or R squared method is the proportion of the variance in the dependent variable that is predicted from the independent variable.
                 plt.title(
-                    'LDA (ACC = ' + str(np.round(lda.score(kns, y), 3)) + ')')
+                    'LDA (test acc = ' + str(np.round(lda.score(k_test, y_test), 3)) + ')')
                 
                 if output_html:
                     html_str += plt2html(plt)
                     plt.close()
                 else:
                     plt.show()
 
@@ -348,80 +367,158 @@
                     print('Exception : ', e)
                 # print('X_pls = ', X_pls)
                 # plt.title('PLS')
                 html_str += '<p>' + str(e) + '</p>'
 
             ######## scatter plot after PLS ########
 
-            try:
-                ''' # using CV
-                kns = np.nan_to_num(kns)
-                pls = PLSRegression(n_components=2, scale=False)
-
-                k_train, k_test, y_train, y_test = train_test_split(
-                    kns, y, test_size=0.3)
-
-                X_pls = pls.fit(k_train, y_train).transform(k_test)
-                X_pls = np.nan_to_num(X_pls)
+            if len(set(y)) == 2: # skip PLS for multi-class cases
 
-                pls.score(k_test, y_test)
-                plot_components_2d(X_pls, y_test, legends=['C1', 'C2'])
-                # the coefficient of determination or R squared method is the proportion of the variance in the dependent variable that is predicted from the independent variable.
-                plt.title(
-                    'PLS (R2 = ' + str(np.round(pls.score(k_test, y_test), 3)) + ')')
-                plt.show()
-                '''
-
-                kns = np.nan_to_num(kns)
-                pls = PLSRegression(n_components=2, scale=False)
-                X_pls = pls.fit(kns, y).transform(kns)
-                X_pls = np.nan_to_num(X_pls)
-
-                pls.score(kns, y)
-                plot_components_2d(X_pls, y)
-                # the coefficient of determination or R squared method is the proportion of the variance in the dependent variable that is predicted from the independent variable.
-                plt.title(
-                    'PLS (R2 = ' + str(np.round(pls.score(kns, y), 3)) + ')')
-                if output_html:
-                    html_str += plt2html(plt)
-                    plt.close()
-                else:
+                try:
+                    ''' # using CV
+                    kns = np.nan_to_num(kns)
+                    pls = PLSRegression(n_components=2, scale=False)
+
+                    k_train, k_test, y_train, y_test = train_test_split(
+                        kns, y, test_size=0.3)
+
+                    X_pls = pls.fit(k_train, y_train).transform(k_test)
+                    X_pls = np.nan_to_num(X_pls)
+
+                    pls.score(k_test, y_test)
+                    plot_components_2d(X_pls, y_test, legends=['C1', 'C2'])
+                    # the coefficient of determination or R squared method is the proportion of the variance in the dependent variable that is predicted from the independent variable.
+                    plt.title(
+                        'PLS (R2 = ' + str(np.round(pls.score(k_test, y_test), 3)) + ')')
                     plt.show()
-            except Exception as e:
-                if verbose:
-                    print('Exception : ', e)
-                # print('X_pls = ', X_pls)
-                # plt.title('PLS')
-                html_str += '<p>' + str(e) + '</p>'
+                    '''
+
+                    kns = np.nan_to_num(kns)
+                    pls = PLSRegression(n_components=2, scale=False)
+                    X_pls = pls.fit(kns, y).transform(kns)
+                    X_pls = np.nan_to_num(X_pls)
+
+                    pls.score(kns, y)
+                    plot_components_2d(X_pls, y)
+                    # the coefficient of determination or R squared method is the proportion of the variance in the dependent variable that is predicted from the independent variable.
+                    plt.title(
+                        'PLS (R2 = ' + str(np.round(pls.score(kns, y), 3)) + ')')
+                    if output_html:
+                        html_str += plt2html(plt)
+                        plt.close()
+                    else:
+                        plt.show()
+                except Exception as e:
+                    if verbose:
+                        print('Exception : ', e)
+                    # print('X_pls = ', X_pls)
+                    # plt.title('PLS')
+                    html_str += '<p>' + str(e) + '</p>'
 
         ###### Classifiction after kernel transformation #######
-        if calc_metrics:
+        if run_clfs:
             # result_html = '<h3>classification</h3>'
-            result_html = run_multiclass_clfs(kns, y, show = False)
+            dic, result_html = run_multiclass_clfs(kns, y, clfs=['LinearDiscriminantAnalysis()'], show = False)
+            dic_test_accs[key] = dic
             if output_html:
                 html_str += result_html
-            else:
+            if plots:
                 IPython.display.display(IPython.display.HTML(result_html))
 
         ###### cla metrics ######
-        if calc_metrics:
+        if do_cla: # disable for now
             kns = np.nan_to_num(np.hstack((kns, np.array(y).reshape(-1, 1))),   # do nan filtering simultaneously for X and y
                                 nan=0, posinf=kns.max(), neginf=kns.min())
-            _, dic_metrics = get_metrics(kns[:, :-1], kns[:, -1].flatten(), verbose = False)
+            _, dic_metrics = get_metrics(kns[:, :-1], kns[:, -1].flatten(), verbose = verbose)
             # dic_metrics['NMD'] = metric_nmd
             all_dic_metrics[key] = dic_metrics
 
-    return all_dic_metrics, html_str
+    pickle.dump((KX, dic_test_accs), open('single_kernels.pkl', 'wb'))
+
+    if run_clfs: # multi-kernel cases
 
+        # find top k kernels
+        best_KX = {}
+        best_top1s = {}
+        for k,v in dic_test_accs.items():
+            if k == 'no kernel':
+                continue
+            
+            best_top1 = 0
+            for kk, vv in v.items():
+                if best_top1 < vv[0]: # top-1 test acc
+                    best_top1 = vv[0]
+            best_top1s[k] = best_top1
+
+        keys = list(best_top1s.keys())
+        values = list(best_top1s.values())
+        sorted_value_index = np.argsort(values)[::-1]
+        sorted_dict = {keys[i]: values[i] for i in sorted_value_index}
+
+        print('Sorted single-kernel test accs: ', sorted_dict)
+
+        for k in sorted_dict: # sorted(best_top1s.items(),  key = lambda kv:(kv[1], kv[0]), reverse=True):
+            best_KX[k] = KX[k]
+            if multi_kernel_topk != -1 and len(best_KX) >= multi_kernel_topk:
+                break
+
+        for multi_kernel in multi_kernels:
+
+            if multi_kernel == 1: # single kernel case, skip
+                continue
+
+            for idx, ks in enumerate(combinations(best_KX, multi_kernel)):
+                combined = np.zeros((len(y),0))
+                mk_title = ''
+                for iidx, k in enumerate(ks):
+                    if iidx == 0:
+                        mk_title += k
+                    else:
+                        mk_title += ' + ' + k
+                    combined = np.hstack((combined, KX[k]))
+                
+                dic, result_html = run_multiclass_clfs(combined, y, clfs=['LinearDiscriminantAnalysis()'], show = False)
+                result_html = '<h3>' + str(multi_kernel) + '-kernel ' + str(idx+1) + '. ' + mk_title + '</h3>' + result_html
+                dic_test_accs[mk_title] = dic
+                if output_html:
+                    html_str += result_html
+                if plots:
+                    IPython.display.display(IPython.display.HTML(result_html))
+
+    return KX, dic_test_accs, all_dic_metrics, html_str
+
+def visualize_kernel_result_dict(dic_test_accs):
+    '''
+    Visualize the result dictionary returned by classify_with_kernels()
+    '''
+
+    top1_accs = []
+    top3_accs = []
+    top5_accs = []
+    html_str = '<table>'
+    for k, v in dic_test_accs.items():
+        accs = [str(round(x,3)) for x in list(v.values())[0]]
+        top1_accs.append(list(v.values())[0][0])
+        top3_accs.append(list(v.values())[0][1])
+        top5_accs.append(list(v.values())[0][2])
+        html_str += '<tr>' + '<td>' + k + '</td>' + '<td>' + accs[0] + '</td>' + '<td>' + accs[1] + '</td>' + '<td>' + accs[2] + '</td></tr>'
+
+    html_str += '<tr>' + '<td>best</td>' + '<td>' + \
+    str(round(np.max(top1_accs),3)) + '</td>' + '<td>' + \
+    str(round(np.max(top3_accs),3)) + '</td>' + '<td>' + \
+    str(round(np.max(top5_accs),3)) + '</td></tr>'
+
+    html_str += '</table>'
+    IPython.display.display(IPython.display.HTML(html_str))
 
 def visualize_metric_dicts(dics, plot=True):
     '''
     Example
     -------
-    dics = preview_kernels(X, y)
+    _, dics, _ = classify_with_kernels(X, y)
     html_str = generate_html_from_dicts(dics)
     display(HTML(html_str)) # use in jupyter notebook
     '''
 
     row_names = []
     column_names = []
 
@@ -510,16 +607,15 @@
             print('Built-in hparams not found. Exit.')
             return
 
     for h in hparams:
         title = (kernel_fullnames[key] if key in kernel_fullnames else key) \
             + ('(' + format(h, '.2g') + ')')
         plt.imshow(kernel_dict[key](X, X, h), cmap=cmap)
-        metric_str = "NMD = %.3g" % nmd(X, y, lambda x, y: kernel_dict[key](x, y, h)) \
-            + "\tACC = %.3g" % acc(X, y, lambda x,
+        metric_str = "ACC = %.3g" % acc(X, y, lambda x,
                                    y: kernel_dict[key](x, y, h))
         plt.axis('off')
         plt.title(title + '\n' + kernel_formulas[key] + '\n' + metric_str)
         plt.show()
 
 
 def cosine_kernel_response_pattern(n=10, cmap='gray', logplot=False, embed_title=False):
@@ -544,16 +640,15 @@
     ax[0].imshow(kns, cmap=cmap)
     ax[0].set_axis_off()
     if logplot:
         ax[1].imshow(1+np.log(kns), cmap=cmap)
         ax[1].set_axis_off()
     plt.axis('off')
 
-    metric_str = "NMD = %.3g" % nmd(X, y, lambda x, y: kernel_dict['cosine'](x, y)) \
-        + "  ACC = %.3g" % acc(X, y, lambda x, y: kernel_dict['cosine'](x, y))
+    metric_str = "ACC = %.3g" % acc(X, y, lambda x, y: kernel_dict['cosine'](x, y))
 
     if embed_title:
         plt.title(kernel_fullnames['cosine'] + '\n' + kernel_formulas['cosine']
                   + '\n' + metric_str + '\n' + comment)
     else:
         IPython.display.display(IPython.display.HTML('<h3>' + kernel_fullnames['cosine'] + '</h3>' + '<p>' +
                                                      kernel_formulas['cosine'].replace(
```

### Comparing `ackl-1.0.6/src/ackl.egg-info/PKG-INFO` & `ackl-1.1.0/src/ackl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ackl
-Version: 1.0.6
+Version: 1.1.0
 Summary: A Python library for kernels used in analytical chemistry
 Home-page: https://github.com/zhangys11/ack
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/ack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,15 +56,15 @@
 import ackl.metrics
 ackl.metrics.linear_response_pattern(20)
 ```
 
 ### Run Kernels on Target Dataset
 
 ```
-dics = ackl.metrics.preview_kernels(X, y,embed_title = False)
+_, dics, _ = ackl.metrics.classify_with_kernels(X, y,embed_title = False)
 ```
 
 Show the result as HTML table and bar charts: 
 
 ```
 html_str = ackl.metrics.visualize_metric_dicts(dics, plot = True)
 display(HTML( html_str ))
```

