# Comparing `tmp/poismf-0.4.0.post6.tar.gz` & `tmp/poismf-0.4.0.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poismf-0.4.0.post6.tar", last modified: Sat Mar 25 16:56:05 2023, max compression
+gzip compressed data, was "poismf-0.4.0.post7.tar", last modified: Mon Jul  3 18:48:43 2023, max compression
```

## Comparing `poismf-0.4.0.post6.tar` & `poismf-0.4.0.post7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:56:05.571497 poismf-0.4.0.post6/
--rw-r--r--   0 david     (1000) david     (1000)     1322 2022-02-23 22:22:19.000000 poismf-0.4.0.post6/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      656 2021-08-24 23:08:41.000000 poismf-0.4.0.post6/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      232 2023-03-25 16:56:05.571497 poismf-0.4.0.post6/PKG-INFO
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:56:05.571497 poismf-0.4.0.post6/poismf/
--rw-r--r--   0 david     (1000) david     (1000)    51160 2022-05-30 19:59:51.000000 poismf-0.4.0.post6/poismf/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      120 2023-03-19 16:12:38.000000 poismf-0.4.0.post6/poismf/cfuns_double.pyx
--rw-r--r--   0 david     (1000) david     (1000)      118 2023-03-19 16:12:36.000000 poismf-0.4.0.post6/poismf/cfuns_float.pyx
--rw-r--r--   0 david     (1000) david     (1000)    13270 2022-02-23 21:18:16.000000 poismf-0.4.0.post6/poismf/poismf_c_wrapper.pxi
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:56:05.571497 poismf-0.4.0.post6/poismf.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      232 2023-03-25 16:56:05.000000 poismf-0.4.0.post6/poismf.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      386 2023-03-25 16:56:05.000000 poismf-0.4.0.post6/poismf.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-03-25 16:56:05.000000 poismf-0.4.0.post6/poismf.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       32 2023-03-25 16:56:05.000000 poismf-0.4.0.post6/poismf.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        7 2023-03-25 16:56:05.000000 poismf-0.4.0.post6/poismf.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       95 2021-06-24 17:47:12.000000 poismf-0.4.0.post6/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       32 2021-06-24 17:47:12.000000 poismf-0.4.0.post6/requirements.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-03-25 16:56:05.571497 poismf-0.4.0.post6/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    11208 2023-03-25 16:55:40.000000 poismf-0.4.0.post6/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:56:05.571497 poismf-0.4.0.post6/src/
--rw-r--r--   0 david     (1000) david     (1000)    13888 2022-02-23 22:22:28.000000 poismf-0.4.0.post6/src/nonnegcg.c
--rw-r--r--   0 david     (1000) david     (1000)    23148 2022-02-23 22:22:34.000000 poismf-0.4.0.post6/src/poismf.c
--rw-r--r--   0 david     (1000) david     (1000)    10465 2022-02-23 22:22:40.000000 poismf-0.4.0.post6/src/poismf.h
--rw-r--r--   0 david     (1000) david     (1000)     9812 2022-02-23 22:22:48.000000 poismf-0.4.0.post6/src/pred.c
--rw-r--r--   0 david     (1000) david     (1000)    66204 2021-07-27 17:42:06.000000 poismf-0.4.0.post6/src/tnc.c
--rw-r--r--   0 david     (1000) david     (1000)     7485 2020-05-29 15:47:53.000000 poismf-0.4.0.post6/src/tnc.h
--rw-r--r--   0 david     (1000) david     (1000)     9976 2022-02-23 22:55:21.000000 poismf-0.4.0.post6/src/topN.c
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/
+-rw-r--r--   0 david     (1000) david     (1000)     1322 2022-02-23 22:22:19.000000 poismf-0.4.0.post7/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      656 2021-08-24 23:08:41.000000 poismf-0.4.0.post7/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      232 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/PKG-INFO
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/poismf/
+-rw-r--r--   0 david     (1000) david     (1000)    51161 2023-07-03 18:46:03.000000 poismf-0.4.0.post7/poismf/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      120 2023-03-19 16:12:38.000000 poismf-0.4.0.post7/poismf/cfuns_double.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      118 2023-03-19 16:12:36.000000 poismf-0.4.0.post7/poismf/cfuns_float.pyx
+-rw-r--r--   0 david     (1000) david     (1000)    13270 2022-02-23 21:18:16.000000 poismf-0.4.0.post7/poismf/poismf_c_wrapper.pxi
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/poismf.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      232 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      386 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       32 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)        7 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       95 2021-06-24 17:47:12.000000 poismf-0.4.0.post7/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       40 2023-07-03 18:41:24.000000 poismf-0.4.0.post7/requirements.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    11208 2023-07-03 18:41:07.000000 poismf-0.4.0.post7/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/src/
+-rw-r--r--   0 david     (1000) david     (1000)    13888 2022-02-23 22:22:28.000000 poismf-0.4.0.post7/src/nonnegcg.c
+-rw-r--r--   0 david     (1000) david     (1000)    23148 2022-02-23 22:22:34.000000 poismf-0.4.0.post7/src/poismf.c
+-rw-r--r--   0 david     (1000) david     (1000)    10465 2022-02-23 22:22:40.000000 poismf-0.4.0.post7/src/poismf.h
+-rw-r--r--   0 david     (1000) david     (1000)     9812 2022-02-23 22:22:48.000000 poismf-0.4.0.post7/src/pred.c
+-rw-r--r--   0 david     (1000) david     (1000)    66204 2021-07-27 17:42:06.000000 poismf-0.4.0.post7/src/tnc.c
+-rw-r--r--   0 david     (1000) david     (1000)     7485 2020-05-29 15:47:53.000000 poismf-0.4.0.post7/src/tnc.h
+-rw-r--r--   0 david     (1000) david     (1000)     9976 2022-02-23 22:55:21.000000 poismf-0.4.0.post7/src/topN.c
```

### Comparing `poismf-0.4.0.post6/LICENSE` & `poismf-0.4.0.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/MANIFEST.in` & `poismf-0.4.0.post7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/poismf/__init__.py` & `poismf-0.4.0.post7/poismf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd, numpy as np
 import multiprocessing, os, warnings, ctypes
