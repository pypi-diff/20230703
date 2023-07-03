# Comparing `tmp/gbd_tools-4.6.0.tar.gz` & `tmp/gbd_tools-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.6.0.tar", last modified: Mon Jul  3 07:46:05 2023, max compression
+gzip compressed data, was "gbd_tools-4.6.2.tar", last modified: Mon Jul  3 12:30:21 2023, max compression
```

## Comparing `gbd_tools-4.6.0.tar` & `gbd_tools-4.6.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.6.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/README.md
--rwxrwxr-x   0 root         (0) root         (0)    12281 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.852690 gbd_tools-4.6.0/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.6.0/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10487 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     2395 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    12223 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     6526 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5356 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12510 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.856690 gbd_tools-4.6.0/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.6.0/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4113 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/benchmark_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     7841 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/feature_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     2574 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3088 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.856690 gbd_tools-4.6.0/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.856690 gbd_tools-4.6.0/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.6.0/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11998 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-07-03 07:45:45.000000 gbd_tools-4.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.6.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    12309 2023-07-03 12:27:26.000000 gbd_tools-4.6.2/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.6.2/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10487 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2395 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    12310 2023-07-03 12:25:07.000000 gbd_tools-4.6.2/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     6526 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5356 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12510 2023-07-03 12:24:04.000000 gbd_tools-4.6.2/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.6.2/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4113 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_init/benchmark_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     8685 2023-07-03 10:15:03.000000 gbd_tools-4.6.2/gbd_init/feature_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     2574 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3088 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.6.2/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11998 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-07-03 12:25:39.000000 gbd_tools-4.6.2/setup.py
```

### Comparing `gbd_tools-4.6.0/LICENSE` & `gbd_tools-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/PKG-INFO` & `gbd_tools-4.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.6.0
+Version: 4.6.2
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.6.0/README.md` & `gbd_tools-4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd.py` & `gbd_tools-4.6.2/gbd.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     init_local(api, rlimits, args.path, args.target_db)
 
 
 def cli_init_generic(api: GBD, args):
     from gbd_init.feature_extractors import init_features_generic
     rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
     context = api.database.dcontext(args.target_db)
-    df = api.query(args.query, args.hashes, [ context + ":local" ], collapse="MIN")
+    df = api.query(args.query, args.hashes, [ context + ":local" ], collapse="MIN", group_by=context + ":hash")
     init_features_generic(args.initfuncname, api, rlimits, df, args.target_db)
 
 
 def cli_trans_cnf2kis(api: GBD, args):
     from gbd_init.benchmark_transformers import init_transform_cnf_to_kis
     rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
     init_transform_cnf_to_kis(api, rlimits, args.query, args.hashes, args.target_db, args.source)
```

### Comparing `gbd_tools-4.6.0/gbd_core/api.py` & `gbd_tools-4.6.2/gbd_core/api.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_core/contexts.py` & `gbd_tools-4.6.2/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_core/database.py` & `gbd_tools-4.6.2/gbd_core/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
                 # first found feature is used: (=feature precedence by database position)
                 if not feature.name in result:
                     result[feature.name] = [ feature ]
                 elif feature.column == "hash" and feature.table == "features": 
                     # first found features table is the one that serves the hash
                     if result[feature.name][0].table != "features":
                         result[feature.name].insert(0, feature)
+                    else:
+                        result[feature.name].append(feature)
                 else:
                     result[feature.name].append(feature)
         return result
 
 
     def query(self, q):
         if self.verbose:
```

### Comparing `gbd_tools-4.6.0/gbd_core/grammar.py` & `gbd_tools-4.6.2/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_core/query.py` & `gbd_tools-4.6.2/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_core/schema.py` & `gbd_tools-4.6.2/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_core/util.py` & `gbd_tools-4.6.2/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_core/util_argparse.py` & `gbd_tools-4.6.2/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_init/benchmark_transformers.py` & `gbd_tools-4.6.2/gbd_init/benchmark_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_init/feature_extractors.py` & `gbd_tools-4.6.2/gbd_init/feature_extractors.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from gbd_core.contexts import suffix_list, identify
 from gbd_core.api import GBD, GBDException
 from gbd_core.util import eprint, confirm
 from gbd_init.initializer import Initializer, InitializerException
 
 try:
-    from gbdc import extract_base_features, extract_gate_features, isohash
+    from gbdc import extract_base_features, extract_gate_features, isohash, extract_red_base_features
 except ImportError:
     def extract_base_features(path, tlim, mlim):
         return [ ]
 
     def extract_gate_features(path, tlim, mlim):
         return [ ]
     
