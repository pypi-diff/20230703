# Comparing `tmp/pyNNRW-0.3.2.tar.gz` & `tmp/pyNNRW-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNNRW-0.3.2.tar", last modified: Fri Apr  7 01:48:53 2023, max compression
+gzip compressed data, was "pyNNRW-0.3.3.tar", last modified: Mon Jul  3 09:52:57 2023, max compression
```

## Comparing `pyNNRW-0.3.2.tar` & `pyNNRW-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 01:48:53.660940 pyNNRW-0.3.2/
--rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 pyNNRW-0.3.2/LICENCE
--rw-rw-rw-   0        0        0     4106 2023-04-07 01:48:53.660940 pyNNRW-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3458 2022-05-10 04:41:05.000000 pyNNRW-0.3.2/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 pyNNRW-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-04-07 01:48:53.663935 pyNNRW-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 01:48:53.263125 pyNNRW-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 01:48:53.632193 pyNNRW-0.3.2/src/pyNNRW/
--rw-rw-rw-   0        0        0     2044 2023-04-07 01:47:56.000000 pyNNRW-0.3.2/src/pyNNRW/__init__.py
--rw-rw-rw-   0        0        0      239 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/aerw.py
--rw-rw-rw-   0        0        0      777 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/dtc.py
--rw-rw-rw-   0        0        0    17243 2022-10-14 01:00:40.000000 pyNNRW-0.3.2/src/pyNNRW/elm.py
--rw-rw-rw-   0        0        0      128 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/knn.py
--rw-rw-rw-   0        0        0    12946 2022-09-08 05:18:51.000000 pyNNRW-0.3.2/src/pyNNRW/knnrw.py
--rw-rw-rw-   0        0        0      509 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/lr.py
--rw-rw-rw-   0        0        0     7233 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/mlp.py
--rw-rw-rw-   0        0        0    22081 2022-10-14 09:17:58.000000 pyNNRW-0.3.2/src/pyNNRW/nnrw.py
--rw-rw-rw-   0        0        0     8033 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/rbfnn.py
--rw-rw-rw-   0        0        0     8632 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/rbm.py
--rw-rw-rw-   0        0        0     8361 2023-04-07 01:09:38.000000 pyNNRW-0.3.2/src/pyNNRW/rvfl.py
--rw-rw-rw-   0        0        0     1436 2022-05-20 11:56:20.000000 pyNNRW-0.3.2/src/pyNNRW/wann.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:48:53.658929 pyNNRW-0.3.2/src/pyNNRW.egg-info/
--rw-rw-rw-   0        0        0     4106 2023-04-07 01:48:53.000000 pyNNRW-0.3.2/src/pyNNRW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-07 01:48:53.000000 pyNNRW-0.3.2/src/pyNNRW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 01:48:53.000000 pyNNRW-0.3.2/src/pyNNRW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-07 01:48:53.000000 pyNNRW-0.3.2/src/pyNNRW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 01:48:53.000000 pyNNRW-0.3.2/src/pyNNRW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.716614 pyNNRW-0.3.3/
+-rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 pyNNRW-0.3.3/LICENCE
+-rw-rw-rw-   0        0        0     4106 2023-07-03 09:52:57.716614 pyNNRW-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3458 2022-05-10 04:41:05.000000 pyNNRW-0.3.3/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 pyNNRW-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-07-03 09:52:57.719615 pyNNRW-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.657069 pyNNRW-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.706614 pyNNRW-0.3.3/src/pyNNRW/
+-rw-rw-rw-   0        0        0     2044 2023-04-07 01:49:33.000000 pyNNRW-0.3.3/src/pyNNRW/__init__.py
+-rw-rw-rw-   0        0        0      239 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/aerw.py
+-rw-rw-rw-   0        0        0      777 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/dtc.py
+-rw-rw-rw-   0        0        0    18109 2023-07-03 09:13:36.000000 pyNNRW-0.3.3/src/pyNNRW/elm.py
+-rw-rw-rw-   0        0        0      128 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/knn.py
+-rw-rw-rw-   0        0        0    13110 2023-07-03 09:52:09.000000 pyNNRW-0.3.3/src/pyNNRW/knnrw.py
+-rw-rw-rw-   0        0        0      509 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/lr.py
+-rw-rw-rw-   0        0        0     7233 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/mlp.py
+-rw-rw-rw-   0        0        0    23963 2023-06-11 14:29:33.000000 pyNNRW-0.3.3/src/pyNNRW/nnrw.py
+-rw-rw-rw-   0        0        0     8033 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/rbfnn.py
+-rw-rw-rw-   0        0        0     8632 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/rbm.py
+-rw-rw-rw-   0        0        0    17134 2023-07-03 09:47:35.000000 pyNNRW-0.3.3/src/pyNNRW/rvfl.py
+-rw-rw-rw-   0        0        0     1436 2022-05-20 11:56:20.000000 pyNNRW-0.3.3/src/pyNNRW/wann.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:52:57.715614 pyNNRW-0.3.3/src/pyNNRW.egg-info/
+-rw-rw-rw-   0        0        0     4106 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 09:52:57.000000 pyNNRW-0.3.3/src/pyNNRW.egg-info/top_level.txt
```

### Comparing `pyNNRW-0.3.2/PKG-INFO` & `pyNNRW-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNNRW
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python library for NNRW (neural network with random weights)
 Home-page: https://github.com/zhangys11/pyNNRW
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/pyNNRW/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyNNRW-0.3.2/README.md` & `pyNNRW-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.2/setup.cfg` & `pyNNRW-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 794e 4e52 570d 0a76 6572 7369   = pyNNRW..versi
-00000020: 6f6e 203d 2030 2e33 2e32 0d0a 6175 7468  on = 0.3.2..auth
+00000020: 6f6e 203d 2030 2e33 2e33 0d0a 6175 7468  on = 0.3.3..auth
 00000030: 6f72 203d 2059 696e 7368 656e 6720 5a68  or = Yinsheng Zh
 00000040: 616e 6720 2850 682e 442e 290d 0a61 7574  ang (Ph.D.)..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6f6f 407a  hor_email = oo@z
 00000060: 6a75 2e65 6475 2e63 6e0d 0a64 6573 6372  ju.edu.cn..descr
 00000070: 6970 7469 6f6e 203d 2041 2050 7974 686f  iption = A Pytho
 00000080: 6e20 6c69 6272 6172 7920 666f 7220 4e4e  n library for NN
 00000090: 5257 2028 6e65 7572 616c 206e 6574 776f  RW (neural netwo
```

### Comparing `pyNNRW-0.3.2/src/pyNNRW/__init__.py` & `pyNNRW-0.3.3/src/pyNNRW/__init__.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.2/src/pyNNRW/dtc.py` & `pyNNRW-0.3.3/src/pyNNRW/dtc.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.2/src/pyNNRW/elm.py` & `pyNNRW-0.3.3/src/pyNNRW/elm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 '''
+Major revisions: 
+1. added multi-class support 
+2. Encapsule ELM into a sklearn compatible estimator 
+
 This ELM implementation is based on https://github.com/otenim/Numpy-ELM: 
 
 MIT License
 
 Copyright (c) 2019 Otenim
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +31,15 @@
 import os
 import numpy as np
 import h5py
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.model_selection import GridSearchCV, train_test_split
 from . import to_categorical
 from sklearn.metrics import log_loss, accuracy_score, recall_score
-from sklearn.datasets import load_iris,load_digits
+from sklearn.preprocessing import OneHotEncoder
 # from keras import losses
 
 def _mean_squared_error(y_true, y_pred):
     return 0.5 * np.mean((y_true - y_pred)**2)
 
 def _mean_absolute_error(y_true, y_pred):
     return np.mean(np.abs(y_true - y_pred))
@@ -141,23 +145,34 @@
                 )
         if len(ret) == 1:
             ret = ret[0]
         elif len(ret) == 0:
             ret = None
         return ret
 
+    def _transform_label(self, y):
+        enc = OneHotEncoder(handle_unknown='ignore')
+        try:
+            target = enc.fit_transform(y).toarray()
+            # print('the label can be transformed directly using onehotencoder')
+        except:
+            target = enc.fit_transform(y.reshape(-1, 1)).toarray()
+            # print('the label must be reshaped before being transformed')
+        return target
 
     def fit(self, x, t):
+        one_hot_target = self._transform_label(t)
+
         H = self.__activation(x.dot(self.__alpha) + self.__bias)
 
         # compute a pseudoinverse of H
         H_pinv = np.linalg.pinv(H)
 
         # update beta
-        self.__beta = H_pinv.dot(t)
+        self.__beta = H_pinv.dot(one_hot_target)
 
     def save(self, filepath):
         with h5py.File(filepath, 'w') as f:
             arc = f.create_dataset('architecture', data=np.array([self.__n_input_nodes, self.__n_hidden_nodes, self.__n_output_nodes]))
             arc.attrs['activation'] = self.__get_activation_name(self.__activation).encode('utf-8')
             arc.attrs['loss'] = self.__get_loss_name(self.__loss).encode('utf-8')
             arc.attrs['name'] = self.name.encode('utf-8')
@@ -294,23 +309,27 @@
     '''
     
     def __init__(self, n_hidden_nodes = 20, activation = 'relu'):
         
         # ===============================
         # ELM parameters
         # ===============================
+        self.model = None # will be instantiated in fit()
+        self.classes_ = 0 # will be instantiated in fit()
+        self.n_features_in_ = 0 # will be instantiated in fit()
+
         self.n_hidden_nodes = n_hidden_nodes #x_train.shape[1]
         self.loss = 'mean_squared_error' # 'mean_absolute_error'
         self.activation = activation # 'sigmoid' # 'identity' # 'relu'
         
     def fit(self, X, y):
+        '''
+        Instantiate an inner ELM and fit it to the data
+        '''
         
-        # ===============================
-        # Instantiate ELM
-        # ===============================
         if len(y.shape) == 2: #one-hot
             n_classes = y.shape[1]
         else:
             n_classes = len(set(y))
 
         self.model = ELM(
             n_input_nodes = X.shape[1],
@@ -319,32 +338,32 @@
             loss = self.loss,
             activation = self.activation,
             name = 'elm'
         )
         
         self.classes_ = np.unique(y)
         self.model.fit(X, y)
+        self.n_features_in_ = X.shape[1] # n_features_in_ is the number of features that an estimator expects.
 
+    def predict_proba(self, X):
         '''
-        n_features_in_ is the number of features that an estimator expects.
-        In most cases, the n_features_in_ attribute exists only once fit has been called, but there are exceptions.
+        This doesn't return the probability directly, but the raw output from the ann.
+        You may call softmax() on the output to get the formalized probability. 
         '''
-        self.n_features_in_ = X.shape[1]
-
-    def predict_proba(self, X):        
-        yh = self.model.predict(X)
-        # print(yh) # array e.g., 0.37854525 0.         0.         
+        yh = self.model.predict(X) # this is a direct output from ann, e.g., 0.37854525 0.         0.         
         return yh
 
     def predict(self, X):
+        '''
+        return the class labels
+        '''
         yh = self.model.predict(X) # (m,  n_classes)
         if (len(yh.shape) <= 1): # e.g., (m, )
             return yh > 0.5 # default 0.5 threshold
         yh = np.argmax(yh, axis=-1)
-        # print(yh.shape)
         return yh
 
     def evaluate(self, val_x, val_y, metrics=['loss', 'accuracy']):
 
         if len(val_y.shape) == 2: #one-hot
             n_classes = val_y.shape[1]
             y_gt = val_y
@@ -403,18 +422,18 @@
         # Prediction
         # ===============================
         print("\n\n========== prediction on the first 10 test samples ===========\n")
         x = x_test[:10]
         t = t_test[:10]
         y_pred = clf.predict_proba(x)
 
-        for i in range(len(y_pred)):
+        for i, y_pred_i in enumerate(y_pred):
             print('---------- prediction %d ----------' % (i+1))
-            class_pred = np.argmax(y_pred[i])
-            prob_pred = y_pred[i][class_pred]
+            class_pred = np.argmax(y_pred_i)
+            prob_pred = y_pred_i[class_pred]
             class_true = np.argmax(t[i])
             print('class: %d, probability: %f' % (class_pred, prob_pred))
             print('class (true): %d' % class_true)
 
         if (save_model_path):
 
             # ===============================
@@ -425,29 +444,31 @@
             # ===============================
             # Load model
             # ===============================
             # clf.load_model(save_model_path)
 
     def run_iris_example():
 
+        from sklean.datasets import load_iris
+
         # ===============================
         # Load dataset
         # ===============================
         iris = load_iris()
         n_classes = len(set(iris.target))
         # stdsc = StandardScaler()
         # irisx = stdsc.fit_transform(iris.data)
         x_train, x_test, t_train, t_test = train_test_split(iris.data, iris.target, test_size=0.2)
         t_train = to_categorical(t_train, n_classes).astype(np.float32)
         t_test = to_categorical(t_test, n_classes).astype(np.float32)
 
         ELMClassifier.run_example(x_train, x_test, t_train, t_test)
 
     def run_mnist_example():
-
+        
         from keras.datasets import mnist
 
         n_classes = 10
         (x_train, t_train), (x_test, t_test) = mnist.load_data()
 
         # ===============================
         # Preprocess
```

### Comparing `pyNNRW-0.3.2/src/pyNNRW/knnrw.py` & `pyNNRW-0.3.3/src/pyNNRW/knnrw.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,18 +241,24 @@
     plt.imshow(cosine_similarity(X,X))
     plt.axis('off')
     plt.title('cosine kernel. \nK(X, Y) = <X, Y> / (||X||*||Y||) \nNo tunable params.')
     plt.show()
 
     return
 
-def KNNRWGridSearch(x_train, x_test, t_train, t_test, verbose = 0):
+def KNNRWClassifierGridSearch(x_train, x_test, t_train, t_test, K=22, verbose = 0):
+    '''
+    Perform a grid search for the best kernel combinations.
+
+    Parameters
+    ----------
+    K : int, the maximum kernel numbers. default = 22
+    '''
 
     N = x_train.shape[1]
-    K = 22
 
     taccs = []
     vaccs = []
         
     # Perform a grid search
     for flavor in ['sum','stack','stack+sum']:
         
@@ -301,28 +307,28 @@
         plt.title(flavor)
         plt.scatter(kernels, taccs[i], label = 'train acc')
         plt.scatter(kernels, vaccs[i], label = 'val acc')
         plt.legend()
         plt.xticks(rotation=-90)
         plt.show()
 
-    return taccs, vaccs    
+    return taccs, vaccs
 
 
 class KNNRWClassifier(BaseEstimator, ClassifierMixin):
     '''
     Encapsulate as a sklearn estimator
     '''
     def __init__(self, N = 1, kernels = 5, flavor = 'stack'):
         self.model = KNNRW(N = N, kernels = kernels, type="classification", flavor=flavor) 
 
     def fit(self, X, y, verbose = 0):     
         
         self.model.fit(X, y, verbose = verbose)
-        self.classes_ = np.array(list(set(y)))
+        # self.classes_ = np.array(list(set(y)))
 
     def predict(self, X_train, X_test):
         return self.model.predict(X_train, X_test)
 
     def predict_proba(self, X_train, X_test):
         return self.model.predict_proba(X_train, X_test)
```

### Comparing `pyNNRW-0.3.2/src/pyNNRW/mlp.py` & `pyNNRW-0.3.3/src/pyNNRW/mlp.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.2/src/pyNNRW/nnrw.py` & `pyNNRW-0.3.3/src/pyNNRW/nnrw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from . import to_categorical
-from .elm import *
-from .rvfl import *
-from .mlp import *
-from .dtc import *
-from .lr import *
-from .knn import *
+import warnings
+warnings.filterwarnings("ignore")
+
+import time
+import numpy as np
 import matplotlib.pyplot as plt
+import matplotlib.ticker as mticker
 from sklearn.base import BaseEstimator, ClassifierMixin
-from sklearn.model_selection import train_test_split, GridSearchCV
-from sklearn.ensemble import StackingClassifier
+from sklearn.model_selection import train_test_split
+from sklearn.linear_model import LogisticRegression
+from sklearn.ensemble import StackingClassifier #,HistGradientBoostingClassifier
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.svm import SVC
-from sklearn.multiclass import OneVsOneClassifier, OneVsRestClassifier
+from sklearn.multiclass import OneVsOneClassifier
 from sklearn.metrics import r2_score
-import numpy as np
-import time
-import matplotlib.ticker as mticker
 
-import warnings
-warnings.filterwarnings("ignore")
+from . import to_categorical
 
 #region Performance Test. Compare NNRW with mainstream classifier models.
 
 def ELMClf(X, y, L = 100, verbose = False):
     '''
     A wrapper for ELM.
     L represents the number of hidden layer nodes.
@@ -409,78 +405,137 @@
     
     return MTacc, MVacc, MT
 
 #endregion
 
 #region ensembles
 
-def homo_stacking(X, y, create_base_estimator, Ns = [1, 2, 5], Ls = [1, 2, 5, 10, 20], repeat = 10, WITH_CONTEXT = True, xlabel = ''):
+class LogisticRegressionX(LogisticRegression, ClassifierMixin):
+    '''
+    An extended version of logistic regression that handles NaN.
+    '''
+    
+    def __init__(
+        self,
+        penalty="l2",
+        tol=1e-4,
+        C=1.0,
+        l1_ratio=None):
+        
+        LogisticRegression.__init__(self, penalty = penalty, tol=tol, C=C, l1_ratio=l1_ratio)
+        
+    def fit(self, X, y):
+
+        X = np.nan_to_num(X)
+        y = np.nan_to_num(y)
+        clf = LogisticRegression.fit(self, X=X, y=y)
+        clf.coef_ = np.nan_to_num(clf.coef_)
+        clf.intercept_ = np.nan_to_num(clf.intercept_)
+        return clf
+
+    def predict_proba(self, X):
+        X = np.nan_to_num(X)       
+        yh = LogisticRegression.predict_proba(self, X=X)
+        yh = np.nan_to_num(yh)
+        return yh
+
+    def predict(self, X):
+        X = np.nan_to_num(X)
+        yp = LogisticRegression.predict(self, X=X)
+        yp = np.nan_to_num(yp)
+        return yp
+    
+    def score(self, X, y):
+        X = np.nan_to_num(X)
+        y = np.nan_to_num(y)
+        return LogisticRegression.score(X=X, y=y)   
+
+def homo_stacking(X, y, create_base_estimator, meta_learner = LogisticRegressionX,
+                  Ns = [1, 2, 5], Ls = [1, 2, 5, 10, 20], 
+                  test_size = .3, 
+                  random_state = None,
+                  WITH_CONTEXT = False, 
+                  xlabel = '',
+                  YLIM = (.5, 1.05)):
     '''
     create_base_estimator # a function that create base learner instanes
     Ns = [1, 2, 5] # number of base estimators
-    Ls = [1, 2, 5, 10, 20] # base learner's specific hyper-parameter
-    repeat = 10 # run multiple times to get the mean
+    Ls = [1, 2, 5, 10, 20] # base learner's specific hyper-parameter    
     '''
 
     # pbar = tqdm(total = repeat * len(Ns) * len(Ls), position=0, leave=True) # stay on top
 
+    X_train, X_test, y_train, y_test = train_test_split(
+        X, y, stratify=y, test_size=test_size, random_state=random_state,
+    )
+        
+    dic_acc = {}
+    repeat = 1 # no need to repeat, each run is now deterministic.
+
     plt.figure(figsize = (14, 6))
 
     for N in Ns:
         ACCs = []
 
         for L in Ls:        
 
-            acc = 0
-
-            for iter in range(repeat):
+            accs = []
 
-                X_train, X_test, y_train, y_test = train_test_split(
-                    X, y
-                )
+            for _ in range(repeat):
 
                 estimators = []
                 for i in range(N):
                     estimators.append((str(i), create_base_estimator(L))) # relu is better than logistic
 
                 clf = StackingClassifier(
-                    estimators=estimators, final_estimator=LogisticRegression(), passthrough = WITH_CONTEXT
+                    estimators=estimators, final_estimator=meta_learner(), passthrough = WITH_CONTEXT
                 )
 
-                acc = acc + clf.fit(X_train, y_train).score(X_test, y_test)
+                # acc = acc + clf.fit(X_train, y_train).score(X_test, y_test)
+                accs.append(clf.fit(X_train, y_train).score(X_test, y_test))
 
                 # pbar.update()
-
-            ACCs.append(acc / repeat)
+            
+            # remove the biggest and smallest from accs and get mean 
+            # print('acc of all runs:', np.round(accs,2))
+            averaged_acc = sum(accs)/repeat
+            if repeat >= 3:
+                averaged_acc = sum(sorted(accs)[1:-1]) / (len(accs) - 2)
+            
+            ACCs.append(averaged_acc)
+            dic_acc[(N, L)] = averaged_acc
 
         plt.plot(Ls, ACCs, '--', label = 'N='+str(N), marker='o') # fillstyle='none'
         # plt.scatter(Ls, ACCs, s = 50)
 
     plt.gca().xaxis.set_major_locator(mticker.MultipleLocator(1)) # only show integer
     plt.legend()
     plt.xlabel('Hyper-parameter' + xlabel)
     plt.ylabel("Classfication Accuracy")
+    plt.ylim(YLIM)
     plt.show()
 
-    return ACCs
+    print('best test accuracy: ', max(dic_acc.values()), 'N, L = ', [key for key, value in dic_acc.items() if value == max(dic_acc.values())])
+
+    return dic_acc
     
 def hetero_stacking(X, y, estimators, repeat = 10, WITH_CONTEXT = True):
     '''
     estimators: a batch of base learners. Each learner should be derived from the BaseEstimator type.    
     '''
     acc = 0
     
     for iter in range(repeat):
 
         X_train, X_test, y_train, y_test = train_test_split(
             X, y
         )
 
         clf = StackingClassifier(
-            estimators=estimators, final_estimator=LogisticRegression(), passthrough = WITH_CONTEXT
+            estimators=estimators, final_estimator=LogisticRegressionCV(), passthrough = WITH_CONTEXT
         )
 
         acc = acc + clf.fit(X_train, y_train).score(X_test, y_test)
     
     return acc / repeat
 
 class FSSE(BaseEstimator, ClassifierMixin):
```

### Comparing `pyNNRW-0.3.2/src/pyNNRW/rbfnn.py` & `pyNNRW-0.3.3/src/pyNNRW/rbfnn.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.2/src/pyNNRW/rbm.py` & `pyNNRW-0.3.3/src/pyNNRW/rbm.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.2/src/pyNNRW/wann.py` & `pyNNRW-0.3.3/src/pyNNRW/wann.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.2/src/pyNNRW.egg-info/PKG-INFO` & `pyNNRW-0.3.3/src/pyNNRW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNNRW
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python library for NNRW (neural network with random weights)
 Home-page: https://github.com/zhangys11/pyNNRW
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/pyNNRW/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

