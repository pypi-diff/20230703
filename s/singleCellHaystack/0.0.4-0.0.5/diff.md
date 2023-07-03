# Comparing `tmp/singleCellHaystack-0.0.4.tar.gz` & `tmp/singleCellHaystack-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singleCellHaystack-0.0.4.tar", last modified: Fri Jan 13 06:39:07 2023, max compression
+gzip compressed data, was "singleCellHaystack-0.0.5.tar", last modified: Mon Jul  3 12:20:36 2023, max compression
```

## Comparing `singleCellHaystack-0.0.4.tar` & `singleCellHaystack-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 diez       (501) staff       (20)        0 2023-01-13 06:39:07.686137 singleCellHaystack-0.0.4/
--rw-r--r--   0 diez       (501) staff       (20)     1067 2022-06-17 05:20:46.000000 singleCellHaystack-0.0.4/LICENSE
--rw-r--r--   0 diez       (501) staff       (20)       38 2022-08-24 04:18:37.000000 singleCellHaystack-0.0.4/MANIFEST.in
--rw-r--r--   0 diez       (501) staff       (20)     4274 2023-01-13 06:39:07.685804 singleCellHaystack-0.0.4/PKG-INFO
--rw-r--r--   0 diez       (501) staff       (20)     2269 2023-01-12 05:32:40.000000 singleCellHaystack-0.0.4/README.md
--rw-r--r--   0 diez       (501) staff       (20)      999 2023-01-13 06:35:49.000000 singleCellHaystack-0.0.4/pyproject.toml
--rw-r--r--   0 diez       (501) staff       (20)       38 2023-01-13 06:39:07.686236 singleCellHaystack-0.0.4/setup.cfg
-drwxr-xr-x   0 diez       (501) staff       (20)        0 2023-01-13 06:39:07.681309 singleCellHaystack-0.0.4/singleCellHaystack/
--rw-r--r--   0 diez       (501) staff       (20)      240 2023-01-04 05:27:48.000000 singleCellHaystack-0.0.4/singleCellHaystack/__init__.py
--rw-r--r--   0 diez       (501) staff       (20)     4100 2023-01-13 06:25:34.000000 singleCellHaystack-0.0.4/singleCellHaystack/_cluster.py
--rw-r--r--   0 diez       (501) staff       (20)      168 2022-08-26 05:34:28.000000 singleCellHaystack-0.0.4/singleCellHaystack/_data.py
--rw-r--r--   0 diez       (501) staff       (20)      893 2022-12-23 05:47:13.000000 singleCellHaystack-0.0.4/singleCellHaystack/_grid.py
--rw-r--r--   0 diez       (501) staff       (20)     6302 2023-01-04 05:27:48.000000 singleCellHaystack-0.0.4/singleCellHaystack/_haystack.py
--rw-r--r--   0 diez       (501) staff       (20)     1315 2022-09-02 08:45:42.000000 singleCellHaystack-0.0.4/singleCellHaystack/_kld.py
--rw-r--r--   0 diez       (501) staff       (20)     2664 2023-01-06 07:22:10.000000 singleCellHaystack-0.0.4/singleCellHaystack/_plot.py
--rw-r--r--   0 diez       (501) staff       (20)     3947 2022-09-02 08:45:42.000000 singleCellHaystack-0.0.4/singleCellHaystack/_pvalue.py
--rw-r--r--   0 diez       (501) staff       (20)     1251 2022-09-02 08:45:42.000000 singleCellHaystack-0.0.4/singleCellHaystack/_randomization.py
-drwxr-xr-x   0 diez       (501) staff       (20)        0 2023-01-13 06:39:07.683518 singleCellHaystack-0.0.4/singleCellHaystack/datasets/
--rw-r--r--   0 diez       (501) staff       (20)   223111 2022-08-24 04:18:37.000000 singleCellHaystack-0.0.4/singleCellHaystack/datasets/toy.h5ad
-drwxr-xr-x   0 diez       (501) staff       (20)        0 2023-01-13 06:39:07.682984 singleCellHaystack-0.0.4/singleCellHaystack.egg-info/
--rw-r--r--   0 diez       (501) staff       (20)     4274 2023-01-13 06:39:07.000000 singleCellHaystack-0.0.4/singleCellHaystack.egg-info/PKG-INFO
--rw-r--r--   0 diez       (501) staff       (20)      562 2023-01-13 06:39:07.000000 singleCellHaystack-0.0.4/singleCellHaystack.egg-info/SOURCES.txt
--rw-r--r--   0 diez       (501) staff       (20)        1 2023-01-13 06:39:07.000000 singleCellHaystack-0.0.4/singleCellHaystack.egg-info/dependency_links.txt
--rw-r--r--   0 diez       (501) staff       (20)       52 2023-01-13 06:39:07.000000 singleCellHaystack-0.0.4/singleCellHaystack.egg-info/requires.txt
--rw-r--r--   0 diez       (501) staff       (20)       19 2023-01-13 06:39:07.000000 singleCellHaystack-0.0.4/singleCellHaystack.egg-info/top_level.txt
+drwxrwxr-x   0 diez      (1000) diez      (1000)        0 2023-07-03 12:20:36.962246 singleCellHaystack-0.0.5/
+-rw-rw-r--   0 diez      (1000) diez      (1000)     1067 2023-05-14 04:37:57.000000 singleCellHaystack-0.0.5/LICENSE
+-rw-rw-r--   0 diez      (1000) diez      (1000)       38 2023-05-14 04:37:57.000000 singleCellHaystack-0.0.5/MANIFEST.in
+-rw-rw-r--   0 diez      (1000) diez      (1000)     4406 2023-07-03 12:20:36.962246 singleCellHaystack-0.0.5/PKG-INFO
+-rw-rw-r--   0 diez      (1000) diez      (1000)     2456 2023-07-01 11:42:33.000000 singleCellHaystack-0.0.5/README.md
+-rw-rw-r--   0 diez      (1000) diez      (1000)     1018 2023-07-03 12:15:51.000000 singleCellHaystack-0.0.5/pyproject.toml
+-rw-rw-r--   0 diez      (1000) diez      (1000)       38 2023-07-03 12:20:36.962246 singleCellHaystack-0.0.5/setup.cfg
+drwxrwxr-x   0 diez      (1000) diez      (1000)        0 2023-07-03 12:20:36.962246 singleCellHaystack-0.0.5/singleCellHaystack/
+-rw-rw-r--   0 diez      (1000) diez      (1000)      262 2023-05-14 04:37:57.000000 singleCellHaystack-0.0.5/singleCellHaystack/__init__.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)     4174 2023-05-14 04:37:57.000000 singleCellHaystack-0.0.5/singleCellHaystack/_cluster.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)      187 2023-07-01 08:25:07.000000 singleCellHaystack-0.0.5/singleCellHaystack/_data.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)      893 2023-05-14 04:37:57.000000 singleCellHaystack-0.0.5/singleCellHaystack/_grid.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)     9401 2023-07-03 09:04:28.000000 singleCellHaystack-0.0.5/singleCellHaystack/_haystack.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)     1990 2023-07-02 07:42:38.000000 singleCellHaystack-0.0.5/singleCellHaystack/_kld.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)     3426 2023-07-03 03:31:33.000000 singleCellHaystack-0.0.5/singleCellHaystack/_plot.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)     3947 2023-07-01 18:30:54.000000 singleCellHaystack-0.0.5/singleCellHaystack/_pvalue.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)     2388 2023-07-03 02:09:58.000000 singleCellHaystack-0.0.5/singleCellHaystack/_randomization.py
+-rw-rw-r--   0 diez      (1000) diez      (1000)      264 2023-05-14 04:37:57.000000 singleCellHaystack-0.0.5/singleCellHaystack/_tools.py
+drwxrwxr-x   0 diez      (1000) diez      (1000)        0 2023-07-03 12:20:36.962246 singleCellHaystack-0.0.5/singleCellHaystack/datasets/
+-rw-rw-r--   0 diez      (1000) diez      (1000)   223111 2023-05-14 04:37:57.000000 singleCellHaystack-0.0.5/singleCellHaystack/datasets/toy.h5ad
+drwxrwxr-x   0 diez      (1000) diez      (1000)        0 2023-07-03 12:20:36.962246 singleCellHaystack-0.0.5/singleCellHaystack.egg-info/
+-rw-rw-r--   0 diez      (1000) diez      (1000)     4406 2023-07-03 12:20:36.000000 singleCellHaystack-0.0.5/singleCellHaystack.egg-info/PKG-INFO
+-rw-rw-r--   0 diez      (1000) diez      (1000)      591 2023-07-03 12:20:36.000000 singleCellHaystack-0.0.5/singleCellHaystack.egg-info/SOURCES.txt
+-rw-rw-r--   0 diez      (1000) diez      (1000)        1 2023-07-03 12:20:36.000000 singleCellHaystack-0.0.5/singleCellHaystack.egg-info/dependency_links.txt
+-rw-rw-r--   0 diez      (1000) diez      (1000)       52 2023-07-03 12:20:36.000000 singleCellHaystack-0.0.5/singleCellHaystack.egg-info/requires.txt
+-rw-rw-r--   0 diez      (1000) diez      (1000)       19 2023-07-03 12:20:36.000000 singleCellHaystack-0.0.5/singleCellHaystack.egg-info/top_level.txt
```

### Comparing `singleCellHaystack-0.0.4/LICENSE` & `singleCellHaystack-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `singleCellHaystack-0.0.4/PKG-INFO` & `singleCellHaystack-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: singleCellHaystack
-Version: 0.0.4
-Summary: An implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) in python.
+Version: 0.0.5
+Summary: A Python implementation of singleCellHaystack.
 Author-email: Diego Diez <diego10ruiz@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Diego Diez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -41,47 +41,54 @@
 ==================
 
 [![Lifecycle:beta](https://img.shields.io/badge/lifecycle-beta-orange.svg)](https://github.com/ddiez/singleCellHaystack-py)
 [![](https://github.com/ddiez/singleCellHaystack-py/actions/workflows/python-package.yml/badge.svg)](https://github.com/ddiez/singleCellHaystack-py/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/singleCellHaystack?logo=PyPI)](https://pypi.org/project/singleCellHaystack)
 [![PyPIDownloads](https://pepy.tech/badge/singleCellHaystack)](https://pepy.tech/project/singleCellHaystack)
 
-This repository contains a python implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) (version >= 1.0.0).
+This repository contains a Python implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) (version >= 1.0.0).
 
 This package is currently in beta. The most important functionality in the R package works, but some features are not yet available. Here is a (probably imcomplete) list of missing features. Some will be added in the future.
 
 * `weights.advanced.Q` (formerly known as `use.advanced.sampling`).
 * `seeding` method for calculating grid points.
+* Hierarchical clustering method for `cluster_genes`.
 
 # Installation
 
 You can install singleCellHaystack from [pypi](https://pypi.org):
 
 ```
 pip install singleCellHaystack
 ```
 
+You can install singleCellHaystack from GitHub with:
+
+```
+pip install git+http://github.com/ddiez/singleCellHaystack-py
+```
+
 >Support for conda installation will be added in the future.
 
 # Example
 
 ```
 import scanpy as sc
 import singleCellHaystack as hs
 
 adata = sc.read_h5ad("data.h5ad")
 
 [... process adata object ...]
 
 res = hs.haystack(adata, coord="pca")
