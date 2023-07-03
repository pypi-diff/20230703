# Comparing `tmp/optim_esm_tools-0.2.1.tar.gz` & `tmp/optim_esm_tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-0.2.1.tar", last modified: Wed Jun 21 16:01:30 2023, max compression
+gzip compressed data, was "optim_esm_tools-0.2.2.tar", last modified: Mon Jul  3 11:43:09 2023, max compression
```

## Comparing `optim_esm_tools-0.2.1.tar` & `optim_esm_tools-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.872875 optim_esm_tools-0.2.1/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/extra_requirements/requirements-tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.872875 optim_esm_tools-0.2.1/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/analyze/xarray_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/optim_esm_tools/cmip_files/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/cmip_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/cmip_files/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/cmip_files/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/synda_files/format_synda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.872875 optim_esm_tools-0.2.1/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-21 16:01:30.000000 optim_esm_tools-0.2.1/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 16:01:30.000000 optim_esm_tools-0.2.1/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:01:30.000000 optim_esm_tools-0.2.1/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:01:30.000000 optim_esm_tools-0.2.1/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 16:01:30.000000 optim_esm_tools-0.2.1/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 16:01:30.000000 optim_esm_tools-0.2.1/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:01:30.876875 optim_esm_tools-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 16:01:27.000000 optim_esm_tools-0.2.1/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.282885 optim_esm_tools-0.2.2/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/extra_requirements/requirements-tests.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.282885 optim_esm_tools-0.2.2/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/format_synda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.282885 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.2.1/PKG-INFO` & `optim_esm_tools-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim_esm_tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,25 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.2.2 / 2023-07-02
+        ------------------
+        * Remove todo by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/67
+        * small tas tweaks by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/68
+        * Add non-tas support by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/69
+        * Match fuzzy for version last by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/70
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.2.1...v0.2.2
+        
+        
         0.2.1 / 2023-06-21
         ------------------
         * Add few badges (#62) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/62
         * Fix few codefactor issues (#63) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/63
         * Delete workspace directory (#64) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/64
         * simplify find_historical (#65) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/65
         * Fix finding (#66) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/66
```

### Comparing `optim_esm_tools-0.2.1/README.md` & `optim_esm_tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/_test_utils.py` & `optim_esm_tools-0.2.2/optim_esm_tools/_test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,29 +75,30 @@
 def synda_test_available():
     """Check if we can run a synda-dependent test"""
     return os.environ.get('ST_HOME') is not None and os.path.exists(
         get_example_data_loc()
     )
 
 
-def minimal_xr_ds():
+def minimal_xr_ds(len_x=513, len_y=181, len_time=10, add_nans=True):
     import numpy as np
     import xarray as xr
 
-    lon = np.linspace(0, 360, 513)[:-1]
-    lat = np.linspace(-90, 90, 181)[:-1]
-    time = np.arange(10)
+    lon = np.linspace(0, 360, len_x)[:-1]
+    lat = np.linspace(-90, 90, len_y)[:-1]
+    time = np.arange(len_time)
     # Totally arbitrary data
     data = (
         np.zeros(len(lat) * len(lon) * len(time)).reshape(len(time), len(lat), len(lon))
         * lon
     )
 
     # Add some NaN values just as an example
-    data[:, :, len(lon) // 2 + 30 : len(lon) // 2 + 50] = np.nan
+    if add_nans:
+        data[:, :, len(lon) // 2 + 30 : len(lon) // 2 + 50] = np.nan
 
     ds_dummy = xr.Dataset(
         data_vars=dict(
             var=(
                 ('time', 'x', 'y'),
                 data,
             )
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-0.2.2/optim_esm_tools/analyze/clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import typing as ty
 from warnings import warn
 
 
 @timed()
 def build_clusters(
     coordinates_deg: np.ndarray,
-    # TODO maybe, this shouldn't be a hardcoded number but depend on the spatial difference between two points
     max_distance_km: ty.Union[float, int] = 750,
     only_core: bool = True,
     min_samples: int = 10,
     cluster_opts: ty.Optional[dict] = None,
 ) -> ty.List[np.ndarray]:
     """Build clusters based on a list of coordinates, use halfsine metric for spherical spatiol data
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-0.2.2/optim_esm_tools/analyze/cmip_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 
 import os
 import xarray as xr
 
 import typing as ty
 from warnings import warn
 
-import xrft
-
-from optim_esm_tools.utils import depricated
+from optim_esm_tools.utils import deprecated
 
 from .globals import _CMIP_HANDLER_VERSION, _FOLDER_FMT
-from .xarray_tools import _native_date_fmt
+from .xarray_tools import _native_date_fmt, _remove_any_none_times, detrend
 from optim_esm_tools.plotting.map_maker import MapMaker, make_title
 from optim_esm_tools.analyze import tipping_criteria
 
 
 def transform_ds(
     ds: xr.Dataset,
     calculate_conditions: ty.Tuple[tipping_criteria._Condition] = None,
@@ -52,69 +50,77 @@
         calculate_conditions
     ):
         raise ValueError(f'One or more non unique descriptions {desc}')
     if condition_kwargs is None:
         condition_kwargs = dict()
 
     ds = _calculate_variables(
-        oet.synda_files.format_synda.recast(ds),
+        ds,
         min_time,
         max_time,
         variable_of_interest,
         strict,
         _ma_window,
         _detrend_type,
         _time_var,
     )
-    for cls in calculate_conditions:
-        condition = cls(**condition_kwargs)
-        condition_array = condition.calculate(ds)
-        condition_array = condition_array.assign_attrs(
-            dict(
-                short_description=cls.short_description,
-                long_description=condition.long_description,
-                name=condition_array.name,
+    for variable in oet.utils.to_str_tuple(variable_of_interest):
+        for cls in calculate_conditions:
+            condition = cls(**condition_kwargs, variable=variable)
+            condition_array = condition.calculate(ds)
+            condition_array = condition_array.assign_attrs(
+                dict(
+                    short_description=cls.short_description,
+                    long_description=condition.long_description,
+                    name=condition_array.name,
+                )
             )
-        )
-        ds[condition.short_description] = condition_array
+            ds[condition.short_description] = condition_array
     return ds
 
 
 @oet.utils.timed()
 def read_ds(
     base: str,
     variable_of_interest: ty.Tuple[str] = ('tas',),
     max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
+    apply_transform: bool = True,
     strict: bool = True,
     _ma_window: int = 10,
     _cache: bool = True,
     _file_name: str = 'merged.nc',
     **kwargs,
 ) -> xr.Dataset:
     """Read a dataset from a folder called "base".
 
     Args:
         base (str): Folder to load the data from
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
         max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
         min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
+        transform_ds: (boolm optional): Apply analysis specific postprocessing algoritms. Defaults to True.
         strict (bool, optional): raise errors on loading, if any. Defaults to True.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
         _cache (bool, optional): cache the dataset with it's extra fields to alow faster (re)loading. Defaults to True.
 
     kwargs:
         any kwargs are passed onto transfor_ds.
 
     Returns:
         xr.Dataset: An xarray dataset with the appropriate variables
     """
     if kwargs:
         oet.config.get_logger().error(f'Not really advised yet to call with {kwargs}')
         _cache = False
+    if not apply_transform:
+        # Don't cache the partial ds
+        _cache = False
+
+    oet.config.get_logger().debug(f'read_ds {variable_of_interest}')
     post_processed_file = _name_cache_file(
         base,
         variable_of_interest,
         min_time,
         max_time,
         _ma_window,
         _CMIP_HANDLER_VERSION,
@@ -128,23 +134,26 @@
         message = f'No dataset at {data_path}'
         if strict:
             raise FileNotFoundError(message)
         warn(message)
         return None
 
     data_set = oet.synda_files.format_synda.load_glob(data_path)
-    data_set = transform_ds(
-        data_set,
-        variable_of_interest=variable_of_interest,
-        max_time=max_time,
-        min_time=min_time,
-        _ma_window=_ma_window,
-        strict=strict,
-        **kwargs,
-    )
+    data_set = oet.synda_files.format_synda.recast(data_set)
+
+    if apply_transform:
+        data_set = transform_ds(
+            data_set,
+            variable_of_interest=variable_of_interest,
+            max_time=max_time,
+            min_time=min_time,
+            _ma_window=_ma_window,
+            strict=strict,
+            **kwargs,
+        )
 
     folders = base.split(os.sep)
 
     # start with -1 (for i==0)
     metadata = {k: folders[-i - 1] for i, k in enumerate(_FOLDER_FMT[::-1])}
     metadata.update(
         dict(path=base, file=post_processed_file, running_mean_period=_ma_window)
@@ -173,18 +182,21 @@
         f'_e{tuple(max_time) if max_time else ""}'
         f'_ma{_ma_window}'
         f'_optimesm_v{version}.nc',
     )
     normalized_path = (
         path.replace('(', '')
         .replace(')', '')
+        .replace(']', '')
+        .replace('[', '')
         .replace(' ', '_')
         .replace(',', '')
         .replace('\'', '')
     )
+    oet.config.get_logger().debug(f'got {normalized_path}')
     return normalized_path
 
 
 @oet.utils.timed()
 def _calculate_variables(
     data_set,
     min_time,
@@ -205,30 +217,27 @@
     # Detrend and run_mean on the fly
     for variable in variable_of_interest:
         if (ds_len := len(data_set[variable])) < _ma_window:
             message = f'This data set is shorter {ds_len} than the moving average window ({_ma_window})'
             if strict:
                 raise ValueError(message)
             oet.config.get_logger().warning(message)
+
         # NB these are DataArrays not Datasets!
         run_mean = data_set[variable].rolling(time=_ma_window, center=True).mean()
-        detrended = xrft.detrend(
-            data_set[variable], _time_var, detrend_type=_detrend_type
-        )
-        detrended_run_mean = xrft.detrend(
-            run_mean.dropna(_time_var), _time_var, detrend_type=_detrend_type
-        )
-        detrended_run_mean.attrs['units'] = data_set[variable].attrs.get(
-            'units', '{units}'
-        )
+        kw = dict(dimension=_time_var, detrend_type=_detrend_type)
+        detrended = detrend(data_set[variable], **kw)
+        detrended_run_mean = detrend(_remove_any_none_times(run_mean, _time_var), **kw)
+
         for det in detrended, detrended_run_mean:
             det.attrs.update(data_set[variable].attrs.copy())
+
         data_set[f'{variable}_run_mean_{_ma_window}'] = run_mean
         data_set[f'{variable}_detrend'] = detrended
         data_set[f'{variable}_detrend_run_mean_{_ma_window}'] = detrended_run_mean
     return data_set
 
 
-class MapMaker(MapMaker):
-    @depricated
-    def __init__(self, *a, **kw):
-        return super().__init__(*a, **kw)
+# class MapMaker(MapMaker):
+#     @depricated
+#     def __init__(self, *a, **kw):
+#         return super().__init__(*a, **kw)
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-0.2.2/optim_esm_tools/analyze/region_finding.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,27 +6,35 @@
 import typing as ty
 from optim_esm_tools.analyze import tipping_criteria
 import logging
 from optim_esm_tools.analyze.cmip_handler import transform_ds, read_ds
 import typing as ty
 import matplotlib.pyplot as plt
 from functools import wraps
-
+import xarray as xr
 import inspect
 from optim_esm_tools.analyze.clustering import build_cluster_mask
 from optim_esm_tools.plotting.plot import setup_map, _show
-from immutabledict import immutabledict
 
 # >>> import scipy
 # >>> scipy.stats.norm.cdf(3)
 # 0.9986501019683699
-_three_sigma_percent = 99.86501019683699
+# >> scipy.stats.norm.cdf(2)
+# 0.9772498680518208
+_two_sigma_percent = 97.72498680518208
 
 
-def mask_xr_ds(ds_masked, da_mask, masked_dims=('x', 'y')):
+# TODO this has too many hardcoded defaults
+def mask_xr_ds(ds_masked, da_mask, masked_dims=('x', 'y'), keep_dims=('time',)):
+    no_drop = set(masked_dims) | set(keep_dims)
+    for spurious_dim in set(ds_masked.dims) - no_drop:
+        oet.config.get_logger().warn(
+            f'Spurious coordinate {spurious_dim} dropping for safety. Keep {no_drop}'
+        )
+        ds_masked = ds_masked.mean(spurious_dim)
     for k, data_array in ds_masked.data_vars.items():
         if all(dim in list(data_array.dims) for dim in masked_dims):
             ds_masked[k] = ds_masked[k].where(da_mask, drop=False)
     return ds_masked
 
 
 def plt_show(*a):
@@ -82,24 +90,24 @@
         path=None,
         dataset=None,
         transform=True,
         save_kw=None,
         extra_opt=None,
         read_ds_kw=None,
     ) -> None:
+        read_ds_kw = dict() if read_ds_kw is None else read_ds_kw
         if path is None:
             if transform:
                 self.log.warning(
                     f'Best is to start {self.__class__.__name__} from a synda path'
                 )
                 self.dataset = transform_ds(dataset)
             else:
                 self.dataset = dataset
         else:
-            read_ds_kw = dict() if read_ds_kw is None else read_ds_kw
             self.dataset = read_ds(path, **read_ds_kw)
         if save_kw is None:
             save_kw = dict(
                 save_in='./',
                 file_types=(
                     'png',
                     'pdf',
@@ -149,27 +157,27 @@
         return self.title.replace(' ', '_') + f'_{self.__class__.__name__}'
 
 
 class MaxRegion(RegionExtractor):
     def get_masks(self) -> dict:
         """Get mask for max of ii and iii and a box arround that"""
         labels = [crit.short_description for crit in self.criteria]
-        masks = {
-            label: self.dataset[label].values == self.dataset[label].values.max()
-            for label in labels
-        }
+
+        def _val(label):
+            return self.dataset[label].values
+
+        def _max(label):
+            return _val(label)[~np.isnan(_val(label))].max()
+
+        masks = {label: _val(label) == _max(label) for label in labels}
         return masks
 
     @plt_show
     def plot_masks(self, masks, ax=None, legend=True):
-        res = self._plot_masks(
-            masks=masks,
-            ax=ax,
-            legend=legend,
-        )
+        self._plot_masks(masks=masks, ax=ax, legend=legend)
         self.save(f'{self.title_label}_map_maxes_{"-".join(self.labels)}')
 
     @apply_options
     def _plot_masks(self, masks, ax=None, legend=True):
         points = {}
         for key, mask_2d in masks.items():
             points[key] = self._mask_to_coord(mask_2d)
@@ -221,14 +229,15 @@
                 f'{self.variable}_detrend_run_mean_10': f'$RM_{{10}}$ {label} at {x:.1f}:{y:.1f}',
                 f'{self.variable}_run_mean_10': f'$RM_{{10}}$ {label} at {x:.1f}:{y:.1f}',
             }
             argwhere = np.argwhere(mask_2d)[0]
             ds_sel = self.dataset.isel(x=argwhere[1], y=argwhere[0])
             mm_sel = MapMaker(ds_sel)
             axes = mm_sel.time_series(
+                variable=self.variable,
                 other_dim=(),
                 interval=False,
                 labels=plot_labels,
                 axes=axes,
                 only_rm=only_rm,
             )
             if time_series_joined is False:
@@ -242,24 +251,25 @@
         for ax in axes:
             ax.legend(**legend_kw)
         plt.suptitle(f'Max. {"-".join(self.labels)} {self.title}', y=0.95)
 
 
 class Percentiles(RegionExtractor):
     @apply_options
-    def get_masks(self, percentiles=_three_sigma_percent) -> dict:
+    def get_masks(self, percentiles=_two_sigma_percent) -> dict:
         """Get mask for max of ii and iii and a box arround that"""
         labels = [crit.short_description for crit in self.criteria]
         masks = []
         vmin_vmax = []
 
         for lab in labels:
             arr = self.dataset[lab].values.T
-            vmin_vmax.append([np.min(arr), np.max(arr)])
-            thr = np.percentile(arr, percentiles)
+            arr_no_nan = arr[~np.isnan(arr)]
+            vmin_vmax.append([np.min(arr_no_nan), np.max(arr_no_nan)])
+            thr = np.percentile(arr_no_nan, percentiles)
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
         masks, clusters = build_cluster_mask(
@@ -268,15 +278,15 @@
         return masks, clusters
 
     @plt_show
     def plot_masks(self, masks_and_clusters, ax=None, legend=True):
         if not len(masks_and_clusters[0]):
             self.log.warning('No clusters found!')
             return
-        res = self._plot_masks(
+        self._plot_masks(
             masks_and_clusters=masks_and_clusters,
             ax=ax,
             legend=legend,
         )
         self.save(f'{self.title_label}_map_clusters_{"-".join(self.labels)}')
 
     @apply_options
@@ -286,14 +296,16 @@
         scatter_medians=True,
         ax=None,
         legend=True,
         mask_cbar_kw=None,
         cluster_kw=None,
     ):
         masks, clusters = masks_and_clusters
+        # if masks == [] or masks == [[]]:
+        #     return
         all_masks = np.zeros(masks[0].shape, np.int16)
 
         for m, c in zip(masks, clusters):
             all_masks[m] = len(c)
         if ax is None:
             setup_map()
             ax = plt.gca()
@@ -375,14 +387,15 @@
                 f'{self.variable}_detrend': f'Cluster {m_i} near ~{x:.1f}:{y:.1f}',
                 f'{self.variable}_detrend_run_mean_10': f'Cluster {m_i} $RM_{{10}}$ near ~{x:.1f}:{y:.1f}',
                 f'{self.variable}_run_mean_10': f'Cluster {m_i} $RM_{{10}}$ near ~{x:.1f}:{y:.1f}',
             }
             ds_sel = mask_xr_ds(self.dataset.copy(), mask)
             mm_sel = MapMaker(ds_sel)
             axes = mm_sel.time_series(
+                variable=self.variable,
                 other_dim=('x', 'y'),
                 interval=True,
                 labels=plot_labels,
                 axes=axes,
                 only_rm=only_rm,
             )
             if time_series_joined == False:
@@ -397,43 +410,50 @@
             for ax in axes:
                 ax.legend(**legend_kw)
         plt.suptitle(f'Clusters {self.title}', y=0.95)
 
 
 class PercentilesHistory(Percentiles):
     @apply_options
-    def get_masks(self, percentiles=_three_sigma_percent, read_ds_kw=None) -> dict:
+    def get_masks(
+        self, percentiles_historical=_two_sigma_percent, read_ds_kw=None
+    ) -> dict:
         if read_ds_kw is None:
             read_ds_kw = dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
-        historical_path = self.find_historical()[0]
-        historical_ds = read_ds(historical_path, **read_ds_kw)
 
+        historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
             arr = self.dataset[lab].values.T
             arr_historical = historical_ds[lab].values.T
-            thr = np.percentile(arr_historical, percentiles)
+            thr = np.percentile(
+                arr_historical[~np.isnan(arr_historical)], percentiles_historical
+            )
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
         masks, clusters = build_cluster_mask(
             all_mask, self.dataset['x'].values, self.dataset['y'].values
         )
         return masks, clusters
 
     @apply_options
     def find_historical(
-        self, match_to='piControl', look_back_extra=1, query_updates=None
+        self,
+        match_to='piControl',
+        look_back_extra=1,
+        query_updates=None,
+        search_kw=None,
     ):
         from optim_esm_tools.config import config
 
         base = os.path.join(
             os.sep,
             *self.dataset.attrs['path'].split(os.sep)[
                 : -len(config['CMIP_files']['folder_fmt'].split()) - look_back_extra
@@ -441,26 +461,164 @@
         )
 
         search = oet.cmip_files.find_matches.folder_to_dict(self.dataset.attrs['path'])
         search['activity_id'] = 'CMIP'
         if search['experiment_id'] == match_to:
             raise NotImplementedError()
         search['experiment_id'] = match_to
-
+        if search_kw:
+            search.update(search_kw)
         if query_updates is None:
             query_updates = [
                 dict(),
                 dict(variant_label='*'),
-                dict(grid='*'),
                 dict(version='*'),
+                # can lead to funny behavior as grid differences may cause breaking compares
+                dict(grid='*'),
             ]
 
         for try_n, update_query in enumerate(query_updates):
             if try_n:
                 self.log.warning(
                     f'No results after {try_n} try, retying with {update_query}'
                 )
             search.update(update_query)
             this_try = oet.cmip_files.find_matches.find_matches(base, **search)
             if this_try:
                 return this_try
         raise RuntimeError(f'Looked for {search}, in {base} found nothing')
+
+    @apply_options
+    def get_historical_ds(self, read_ds_kw=None, **kw):
+        if read_ds_kw is None:
+            read_ds_kw = dict()
+        for k, v in dict(min_time=None, max_time=None).items():
+            read_ds_kw.setdefault(k, v)
+        historical_path = self.find_historical(**kw)[0]
+        return read_ds(historical_path, **read_ds_kw)
+
+
+class ProductPercentiles(Percentiles):
+    @staticmethod
+    def var_to_perc(ds: xr.Dataset, dest_var: str, source_var: str) -> xr.Dataset:
+        """Calculate the percentile score of each of the data var, and assign it to the data set to get
+
+        Args:
+            ds (xr.Dataset): dataset with data-var to calculate the percentiles of
+            dest_var (str): under wich name the scores should be combined under.
+            source_var (str): property to calculate the percentiles of
+
+        Returns:
+            xr.Dataset: Original dataset with one extra colum (dest_var)
+        """
+        from scipy.stats import percentileofscore
+
+        a = ds[source_var].values
+        a_flat = a[~np.isnan(a)].flatten()
+        pcts = [
+            [percentileofscore(a_flat, i, kind='strict') / 100 for i in aa]
+            for aa in oet.utils.tqdm(a)
+        ]
+        ds[dest_var] = (ds[source_var].dims, pcts)
+        return ds
+
+    @apply_options
+    def get_masks(self, product_percentiles=_two_sigma_percent) -> dict:
+        """Get mask for max of ii and iii and a box arround that"""
+        labels = [crit.short_description for crit in self.criteria]
+        masks = []
+
+        ds = self.dataset.copy()
+        combined_score = np.ones_like(ds[labels[0]].values)
+        for label in labels:
+            _name = f'percentile {label}'
+            combined_score *= self.var_to_perc(ds, _name, label)[_name].values
+
+        # Combined score is fraction, not percent!
+        all_mask = (combined_score > (product_percentiles / 100)).T
+
+        masks, clusters = build_cluster_mask(
+            all_mask, self.dataset['x'].values, self.dataset['y'].values
+        )
+        return masks, clusters
+
+
+class LocalHistory(PercentilesHistory):
+    @apply_options
+    def get_masks(self, n_times_historical=4, read_ds_kw=None) -> dict:
+        if read_ds_kw is None:
+            read_ds_kw = dict()
+        for k, v in dict(min_time=None, max_time=None).items():
+            read_ds_kw.setdefault(k, v)
+
+        historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
+        labels = [crit.short_description for crit in self.criteria]
+        masks = []
+
+        for lab in labels:
+            arr = self.dataset[lab].values.T
+            arr_historical = historical_ds[lab].values.T
+            mask_divide = arr / arr_historical > n_times_historical
+            # If arr_historical is 0, the devision is going to get a nan assigned,
+            # despite this being the most interesting region (no historical
+            # changes, only in the scenario's)!
+            mask_no_std = (arr_historical == 0) & (arr > 0)
+            masks.append(mask_divide | mask_no_std)
+
+        all_mask = np.ones_like(masks[0])
+        for m in masks:
+            all_mask &= m
+
+        masks, clusters = build_cluster_mask(
+            all_mask, self.dataset['x'].values, self.dataset['y'].values
+        )
+        return masks, clusters
+
+    @apply_options
+    def _plot_basic_map(self, read_ds_kw=None):
+        if read_ds_kw is None:
+            read_ds_kw = dict()
+        for k, v in dict(min_time=None, max_time=None).items():
+            read_ds_kw.setdefault(k, v)
+        ds_historical = self.get_historical_ds(read_ds_kw=read_ds_kw)
+
+        class TempMapMaker(MapMaker):
+            def __getattr__(self, item):
+                if item in self.conditions:
+                    condition = self.conditions[item]
+                    da = self.data_set[condition.short_description]
+                    da_historical = ds_historical[condition.short_description]
+
+                    result = da / da_historical
+                    ret_array = result.values
+                    if len(ret_array) == 0:
+                        raise ValueError(
+                            f'Empty ret array, perhaps {da.shape} and {da_historical.shape} don\'t match?'
+                            f'\nGot\n{ret_array}\n{result}\n{da}\n{da_historical}'
+                        )
+                    max_val = np.nanmax(ret_array)
+                    mask_divide_by_zero = (da_historical == 0) & (da > 0)
+                    ret_array[mask_divide_by_zero.values] = 10 * max_val
+                    result.data = ret_array
+                    current_norm = self.normalizations.copy()
+
+                    current_norm.update(dict(item=[None, max_val]))
+
+                    self.set_normalizations(current_norm)
+
+                    result.assign_attrs(
+                        dict(
+                            short_description=condition.short_description,
+                            long_description=condition.long_description,
+                            name=f'Change w.r.t. historical of\n{da.name}',
+                        )
+                    )
+
+                    return result
+                return self.__getattribute__(item)
+
+        mm = TempMapMaker(self.dataset)
+        axes = mm.plot_all(2)
+        # masks = self.get_masks()
+        # for ax in axes:
+        #     self._plot_masks(masks, ax=ax, legend=False)
+        plt.suptitle(self.title, y=0.95)
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-0.2.2/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .xarray_tools import apply_abs, _native_date_fmt
+from .xarray_tools import apply_abs, _native_date_fmt, _remove_any_none_times
 from optim_esm_tools.utils import check_accepts, timed
 import xarray as xr
 import numpy as np
 import typing as ty
 from .globals import _SECONDS_TO_YEAR
 import abc
 from immutabledict import immutabledict
@@ -115,15 +115,15 @@
 
 
 @timed
 @apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def running_mean_diff(
     data_set: xr.Dataset,
-    variable: str = 'tas',
+    variable: str,
     time_var: str = 'time',
     naming: str = '{variable}_run_mean_{running_mean}',
     running_mean: int = 10,
     rename_to: str = 'long_name',
     unit: str = 'absolute',
     apply_abs: bool = True,
     _t_0_date: ty.Optional[tuple] = None,
@@ -167,15 +167,15 @@
         t_1 = _native_date_fmt(_time_values, _t_1_date)
         data_t_1 = data_var.sel(time=t_1, method='nearest')
     else:
         data_t_1 = data_var.isel(time=-1)
 
     result = data_t_1 - data_t_0
     result = result.copy()
-    var_unit = data_var.attrs.get('units', '{units}')
+    var_unit = data_var.attrs.get('units', '{units}').replace('%', '\%')
     name = data_var.attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f't[-1] - t[0] for {name} [{var_unit}]'
         return result
 
     if unit == 'relative':
@@ -191,26 +191,26 @@
 
 
 @timed
 @apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def running_mean_std(
     data_set: xr.Dataset,
-    variable: str = 'tas',
+    variable: str,
     time_var: str = 'time',
     naming: str = '{variable}_detrend_run_mean_{running_mean}',
     running_mean: int = 10,
     rename_to: str = 'long_name',
     apply_abs: bool = True,
     unit: str = 'absolute',
 ) -> xr.Dataset:
     data_var = naming.format(variable=variable, running_mean=running_mean)
     result = data_set[data_var].std(dim=time_var)
     result = result.copy()
-    var_unit = data_set[data_var].attrs.get('units', '{units}')
+    var_unit = data_set[data_var].attrs.get('units', '{units}').replace('%', '\%')
     name = data_set[data_var].attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f'Std. {name} [{var_unit}]'
         return result
 
     if unit == 'relative':
@@ -225,15 +225,15 @@
 
 
 @timed
 @apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def max_change_xyr(
     data_set: xr.Dataset,
-    variable: str = 'tas',
+    variable: str,
     time_var: str = 'time',
     naming: str = '{variable}_run_mean_{running_mean}',
     x_yr: ty.Union[int, float] = 10,
     running_mean: int = 10,
     rename_to: str = 'long_name',
     apply_abs: bool = True,
     unit: str = 'absolute',
@@ -242,15 +242,15 @@
     plus_x_yr = data_set.isel({time_var: slice(x_yr, None)})[data_var]
     to_min_x_yr = data_set.isel({time_var: slice(None, -x_yr)})[data_var]
 
     # Keep the metadata (and time stamps of the to_min_x_yr)
     result = to_min_x_yr.copy(data=plus_x_yr.values - to_min_x_yr.values)
 
     result = result.max(dim=time_var).copy()
-    var_unit = data_set[data_var].attrs.get('units', '{units}')
+    var_unit = data_set[data_var].attrs.get('units', '{units}').replace('%', '\%')
     name = data_set[data_var].attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f'{x_yr} yr diff. {name} [{var_unit}]'
         return result
 
     if unit == 'relative':
@@ -265,28 +265,28 @@
 
 
 @timed
 @apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def max_derivative(
     data_set: xr.Dataset,
-    variable: str = 'tas',
+    variable: str,
     time_var: str = 'time',
     naming: str = '{variable}_run_mean_{running_mean}',
     running_mean: int = 10,
     rename_to: str = 'long_name',
     apply_abs: bool = True,
     unit: str = 'absolute',
 ) -> xr.Dataset:
     var_name = naming.format(variable=variable, running_mean=running_mean)
 
     data_array = _remove_any_none_times(data_set[var_name], time_var)
     result = data_array.differentiate(time_var).max(dim=time_var) * _SECONDS_TO_YEAR
 
-    var_unit = data_array.attrs.get('units', '{units}')
+    var_unit = data_array.attrs.get('units', '{units}').replace('%', '\%')
     name = data_array.attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f'Max $\partial/\partial t$ {name} [{var_unit}/yr]'
         return result
 
     if unit == 'relative':
@@ -295,31 +295,7 @@
         return result
 
     if unit == 'std':
         # A local unit of sigma might be better X.std(dim=time_var)
         result = result / data_array.std()
         result.name = f'Max $\partial/\partial t$ {name} [$\sigma$/yr]'
         return result
-
-
-def _remove_any_none_times(da, time_dim):
-    data_var = da.copy()
-    time_null = data_var.isnull().all(dim=set(data_var.dims) - {time_dim})
-    if np.all(time_null):
-        # If we take a running mean of 10 (the default), and the array is shorter than
-        # 10 years we will run into issues here because a the window is longer than the
-        # array. Perhaps we should raise higher up.
-        raise ValueError(
-            f'This array only has NaN values, perhaps array too short ({len(time_null)} < 10)?'
-        )
-    if np.any(time_null):
-        try:
-            # For some reason only alt_calc seems to work even if it should be equivalent to the data_var
-            # I think there is some fishy indexing going on in pandas <-> dask
-            # Maybe worth raising an issue?
-            alt_calc = xr.where(~time_null, da, np.nan).dropna('time')
-            data_var = data_var.load().where(~time_null, drop=True)
-            assert np.all((alt_calc == data_var).values)
-        except IndexError as e:
-            print(e)
-            return alt_calc
-    return data_var
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/cmip_files/io.py` & `optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         rename_cmip6,
         broadcast_lonlat,
     )
 
     ds = data_set.copy()
     # See https://github.com/jbusecke/xMIP/issues/299
     for k, v in {'longitude': 'lon', 'latitude': 'lat'}.items():
-        if k in ds:
+        if k in ds and v not in ds:
             ds = ds.rename({k: v})
     ds = rename_cmip6(ds)
     ds = promote_empty_dims(ds)
     ds = broadcast_lonlat(ds)
     import xmip.preprocessing
 
     xmip.preprocessing._interp_nominal_lon = _interp_nominal_lon_new
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/config.py` & `optim_esm_tools-0.2.2/optim_esm_tools/config.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/plotting/map_maker.py` & `optim_esm_tools-0.2.2/optim_esm_tools/plotting/map_maker.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing as ty
 import collections
 from warnings import warn
 
 import matplotlib.pyplot as plt
 
 from immutabledict import immutabledict
-
+from .plot import default_variable_labels
 
 # import xrft
 
 from optim_esm_tools.analyze.globals import _SECONDS_TO_YEAR
 from optim_esm_tools.analyze.tipping_criteria import (
     StartEndDifference,
     StdDetrended,
@@ -25,14 +25,25 @@
 
 class MapMaker(object):
     data_set: xr.Dataset
     labels = tuple('i ii iii iv v vi vii viii ix x'.split())
     kw: ty.Mapping
     contitions: ty.Mapping
 
+    def __init__(
+        self,
+        data_set: xr.Dataset,
+        normalizations: ty.Union[None, ty.Mapping, ty.Iterable] = None,
+        **conditions,
+    ):
+        self.data_set = data_set
+        self.set_kw()
+        self.set_conditions(**conditions)
+        self.set_normalizations(normalizations)
+
     def set_kw(self):
         import cartopy.crs as ccrs
 
         self.kw = immutabledict(
             fig=dict(dpi=200, figsize=(14, 10)),
             title=dict(fontsize=12),
             gridspec=dict(hspace=0.3),
@@ -51,23 +62,18 @@
         }
         self.labels = tuple(self.conditions.keys())
 
     normalizations: ty.Optional[ty.Mapping] = None
 
     _cache: bool = False
 
-    def __init__(
+    def set_normalizations(
         self,
-        data_set: xr.Dataset,
         normalizations: ty.Union[None, ty.Mapping, ty.Iterable] = None,
-        **conditions,
     ):
-        self.data_set = data_set
-        self.set_kw()
-        self.set_conditions(**conditions)
         if normalizations is None:
             self.normalizations = {i: [None, None] for i in self.conditions.keys()}
         elif isinstance(normalizations, collections.abc.Mapping):
             self.normalizations = normalizations
         elif isinstance(normalizations, collections.abc.Iterable):
             self.normalizations = {
                 i: normalizations[j] for j, i in enumerate(self.conditions.keys())
@@ -208,15 +214,15 @@
         )
         plot_kw['label'] = labels.get(
             f'{variable}_run_mean_{running_mean}',
             f'{variable} running mean {running_mean}',
         )
         self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
 
-        plt.ylabel('T [K]')
+        plt.ylabel(f'{self.variable_name(variable)} [{self.unit(variable)}]')
         plt.legend()
         plt.title('')
 
     def _det_ts(
         self,
         variable,
         ds=None,
@@ -241,15 +247,15 @@
             ds, f'{variable}_detrend_run_mean_{running_mean}', other_dim
         )
         plot_kw['label'] = labels.get(
             f'{variable}_detrend_run_mean_{running_mean}',
             f'detrended {variable} running mean {running_mean}',
         )
         self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
-        plt.ylabel('detrend(T) [K]')
+        plt.ylabel(f'Detrend {self.variable_name(variable)} [{self.unit(variable)}]')
         plt.legend()
         plt.title('')
 
     def _ddt_ts(
         self,
         variable,
         ds=None,
@@ -286,15 +292,17 @@
         label = f"{labels.get(variable_rm, f'{variable} running mean {running_mean}')}"
         dy_dt_rm.plot(label=label, **plot_kw)
         # mean, std = self._mean_and_std(dy_dt_rm, variable=None, other_dim=other_dim)
         # plot_kw['label'] = variable
         # self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
 
         plt.ylim(dy_dt_rm.min() / 1.05, dy_dt_rm.max() * 1.05)
-        plt.ylabel('$\partial T/\partial t$ [K/yr]')
+        plt.ylabel(
+            f'$\partial \mathrm{{{self.variable_name(variable)}}} /\partial t$ [{self.unit(variable)}/yr]'
+        )
         plt.legend()
         plt.title('')
 
     @staticmethod
     def _mean_and_std(ds, variable, other_dim):
         if variable is None:
             da = ds
@@ -311,17 +319,14 @@
         time='time',
         other_dim=('x', 'y'),
         running_mean=10,
         interval=True,
         axes=None,
         **kw,
     ):
-        if variable != 'tas':
-            raise NotImplementedError('Currently only works for tas')
-
         ds = self.data_set
         if interval is False:
             ds = ds.copy().mean(other_dim)
             other_dim = None
 
         plot_kw = dict(**kw)
 
@@ -355,12 +360,25 @@
         warn('MapMaker.ds is depricated, use MapMaker.data_set')
         return self.data_set
 
     @property
     def title(self):
         return make_title(self.data_set)
 
+    def variable_name(self, variable):
+        return default_variable_labels().get(
+            variable,
+            variable,  # self.data_set[variable].attrs.get('long_name', variable)
+        )
+
+    def unit(self, variable):
+        return (
+            self.data_set[variable]
+            .attrs.get('units', f'?{variable}?')
+            .replace('%', '\%')
+        )
+
 
 def make_title(ds):
     return '{institution_id} {source_id} {experiment_id} {variant_label} {variable_id} {version}'.format(
         **ds.attrs
     )
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-0.2.2/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools/utils.py` & `optim_esm_tools-0.2.2/optim_esm_tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,15 @@
             return response
 
         return somedec_inner
 
     return somedec_outer
 
 
-def depricated(func, message='is depricated'):
+def deprecated(func, message='is deprecated'):
     @wraps(func)
     def dep_fun(*args, **kwargs):
         warnings.warn(
             f'calling {func.__name__} {message}',
             category=DeprecationWarning,
         )
         return func(*args, **kwargs)
@@ -333,15 +333,19 @@
         @wraps(fn)
         def timed_func(*args, **kwargs):
             t0 = time.time()
             res = fn(*args, **kwargs)
             dt = time.time() - t0
             if dt > seconds:
                 hours = '' if dt < 3600 else f' ({dt/3600:{_fmt}} h) '
-                message = f'{fn.__name__} took {dt:{_fmt}} s{hours} (for {_chopped_string(args, _args_max)}, {_chopped_string(kwargs,_args_max)})'
+                message = (
+                    f'{fn.__name__} took {dt:{_fmt}} s{hours} (for '
+                    f'{_chopped_string(args, _args_max)}, '
+                    f'{_chopped_string(kwargs,_args_max)})'
+                ).replace('\n', ' ')
                 if _report == 'print':
                     print(message)
                 else:
                     from .config import get_logger
 
                     getattr(get_logger(), _report)(message)
             return res
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-0.2.2/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim-esm-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,25 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.2.2 / 2023-07-02
+        ------------------
+        * Remove todo by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/67
+        * small tas tweaks by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/68
+        * Add non-tas support by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/69
+        * Match fuzzy for version last by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/70
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.2.1...v0.2.2
+        
+        
         0.2.1 / 2023-06-21
         ------------------
         * Add few badges (#62) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/62
         * Fix few codefactor issues (#63) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/63
         * Delete workspace directory (#64) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/64
         * simplify find_historical (#65) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/65
         * Fix finding (#66) by @JoranAngevarae in https://github.com/JoranAngevaare/optim_esm_tools/pull/66
```

### Comparing `optim_esm_tools-0.2.1/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-0.2.2/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.1/setup.py` & `optim_esm_tools-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='0.2.1',
+    version='0.2.2',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages() + ['extra_requirements'],
     package_dir={
```

### Comparing `optim_esm_tools-0.2.1/test/test_clustering.py` & `optim_esm_tools-0.2.2/test/test_clustering.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.1/test/test_find_matches.py` & `optim_esm_tools-0.2.2/test/test_find_matches.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 )
 
 
 @unittest.skipIf(not synda_test_available(), 'synda data not available')
 class TestMatches(unittest.TestCase):
     def test_find_matches(self):
         head = os.path.join(get_synda_loc(), 'CMIP6')
-        kw = oet.cmip_files.find_matches.folder_to_dict(get_example_data_loc())
+        path = get_example_data_loc()
+        kw = oet.cmip_files.find_matches.folder_to_dict(path)
         assert len(
             oet.cmip_files.find_matches.find_matches(
                 base=head,
+                required_file=os.path.split(path)[1],
                 **kw,
             )
         )
```

### Comparing `optim_esm_tools-0.2.1/test/test_region_finding.py` & `optim_esm_tools-0.2.2/test/test_region_finding.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,20 @@
         year_path = optim_esm_tools._test_utils.year_means(path, refresh=refresh)
         assert year_path
         assert os.path.exists(year_path)
         return year_path
 
     def test_max_region(self, make='MaxRegion', new_opt=None):
         cls = getattr(region_finding, make)
-        extra_opt = dict(time_series_joined=True, scatter_medians=True, percentiles=50)
+        extra_opt = dict(
+            time_series_joined=True,
+            scatter_medians=True,
+            percentiles=50,
+            search_kw=dict(required_file=os.path.split(self.get_path('ssp585'))[1]),
+        )
         if new_opt:
             extra_opt.update(new_opt)
         with tempfile.TemporaryDirectory() as temp_dir:
             save_kw = dict(
                 save_in=temp_dir,
                 sub_dir=None,
                 file_types=('png',),
@@ -54,7 +59,13 @@
         self.test_max_region('Percentiles', new_opt=dict(time_series_joined=False))
 
     def test_percentiles_history(self):
         region_finder = self.test_max_region('PercentilesHistory')
         with self.assertRaises(RuntimeError):
             # We only have piControl (so this should fail)!
             region_finder.find_historical('historical')
+
+    def test_percentiles_product(self):
+        self.test_max_region('ProductPercentiles')
+
+    def test_local_history(self):
+        self.test_max_region('LocalHistory')
```

### Comparing `optim_esm_tools-0.2.1/test/test_utils.py` & `optim_esm_tools-0.2.2/test/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,17 @@
             [0, 'debug', 1, '.06'],
             [0, 'warning', 1, '.1f'],
         ],
     )
     def test_timing(self, seconds, report, args_max, fmt):
         kw = dict(seconds=seconds, _report=report, _args_max=args_max, _fmt=fmt)
         self._timeing_decorator(**kw)
+
+
+class TestDepricated(unittest.TestCase):
+    def test(self):
+        @oet.utils.deprecated
+        def bla(a):
+            return a
+
+        with self.assertWarns(DeprecationWarning):
+            bla(1)
```

### Comparing `optim_esm_tools-0.2.1/test/test_viewer.py` & `optim_esm_tools-0.2.2/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.1/test/test_workflow.py` & `optim_esm_tools-0.2.2/test/test_workflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         )
 
     def setUp(self):
         self.from_amon_to_ayear()
         super().setUp()
 
     def test_read_data(self):
-        data_set = oet.synda_files.format_synda.load_glob(self.ayear_file)
+        data_set = oet.cmip_files.io.load_glob(self.ayear_file)
 
     def test_make_map(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
-        oet.analyze.cmip_handler.MapMaker(data_set=data_set).plot_all(2)
+        oet.plotting.map_maker.MapMaker(data_set=data_set).plot_all(2)
         plt.clf()
 
     def test_map_maker_time_series(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
-        oet.analyze.cmip_handler.MapMaker(data_set=data_set).time_series()
+        oet.plotting.map_maker.MapMaker(data_set=data_set).time_series()
         plt.clf()
 
     @classmethod
     def tearDownClass(cls) -> None:
         os.remove(cls.ayear_file)
         return super().tearDownClass()
 
@@ -63,11 +63,11 @@
                 year_means(
                     get_file_from_pangeo('ssp585', refresh=refresh), refresh=refresh
                 )
             )[0],
             condition_kwargs=dict(unit=unit),
             _file_name='test_merged.nc',
         )
-        mm = oet.analyze.cmip_handler.MapMaker(data_set=data_set)
+        mm = oet.plotting.map_maker.MapMaker(data_set=data_set)
 
     def test_apply_std_unit(self):
         self.test_apply_relative_units(unit='std')
```

