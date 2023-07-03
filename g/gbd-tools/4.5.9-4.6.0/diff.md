# Comparing `tmp/gbd_tools-4.5.9.tar.gz` & `tmp/gbd_tools-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.5.9.tar", last modified: Fri May 12 14:39:37 2023, max compression
+gzip compressed data, was "gbd_tools-4.6.0.tar", last modified: Mon Jul  3 07:46:05 2023, max compression
```

## Comparing `gbd_tools-4.5.9.tar` & `gbd_tools-4.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.9/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.9/README.md
--rwxrwxr-x   0 root         (0) root         (0)    12709 2023-05-12 14:36:20.000000 gbd_tools-4.5.9/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.9/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10378 2023-05-12 14:36:28.000000 gbd_tools-4.5.9/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10844 2023-05-12 14:34:38.000000 gbd_tools-4.5.9/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-10 11:45:07.000000 gbd_tools-4.5.9/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2023-05-10 15:10:05.000000 gbd_tools-4.5.9/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.9/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.9/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.9/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7756 2023-05-10 08:09:50.000000 gbd_tools-4.5.9/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.9/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.427838 gbd_tools-4.5.9/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.9/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.9/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.9/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.9/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-12 14:39:37.000000 gbd_tools-4.5.9/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11998 2023-05-11 12:09:25.000000 gbd_tools-4.5.9/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 14:39:37.431838 gbd_tools-4.5.9/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-12 14:38:56.000000 gbd_tools-4.5.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.6.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    12281 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.852690 gbd_tools-4.6.0/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.6.0/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10487 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2395 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    12223 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     6526 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5356 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12510 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.856690 gbd_tools-4.6.0/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.6.0/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4113 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/benchmark_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     7841 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/feature_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     2574 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3088 2023-07-03 07:45:22.000000 gbd_tools-4.6.0/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.856690 gbd_tools-4.6.0/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.856690 gbd_tools-4.6.0/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.6.0/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.6.0/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 07:46:05.000000 gbd_tools-4.6.0/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11998 2023-05-19 07:01:54.000000 gbd_tools-4.6.0/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 07:46:05.860690 gbd_tools-4.6.0/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-07-03 07:45:45.000000 gbd_tools-4.6.0/setup.py
```

### Comparing `gbd_tools-4.5.9/LICENSE` & `gbd_tools-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/PKG-INFO` & `gbd_tools-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.5.9
+Version: 4.6.0
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.9/README.md` & `gbd_tools-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd.py` & `gbd_tools-4.6.0/gbd.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,52 +18,46 @@
 import sys
 import traceback
 
 from gbd_core.api import GBD, GBDException
 from gbd_core.grammar import ParserException
 from gbd_core import util, contexts, schema
 from gbd_core.util_argparse import *
+from gbd_init.feature_extractors import generic_extractors
 
 
 ### Command-Line Interface Entry Points
 def cli_hash(api: GBD, args):
-    from gbd_init.gbdhash import identify
+    from gbd_core.contexts import identify
     print(identify(args.path))
 
 
 def cli_init_local(api: GBD, args):
-    from gbd_init.cnf_extractors import init_local
+    from gbd_init.feature_extractors import init_local
     rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
-    init_local(api, args.context, rlimits, args.path, target_db=args.target_db)
+    init_local(api, rlimits, args.path, args.target_db)
 
-def cli_init_base_features(api: GBD, args):
-    from gbd_init.cnf_extractors import init_base_features
-    rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
-    init_base_features(api, args.context, rlimits, args.query, args.hashes, target_db=args.target_db)
-
-def cli_init_gate_features(api: GBD, args):
-    from gbd_init.cnf_extractors import init_gate_features
-    rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
-    init_gate_features(api, args.context, rlimits, args.query, args.hashes, target_db=args.target_db)
 
-def cli_init_iso(api: GBD, args):
-    from gbd_init.cnf_extractors import init_isohash
+def cli_init_generic(api: GBD, args):
+    from gbd_init.feature_extractors import init_features_generic
     rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
-    init_isohash(api, args.context, rlimits, args.query, args.hashes, target_db=args.target_db)
+    context = api.database.dcontext(args.target_db)
+    df = api.query(args.query, args.hashes, [ context + ":local" ], collapse="MIN")
+    init_features_generic(args.initfuncname, api, rlimits, df, args.target_db)
 
 
-def cli_init_cnf2kis(api: GBD, args):
-    from gbd_init.cnf_transformers import init_transform_cnf_to_kis
+def cli_trans_cnf2kis(api: GBD, args):
+    from gbd_init.benchmark_transformers import init_transform_cnf_to_kis
     rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
-    init_transform_cnf_to_kis(api, args.context, rlimits, args.query, args.hashes, target_db=args.target_db)
+    init_transform_cnf_to_kis(api, rlimits, args.query, args.hashes, args.target_db, args.source)
 
-def cli_init_sani(api: GBD, args):
-    from gbd_init.cnf_transformers import init_sani
+def cli_trans_sani(api: GBD, args):
+    from gbd_init.benchmark_transformers import init_sani
     rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
-    init_sani(api, args.context, rlimits, args.query, args.hashes, target_db=args.target_db)
+    init_sani(api, rlimits, args.query, args.hashes, args.target_db, args.source)
 
 
 def cli_create(api: GBD, args):
     api.create_feature(args.name, args.unique, args.target_db)
 
 def cli_delete(api: GBD, args):
     if args.hashes and len(args.hashes) or args.values and len(args.values):
@@ -103,15 +97,15 @@
             if len(api.get_features(dbname)):
                 print("\nDatabase: {}".format(api.get_database_path(dbname)))
                 print("Name: " + dbname)
                 feat = api.get_features(dbname)
                 print("Features: " + " ".join(feat))
                 if args.verbose:
                     for f in feat:
-                        info = api.database.finfo(f, dbname)
+                        info = api.database.find(":".join([ dbname, f ]))
                         print(info)
     else:
         info = api.get_feature_info(args.name)
         for key in info:
             print("{}: {}".format(key, info[key]))
 
 
@@ -120,43 +114,45 @@
     parser = get_gbd_argparser()
 
     subparsers = parser.add_subparsers(help='Available Commands:', required=True, dest='gbd command')
 
     # INITIALIZATION 
     parser_init = subparsers.add_parser('init', help='Initialize Database')
     add_resource_limits_arguments(parser_init)