-from scipy.sparse import coo_matrix, csr_matrix, csc_matrix, isspmatrix_coo, isspmatrix_csr
+from scipy.sparse import issparse, coo_array
 from copy import deepcopy
 from . import c_funs_double, c_funs_float
 
 __all__ = ["PoisMF"]
 
 class PoisMF:
     """
@@ -140,15 +140,15 @@
     random_state : int, RandomState, or Generator
         Random seed to use to initialize model parameters. If passing a NumPy
         'RandomState', will use it to draw a random integer as initial seed.
         If passing a NumPy 'Generator', will use it directly for drawing
         random numbers.
     reindex : bool
         Whether to reindex data internally. Will be ignored if passing a sparse
-        COO matrix to 'fit'.
+        COO array/matrix to 'fit'.
     copy_data : bool
         Whether to make deep copies of the data in order to avoid modifying it in-place.
         Passing 'False' is faster, but might modify the 'X' inputs in-place if they
         are DataFrames.
     produce_dicts : bool
         Whether to produce Python dictionaries for users and items, which
         are used to speed-up the prediction API of this package. You can still
@@ -341,15 +341,15 @@
         ----------
         X : Pandas DataFrame (nobs, 3) or COO(m, n)
             Counts atrix to factorize, in sparse triplets format. Can be passed either
             as a SciPy sparse COO matrix (recommended) with users being rows and
             items being columns, or as a Pandas DataFrame, in which case it should
             have the following columns: 'UserId', 'ItemId', 'Count'.
             Combinations of users and items not present are implicitly assumed to be zero by the model. The non-missing entries must all be greater than zero.
-            If passing a COO matrix, will force 'reindex' to 'False'.
+            If passing a COO array/matrix, will force 'reindex' to 'False'.
 
         Returns
         -------
         self : obj
             This object
         """
         self._init(
@@ -373,15 +373,15 @@
         self.is_fitted = True
         return self
     
     def _process_data(self, X):
         if self.copy_data:
             X = X.copy()
 
-        if isspmatrix_coo(X):
+        if issparse(X) and (X.format == "coo"):
             self.nusers = X.shape[0]
             self.nitems = X.shape[1]
             self.reindex = False
             coo = X
 
         elif isinstance(X, pd.DataFrame):
             cols_require = ["UserId", "ItemId", "Count"]
@@ -395,22 +395,22 @@
                 X['ItemId'], self.item_mapping_ = pd.factorize(X.ItemId)
                 ### https://github.com/pandas-dev/pandas/issues/30618
                 self.user_mapping_ = self.user_mapping_.to_numpy()
                 self.item_mapping_ = self.item_mapping_.to_numpy()
                 self.user_mapping_ = self.user_mapping_
                 self.item_mapping_ = self.item_mapping_
 
-            coo = coo_matrix((X.Count, (X.UserId, X.ItemId)))
+            coo = coo_array((X.Count, (X.UserId, X.ItemId)))
 
         else:
             raise ValueError("'X' must be a pandas DataFrame or SciPy COO matrix.")
 
         self.nusers, self.nitems = coo.shape[0], coo.shape[1]
-        csr = csr_matrix(coo)
-        csc = csc_matrix(coo)
+        csr = coo.tocsr()
+        csc = coo.tocsc()
 
         csr.indptr  = csr.indptr.astype(ctypes.c_size_t)
         csr.indices = csr.indices.astype(ctypes.c_size_t)
         if csr.data.dtype != self._dtype:
             csr.data  = csr.data.astype(self._dtype)
         csc.indptr  = csc.indptr.astype(ctypes.c_size_t)
         csc.indices = csc.indices.astype(ctypes.c_size_t)
@@ -650,16 +650,16 @@
         X : DataFrame(nnz, 3), CSR(n_new, nitems), or COO(n_new, nitems)
             New matrix for which to determine latent factors. The items/columns
             must be the same ones as passed to 'fit', while the rows correspond
             to new entries that were not passed to 'fit'.
                 * If passing a DataFrame, must have columns 'UserId', 'ItemId', 'Count'.
                   The 'UserId' column will be remapped, with the mapping returned as
                   part of the output.
-                * If passing a COO matrix, will be casted to CSR.
-                * If passing a CSR matrix (recommended), will use it as-is and will
+                * If passing a COO array/matrix, will be casted to CSR.
+                * If passing a CSR array/matrix (recommended), will use it as-is and will
                   not return a mapping as the output will match row-by-row with 'X'.
         y : None
             Ignored. Kept in place for compatibility with SciKit-Learn pipelining.
 
         Returns
         -------
         A_new : array(n_new, k)
@@ -704,21 +704,21 @@
         if isinstance(X, pd.DataFrame):
             cols_require = ["UserId", "ItemId", "Count"]
             if np.setdiff1d(np.array(cols_require), X.columns.values).shape[0]:
                 raise ValueError("'X' must contain columns " + ", ".join(cols_require))
             X["UserId"], user_mapping_ = pd.factorize(X.UserId)
             if self.reindex:
                 X["ItemId"] = pd.Categorical(X.ItemId, self.item_mapping_).codes
-            X = csr_matrix(coo_matrix((X.Count, (X.UserId, X.ItemId))))
+            X = coo_array((X.Count, (X.UserId, X.ItemId))).tocsr()
         else:
             if self.reindex:
                 raise ValueError("'X' must be a DataFrame if using 'reindex=True'.")
-            if isspmatrix_coo(X):
-                X = csr_matrix(X)
-            elif not isspmatrix_csr(X):
+            if issparse(X) and (X.format != "csr"):
+                X = X.tocsr()
+            else:
                 raise ValueError("'X' must be a DataFrame, CSR matrix, or COO matrix.")
             user_mapping_ = np.empty(0, dtype=int)
 
         if X.shape[1] > self.nitems:
             raise ValueError("'X' must have the same columns (items) as passed to 'fit'.")
 
         return (
@@ -1129,17 +1129,17 @@
             return (
                 X_test.UserId.to_numpy(),
                 X_test.ItemId.to_numpy(),
                 X_test.Count.to_numpy()
             )
         else:
             if isinstance(X_test, pd.DataFrame):
-                X_test = coo_matrix((X_test.Count, (X_test.UserId, X_test.ItemId)))
+                X_test = coo_array((X_test.Count, (X_test.UserId, X_test.ItemId)))
             else:
-                if isspmatrix_coo(X_test):
+                if not (issparse(X_test) and (X_test.format == "coo")):
                     raise ValueError("'X_test' must be a DataFrame or COO matrix.")
 
         if X_test.shape[0] > self.nusers:
             raise ValueError("'X_test' cannot contain new users/rows.")
         if X_test.shape[1] > self.nitems:
             raise ValueError("'X_test' cannot contain new items/columns.")
```

### Comparing `poismf-0.4.0.post6/poismf/poismf_c_wrapper.pxi` & `poismf-0.4.0.post7/poismf/poismf_c_wrapper.pxi`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/setup.py` & `poismf-0.4.0.post7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 from_rtd = os.environ.get('READTHEDOCS') == 'True'
 if not from_rtd:
     setup(
         name  = "poismf",
         packages = ["poismf"],
         author = 'David Cortes',
         url = 'https://github.com/david-cortes/poismf',
-        version = '0.4.0-6',
+        version = '0.4.0-7',
         install_requires = ['numpy', 'pandas>=0.24', 'cython', 'scipy'],
         description = 'Fast and memory-efficient Poisson factorization for sparse count matrices',
         cmdclass = {'build_ext': build_ext_subclass},
         ext_modules = [
             Extension("poismf.c_funs_double",
                 sources=["poismf/cfuns_double.pyx",
                          "src/poismf.c", "src/topN.c", "src/pred.c",
```

### Comparing `poismf-0.4.0.post6/src/nonnegcg.c` & `poismf-0.4.0.post7/src/nonnegcg.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/src/poismf.c` & `poismf-0.4.0.post7/src/poismf.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/src/poismf.h` & `poismf-0.4.0.post7/src/poismf.h`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/src/pred.c` & `poismf-0.4.0.post7/src/pred.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/src/tnc.c` & `poismf-0.4.0.post7/src/tnc.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/src/tnc.h` & `poismf-0.4.0.post7/src/tnc.h`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post6/src/topN.c` & `poismf-0.4.0.post7/src/topN.c`

 * *Files identical despite different names*

