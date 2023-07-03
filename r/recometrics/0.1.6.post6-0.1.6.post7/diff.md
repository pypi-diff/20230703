# Comparing `tmp/recometrics-0.1.6.post6.tar.gz` & `tmp/recometrics-0.1.6.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recometrics-0.1.6.post6.tar", last modified: Sat Mar 25 16:57:14 2023, max compression
+gzip compressed data, was "recometrics-0.1.6.post7.tar", last modified: Mon Jul  3 18:57:17 2023, max compression
```

## Comparing `recometrics-0.1.6.post6.tar` & `recometrics-0.1.6.post7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:57:14.878817 recometrics-0.1.6.post6/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2021-06-22 23:08:42.000000 recometrics-0.1.6.post6/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      700 2021-07-12 00:19:42.000000 recometrics-0.1.6.post6/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      248 2023-03-25 16:57:14.878817 recometrics-0.1.6.post6/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)       95 2022-01-20 17:22:42.000000 recometrics-0.1.6.post6/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:57:14.878817 recometrics-0.1.6.post6/recometrics/
--rw-r--r--   0 david     (1000) david     (1000)    38824 2021-07-25 03:35:54.000000 recometrics-0.1.6.post6/recometrics/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      951 2023-03-19 19:44:14.000000 recometrics-0.1.6.post6/recometrics/wrapper.h
--rw-r--r--   0 david     (1000) david     (1000)    27794 2023-03-19 17:25:07.000000 recometrics-0.1.6.post6/recometrics/wrapper.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:57:14.878817 recometrics-0.1.6.post6/recometrics.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      248 2023-03-25 16:57:14.000000 recometrics-0.1.6.post6/recometrics.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      371 2023-03-25 16:57:14.000000 recometrics-0.1.6.post6/recometrics.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-03-25 16:57:14.000000 recometrics-0.1.6.post6/recometrics.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       26 2023-03-25 16:57:14.000000 recometrics-0.1.6.post6/recometrics.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       12 2023-03-25 16:57:14.000000 recometrics-0.1.6.post6/recometrics.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-03-25 16:57:14.878817 recometrics-0.1.6.post6/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    13482 2023-03-25 16:56:46.000000 recometrics-0.1.6.post6/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:57:14.878817 recometrics-0.1.6.post6/src/
--rw-r--r--   0 david     (1000) david     (1000)    64977 2023-02-16 17:41:12.000000 recometrics-0.1.6.post6/src/recometrics.hpp
--rw-r--r--   0 david     (1000) david     (1000)    10477 2021-07-25 03:17:47.000000 recometrics-0.1.6.post6/src/recometrics_instantiated.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7426 2021-07-25 03:17:28.000000 recometrics-0.1.6.post6/src/recometrics_signatures.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/
+-rw-r--r--   0 david     (1000) david     (1000)     1317 2021-06-22 23:08:42.000000 recometrics-0.1.6.post7/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      700 2021-07-12 00:19:42.000000 recometrics-0.1.6.post7/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)       95 2022-01-20 17:22:42.000000 recometrics-0.1.6.post7/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/recometrics/
+-rw-r--r--   0 david     (1000) david     (1000)    38717 2023-07-03 18:56:28.000000 recometrics-0.1.6.post7/recometrics/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      951 2023-07-03 18:55:43.000000 recometrics-0.1.6.post7/recometrics/wrapper.h
+-rw-r--r--   0 david     (1000) david     (1000)    27792 2023-07-03 18:53:43.000000 recometrics-0.1.6.post7/recometrics/wrapper.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/recometrics.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      371 2023-07-03 18:57:17.000000 recometrics-0.1.6.post7/recometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       26 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       12 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    13482 2023-07-03 18:49:26.000000 recometrics-0.1.6.post7/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/src/
+-rw-r--r--   0 david     (1000) david     (1000)    64977 2023-02-16 17:41:12.000000 recometrics-0.1.6.post7/src/recometrics.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    10477 2021-07-25 03:17:47.000000 recometrics-0.1.6.post7/src/recometrics_instantiated.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7426 2021-07-25 03:17:28.000000 recometrics-0.1.6.post7/src/recometrics_signatures.hpp
```

### Comparing `recometrics-0.1.6.post6/LICENSE` & `recometrics-0.1.6.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post6/MANIFEST.in` & `recometrics-0.1.6.post7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post6/recometrics/__init__.py` & `recometrics-0.1.6.post7/recometrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np, pandas as pd
 from . import cpp_funs
-from scipy.sparse import issparse, isspmatrix_csr, csr_matrix
+from scipy.sparse import issparse, csr_array
 from warnings import warn
 import re
 import multiprocessing
 import ctypes
 
 __all__ = ["calc_reco_metrics", "split_reco_train_test"]
 