-    parser_init.add_argument('--target_db', help='Target database (default: first in list)', default=None)
-    parser_init.add_argument('-c', '--context', default='cnf', choices=contexts.contexts(), help='Select context (affects selection of hash selection and initializers)')
+    parser_init.add_argument('--target_db', help='Target database; determines target context (default: first db in list)', default=None)
 
     parser_init_subparsers = parser_init.add_subparsers(help='Select Initialization Procedure:', required=True, dest='init what?')
 
     # init local paths:
     parser_init_local = parser_init_subparsers.add_parser('local', help='Initialize Local Hash/Path Entries')
     parser_init_local.add_argument('path', type=directory_type, help="Path to benchmarks")
     parser_init_local.set_defaults(func=cli_init_local)
-    # init base features:
-    parser_init_base_features = parser_init_subparsers.add_parser('base_features', help='Initialize Base Features')
-    add_query_and_hashes_arguments(parser_init_base_features)
-    parser_init_base_features.set_defaults(func=cli_init_base_features)
-    # init gate features:
-    parser_init_gate_features = parser_init_subparsers.add_parser('gate_features', help='Initialize Gate Features')
-    add_query_and_hashes_arguments(parser_init_gate_features)
-    parser_init_gate_features.set_defaults(func=cli_init_gate_features)
+
+    # hooks for generic feature extractors:
+    for key in generic_extractors.keys():
+        parser_init_generic = parser_init_subparsers.add_parser(key, help='Initialize Featureset {}, valid contexts are: {}'.format(key, ", ".join(generic_extractors[key]["contexts"])))
+        add_query_and_hashes_arguments(parser_init_generic)
+        parser_init_generic.set_defaults(func=cli_init_generic, initfuncname=key)
+
+    # TRANSFORMATION
+    parser_trans = subparsers.add_parser('transform', help='Transform Benchmarks')
+    add_resource_limits_arguments(parser_trans)
+    parser_trans.add_argument('--source', help='Source context', default='cnf')
+    parser_trans.add_argument('--target_db', help='Target database; determines target context (default: first db in list)', default=None)
+
+    parser_trans_subparsers = parser_trans.add_subparsers(help='Select Transformation Procedure:', required=True, dest='transform how?')
+    
     # generate kis instances from cnf instances:
-    parser_init_cnf2kis = parser_init_subparsers.add_parser('cnf2kis', help='Generate KIS Instances from CNF Instances')
-    add_query_and_hashes_arguments(parser_init_cnf2kis)
-    parser_init_cnf2kis.set_defaults(func=cli_init_cnf2kis)
-    # init iso-hash:
-    parser_init_iso = parser_init_subparsers.add_parser('isohash', help='Initialize Isomorphic Hash (MD5 of sorted degree sequence)')
-    add_query_and_hashes_arguments(parser_init_iso)
-    parser_init_iso.set_defaults(func=cli_init_iso)
+    parser_trans_cnf2kis = parser_trans_subparsers.add_parser('cnf2kis', help='Generate KIS Instances from CNF Instances')
+    add_query_and_hashes_arguments(parser_trans_cnf2kis)
+    parser_trans_cnf2kis.set_defaults(func=cli_trans_cnf2kis)
     # init sanitized:
-    parser_init_sani = parser_init_subparsers.add_parser('sanitize', help='Initialize sanitized benchmarks')
-    add_query_and_hashes_arguments(parser_init_sani)
-    parser_init_sani.set_defaults(func=cli_init_sani)
+    parser_trans_sani = parser_trans_subparsers.add_parser('sanitize', help='Initialize sanitized benchmarks')
+    add_query_and_hashes_arguments(parser_trans_sani)
+    parser_trans_sani.set_defaults(func=cli_trans_sani)
 
     # GBD HASH
     parser_hash = subparsers.add_parser('hash', help='Print hash for a single file')
     parser_hash.add_argument('path', type=file_type, help="Path to one benchmark")
     parser_hash.set_defaults(func=cli_hash)
 
     # GBD GET $QUERY
```

### Comparing `gbd_tools-4.5.9/gbd_core/api.py` & `gbd_tools-4.6.0/gbd_core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
             Args:
                 path (str): path to benchmark
 
             Returns:
                 str: GBD hash
         """
-        from gbd_init.gbdhash import identify
+        from gbd_core.contexts import identify
         return identify(path)
 
 
     def query(self, gbd_query=None, hashes=[], resolve=[], collapse="group_concat", group_by="hash", join_type="LEFT"):
         query_builder = GBDQuery(self.database, gbd_query)
         try:
             sql = query_builder.build_query(hashes, resolve or [], group_by or "hash", join_type, collapse)
@@ -71,15 +71,17 @@
             raise GBDException("Parser Error with Query '{}': {}".format(gbd_query, str(err)))
         try:
             result = self.database.query(sql)
         except sqlite3.OperationalError as err:
             if self.verbose:
                 util.eprint(traceback.format_exc())
             raise GBDException("Database Operational Error: {}".format(str(err)))
-        return pd.DataFrame(result, columns=[ group_by ] + (resolve or []))
+        cols = [ p.split(':') for p in [ group_by ] + (resolve or []) ]
+        cols = [ c[0] if len(c) == 1 else c[1] for c in cols ]
+        return pd.DataFrame(result, columns=cols)
 
 
     def set_values(self, name, value, hashes, target_db=None):
         """ Set feature value for given hashes 
             
             Args:
                 name (str): feature name