-res["results"]
+res.top_features(n=10)
 ```
 
 # References
 
-- Our manuscript describing the updated, more generally applicable version of `singleCellHaystack` inclusing this python implementation is available on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.13.516355v1).
+- Our manuscript describing the updated, more generally applicable version of `singleCellHaystack` including this Python implementation is available on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.13.516355v1).
 
 - Our manuscript describing the original implementation of `singleCellHaystack` for R ([version 0.3.4](https://github.com/alexisvdb/singleCellHaystack/tree/binary)) was published in [Nature Communications](https://doi.org/10.1038/s41467-020-17900-3).
 
 If you use `singleCellHaystack` in your research please cite our work using:
 
 Vandenbon A, Diez D (2020). “A clustering-independent method for finding differentially expressed genes in single-cell transcriptome data.” *Nature Communications*, *11*(1), 4318. [doi:10.1038/s41467-020-17900-3](https://doi.org/10.1038/s41467-020-17900-3).
```

### Comparing `singleCellHaystack-0.0.4/README.md` & `singleCellHaystack-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,47 +2,54 @@
 ==================
 
 [![Lifecycle:beta](https://img.shields.io/badge/lifecycle-beta-orange.svg)](https://github.com/ddiez/singleCellHaystack-py)
 [![](https://github.com/ddiez/singleCellHaystack-py/actions/workflows/python-package.yml/badge.svg)](https://github.com/ddiez/singleCellHaystack-py/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/singleCellHaystack?logo=PyPI)](https://pypi.org/project/singleCellHaystack)
 [![PyPIDownloads](https://pepy.tech/badge/singleCellHaystack)](https://pepy.tech/project/singleCellHaystack)
 
-This repository contains a python implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) (version >= 1.0.0).
+This repository contains a Python implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) (version >= 1.0.0).
 
 This package is currently in beta. The most important functionality in the R package works, but some features are not yet available. Here is a (probably imcomplete) list of missing features. Some will be added in the future.
 
 * `weights.advanced.Q` (formerly known as `use.advanced.sampling`).
 * `seeding` method for calculating grid points.
+* Hierarchical clustering method for `cluster_genes`.
 
 # Installation
 
 You can install singleCellHaystack from [pypi](https://pypi.org):
 
 ```
 pip install singleCellHaystack
 ```
 
+You can install singleCellHaystack from GitHub with:
+
+```
+pip install git+http://github.com/ddiez/singleCellHaystack-py
+```
+
 >Support for conda installation will be added in the future.
 
 # Example
 
 ```
 import scanpy as sc
 import singleCellHaystack as hs
 
 adata = sc.read_h5ad("data.h5ad")
 
 [... process adata object ...]
 
 res = hs.haystack(adata, coord="pca")
-res["results"]
+res.top_features(n=10)
 ```
 
 # References
 
-- Our manuscript describing the updated, more generally applicable version of `singleCellHaystack` inclusing this python implementation is available on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.13.516355v1).
+- Our manuscript describing the updated, more generally applicable version of `singleCellHaystack` including this Python implementation is available on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.13.516355v1).
 
 - Our manuscript describing the original implementation of `singleCellHaystack` for R ([version 0.3.4](https://github.com/alexisvdb/singleCellHaystack/tree/binary)) was published in [Nature Communications](https://doi.org/10.1038/s41467-020-17900-3).
 
 If you use `singleCellHaystack` in your research please cite our work using:
 
 Vandenbon A, Diez D (2020). “A clustering-independent method for finding differentially expressed genes in single-cell transcriptome data.” *Nature Communications*, *11*(1), 4318. [doi:10.1038/s41467-020-17900-3](https://doi.org/10.1038/s41467-020-17900-3).
```

### Comparing `singleCellHaystack-0.0.4/pyproject.toml` & `singleCellHaystack-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "singleCellHaystack"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Diego Diez", email="diego10ruiz@gmail.com" },
 ]
-description = "An implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) in python."
+description = "A Python implementation of singleCellHaystack."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -32,8 +32,13 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ddiez/singleCellHaystack-py"
 "Bug Tracker" = "https://github.com/ddiez/singleCellHaystack-py/issues"
 
 [tool.setuptools]
-packages = ["singleCellHaystack"]
+packages = ["singleCellHaystack"]
+
+[tool.pytest.ini_options]
+testpaths = [
+    "singleCellHaystack/tests"
+]
```

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack/_cluster.py` & `singleCellHaystack-0.0.5/singleCellHaystack/_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     scores[:,k] = np.squeeze(np.mean(m, axis=1))
   
   return {
     "scores": scores,
     "clusters": clusters
   }
 
-def plot_gene_clusters(adata, gene_clusters, basis=None, ncols=4, figsize=None, color_map="coolwarm", return_scores=False):
+def plot_gene_clusters(adata, gene_clusters, basis=None, ncols=None, figsize=None, color_map="coolwarm", return_scores=False):
   """
   Plot gene clusters returned by cluster_genes.
 
   :param adata: AnnData object.
   :param gene_clusters: pandas DataFrame output by cluster_genes.
   :param basis: the embedding to use.
   :param ncols: numner of columns for plot.
@@ -106,14 +106,17 @@
   coord = adata.obsm[basis_key]
 
   scores = calculate_cluster_scores(adata=adata, gene_clusters=gene_clusters)
   clusters = scores["clusters"]
   scores = scores["scores"]
 
   nclusters = scores.shape[1]
+
+  if ncols is None:
+    ncols = np.int32(np.ceil(np.sqrt(nclusters)))
   nrows = int(np.ceil(nclusters/ncols))
 
   fig, ax = plt.subplots(nrows=nrows, ncols=ncols, figsize=figsize)
 
   for i in range(nrows):
     for j in range(ncols):
       ax[i, j].grid(False)
```

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack/_grid.py` & `singleCellHaystack-0.0.5/singleCellHaystack/_grid.py`

 * *Files identical despite different names*

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack/_haystack.py` & `singleCellHaystack-0.0.5/singleCellHaystack/_haystack.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,169 @@
 from ._randomization import *
 from ._pvalue import *
 from ._grid import *
 from ._kld import *
+from ._tools import *
 
 from scipy.sparse import isspmatrix
 
 # haystack
 # Main function. Can accept AnnData, numpy array and scipy sparse matrices.
 # Does not accept numpay matrix objects.
-def haystack(x, coord, features=None, scale_coords=True, ngrid_points=100,
-    n_genes_to_randomize=100, select_genes_randomize_method="heavytails",
-    spline_method="bs", n_randomizations=100, grid_points=None, pseudo=1e-300, verbose=True):
+def haystack(x, coord, features=None, layer=None, dims=None, scale_coord=True, ngrid_points=100,
+    n_genes_to_randomize=100, select_genes_randomize_method="heavytails", genes_to_randomize=None,
+    spline_method="bs", n_randomizations=100, grid_points=None, pseudo=1e-300, random_state=None, verbose=True, kld_method="original"):
 
   """
   Runs singleCellHaystack.
 
   :param x: AnnData, numpy array or scipy sparse matrix.
   :param coord: a numpy array with 1D pseudotime, 2D or 3D spatial coordinates or an embedding with any number of dimansions.
+  :param features: a list of strings with feature names. If None for AnnData objects is adata.var_names and a numeric index for arrays.
+  :param layer: layer to use for AnnData objects. If None then adata.X is used.
+  :param scale_coord: whether to scale input coordinates.
+  :param ngrid_points: number of grid points.
+  :param n_genes_to_randomize: number of genes to use for randomization.
+  :param select_genes_randomize_method: method used to select genes for randomization. One of "heavytails" (default) or uniform.
+  :param genes_to_randomize: list of genes to randomize.
+  :param spline_method: spline method used for randomizations. One of bs (default) or ns.
+  :param n_randomizations: number of randomizations.
+  :param grid_points: array with grid coordinates.
+  :param pseudo: pseudo count added to counts.
+  :param random_state: random seed or random state.
+  :param verbose: whether to output messages when running haystack.
+  :param kld_method: method used to compute KLD.
   :return: A list with singleCellHaystack results.
   :rtype: list
 
   """
   from anndata import AnnData
   from numpy import ndarray
 
+  res = None
+
   if isinstance(x, AnnData) and isinstance(coord, str):
-    res = haystack_adata(adata=x, basis=coord, dims=None, scale_coords=scale_coords,
+    res = haystack_adata(adata=x, basis=coord, layer=layer, dims=dims, scale_coord=scale_coord,
         ngrid_points=ngrid_points, n_genes_to_randomize=n_genes_to_randomize,
-        select_genes_randomize_method=select_genes_randomize_method, spline_method=spline_method,
-        n_randomizations=n_randomizations, grid_points=grid_points, pseudo=pseudo, verbose=verbose)
+        select_genes_randomize_method=select_genes_randomize_method, genes_to_randomize=genes_to_randomize, spline_method=spline_method,
+        n_randomizations=n_randomizations, grid_points=grid_points, pseudo=pseudo, random_state=random_state, verbose=verbose, kld_method=kld_method)
 
   if (isinstance(x, ndarray) or isspmatrix(x)) and isinstance(coord, ndarray):
-    res = haystack_array(weights=x, coord=coord, features=features, scale_coords=scale_coords,
+    res = haystack_array(weights=x, coord=coord, features=features, scale_coord=scale_coord,
         ngrid_points=ngrid_points, n_genes_to_randomize=n_genes_to_randomize,
-        select_genes_randomize_method=select_genes_randomize_method, spline_method=spline_method,
-        n_randomizations=n_randomizations, grid_points=grid_points, pseudo=pseudo, verbose=verbose)
+        select_genes_randomize_method=select_genes_randomize_method, genes_to_randomize=genes_to_randomize, spline_method=spline_method,
+        n_randomizations=n_randomizations, grid_points=grid_points, pseudo=pseudo, random_state=random_state, verbose=verbose, kld_method=kld_method)
 
-  return(res)
+  if res is None:
+    print(
+  """
+    ERROR: Some of the input data didn't match the expected type:
+      * If x is an AnnData object then coord must be a string with the name of the basis to use.
+      * If x is a numpy or scipy sparse array then coord must be a numpy array.
+  """)
+  else:
+    return(res)
 
 # haystack_array
 # Method for numpy array and scipy sparse matrix objects.
-def haystack_array(weights, coord, features=None, scale_coords=True, ngrid_points=100,
-    n_genes_to_randomize=100, select_genes_randomize_method="heavytails",
-    spline_method="bs", n_randomizations=100, grid_points=None, pseudo=1e-300, verbose=True):
+def haystack_array(weights, coord, features=None, scale_coord=True, ngrid_points=100,
+    n_genes_to_randomize=100, select_genes_randomize_method="heavytails", genes_to_randomize=None,
+    spline_method="bs", n_randomizations=100, grid_points=None, pseudo=1e-300, random_state=None, verbose=True, kld_method="original"):
 
   from pandas import DataFrame
   from sklearn.preprocessing import StandardScaler
+  from numpy.random import RandomState
+
+  if random_state is not None:
+    if isinstance(random_state, int):
+      random_state = RandomState(random_state)
+
+    if not isinstance(random_state, RandomState):
+      print("_ERROR_ invalid random state.")
+      return(None)
 
   if (verbose):
     print("> entering array method ...")
 
   exprs = weights
 
   # Features included?
   if features is None:
     features = np.array(range(exprs.shape[1]))
 
   # Scale coords.
-  if scale_coords:
+  coord_mean = None
+  coord_std = None
+  if scale_coord:
     if (verbose):
       print("> scaling coordinates ...")
 
     coord_mean = np.mean(coord, axis=0)
     coord_std = np.std(coord, axis=0)
     coord = (coord - coord_mean) / coord_std
 
+    #coord, coord_mean, coord_std = scale(coord)
+
   # Check for negative values.
   if (np.sum(exprs < 0).astype(bool)):
     print("_ERROR_ negative values in your data.")
     return(None)
 
   # filter genes with zero stdev.
   if (verbose):
     print("> calculating feature stds ...")
   scaler = StandardScaler(with_mean=False)
   scaler_fit = scaler.fit(exprs)
   exprs_sd = np.sqrt(scaler_fit.var_)
   exprs_mean = scaler_fit.mean_
 
-  #exprs_sd = np.std(exprs, axis=0)
   sel_zero = exprs_sd == 0
   n_zero = np.sum(sel_zero)
   if (n_zero > 0):
     if (verbose):
       print("> removing", str(n_zero), "genes with zero variance ...")
     sel_nozero = np.invert(sel_zero)
-  #   genes = genes[sel_nozero]
     exprs_sd = exprs_sd[sel_nozero] + pseudo
     exprs_mean = exprs_mean[sel_nozero] + pseudo
     exprs = exprs[:, sel_nozero]
     features = features[sel_nozero]
 
   ncells = exprs.shape[0]
   ngenes = exprs.shape[1]
 
   # Calculate KLD.
   if grid_points is None:
-    grid_points = calculate_grid_points(coord, ngrid_points, verbose=verbose)
+    grid_points = calculate_grid_points(coord, ngrid_points, random_state=random_state, verbose=verbose)
   grid_dist = calculate_dist_to_cells(coord, grid_points, verbose=verbose)
   grid_density = calculate_density(grid_dist, verbose=verbose)
 
   Q = calculate_Q_dist(grid_density, pseudo=pseudo, verbose=verbose)
+  P = None
 
-  KLD = calculate_KLD(grid_density, exprs, Q, verbose=verbose)
+  if kld_method == "original":
+    KLD = calculate_KLD(grid_density, exprs, Q, verbose=verbose)
+  
+  if kld_method == "new":
+    P = calculate_P_matrix(grid_density, exprs, pseudo=pseudo, verbose=verbose)
+    KLD = calculate_KLD2(P, Q, verbose=verbose)
 
   # Calculate CV
   if (verbose):
     print("> calculating feature's CV ...")
   exprs_cv = exprs_sd / exprs_mean
 
-  genes_to_randomize = select_genes_to_randomize(exprs_cv, n_genes_to_randomize, method=select_genes_randomize_method, verbose=verbose)
+  if genes_to_randomize is None:
+    genes_to_randomize = select_genes_to_randomize(exprs_cv, n_genes_to_randomize, method=select_genes_randomize_method, verbose=verbose)
 
   # Randomizations.
-  KLD_rand = randomize_KLD(grid_density, exprs[:, genes_to_randomize], Q, n_randomizations=n_randomizations, verbose=verbose)
+  if kld_method == "original":
+    KLD_rand = randomize_KLD(grid_density, exprs[:, genes_to_randomize], Q, n_randomizations=n_randomizations, random_state=random_state, verbose=verbose)
+  
+  if kld_method == "new":
+    KLD_rand = randomize_KLD2(grid_density, exprs[:, genes_to_randomize], Q, n_randomizations=n_randomizations, random_state=random_state, verbose=verbose)
 
   # Calculate p.values:
   pvalData = calculate_Pval(KLD, KLD_rand, exprs_cv, exprs_cv[genes_to_randomize], method=spline_method, verbose=verbose)
   pval = pvalData["pval"]
   logpval = pvalData["logpval"]
   #pval_adj = pval * pval.size # Bonferroni correction
   logpval_adj = logpval + np.log10(logpval.size)
@@ -126,61 +173,83 @@
   if (verbose):
     print("> done.")
 
   # Return results.
   df = DataFrame({
     "gene": features,
     "KLD": KLD,
+    "CV": exprs_cv,
     "pval": pval,
     "pval_adj": pval_adj,
     "logpval": logpval,
     "logpval_adj": logpval_adj
   })
 
-  df = df.sort_values("logpval")
+  #df = df.sort_values("logpval")
 
   info = {
     "grid_points": grid_points,
     "grid_dist": grid_dist,
     "grid_density": grid_density,
     "Q": Q,
+    "P": P,
     "KLD_rand": KLD_rand,
     "pval_info": pvalData,
     "genes_to_randomize": genes_to_randomize,
     "exprs_cv": exprs_cv,
+    "coord_mean": coord_mean,
+    "coord_std": coord_std
   }
 
-  return {
-    "results": df,
-    "info": info
-  }
+  res = HaystackResult(result=df, info=info)
+  return res
 
 # haystack_adata
 # method for AnnData objects.
-def haystack_adata(adata, basis="pca", dims=None, scale_coords=True, ngrid_points=100,
-    n_genes_to_randomize=100, select_genes_randomize_method="heavytails", spline_method="bs",
-    n_randomizations=100, grid_points=None, pseudo=1e-300, verbose=True):
+def haystack_adata(adata, basis="pca", layer=None, dims=None, scale_coord=True, ngrid_points=100,
+    n_genes_to_randomize=100, select_genes_randomize_method="heavytails", genes_to_randomize=None, spline_method="bs",
+    n_randomizations=100, grid_points=None, pseudo=1e-300, random_state=None, verbose=True, kld_method="original"):
 
   if (verbose):
     print("> starting haystack ...")
 
   if basis in adata.obsm.keys():
     basis_key = basis
   elif f"X_{basis}" in adata.obsm.keys():
     basis_key = f"X_{basis}"
 
   coord = adata.obsm[basis_key]
-  exprs = adata.X
+  if layer is None:
+    exprs = adata.X
+  else:
+    exprs = adata.layers[layer]
   genes = adata.var_names
 
   # Check for negative values.
   if (np.sum(exprs < 0).astype(bool)):
     print("_ERROR_ negative values in your data. Hint: pass adata.raw.to_adata() or adata.layers[\"count\"]")
     return(None)
 
   if dims is not None:
-    coord = coord[:, dims]
+    coord = coord[:, :dims]
 
-  res = haystack_array(exprs, coord, features=genes, scale_coords=scale_coords, ngrid_points=ngrid_points,
-      n_genes_to_randomize=n_genes_to_randomize, select_genes_randomize_method=select_genes_randomize_method,
-      spline_method=spline_method, n_randomizations=n_randomizations, grid_points=grid_points, pseudo=pseudo, verbose=verbose)
+  res = haystack_array(exprs, coord, features=genes, scale_coord=scale_coord, ngrid_points=ngrid_points,
+      n_genes_to_randomize=n_genes_to_randomize, select_genes_randomize_method=select_genes_randomize_method, genes_to_randomize=genes_to_randomize,
+      spline_method=spline_method, n_randomizations=n_randomizations, grid_points=grid_points, pseudo=pseudo, random_state=random_state, verbose=verbose, kld_method=kld_method)
   return(res)
+
+class HaystackResult:
+  result = None
+  info = None
+
+  def __init__(self, result, info):
+    self.result=result
+    self.info=info
+
+  def top_features(self, n=None, sort_by="logpval_adj"):
+    sum = self.result
+    sum = sum.sort_values(sort_by)
+
+    if n is not None:
+      sum = sum.head(n)
+    
+    return sum
```

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack/_kld.py` & `singleCellHaystack-0.0.5/singleCellHaystack/_kld.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   if (isspmatrix(weights)):
     index = weights.nonzero()[0]
     P = density[index, :] * weights.data.reshape(-1,1)
 
   if (isinstance(weights, ndarray)):
     P = density * weights.reshape(-1,1)
 
-  P = np.sum(P, 0)
+  P = np.sum(P, axis=0)
   P = P + pseudo
   P = P / np.sum(P)
   return P
 
 def calculate_KLD(density, weights, Q, pseudo=1e-300, verbose=False):
 
   if (isspmatrix(weights)):
@@ -41,13 +41,39 @@
   if (verbose):
     print("> calculating KLD for " + str(ngenes) + " features ...")
     pbar = tqdm(total=ngenes)
 
   # FIXME: vectorize this computation.
   res = np.zeros(ngenes)
   for k in range(ngenes):
-    P = calculate_P_dist(density, weights[:, k])
+    P = calculate_P_dist(density, weights[:, k], pseudo=pseudo)
     res[k] = np.sum(P * np.log(P / Q))
     if (verbose):
       pbar.update(n=1)
 
   return res
+
+def calculate_P_matrix(density, weights, pseudo=1e-300, verbose=False):
+  if (isspmatrix(weights)):
+    weights = weights.tocsc()
+
+  ngenes = weights.shape[1]
+  ngrid_points = density.shape[1]
+
+  if (verbose):
+    print("> calculating P for " + str(ngenes) + " features ...")
+    pbar = tqdm(total=ngenes)
+
+  res = np.zeros([ngenes, ngrid_points])
+  for k in range(ngenes):
+    res[k, :] = calculate_P_dist(density, weights[:, k], pseudo=pseudo)
+    if (verbose):
+      pbar.update(n=1)
+  
+  return res
+
+def calculate_KLD2(P, Q, verbose=False):
+  if (verbose):
+    print("> calculating KLD ...")
+  
+  kld = np.sum(P * np.log(P / Q), axis=1)
+  return kld
```

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack/_plot.py` & `singleCellHaystack-0.0.5/singleCellHaystack/_plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   Plot singleCellHaystack randomization information.
 
   :param x: singleCellHaystack result.
   :param type: one of "mean" or "sd".
 
   """
 
-  data = x["info"]["pval_info"]
+  data = x.info["pval_info"]
 
   x = data["CV"]
   method = data["method"]
 
   if type == "mean":
     y = data["rand_mean"]
     y_hat = data["rand_mean_hat"]
@@ -46,15 +46,15 @@
   """
   Plot singleCellHaystack p.value rank.
 
   :param x: singleCellHaystack result.
 
   """
 
-  data = x["info"]["pval_info"]
+  data = x.info["pval_info"]
 
   x = np.sort(data["logpval"])
 
   plt.plot(x, color="black")
   plt.xlabel("Rank")
   plt.ylabel("logpval")
   plt.show()
@@ -63,19 +63,21 @@
   """
   Plot singleCellHaystack p.value histogram.
 
   :param x: singleCellHaystack result.
 
   """
 
-  data = x["info"]["pval_info"]
+  data = x.info["pval_info"]
 
   x = data["pval"]
 
   h = plt.hist(x, color="black", bins=30)
+  plt.xlabel("P value")
+  plt.ylabel("count")
   plt.xlim([0, 1])
   plt.show()
 
 def plot_compare_ranks(res1, res2, sort_by="logpval", xlabel=None, ylabel=None):
   """
   Plot the rank of two singleCellHaystack results.
 
@@ -87,16 +89,22 @@
   :param xlabel: label for x-axis (res1).
   :param ylabel: label for y-axis (res2).
 
   """
 
   import pandas as pd
 
-  sum1 = res1["results"].sort_values(sort_by)
-  sum2 = res2["results"].sort_values(sort_by)
+  sum1 = res1.result.sort_values(sort_by)
+  sum2 = res2.result.sort_values(sort_by)
+
+  if xlabel is None:
+    xlabel = sort_by + "_1"
+
+  if ylabel is None:
+    ylabel = sort_by + "_2"
 
   r1 = pd.DataFrame({
     "gene1": sum1.index,
     "rank1": list(range(sum1.index.shape[0])),
   })
 
   r2 = pd.DataFrame({
@@ -111,7 +119,29 @@
   r2 = r2.reset_index(drop=True)
 
   d = r1.join(r2)
 
   plt.plot(d.rank1, d.rank2, "bo", markersize=1)
   plt.xlabel(xlabel)
   plt.ylabel(ylabel)
+
+def plot_rand_kld(x, gene=0):
+    from scipy.stats import norm
+    
+    kld_rand = x.info["KLD_rand"]
+    X = kld_rand[gene, :]
+    X_m = np.mean(X)
+    X_s = np.std(X)
+
+    q95 = np.quantile(X, 0.95)
+    n95 = norm(loc=X_m, scale=X_s).ppf(0.95)
+    
+    plt.hist(X, color="black", bins=30)
+    plt.grid(False)
+    plt.axvline(X_m, color="green", linewidth=1)
+    plt.axvline(X_m + X_s, color="purple", linewidth=1)
+    plt.axvline(X_m - X_s, color="purple", linewidth=1)
+    plt.axvline(q95, color="blue", linewidth=1)
+    plt.axvline(n95, color="red", linewidth=1)
+    plt.xlabel("KLD_rand")
+    plt.ylabel("count")
+    plt.show()
```

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack/_pvalue.py` & `singleCellHaystack-0.0.5/singleCellHaystack/_pvalue.py`

 * *Files identical despite different names*

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack/datasets/toy.h5ad` & `singleCellHaystack-0.0.5/singleCellHaystack/datasets/toy.h5ad`

 * *Files identical despite different names*

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack.egg-info/PKG-INFO` & `singleCellHaystack-0.0.5/singleCellHaystack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: singleCellHaystack
-Version: 0.0.4
-Summary: An implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) in python.
+Version: 0.0.5
+Summary: A Python implementation of singleCellHaystack.
 Author-email: Diego Diez <diego10ruiz@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Diego Diez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -41,47 +41,54 @@
 ==================
 
 [![Lifecycle:beta](https://img.shields.io/badge/lifecycle-beta-orange.svg)](https://github.com/ddiez/singleCellHaystack-py)
 [![](https://github.com/ddiez/singleCellHaystack-py/actions/workflows/python-package.yml/badge.svg)](https://github.com/ddiez/singleCellHaystack-py/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/singleCellHaystack?logo=PyPI)](https://pypi.org/project/singleCellHaystack)
 [![PyPIDownloads](https://pepy.tech/badge/singleCellHaystack)](https://pepy.tech/project/singleCellHaystack)
 
-This repository contains a python implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) (version >= 1.0.0).
+This repository contains a Python implementation of [singleCellHaystack](https://github.com/alexisvdb/singleCellHaystack) (version >= 1.0.0).
 
 This package is currently in beta. The most important functionality in the R package works, but some features are not yet available. Here is a (probably imcomplete) list of missing features. Some will be added in the future.
 
 * `weights.advanced.Q` (formerly known as `use.advanced.sampling`).
 * `seeding` method for calculating grid points.
+* Hierarchical clustering method for `cluster_genes`.
 
 # Installation
 
 You can install singleCellHaystack from [pypi](https://pypi.org):
 
 ```
 pip install singleCellHaystack
 ```
 
+You can install singleCellHaystack from GitHub with:
+
+```
+pip install git+http://github.com/ddiez/singleCellHaystack-py
+```
+
 >Support for conda installation will be added in the future.
 
 # Example
 
 ```
 import scanpy as sc
 import singleCellHaystack as hs
 
 adata = sc.read_h5ad("data.h5ad")
 
 [... process adata object ...]
 
 res = hs.haystack(adata, coord="pca")
-res["results"]
+res.top_features(n=10)
 ```
 
 # References
 
-- Our manuscript describing the updated, more generally applicable version of `singleCellHaystack` inclusing this python implementation is available on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.13.516355v1).
+- Our manuscript describing the updated, more generally applicable version of `singleCellHaystack` including this Python implementation is available on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.13.516355v1).
 
 - Our manuscript describing the original implementation of `singleCellHaystack` for R ([version 0.3.4](https://github.com/alexisvdb/singleCellHaystack/tree/binary)) was published in [Nature Communications](https://doi.org/10.1038/s41467-020-17900-3).
 
 If you use `singleCellHaystack` in your research please cite our work using:
 
 Vandenbon A, Diez D (2020). “A clustering-independent method for finding differentially expressed genes in single-cell transcriptome data.” *Nature Communications*, *11*(1), 4318. [doi:10.1038/s41467-020-17900-3](https://doi.org/10.1038/s41467-020-17900-3).
```

### Comparing `singleCellHaystack-0.0.4/singleCellHaystack.egg-info/SOURCES.txt` & `singleCellHaystack-0.0.5/singleCellHaystack.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 singleCellHaystack/_data.py
 singleCellHaystack/_grid.py
 singleCellHaystack/_haystack.py
 singleCellHaystack/_kld.py
 singleCellHaystack/_plot.py
 singleCellHaystack/_pvalue.py
 singleCellHaystack/_randomization.py
+singleCellHaystack/_tools.py
 singleCellHaystack.egg-info/PKG-INFO
 singleCellHaystack.egg-info/SOURCES.txt
 singleCellHaystack.egg-info/dependency_links.txt
 singleCellHaystack.egg-info/requires.txt
 singleCellHaystack.egg-info/top_level.txt
 singleCellHaystack/datasets/toy.h5ad
```