@@ -27,14 +27,23 @@
 def _cast_indices_to_int32(X):
     if (X.indptr.dtype != np.int32) or (X.indices.dtype != np.int32):
         X = X.copy()
         X.indptr = X.indptr.astype(np.int32)
         X.indices = X.indices.astype(np.int32)
     return X
 
+def _as_csr(X):
+    if issparse(X):
+        if X.format != "csr":
+            X = X.tocsr()
+        X.sort_indices()
+        return X
+    else:
+        return csr_array(X)
+
 
 def calc_reco_metrics(
     X_train, X_test,
     A, B,
     k = 5,
     item_biases = None,
     as_df = True,
@@ -249,15 +258,15 @@
     X_train : CSR(m, n) or None
         Training data for user-item interactions, with users denoting rows,
         items denoting columns, and values corresponding to confidence scores.
         Entries in ``X_train`` and ``X_test`` for each user should not intersect (that is,
         if an item is the training data as a non-missing entry, it should not be in
         the test data as non-missing, and vice versa).
         
-        Should be passed as a sparse matrix in CSR format
+        Should be passed as a sparse array/matrix in CSR format
         from SciPy. Items not consumed by the user should not
         be present in this matrix.
         
         Alternatively, if there is no training data, can pass ``None``, in which case it
         will look only at the test data.
         
         This matrix and ``X_test`` are not meant to contain negative values, and if
@@ -456,15 +465,15 @@
     if (B.shape[0] > X_test.shape[1]):
         warn("'B' has more items than 'X_test'.")
         B = B[:X_test.shape[1], :]
 
     use_float = (A.dtype == ctypes.c_float) and (B.dtype == ctypes.c_float)
 
     if X_train is None:
-        X_train = csr_matrix(X_test.shape, dtype=ctypes.c_double if not use_float else ctypes.c_float)
+        X_train = csr_array(X_test.shape, dtype=ctypes.c_double if not use_float else ctypes.c_float)
         consider_cold_start = True
 
     assert issparse(X_train)
     assert X_train.shape[1] == X_test.shape[1]
     if (X_train.shape[0] < X_test.shape[0]):
         raise ValueError("'X_train' and 'X_test' should have the same number of rows.")
     elif (X_train.shape[0] > X_test.shape[0]):
@@ -537,24 +546,16 @@
             warn("'item_biases' has more items than 'X_test'.")
         
         item_biases = _cast_to_dtype(item_biases, use_float)
         A = np.c_[A, np.ones((A.shape[0], 1), dtype=ctypes.c_double if not use_float else ctypes.c_float)]
         B = np.c_[B, item_biases.reshape((-1,1))]
         item_biases = None
 
-    if not isspmatrix_csr(X_train):
-        X_train = csr_matrix(X_train)
-    else:
-        X_train.sort_indices()
-
-    if not isspmatrix_csr(X_test):
-        X_test = csr_matrix(X_test)
-    else:
-        if (not roc_auc) and (not pr_auc):
-            X_test.sort_indices()
+    X_train = _as_csr(X_train)
+    X_test = _as_csr(X_test)
     
     X_train = _cast_indices_to_int32(X_train)
     X_test = _cast_to_dtype(X_test, use_float)
     X_test = _cast_indices_to_int32(X_test)
     A = _cast_to_dtype(A, use_float)
     A, lda = _as_row_major(A)
     B = _cast_to_dtype(B, use_float)
@@ -681,15 +682,15 @@
           capabilities for producing factors/recommendations for users which where not in the
           training data, and this option then comes in handy.
 
     Parameters
     ----------
     X : CSR(m, n)
         The implicit feedback data to split into training-testing-remainder
-        for evaluating recommender systems. Should be passed as a sparse CSR matrix from
+        for evaluating recommender systems. Should be passed as a sparse CSR array/matrix from
         SciPy, or will be converted to CSR if it isn't. Users should correspond to rows, items
         to columns, and non-zero values to observed user-item interactions.
 
         Note that the indices of this matrix will be sorted in-place if it is passed as CSR.
         The data must be of type ``np.float32`` or ``np.float64`` - will be converted to
         ``np.float64`` if it is of a different type.
     split_type : str
@@ -743,19 +744,19 @@
 
     Returns
     -------
     split : tuple
         Will return a tuple with two to four elements depending on the requested split
         type:
             * If passing ``split_type='all'``, will output 2 elements: "X_train" and "X_test",
-              both of which will be sparse CSR matrices
+              both of which will be sparse CSR array/matrices
               with the same number of rows and columns as the ``X`` that was passed as input.
             * If passing ``split_type='separated'``, will output 4 elements: "X_train" and "X_test"
               as above (but with a number of rows corresponding to the number of selected test
-              users instead), plus another CSR matrix "X_rem" which will contain the
+              users instead), plus another CSR array/matrix "X_rem" which will contain the
               data for the remainder of the users (those which were not selected for testing and
               on which the recommendation model is meant to be fitted), and finally "users_test"
               which will be an integer vector containing the indices of the users/rows in ``X``
               which were selected for testing. The selected test users will be in sorted order,
               and the remaining data will remain in sorted order with the test users removed
               (e.g. if there's 5 users, with the second and fifth selected for testing, then
               "X_train" and "X_test" will contain rows [2,5] of ``X``, while "X_rem" will contain
@@ -809,18 +810,15 @@
             n_users_take = round(n_users_take)
             n_users_take = min(n_users_take, max_test_users)
         else:
             if max_test_users > X.shape[0]:
                 warn("'max_test_users' is larger than number of users. Will take all.")
             n_users_take = min(max_test_users, X.shape[0])
 
-    if not isspmatrix_csr(X):
-        X = csr_matrix(X)
-    else:
-        X.sort_indices()
+    X = _as_csr(X)
     if (not X.shape[0]) or (not X.shape[1]):
         raise ValueError("'X' cannot be empty.")
     if X.dtype not in (np.float32, np.float64):
         X = X.astype(np.float64)
     if not X.data.shape[0]:
         raise ValueError("'X' contains no non-zero entries.")
     X = _cast_indices_to_int32(X)
```

### Comparing `recometrics-0.1.6.post6/recometrics/wrapper.h` & `recometrics-0.1.6.post7/recometrics/wrapper.h`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post6/recometrics/wrapper.pyx` & `recometrics-0.1.6.post7/recometrics/wrapper.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #cython: language_level=3
 import numpy as np
 cimport numpy as np
 from libcpp cimport bool as c_bool
 from libcpp.vector cimport vector
 from libc.string cimport memcpy
 from libc.stdint cimport int32_t, uint64_t
-from scipy.sparse import csr_matrix
+from scipy.sparse import csr_array
 import ctypes
 from scipy.linalg.cython_blas cimport ddot, sdot
 
 ### TODO: here cython fails to compile the functions using fused types or templates,
 ### and depending on how it's done (fused/templates), might produce something compilable
 ### with gcc/clang but not with msvc. Find out why it fails and avoid this duplication
 ### of code. Perhaps it has to do with this issue:
@@ -512,15 +512,15 @@
     vector[generic_t] Xcsr,
     int32_t n
 ):
     cdef np.ndarray[int32_t, ndim=1] Xcsr_p_ = cppvec_to_numpy[int32_t](Xcsr_p)
     cdef np.ndarray[int32_t, ndim=1] Xcsr_i_ = cppvec_to_numpy[int32_t](Xcsr_i)
     cdef np.ndarray[generic_t, ndim=1] Xcsr_ = cppvec_to_numpy[generic_t](Xcsr)
     cdef int m = Xcsr_p_.shape[0] - 1
-    return csr_matrix((Xcsr_, Xcsr_i_, Xcsr_p_), shape=(m, n))
+    return csr_array((Xcsr_, Xcsr_i_, Xcsr_p_), shape=(m, n))
 
 cdef tuple split_csr_selected_users_double(
     X_csr_scipy,
     const double test_fraction,
     uint64_t seed = 1
 ):
     cdef np.ndarray[int32_t, ndim=1] X_csr_p = X_csr_scipy.indptr
```

### Comparing `recometrics-0.1.6.post6/setup.py` & `recometrics-0.1.6.post7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
                 e.define_macros += [("SUPPORTS_RESTRICT", "1")]
 
 
 
 setup(
     name  = "recometrics",
     packages = ["recometrics"],
-    version = '0.1.6-6',
+    version = '0.1.6-7',
     cmdclass = {'build_ext': build_ext_subclass},
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/recometrics',
     install_requires = ['numpy', 'scipy', 'cython', 'pandas'],
     description = 'Library-agnostic evaluation framework for implicit-feedback recommender systems',
     ext_modules = [
         Extension("recometrics.cpp_funs",
```

### Comparing `recometrics-0.1.6.post6/src/recometrics.hpp` & `recometrics-0.1.6.post7/src/recometrics.hpp`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post6/src/recometrics_instantiated.cpp` & `recometrics-0.1.6.post7/src/recometrics_instantiated.cpp`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post6/src/recometrics_signatures.hpp` & `recometrics-0.1.6.post7/src/recometrics_signatures.hpp`

 * *Files identical despite different names*

