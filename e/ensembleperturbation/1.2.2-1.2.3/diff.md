# Comparing `tmp/ensembleperturbation-1.2.2.tar.gz` & `tmp/ensembleperturbation-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembleperturbation-1.2.2.tar", max compression
+gzip compressed data, was "ensembleperturbation-1.2.3.tar", max compression
```

## Comparing `ensembleperturbation-1.2.2.tar` & `ensembleperturbation-1.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     7048 2023-06-26 13:45:23.157278 ensembleperturbation-1.2.2/LICENSE
--rw-r--r--   0        0        0     1554 2023-06-26 13:45:23.157278 ensembleperturbation-1.2.2/README.md
--rw-r--r--   0        0        0        3 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/__init__.py
--rw-r--r--   0        0        0     3803 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/combine_results.py
--rw-r--r--   0        0        0     1952 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/make_storm_ensemble.py
--rw-r--r--   0        0        0     5792 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/perturb_tracks.py
--rw-r--r--   0        0        0     2566 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/client/plot_results.py
--rw-r--r--   0        0        0        0 2023-06-26 13:45:23.169278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/__init__.py
--rw-r--r--   0        0        0    32929 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/adcirc.py
--rw-r--r--   0        0        0    24828 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/comparison.py
--rw-r--r--   0        0        0    46714 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/schism.py
--rw-r--r--   0        0        0      545 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/parsing/utilities.py
--rw-r--r--   0        0        0        0 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/perturbation/__init__.py
--rw-r--r--   0        0        0    75293 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/perturbation/atcf.py
--rw-r--r--   0        0        0        0 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/__init__.py
--rw-r--r--   0        0        0    10510 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/gdal_dataset.py
--rw-r--r--   0        0        0     5453 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/geometry.py
--rw-r--r--   0        0        0     1590 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/map.py
--rw-r--r--   0        0        0     9135 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/nodes.py
--rw-r--r--   0        0        0    14013 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/perturbation.py
--rw-r--r--   0        0        0    20101 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/surrogate.py
--rw-r--r--   0        0        0     4623 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/taylor_diagram.py
--rw-r--r--   0        0        0      908 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/plotting/utilities.py
--rw-r--r--   0        0        0        0 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/__init__.py
--rw-r--r--   0        0        0     2663 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/ensemble_array.py
--rw-r--r--   0        0        0    11112 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
--rw-r--r--   0        0        0     5332 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
--rw-r--r--   0        0        0    23410 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/surrogate.py
--rw-r--r--   0        0        0     5066 2023-06-26 13:45:23.173278 ensembleperturbation-1.2.2/ensembleperturbation/utilities.py
--rw-r--r--   0        0        0     2326 2023-06-26 13:45:30.097446 ensembleperturbation-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3723 2023-06-26 13:45:31.101437 ensembleperturbation-1.2.2/setup.py
--rw-r--r--   0        0        0     3731 2023-06-26 13:45:31.101974 ensembleperturbation-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-07-03 13:55:29.074694 ensembleperturbation-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1554 2023-07-03 13:55:29.074694 ensembleperturbation-1.2.3/README.md
+-rw-r--r--   0        0        0        3 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/__init__.py
+-rw-r--r--   0        0        0     3803 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/combine_results.py
+-rw-r--r--   0        0        0     1952 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/make_storm_ensemble.py
+-rw-r--r--   0        0        0     5792 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/perturb_tracks.py
+-rw-r--r--   0        0        0     2566 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/plot_results.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/__init__.py
+-rw-r--r--   0        0        0    32929 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/adcirc.py
+-rw-r--r--   0        0        0    24828 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/comparison.py
+-rw-r--r--   0        0        0    46714 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/schism.py
+-rw-r--r--   0        0        0      545 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/utilities.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/perturbation/__init__.py
+-rw-r--r--   0        0        0    75293 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/perturbation/atcf.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/__init__.py
+-rw-r--r--   0        0        0    10510 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/gdal_dataset.py
+-rw-r--r--   0        0        0     5453 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/geometry.py
+-rw-r--r--   0        0        0     1590 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/map.py
+-rw-r--r--   0        0        0     9135 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/nodes.py
+-rw-r--r--   0        0        0    14013 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/perturbation.py
+-rw-r--r--   0        0        0    20066 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/surrogate.py
+-rw-r--r--   0        0        0     4623 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/taylor_diagram.py
+-rw-r--r--   0        0        0      908 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/utilities.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/__init__.py
+-rw-r--r--   0        0        0     2663 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/ensemble_array.py
+-rw-r--r--   0        0        0    11112 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
+-rw-r--r--   0        0        0     5332 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
+-rw-r--r--   0        0        0    23410 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/surrogate.py
+-rw-r--r--   0        0        0     5066 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/utilities.py
+-rw-r--r--   0        0        0     2326 2023-07-03 13:55:35.030723 ensembleperturbation-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3723 2023-07-03 13:55:35.847128 ensembleperturbation-1.2.3/setup.py
+-rw-r--r--   0        0        0     3731 2023-07-03 13:55:35.847636 ensembleperturbation-1.2.3/PKG-INFO
```

### Comparing `ensembleperturbation-1.2.2/LICENSE` & `ensembleperturbation-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/README.md` & `ensembleperturbation-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/client/combine_results.py` & `ensembleperturbation-1.2.3/ensembleperturbation/client/combine_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/client/make_storm_ensemble.py` & `ensembleperturbation-1.2.3/ensembleperturbation/client/make_storm_ensemble.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/client/perturb_tracks.py` & `ensembleperturbation-1.2.3/ensembleperturbation/client/perturb_tracks.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/client/plot_results.py` & `ensembleperturbation-1.2.3/ensembleperturbation/client/plot_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/parsing/adcirc.py` & `ensembleperturbation-1.2.3/ensembleperturbation/parsing/adcirc.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/parsing/comparison.py` & `ensembleperturbation-1.2.3/ensembleperturbation/parsing/comparison.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/parsing/schism.py` & `ensembleperturbation-1.2.3/ensembleperturbation/parsing/schism.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/parsing/utilities.py` & `ensembleperturbation-1.2.3/ensembleperturbation/parsing/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/perturbation/atcf.py` & `ensembleperturbation-1.2.3/ensembleperturbation/perturbation/atcf.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/gdal_dataset.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/gdal_dataset.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/geometry.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/geometry.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/map.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/map.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/nodes.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/nodes.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/perturbation.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/perturbation.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/surrogate.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/surrogate.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,17 +288,15 @@
         wspace=0,
         hspace=0,
     )
     map_crs = cartopy.crs.PlateCarree()
 
     for order_index, order in enumerate(sensitivities['order']):
         for variable_index, variable in enumerate(sensitivities['variable']):