@@ -49,14 +49,20 @@
 
 ## Base Features
 def compute_base_features(hash, path, limits):
     eprint('Extracting base features from {} {}'.format(hash, path))
     rec = extract_base_features(path, limits['tlim'], limits['mlim'])
     return [ (key, hash, int(value) if isinstance(value, float) and value.is_integer() else value) for key, value in rec.items() ]
 
+## Base Features
+def compute_reduced_base_features(hash, path, limits):
+    eprint('Extracting reduced base features from {} {}'.format(hash, path))
+    rec = extract_red_base_features(path, limits['tlim'], limits['mlim'])
+    return [ (key, hash, int(value) if isinstance(value, float) and value.is_integer() else value) for key, value in rec.items() ]
+
 ## Gate Features
 def compute_gate_features(hash, path, limits):
     eprint('Extracting gate features from {} {}'.format(hash, path))
     rec = extract_gate_features(path, limits['tlim'], limits['mlim'])
     return [ (key, hash, int(value) if isinstance(value, float) and value.is_integer() else value) for key, value in rec.items() ]   
 
 
@@ -72,14 +78,21 @@
             ("balance_clause_mean", "empty"), ("balance_clause_variance", "empty"), ("balance_clause_min", "empty"), ("balance_clause_max", "empty"), ("balance_clause_entropy", "empty"),
             ("balance_vars_mean", "empty"), ("balance_vars_variance", "empty"), ("balance_vars_min", "empty"), ("balance_vars_max", "empty"), ("balance_vars_entropy", "empty"),
             ("vcg_vdegrees_mean", "empty"), ("vcg_vdegrees_variance", "empty"), ("vcg_vdegrees_min", "empty"), ("vcg_vdegrees_max", "empty"), ("vcg_vdegrees_entropy", "empty"),
             ("vcg_cdegrees_mean", "empty"), ("vcg_cdegrees_variance", "empty"), ("vcg_cdegrees_min", "empty"), ("vcg_cdegrees_max", "empty"), ("vcg_cdegrees_entropy", "empty"),
             ("cg_degrees_mean", "empty"), ("cg_degrees_variance", "empty"), ("cg_degrees_min", "empty"), ("cg_degrees_max", "empty"), ("cg_degrees_entropy", "empty") ],
         "compute" : compute_base_features,
     },
+    "base_reduced" : {
+        "contexts" : [ "cnf" ],
+        "features" : [ ("clauses", "empty"), ("variables", "empty"), ("clause_size_1", "empty"), ("clause_size_2", "empty"), ("clause_size_3", "empty"), 
+            ("clause_size_4", "empty"), ("clause_size_5", "empty"), ("clause_size_6", "empty"), ("clause_size_7", "empty"), 
+            ("clause_size_8", "empty"), ("clause_size_9", "empty") ],
+        "compute" : compute_reduced_base_features,
+    },
     "gate" : {
         "contexts" : [ "cnf" ],
         "features" : [ ("gate_features_runtime", "empty"), ("n_vars", "empty"), ("n_gates", "empty"), ("n_roots", "empty"),
             ("n_none", "empty"), ("n_generic", "empty"), ("n_mono", "empty"), ("n_and", "empty"), ("n_or", "empty"), ("n_triv", "empty"), ("n_equiv", "empty"), ("n_full", "empty"),
             ("levels_mean", "empty"), ("levels_variance", "empty"), ("levels_min", "empty"), ("levels_max", "empty"), ("levels_entropy", "empty"),
             ("levels_none_mean", "empty"), ("levels_none_variance", "empty"), ("levels_none_min", "empty"), ("levels_none_max", "empty"), ("levels_none_entropy", "empty"),
             ("levels_generic_mean", "empty"), ("levels_generic_variance", "empty"), ("levels_generic_min", "empty"), ("levels_generic_max", "empty"), ("levels_generic_entropy", "empty"),
```

### Comparing `gbd_tools-4.6.0/gbd_init/gbdhash.py` & `gbd_tools-4.6.2/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_init/initializer.py` & `gbd_tools-4.6.2/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.6.2/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_server/static/main.css` & `gbd_tools-4.6.2/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_server/static/w3.js` & `gbd_tools-4.6.2/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_server/templates/index.html` & `gbd_tools-4.6.2/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.6.2/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.6.0
+Version: 4.6.2
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.6.0/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.6.2/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/server.py` & `gbd_tools-4.6.2/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.0/setup.py` & `gbd_tools-4.6.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.6.0',
+  version='4.6.2',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