@@ -158,15 +160,15 @@
             Returns: path to database
         """
         return self.database.dpath(dbname)
 
 
     # Retrieve information about a specific feature
     def get_feature_info(self, fname):
-        finfo = self.database.finfo(fname)
+        finfo = self.database.find(fname)
         df = self.query(resolve=[ fname ], collapse=None)
         numcol = df[fname].apply(lambda x: pd.to_numeric(x, errors = 'coerce'))
         return {
             'feature_name': fname,
             'feature_count': len(df.index),
             'feature_default': finfo.default,
             'feature_min': numcol.min(),
```

### Comparing `gbd_tools-4.5.9/gbd_core/contexts.py` & `gbd_tools-4.6.0/gbd_core/contexts.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,50 +9,66 @@
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
 
+from gbd_init.gbdhash import cnf_hash, opb_hash
 
-packed = [ "", ".gz", ".lzma", ".xz", ".bz2" ]
 
+packed = [ "", ".gz", ".lzma", ".xz", ".bz2" ]
+# EDACC by Balint
 context_data = {
     "cnf" : {
         "id" : 100,
-        "suffixes" : [ ".cnf" + p for p in packed ],
         "description" : "Conjunctive Normal Form (CNF) in DIMACS format",
+        "suffixes" : [ ".cnf" + p for p in packed ],
+        "hash": cnf_hash,
     },
     "sancnf" : {
         "id" : 101,
-        "suffixes" : [ ".sanitized.cnf" + p for p in packed ],
         "description" : "Sanitized Conjunctive Normal Form (CNF) in DIMACS format",
+        "suffixes" : [ ".sanitized.cnf" + p for p in packed ],
+        "hash": cnf_hash,
     },
     "kis" : {
         "id" : 200,
-        "suffixes" : [ ".kis" + p for p in packed ],
         "description" : "k-Independent Set (KIS) in DIMACS-like graph format",
+        "suffixes" : [ ".kis" + p for p in packed ],
+        "hash": cnf_hash,
     },
     "opb" : {
         "id" : 300,
-        "suffixes" : [ ".opb" + p for p in packed ],
         "description" : "Pseudo-Boolean Optimization Problem in OPB format",
+        "suffixes" : [ ".opb" + p for p in packed ],
+        "hash": opb_hash,
     },
     "wecnf" : {
         "id" : 400,
-        "suffixes" : [ ".wecnf" + p for p in packed ],
         "description" : "Weighted Extended Conjunctive Normal Form (WECNF)",
+        "suffixes" : [ ".wecnf" + p for p in packed ],
+        "hash": cnf_hash,
     },
 }
 
 def suffix_list(context):
     return context_data[context]['suffixes']
 
 def contexts():
     return context_data.keys()
 
-def get_context_by_suffix(filename):
+def get_context_by_suffix(benchmark):
     for context in contexts():
         for suffix in suffix_list(context):
-            if filename.endswith(suffix):
+            if benchmark.endswith(suffix):
                 return context
     return None
+    
+
+def identify(path, ct=None):
+    context = ct or get_context_by_suffix(path)    
+    if context is None:
+        raise Exception("Unable to associate context: " + path)
+    else:
+        idfunc = context_data[context]['hash']
+        return idfunc(path)
```

### Comparing `gbd_tools-4.5.9/gbd_core/database.py` & `gbd_tools-4.6.0/gbd_core/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -130,47 +130,72 @@
         
     def dtables(self, dbname):
         if not dbname in self.schemas:
             raise DatabaseException("Database {} not found".format(dbname))
         return self.schemas[dbname].get_tables()
 
 
-    def finfos(self, fname, db=None):
-        if not self.fexists(fname):
-            return [ ]
-        return [ info for info in self.features[fname] if (db is None or info.database == db) ]
-
     def finfo(self, fname, db=None):
-        infos = self.finfos(fname, db)
-        if len(infos) == 0:
-            raise DatabaseException("Feature {} does not exists in database {}".format(fname, db))
-        return infos[0]
-
-    def fexists(self, fname):
-        return fname in self.features
+        if fname in self.features and len(self.features[fname]) > 0:
+            if db is None:
+                return self.features[fname][0]
+            else:
+                infos = [ info for info in self.features[fname] if info.database == db ]
+                if len(infos) == 0:
+                    raise DatabaseException("Feature {} does not exists in database {}".format(fname, db))
+                return infos[0]
+        else:
+            raise DatabaseException("Feature {} does not exists".format(fname))
+        
 
-    def faddr_column(self, feature, db=None):
-        finfo = self.finfo(feature, db)
+    def faddr_column(self, feature):
+        finfo = self.find(feature)
         return "{}.{}.{}".format(finfo.database, finfo.table, finfo.column)
 
-    def faddr_table(self, feature, db=None):
-        finfo = self.finfo(feature, db)
+    def faddr_table(self, feature):
+        finfo = self.find(feature)
         return "{}.{}".format(finfo.database, finfo.table)
+    
 
-    def find(self, fid: str):
+    def find(self, fid: str, db: str=None):
+        """ Find feature by name or feature identifier
+        
+            Args:
+                fid: feature identifier, of the form "database:feature", "context:feature" or "feature"
+                db: database name (optional), if given fid is unique without database: or context: prefix
+
+            Returns:
+                FeatureInfo object: the info object for the first found feature
+                    feature precedence is according to the order of databases in the path list
+                    ambiguity can be resolved by using one of the following methods:
+                        - by giving a database name as the second argument or
+                        - by using the fid syntax "database:feature"
+                        - by using the fid syntax "context:feature" (note that this does not necessarily resolve all ambiguity)
+
+            Raises:
+                DatabaseException: if feature is not found or given database info is ambiguous
+        """
         parts = fid.split(":")
-        if len(parts) == 1:
+        if db is not None:
+            if len(parts) > 1:
+                if parts[0] != db:
+                    raise DatabaseException("Ambiguous database identifiers: '{}' and '{}'".format(parts[0], db))
+                else:
+                    return self.finfo(parts[1], parts[0])
+            return self.finfo(fid, db)
+        elif len(parts) == 1:
             return self.finfo(fid)
         elif parts[0] in self.get_databases():
             return self.finfo(parts[1], parts[0])
         elif parts[0] in self.get_contexts():
             db = self.get_databases(parts[0])[0]
             return self.finfo(parts[1], db)
         else:
             raise DatabaseException("Feature '{}' not found".format(fid))
+        
 
     def faddr(self, fid: str, with_column=True):
         finfo = self.find(fid)
 
         if with_column:
             return "{}.{}.{}".format(finfo.database, finfo.table, finfo.column)
         else:
@@ -259,12 +284,12 @@
     def delete_hashes_entirely(self, hashes, target_db=None):
         tables = self.get_tables([ target_db ])
         for table in tables:
             self.execute("DELETE FROM {}.{} WHERE hash IN ('{h}')".format(target_db, table, h="', '".join(hashes)))
 
 
     def copy_feature(self, old_name, new_name, target_db, hashlist=[]):
-        old_finfo = self.finfo(old_name)
+        old_finfo = self.find(old_name)
         data = self.query("SELECT hash, {col} FROM {d}.{tab} WHERE hash IN ('{h}')".format(d=old_finfo.database, col=old_finfo.column, tab=old_finfo.table, h="', '".join(hashlist)))
         for (hash, value) in data:
             self.set_values(new_name, value, [hash], target_db)
```

### Comparing `gbd_tools-4.5.9/gbd_core/grammar.py` & `gbd_tools-4.6.0/gbd_core/grammar.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,17 +36,17 @@
             | left:query qop:("and" | "or") ~ right:query 
             | constraint 
             | "(" q:query ")" 
             ;
 
         constraint 
             = 
-            | col:(column | dbname ":" column) cop:("=" | "!=") str:string 
-            | col:(column | dbname ":" column) cop:("=" | "!=" | "<=" | ">=" | "<" | ">" ) ter:termstart
-            | col:(column | dbname ":" column) cop:("like" | "unlike") ~ lik:(["%"] string ["%"])
+            | col:(dbname ":" column | column) cop:("=" | "!=") str:string 
+            | col:(dbname ":" column | column) cop:("=" | "!=" | "<=" | ">=" | "<" | ">" ) ter:termstart
+            | col:(dbname ":" column | column) cop:("like" | "unlike") ~ lik:(["%"] string ["%"])
             ;
 
         termstart 
             = 
             t:term
             ;
 
@@ -55,15 +55,15 @@
             | left:(term | termend) top:("+" | "-" | "*" | "/") right:(term | termend)
             | ("(") t:(term | termend) (")")
             | constant:number
             ;
 
         termend
             =
-            col:(column | dbname ":" column)
+            col:(dbname ":" column | column)
             ;
 
         number = /[-]?[0-9]+[.]?[0-9]*/ ;
         string = /[a-zA-Z0-9_\.\-\/\,\:]+/ ;
         column = /[a-zA-Z][a-zA-Z0-9_]*/ ;
         dbname = /[a-zA-Z][a-zA-Z0-9_]*/ ;
     '''
@@ -93,17 +93,17 @@
             if "q" in ast:
                 return self.get_features(ast["q"])
             elif "t" in ast:
                 return self.get_features(ast["t"])
             elif "qop" in ast or "top" in ast:
                 return self.get_features(ast["left"]) | self.get_features(ast["right"])
             elif "cop" in ast and "ter" in ast:
-                return { ast["col"] } | self.get_features(ast["ter"])
+                return { "".join(ast["col"]) } | self.get_features(ast["ter"])
             elif "col" in ast:
-                return { ast["col"] }
+                return { "".join(ast["col"]) }
             else: 
                 return set()
         except TypeError as e:
             raise ParserException("Failed to parse query: {}".format(str(e)))
 
 
     def get_sql(self, db: Database, ast=None):
@@ -116,41 +116,41 @@
             elif "qop" in ast or "top" in ast: # query operator or term operator
                 operator = ast["qop"] if ast["qop"] else ast["top"]
                 left = self.get_sql(db, ast["left"])
                 right = self.get_sql(db, ast["right"])
                 return "{} {} {}".format(left, operator, right)
             elif "cop" in ast: # constraint operator
                 operator = "not like" if ast["cop"] == "unlike" else ast["cop"]
-                feat = db.faddr(ast["col"])
-                feat_is_1_n = db.finfo(ast["col"]).default is None
+                feat = db.faddr("".join(ast["col"]))
+                feat_is_1_n = db.find("".join(ast["col"])).default is None
                 if "str" in ast: # cop:("=" | "!=")
                     if feat_is_1_n:
-                        table = db.faddr_table(ast["col"])
+                        table = db.faddr_table("".join(ast["col"]))
                         setop = "IN" if ast["cop"] == "=" else "NOT IN"
                         return "{t}.hash {o} (SELECT {t}.hash FROM {t} WHERE {f} = '{s}')".format(o=setop, t=table, f=feat, s=ast["str"])
                     else:
                         return "{} {} '{}'".format(feat, operator, ast["str"])
                 elif "lik" in ast: # cop:("like" | "unlike")
                     if feat_is_1_n:
-                        table = db.faddr_table(ast["col"])
+                        table = db.faddr_table("".join(ast["col"]))
                         setop = "IN" if ast["cop"] == "like" else "NOT IN"
                         return "{t}.hash {o} (SELECT {t}.hash FROM {t} WHERE {f} like '{s}')".format(o=setop, t=table, f=feat, s="".join([ t for t in ast["lik"] if t ]))
                     else:
                         return "{} {} '{}'".format(feat, operator, "".join([ t for t in ast["lik"] if t ]))
                 elif "ter" in ast: # cop:("=" | "!=" | "<=" | ">=" | "<" | ">" )
                     if feat_is_1_n and ast["cop"] == "!=":
-                        table = db.faddr_table(ast["col"])
+                        table = db.faddr_table("".join(ast["col"]))
                         setop = "NOT IN" if ast["cop"] == "!=" else "IN"
                         cop = "=" if ast["cop"] == "!=" else ast["cop"]
                         return "{t}.hash {o} (SELECT {t}.hash FROM {t} WHERE CAST({f} AS FLOAT) {c} {s})".format(o=setop, c=cop, t=table, f=feat, s=self.get_sql(db, ast["ter"]))
                     else:
                         return "CAST({} AS FLOAT) {} {}".format(feat, operator, self.get_sql(db, ast["ter"]))
                 raise ParserException("Missing right-hand side of constraint")
             elif "col" in ast:
-                feature = db.faddr(ast["col"])
+                feature = db.faddr("".join(ast["col"]))
                 return "CAST({} AS FLOAT)".format(feature)
             elif "constant" in ast:
                 return ast["constant"]
             else:
                 return "1=1"
         except TypeError as e:
             raise ParserException("Failed to parse query: {}".format(str(e)))
```

### Comparing `gbd_tools-4.5.9/gbd_core/query.py` & `gbd_tools-4.6.0/gbd_core/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,15 @@
         self.db = db
         self.parser = Parser(query)
         self.features = self.parser.get_features()
 
 
     def features_exist_or_throw(self, features):
         for feature in features:
-            if not feature in self.db.get_features():
-                raise DatabaseException("Unknown feature '{}'".format(feature))
+            self.db.find(feature)
 
 
     # Generate SQL Query from given GBD Query 
     def build_query(self, hashes=[], resolve=[], group_by="hash", join_type="LEFT", collapse=None):
         self.features_exist_or_throw(resolve + [group_by] + list(self.features))
 
         sql_select = self.build_select(group_by, resolve, collapse)
@@ -56,34 +55,34 @@
         return "SELECT DISTINCT " + ", ".join(result)
 
 
     def find_translator_feature(self, source_context, target_context):
         for dbname in self.db.get_databases(source_context):
             #eprint("Checking database {} for translator".format(dbname))
             if "to_"+target_context in self.db.get_features([ dbname ]):
-                return self.db.finfo("to_"+target_context, dbname)
+                return self.db.find("to_"+target_context, dbname)
         
         for dbname in self.db.get_databases(target_context):
             #eprint("Checking database {} for translator".format(dbname))
             if "to_"+source_context in self.db.get_features([ dbname ]):
-                return self.db.finfo("to_"+source_context, dbname)
+                return self.db.find("to_"+source_context, dbname)
         
         raise DatabaseException("No translator feature found for contexts {} and {}".format(source_context, target_context))
 
 
     def build_from(self, group, features, join_type="LEFT"):
         result = dict()
 
-        gdatabase = self.db.finfo(group).database
-        gtable = self.db.finfo(group).table
+        gdatabase = self.db.find(group).database
+        gtable = self.db.find(group).table
         gcontext = self.db.dcontext(gdatabase)
         gaddress = gdatabase + "." + gtable
         result[gaddress] = "FROM {}".format(gaddress)
 
-        tables = set([ (finfo.database, finfo.table) for finfo in [ self.db.finfo(f) for f in features ] ])
+        tables = set([ (finfo.database, finfo.table) for finfo in [ self.db.find(f) for f in features ] ])
         for (fdatabase, ftable) in tables:
             faddress = fdatabase + "." + ftable
             if not faddress in result: # join only once
                 fcontext = self.db.dcontext(fdatabase)
                 if fcontext == gcontext:
                     if ftable == "features": # join features table directly
                         result[faddress] = "{} JOIN {} ON {}.hash = {}.hash".format(join_type, faddress, gaddress, faddress)
```

### Comparing `gbd_tools-4.5.9/gbd_core/schema.py` & `gbd_tools-4.6.0/gbd_core/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 import csv
 import re
 
 from dataclasses import dataclass
 
 from gbd_core import contexts
-from gbd_core.util import eprint
+from gbd_core.util import eprint, confirm
 
 
 class SchemaException(Exception):
     pass
 
 
 @dataclass
@@ -46,23 +46,25 @@
         self.features = features
         self.context = context
         self.dbcon = dbcon
         self.csv = csv
 
     @classmethod
     def is_database(cls, path):
-        if not os.path.isfile(path): 
-            eprint("Creating Database {}".format(path))
+        if os.path.isfile(path):
+            sz = os.path.getsize(path)
+            if sz == 0: return True  # new sqlite3 files can be empty
+            if sz < 100: return False  # sqlite header is 100 bytes
+            with open(path, 'rb') as fd: header = fd.read(100)  # validate header
+            return (header[:16] == b'SQLite format 3\x00')
+        elif confirm("Database '{}' does not exist. Create new database?".format(path)): 
             sqlite3.connect(path).close()
             return True
-        sz = os.path.getsize(path)
-        if sz == 0: return True  # new sqlite3 files can be empty
-        if sz < 100: return False  # sqlite header is 100 bytes
-        with open(path, 'rb') as fd: header = fd.read(100)  # validate header
-        return (header[:16] == b'SQLite format 3\x00')
+        else:
+            raise SchemaException("Database '{}' does not exist".format(path))
 
     @classmethod
     def create(cls, path):
         try:
             if cls.is_database(path):
                 return cls.from_database(path)
             else:
```

### Comparing `gbd_tools-4.5.9/gbd_core/util.py` & `gbd_tools-4.6.0/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_core/util_argparse.py` & `gbd_tools-4.6.0/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_init/cnf_extractors.py` & `gbd_tools-4.6.0/gbd_init/feature_extractors.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,107 +13,121 @@
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
 
 import pandas as pd
 import os
 import glob
 
-from gbd_core.contexts import suffix_list
+from gbd_core.contexts import suffix_list, identify
 from gbd_core.api import GBD, GBDException
 from gbd_core.util import eprint, confirm
-from gbd_init.initializer import Initializer
-from gbd_init.gbdhash import identify
+from gbd_init.initializer import Initializer, InitializerException
 
-from gbdc import extract_base_features, extract_gate_features, isohash
+try:
+    from gbdc import extract_base_features, extract_gate_features, isohash
+except ImportError:
+    def extract_base_features(path, tlim, mlim):
+        return [ ]
+
+    def extract_gate_features(path, tlim, mlim):
+        return [ ]
+    
+    def isohash(path):
+        return [ ]
 
 
 ## GBDHash
 def compute_hash(hash, path, limits):
     eprint('Hashing {}'.format(path))
     hash = identify(path)
     return [ ("local", hash, path), ("filename", hash, os.path.basename(path)) ]
 
-def init_local(api: GBD, context, rlimits, root, target_db):
-    features = [ ("local", None), ("filename", None) ]
-    extractor = Initializer([ context ], [ context ], api, context, rlimits, target_db, features, compute_hash)
-    extractor.create_features()
-
-    df = api.query(group_by="local")
-    
-    dfilter = df["local"].apply(lambda x: not x or not os.path.isfile(x))
-    missing = df[dfilter]
-    if len(missing) and api.verbose:
-        for path in missing["local"].tolist():
-            eprint(path)
-    if len(missing) and confirm("{} files not found. Remove stale entries from local table?".format(len(missing))):
-        api.reset_values("local", values=missing["local"].tolist())
-
-    paths = [ path for suffix in suffix_list(context) for path in glob.iglob(root + "/**/*" + suffix, recursive=True) ]
-    df2 = pd.DataFrame([(None, path) for path in paths if not path in df["local"].to_list()], columns=["hash", "local"])
-    
-    extractor.run(df2)
-
-
 ## ISOHash
 def compute_isohash(hash, path, limits):
     eprint('Computing ISOHash for {}'.format(path))
     ihash = isohash(path)
     return [ ('isohash', hash, ihash) ]
 
-# Initialize degree_sequence_hash for given instances
-def init_isohash(api: GBD, context, rlimits, query, hashes, target_db):
-    contexts = [ 'cnf', 'sancnf' ]
-    features = [ ('isohash', 'empty') ]
-    extractor = Initializer(contexts, contexts, api, context, rlimits, target_db, features, compute_isohash)
-    extractor.create_features()
-    df = api.query(query, hashes, ["local"], collapse="MIN")
-    extractor.run(df)
-
-
 ## Base Features
 def compute_base_features(hash, path, limits):
     eprint('Extracting base features from {} {}'.format(hash, path))
     rec = extract_base_features(path, limits['tlim'], limits['mlim'])
     return [ (key, hash, int(value) if isinstance(value, float) and value.is_integer() else value) for key, value in rec.items() ]
 
-def init_base_features(api: GBD, context, rlimits, query, hashes, target_db):
-    contexts = [ 'cnf', 'sancnf' ]
-    features = [ ("base_features_runtime", "empty"), ("clauses", "empty"), ("variables", "empty"), ("clause_size_1", "empty"), ("clause_size_2", "empty"), ("clause_size_3", "empty"), 
-        ("clause_size_4", "empty"), ("clause_size_5", "empty"), ("clause_size_6", "empty"), ("clause_size_7", "empty"), ("clause_size_8", "empty"), ("clause_size_9", "empty"), 
-        ("horn_clauses", "empty"), ("inv_horn_clauses", "empty"), ("positive_clauses", "empty"), ("negative_clauses", "empty"),
-        ("horn_vars_mean", "empty"), ("horn_vars_variance", "empty"), ("horn_vars_min", "empty"), ("horn_vars_max", "empty"), ("horn_vars_entropy", "empty"),
-        ("inv_horn_vars_mean", "empty"), ("inv_horn_vars_variance", "empty"), ("inv_horn_vars_min", "empty"), ("inv_horn_vars_max", "empty"), ("inv_horn_vars_entropy", "empty"),
-        ("vg_degrees_mean", "empty"), ("vg_degrees_variance", "empty"), ("vg_degrees_min", "empty"), ("vg_degrees_max", "empty"), ("vg_degrees_entropy", "empty"),
-        ("balance_clause_mean", "empty"), ("balance_clause_variance", "empty"), ("balance_clause_min", "empty"), ("balance_clause_max", "empty"), ("balance_clause_entropy", "empty"),
-        ("balance_vars_mean", "empty"), ("balance_vars_variance", "empty"), ("balance_vars_min", "empty"), ("balance_vars_max", "empty"), ("balance_vars_entropy", "empty"),
-        ("vcg_vdegrees_mean", "empty"), ("vcg_vdegrees_variance", "empty"), ("vcg_vdegrees_min", "empty"), ("vcg_vdegrees_max", "empty"), ("vcg_vdegrees_entropy", "empty"),
-        ("vcg_cdegrees_mean", "empty"), ("vcg_cdegrees_variance", "empty"), ("vcg_cdegrees_min", "empty"), ("vcg_cdegrees_max", "empty"), ("vcg_cdegrees_entropy", "empty"),
-        ("cg_degrees_mean", "empty"), ("cg_degrees_variance", "empty"), ("cg_degrees_min", "empty"), ("cg_degrees_max", "empty"), ("cg_degrees_entropy", "empty") ]
-    extractor = Initializer(contexts, contexts, api, context, rlimits, target_db, features, compute_base_features)
-    extractor.create_features()
-    df = api.query(query, hashes, ["local"], collapse="MIN")
-    extractor.run(df)
-
-
 ## Gate Features
 def compute_gate_features(hash, path, limits):
     eprint('Extracting gate features from {} {}'.format(hash, path))
     rec = extract_gate_features(path, limits['tlim'], limits['mlim'])
-    return [ (key, hash, int(value) if isinstance(value, float) and value.is_integer() else value) for key, value in rec.items() ]
+    return [ (key, hash, int(value) if isinstance(value, float) and value.is_integer() else value) for key, value in rec.items() ]   
+
+
+generic_extractors = {
+    "base" : {
+        "contexts" : [ "cnf" ],
+        "features" : [ ("base_features_runtime", "empty"), ("clauses", "empty"), ("variables", "empty"), ("clause_size_1", "empty"), ("clause_size_2", "empty"), ("clause_size_3", "empty"), 
+            ("clause_size_4", "empty"), ("clause_size_5", "empty"), ("clause_size_6", "empty"), ("clause_size_7", "empty"), ("clause_size_8", "empty"), ("clause_size_9", "empty"), 
+            ("horn_clauses", "empty"), ("inv_horn_clauses", "empty"), ("positive_clauses", "empty"), ("negative_clauses", "empty"),
+            ("horn_vars_mean", "empty"), ("horn_vars_variance", "empty"), ("horn_vars_min", "empty"), ("horn_vars_max", "empty"), ("horn_vars_entropy", "empty"),
+            ("inv_horn_vars_mean", "empty"), ("inv_horn_vars_variance", "empty"), ("inv_horn_vars_min", "empty"), ("inv_horn_vars_max", "empty"), ("inv_horn_vars_entropy", "empty"),
+            ("vg_degrees_mean", "empty"), ("vg_degrees_variance", "empty"), ("vg_degrees_min", "empty"), ("vg_degrees_max", "empty"), ("vg_degrees_entropy", "empty"),
+            ("balance_clause_mean", "empty"), ("balance_clause_variance", "empty"), ("balance_clause_min", "empty"), ("balance_clause_max", "empty"), ("balance_clause_entropy", "empty"),
+            ("balance_vars_mean", "empty"), ("balance_vars_variance", "empty"), ("balance_vars_min", "empty"), ("balance_vars_max", "empty"), ("balance_vars_entropy", "empty"),
+            ("vcg_vdegrees_mean", "empty"), ("vcg_vdegrees_variance", "empty"), ("vcg_vdegrees_min", "empty"), ("vcg_vdegrees_max", "empty"), ("vcg_vdegrees_entropy", "empty"),
+            ("vcg_cdegrees_mean", "empty"), ("vcg_cdegrees_variance", "empty"), ("vcg_cdegrees_min", "empty"), ("vcg_cdegrees_max", "empty"), ("vcg_cdegrees_entropy", "empty"),
+            ("cg_degrees_mean", "empty"), ("cg_degrees_variance", "empty"), ("cg_degrees_min", "empty"), ("cg_degrees_max", "empty"), ("cg_degrees_entropy", "empty") ],
+        "compute" : compute_base_features,
+    },
+    "gate" : {
+        "contexts" : [ "cnf" ],
+        "features" : [ ("gate_features_runtime", "empty"), ("n_vars", "empty"), ("n_gates", "empty"), ("n_roots", "empty"),
+            ("n_none", "empty"), ("n_generic", "empty"), ("n_mono", "empty"), ("n_and", "empty"), ("n_or", "empty"), ("n_triv", "empty"), ("n_equiv", "empty"), ("n_full", "empty"),
+            ("levels_mean", "empty"), ("levels_variance", "empty"), ("levels_min", "empty"), ("levels_max", "empty"), ("levels_entropy", "empty"),
+            ("levels_none_mean", "empty"), ("levels_none_variance", "empty"), ("levels_none_min", "empty"), ("levels_none_max", "empty"), ("levels_none_entropy", "empty"),
+            ("levels_generic_mean", "empty"), ("levels_generic_variance", "empty"), ("levels_generic_min", "empty"), ("levels_generic_max", "empty"), ("levels_generic_entropy", "empty"),
+            ("levels_mono_mean", "empty"), ("levels_mono_variance", "empty"), ("levels_mono_min", "empty"), ("levels_mono_max", "empty"), ("levels_mono_entropy", "empty"),
+            ("levels_and_mean", "empty"), ("levels_and_variance", "empty"), ("levels_and_min", "empty"), ("levels_and_max", "empty"), ("levels_and_entropy", "empty"),
+            ("levels_or_mean", "empty"), ("levels_or_variance", "empty"), ("levels_or_min", "empty"), ("levels_or_max", "empty"), ("levels_or_entropy", "empty"),
+            ("levels_triv_mean", "empty"), ("levels_triv_variance", "empty"), ("levels_triv_min", "empty"), ("levels_triv_max", "empty"), ("levels_triv_entropy", "empty"),
+            ("levels_equiv_mean", "empty"), ("levels_equiv_variance", "empty"), ("levels_equiv_min", "empty"), ("levels_equiv_max", "empty"), ("levels_equiv_entropy", "empty"),
+            ("levels_full_mean", "empty"), ("levels_full_variance", "empty"), ("levels_full_min", "empty"), ("levels_full_max", "empty"), ("levels_full_entropy", "empty") ],
+        "compute" : compute_gate_features,
+    },
+    "isohash" : {
+        "contexts" : [ "cnf" ],
+        "features" : [ ("isohash", "empty") ],
+        "compute" : compute_isohash,
+    },
+}
+
+
+def init_features_generic(key: str, api: GBD, rlimits, df, target_db):
+    einfo = generic_extractors[key]
+    context = api.database.dcontext(target_db)
+    if not context in einfo["contexts"]:
+        raise InitializerException("Target database context must be in {}".format(einfo["contexts"]))
+    extractor = Initializer(api, rlimits, target_db, einfo["features"], einfo["compute"])
+    extractor.create_features()
+    extractor.run(df)
+
 
-def init_gate_features(api: GBD, context, rlimits, query, hashes, target_db):
-    contexts = [ 'cnf', 'sancnf' ]
-    features = [ ("gate_features_runtime", "empty"), ("n_vars", "empty"), ("n_gates", "empty"), ("n_roots", "empty"),
-        ("n_none", "empty"), ("n_generic", "empty"), ("n_mono", "empty"), ("n_and", "empty"), ("n_or", "empty"), ("n_triv", "empty"), ("n_equiv", "empty"), ("n_full", "empty"),
-        ("levels_mean", "empty"), ("levels_variance", "empty"), ("levels_min", "empty"), ("levels_max", "empty"), ("levels_entropy", "empty"),
-        ("levels_none_mean", "empty"), ("levels_none_variance", "empty"), ("levels_none_min", "empty"), ("levels_none_max", "empty"), ("levels_none_entropy", "empty"),
-        ("levels_generic_mean", "empty"), ("levels_generic_variance", "empty"), ("levels_generic_min", "empty"), ("levels_generic_max", "empty"), ("levels_generic_entropy", "empty"),
-        ("levels_mono_mean", "empty"), ("levels_mono_variance", "empty"), ("levels_mono_min", "empty"), ("levels_mono_max", "empty"), ("levels_mono_entropy", "empty"),
-        ("levels_and_mean", "empty"), ("levels_and_variance", "empty"), ("levels_and_min", "empty"), ("levels_and_max", "empty"), ("levels_and_entropy", "empty"),
-        ("levels_or_mean", "empty"), ("levels_or_variance", "empty"), ("levels_or_min", "empty"), ("levels_or_max", "empty"), ("levels_or_entropy", "empty"),
-        ("levels_triv_mean", "empty"), ("levels_triv_variance", "empty"), ("levels_triv_min", "empty"), ("levels_triv_max", "empty"), ("levels_triv_entropy", "empty"),
-        ("levels_equiv_mean", "empty"), ("levels_equiv_variance", "empty"), ("levels_equiv_min", "empty"), ("levels_equiv_max", "empty"), ("levels_equiv_entropy", "empty"),
-        ("levels_full_mean", "empty"), ("levels_full_variance", "empty"), ("levels_full_min", "empty"), ("levels_full_max", "empty"), ("levels_full_entropy", "empty") ]
-    extractor = Initializer(contexts, contexts, api, context, rlimits, target_db, features, compute_gate_features)
+def init_local(api: GBD, rlimits, root, target_db):
+    context = api.database.dcontext(target_db)
+    
+    features = [ ("local", None), ("filename", None) ]
+    extractor = Initializer(api, rlimits, target_db, features, compute_hash)
     extractor.create_features()
-    df = api.query(query, hashes, ["local"], collapse="MIN")
-    extractor.run(df)
+
+    # Cleanup stale entries
+    df = api.query(group_by=context + ":local")
+    dfilter = df["local"].apply(lambda x: not x or not os.path.isfile(x))
+    missing = df[dfilter]
+    if len(missing) and api.verbose:
+        for path in missing["local"].tolist():
+            eprint(path)
+    if len(missing) and confirm("{} files not found. Remove stale entries from local table?".format(len(missing))):
+        api.reset_values("local", values=missing["local"].tolist())
+
+    # Create df with paths not yet in local table
+    paths = [ path for suffix in suffix_list(context) for path in glob.iglob(root + "/**/*" + suffix, recursive=True) ]
+    df2 = pd.DataFrame([(None, path) for path in paths if not path in df["local"].to_list()], columns=["hash", "local"])
+    
+    extractor.run(df2)
```

### Comparing `gbd_tools-4.5.9/gbd_init/cnf_transformers.py` & `gbd_tools-4.6.0/gbd_init/benchmark_transformers.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import os
 from functools import reduce
 
 from gbd_core import contexts
 from gbd_core.api import GBD, GBDException
 from gbd_core import util
 
-from gbd_init.gbdhash import identify
-from gbd_init.initializer import Initializer
+from gbd_core.contexts import identify
+from gbd_init.initializer import Initializer, InitializerException
 
 import gbdc
 
 
 # Transform SAT Problem to k-Independent Set Problem
 def kis_filename(path):
     kispath = reduce(lambda path, suffix: path[:-len(suffix)] if path.endswith(suffix) else path, contexts.suffix_list('cnf'), path)
@@ -46,22 +46,24 @@
     except Exception as e:
         util.eprint(str(e))
         if os.path.exists(kispath):
             os.remove(kispath)
 
     return [ ]
 
-def init_transform_cnf_to_kis(api: GBD, context, rlimits, query, hashes, target_db=None):
-    source_contexts = [ 'cnf', 'sancnf' ]
-    target_contexts = [ 'kis' ]
+def init_transform_cnf_to_kis(api: GBD, rlimits, query, hashes, target_db, source):
+    if source != 'cnf':
+        raise InitializerException("Source database must be in context 'cnf'")
+    if api.database.dcontext(target_db) != 'kis':
+        raise InitializerException("Target database must be in context 'kis'")
     features = [ ('local', None), ('to_cnf', None), ('nodes', 'empty'), ('edges', 'empty'), ('k', 'empty') ]
-    transformer = Initializer(source_contexts, target_contexts, api, context, rlimits, target_db, features, cnf2kis)
+    transformer = Initializer(api, rlimits, target_db, features, cnf2kis)
     transformer.create_features()
 
-    df = api.query(query, hashes, ["local"], collapse=None)
+    df = api.query(query, hashes, [source+":local"], collapse=None)
     dfilter = df['local'].apply(lambda x: x and not os.path.isfile(kis_filename(x)))
 
     transformer.run(df[dfilter])
 
 
 # Sanitize CNF
 def sanitized_filename(path):
@@ -81,19 +83,21 @@
                 raise GBDException("Sanitization failed for {}".format(path))
     except Exception as e:
         util.eprint(str(e))
         os.remove(sanname)
 
     return [ ]
 
-def init_sani(api: GBD, context, rlimits, query, hashes, target_db=None):
-    source_contexts = [ 'cnf', 'sancnf' ]
-    target_contexts = [ 'sancnf' ]
+def init_sani(api: GBD, rlimits, query, hashes, target_db, source):
+    if source != 'cnf':
+        raise InitializerException("Source database must be in context 'cnf'")
+    if api.database.dcontext(target_db) != 'sancnf':
+        raise InitializerException("Target database must be in context 'sancnf'")
     features = [ ('local', None) , ('to_cnf', None) ]
-    transformer = Initializer(source_contexts, target_contexts, api, context, rlimits, target_db, features, sanitize_cnf)
+    transformer = Initializer(api, rlimits, target_db, features, sanitize_cnf)
     transformer.create_features()
 
-    df = api.query(query, hashes, ["local"], collapse=None)
+    df = api.query(query, hashes, [source+":local"], collapse=None)
     dfilter = df['local'].apply(lambda x: x and not os.path.isfile(sanitized_filename(x)))
 
     transformer.run(df[dfilter])
```

### Comparing `gbd_tools-4.5.9/gbd_init/gbdhash.py` & `gbd_tools-4.6.0/gbd_init/gbdhash.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,29 +16,34 @@
 import io
 import hashlib
 
 import gzip
 import bz2
 import lzma
 
-from gbd_core.contexts import get_context_by_suffix
-
 
 def open_file(filename, mode):
     if filename.endswith('.gz'):
         return gzip.open(filename, mode)
     elif filename.endswith('.bz2'):
         return bz2.open(filename, mode)
     elif filename.endswith('.lzma') or filename.endswith('.xz'):
         return lzma.open(filename, mode)
     else:
         return open(filename, mode)
 
 
 try:
+    from gbdc import opbhash as opb_hash
+except ImportError:
+    def opb_hash(filename):
+        raise Exception("Unable to import opbhash. Please install or update gbdc: https://github.com/Udopia/gbdc")
+    
+
+try:
     from gbdc import gbdhash as cnf_hash
 except ImportError:
     try:
         from gbdhashc import gbdhash as cnf_hash
     except ImportError:
         def cnf_hash(filename):
             file = open_file(filename, 'rb')
@@ -65,26 +70,8 @@
                     skip = True  # do not hash comment and header line
 
             if not cldelim:
                 hash_md5.update(b' 0')
 
             file.close()
 
-            return hash_md5.hexdigest()
-
-
-try:
-    from gbdc import opbhash as opb_hash
-except ImportError:
-    raise Exception("Unable to import opbhash. Please install or update gbdc.")
-    
-
-def identify(path, ct=None):
-    context = ct or get_context_by_suffix(path)
-    if context is None:
-        raise Exception("Unable to associate context: " + path)
-    elif context in ['cnf', 'sancnf', 'kis', 'wecnf']:
-        return cnf_hash(path)
-    elif context in ['opb']:
-        return opb_hash(path)
-    else:
-        raise Exception("Unable to identify: " + path)
+            return hash_md5.hexdigest()
```

### Comparing `gbd_tools-4.5.9/gbd_init/initializer.py` & `gbd_tools-4.6.0/gbd_init/initializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,28 +17,26 @@
 import pebble
 from concurrent.futures import as_completed
 import pandas as pd
 
 from gbd_core.api import GBD, GBDException
 from gbd_core import util
 
+class InitializerException(Exception):
+    pass
 
 class Initializer:
 
-    def __init__(self, source_contexts: list, target_contexts: list, api: GBD, context: str, rlimits: dict, target_db: str, features: list, initfunc):
+    def __init__(self, api: GBD, rlimits: dict, target_db: str, features: list, initfunc):
         self.api = api
         self.api.database.set_auto_commit(False)
         self.target_db = target_db
         self.features = features
         self.initfunc = initfunc
         self.rlimits = rlimits
-        if not context in source_contexts:
-            raise GBDException("Context '{}' not supported by '{}'".format(context, self.__class__.__name__))
-        if not api.database.dcontext(target_db) in target_contexts:
-            raise GBDException("Target database '{}' has incompatible context '{}'. Database context can be specified by filename prefix.".format(target_db, api.database.dcontext(target_db)))
 
 
     def create_features(self):
         for (name, default) in self.features:
             self.api.database.create_feature(name, default, self.target_db, True)
         self.api.database.commit()
```

### Comparing `gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.6.0/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.6.0/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_server/static/main.css` & `gbd_tools-4.6.0/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_server/static/w3.js` & `gbd_tools-4.6.0/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_server/templates/index.html` & `gbd_tools-4.6.0/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.6.0/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.5.9
+Version: 4.6.0
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.9/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.6.0/gbd_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 gbd_core/database.py
 gbd_core/grammar.py
 gbd_core/query.py
 gbd_core/schema.py
 gbd_core/util.py
 gbd_core/util_argparse.py
 gbd_init/__init__.py
-gbd_init/cnf_extractors.py
-gbd_init/cnf_transformers.py
+gbd_init/benchmark_transformers.py
+gbd_init/feature_extractors.py
 gbd_init/gbdhash.py
 gbd_init/initializer.py
 gbd_server/__init__.py
 gbd_server/static/main.css
 gbd_server/static/w3.js
 gbd_server/static/img/gbd_logo.jpg
 gbd_server/static/img/gbd_logo.png
```

### Comparing `gbd_tools-4.5.9/server.py` & `gbd_tools-4.6.0/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.9/setup.py` & `gbd_tools-4.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.5.9',
+  version='4.6.0',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