-            axis = figure.add_subplot(
-                grid[order_index, variable_index]
-            )  # , projection=map_crs)
+            axis = figure.add_subplot(grid[order_index, variable_index], projection=map_crs)
             order_variable_sensitivities = sensitivities.sel(order=order, variable=variable)
 
             plot_node_map(
                 order_variable_sensitivities,
                 map_title=None,
                 colors=order_variable_sensitivities['sensitivities']
                 if 'element' not in sensitivities
```

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/taylor_diagram.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/taylor_diagram.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/plotting/utilities.py` & `ensembleperturbation-1.2.3/ensembleperturbation/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/ensemble_array.py` & `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/ensemble_array.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py` & `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py` & `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/uncertainty_quantification/surrogate.py` & `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/ensembleperturbation/utilities.py` & `ensembleperturbation-1.2.3/ensembleperturbation/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.2/pyproject.toml` & `ensembleperturbation-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'ensembleperturbation'
-version = "1.2.2"
+version = "1.2.3"
 description = 'perturbation of coupled model input over a space of input variables'
 authors = ['Zach Burnett <zachary.burnett@noaa.gov>']
 license = 'CC0-1.0'
 readme = 'README.md'
 repository = 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git'
 documentation = 'https://ensembleperturbation.readthedocs.io'
```

### Comparing `ensembleperturbation-1.2.2/setup.py` & `ensembleperturbation-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                      'perturb_tracks = '
                      'ensembleperturbation.client.perturb_tracks:main',
                      'plot_results = '
                      'ensembleperturbation.client.plot_results:main']}
 
 setup_kwargs = {
     'name': 'ensembleperturbation',
-    'version': '1.2.2',
+    'version': '1.2.3',
     'description': 'perturbation of coupled model input over a space of input variables',
     'long_description': '# Ensemble Perturbation\n\n[![tests](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/tests/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Atests)\n[![codecov](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation/branch/main/graph/badge.svg?token=4DwZePHp18)](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation)\n[![build](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/build/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Abuild)\n[![version](https://img.shields.io/pypi/v/EnsemblePerturbation)](https://pypi.org/project/EnsemblePerturbation)\n[![license](https://img.shields.io/github/license/noaa-ocs-modeling/EnsemblePerturbation)](https://creativecommons.org/share-your-work/public-domain/cc0)\n[![style](https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw)](https://sourceforge.net/p/oitnb/code)\n[![documentation](https://readthedocs.org/projects/ensembleperturbation/badge/?version=latest)](https://ensembleperturbation.readthedocs.io/en/latest/?badge=latest)\n\nPython library for perturbing coupled model inputs into ensemble runs. Provides\nperturbation and results comparison.\n\n```bash\npip install ensembleperturbation\n```\n\nDocumentation can be found at https://ensembleperturbation.readthedocs.io\n\n## Command-line interface\n\n`ensembleperturbation` exposes the following CLI commands:\n\n- `make_storm_ensemble`\n- `perturb_tracks`\n- `combine_results`\n- `plot_results`\n',
     'author': 'Zach Burnett',
     'author_email': 'zachary.burnett@noaa.gov',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git',
```

### Comparing `ensembleperturbation-1.2.2/PKG-INFO` & `ensembleperturbation-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembleperturbation
-Version: 1.2.2
+Version: 1.2.3
 Summary: perturbation of coupled model input over a space of input variables
 Home-page: https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git
 License: CC0-1.0
 Author: Zach Burnett
 Author-email: zachary.burnett@noaa.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

