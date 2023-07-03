# Comparing `tmp/gbd_tools-4.6.2.tar.gz` & `tmp/gbd_tools-4.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.6.2.tar", last modified: Mon Jul  3 12:30:21 2023, max compression
+gzip compressed data, was "gbd_tools-4.6.3.tar", last modified: Mon Jul  3 13:26:49 2023, max compression
```

## Comparing `gbd_tools-4.6.2.tar` & `gbd_tools-4.6.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.6.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/README.md
--rwxrwxr-x   0 root         (0) root         (0)    12309 2023-07-03 12:27:26.000000 gbd_tools-4.6.2/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.6.2/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10487 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     2395 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    12310 2023-07-03 12:25:07.000000 gbd_tools-4.6.2/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     6526 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5356 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12510 2023-07-03 12:24:04.000000 gbd_tools-4.6.2/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.6.2/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4113 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_init/benchmark_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     8685 2023-07-03 10:15:03.000000 gbd_tools-4.6.2/gbd_init/feature_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     2574 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3088 2023-07-03 07:45:22.000000 gbd_tools-4.6.2/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.633421 gbd_tools-4.6.2/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.6.2/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.6.2/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 12:30:21.000000 gbd_tools-4.6.2/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11998 2023-05-19 07:01:54.000000 gbd_tools-4.6.2/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:30:21.637421 gbd_tools-4.6.2/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-07-03 12:25:39.000000 gbd_tools-4.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.6.3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-05-19 07:01:54.000000 gbd_tools-4.6.3/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    12319 2023-07-03 13:08:19.000000 gbd_tools-4.6.3/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.6.3/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10579 2023-07-03 13:16:45.000000 gbd_tools-4.6.3/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     2395 2023-07-03 07:45:22.000000 gbd_tools-4.6.3/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    12310 2023-07-03 12:25:07.000000 gbd_tools-4.6.3/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     6526 2023-07-03 07:45:22.000000 gbd_tools-4.6.3/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5657 2023-07-03 13:16:24.000000 gbd_tools-4.6.3/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12510 2023-07-03 12:24:04.000000 gbd_tools-4.6.3/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-05-19 07:01:54.000000 gbd_tools-4.6.3/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-19 07:01:54.000000 gbd_tools-4.6.3/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.6.3/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4113 2023-07-03 07:45:22.000000 gbd_tools-4.6.3/gbd_init/benchmark_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     8685 2023-07-03 10:15:03.000000 gbd_tools-4.6.3/gbd_init/feature_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     2574 2023-07-03 07:45:22.000000 gbd_tools-4.6.3/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3088 2023-07-03 07:45:22.000000 gbd_tools-4.6.3/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.6.3/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.6.3/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.6.3/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.6.3/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-05-19 07:01:54.000000 gbd_tools-4.6.3/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.6.3/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-05-19 07:01:54.000000 gbd_tools-4.6.3/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:26:49.949233 gbd_tools-4.6.3/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-07-03 13:26:49.000000 gbd_tools-4.6.3/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-03 13:26:49.000000 gbd_tools-4.6.3/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 13:26:49.000000 gbd_tools-4.6.3/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-03 13:26:49.000000 gbd_tools-4.6.3/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-03 13:26:49.000000 gbd_tools-4.6.3/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 13:26:49.000000 gbd_tools-4.6.3/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11998 2023-05-19 07:01:54.000000 gbd_tools-4.6.3/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 13:26:49.953233 gbd_tools-4.6.3/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-07-03 13:18:08.000000 gbd_tools-4.6.3/setup.py
```

### Comparing `gbd_tools-4.6.2/LICENSE` & `gbd_tools-4.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/PKG-INFO` & `gbd_tools-4.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.6.2
+Version: 4.6.3
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.6.2/README.md` & `gbd_tools-4.6.3/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd.py` & `gbd_tools-4.6.3/gbd.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,19 +154,19 @@
     parser_hash = subparsers.add_parser('hash', help='Print hash for a single file')
     parser_hash.add_argument('path', type=file_type, help="Path to one benchmark")
     parser_hash.set_defaults(func=cli_hash)
 
     # GBD GET $QUERY
     parser_get = subparsers.add_parser('get', help='Get data by query (or hash-list via stdin)')
     add_query_and_hashes_arguments(parser_get)
-    parser_get.add_argument('-r', '--resolve', help='List of features to resolve against', nargs='+')
+    parser_get.add_argument('-r', '--resolve', help='List of features to resolve against', nargs='+', default=[])
     parser_get.add_argument('-c', '--collapse', default='group_concat', 
                             choices=['group_concat', 'min', 'max', 'avg', 'count', 'sum', 'none'], 
                             help='Treatment of multiple values per hash (or grouping value resp.)')
-    parser_get.add_argument('-g', '--group_by', default='hash', help='Group by specified attribute value')
+    parser_get.add_argument('-g', '--group_by', default=None, help='Group by specified attribute value')
     parser_get.add_argument('--join-type', help='Join Type: treatment of missing values in queries', choices=['INNER', 'OUTER', 'LEFT'], default="LEFT")
     parser_get.set_defaults(func=cli_get)
 
     # GBD SET
     parser_set = subparsers.add_parser('set', help='Set specified attribute-value for query result')
     parser_set.add_argument('assign', type=key_value_type, help='key=value')
     parser_set.add_argument('-c', '--create', help='Create given hashes if they do not exist yet (otherwise intersect with existing hashes)', action='store_true')
```

### Comparing `gbd_tools-4.6.2/gbd_core/api.py` & `gbd_tools-4.6.3/gbd_core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,29 +57,31 @@
             Returns:
                 str: GBD hash
         """
         from gbd_core.contexts import identify
         return identify(path)
 
 
-    def query(self, gbd_query=None, hashes=[], resolve=[], collapse="group_concat", group_by="hash", join_type="LEFT"):
+    def query(self, gbd_query=None, hashes=[], resolve=[], collapse="group_concat", group_by=None, join_type="LEFT"):
         query_builder = GBDQuery(self.database, gbd_query)
         try:
-            sql = query_builder.build_query(hashes, resolve or [], group_by or "hash", join_type, collapse)
+            sql = query_builder.build_query(hashes, resolve, group_by, join_type, collapse)
         except tatsu.exceptions.FailedParse as err:
             if self.verbose:
                 util.eprint(traceback.format_exc())
             raise GBDException("Parser Error with Query '{}': {}".format(gbd_query, str(err)))
         try:
             result = self.database.query(sql)
         except sqlite3.OperationalError as err:
             if self.verbose:
                 util.eprint(traceback.format_exc())
             raise GBDException("Database Operational Error: {}".format(str(err)))
-        cols = [ p.split(':') for p in [ group_by ] + (resolve or []) ]
+        f = "hash" if not len(resolve) else resolve[0]
+        group = query_builder.determine_group_by(resolve)
+        cols = [ p.split(':') for p in [ group ] + (resolve or []) ]
         cols = [ c[0] if len(c) == 1 else c[1] for c in cols ]
         return pd.DataFrame(result, columns=cols)
 
 
     def set_values(self, name, value, hashes, target_db=None):
         """ Set feature value for given hashes
```

### Comparing `gbd_tools-4.6.2/gbd_core/contexts.py` & `gbd_tools-4.6.3/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_core/database.py` & `gbd_tools-4.6.3/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_core/grammar.py` & `gbd_tools-4.6.3/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_core/query.py` & `gbd_tools-4.6.3/gbd_core/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,37 @@
 
     def features_exist_or_throw(self, features):
         for feature in features:
             self.db.find(feature)
 
 
     # Generate SQL Query from given GBD Query 
-    def build_query(self, hashes=[], resolve=[], group_by="hash", join_type="LEFT", collapse=None):
-        self.features_exist_or_throw(resolve + [group_by] + list(self.features))
+    def build_query(self, hashes=[], resolve=[], group_by=None, join_type="LEFT", collapse=None):
+        group = group_by or self.determine_group_by(resolve)
 
-        sql_select = self.build_select(group_by, resolve, collapse)
+        self.features_exist_or_throw(resolve + [group] + list(self.features))
 
-        sql_from = self.build_from(group_by, set(resolve) | self.features, join_type)
+        sql_select = self.build_select(group, resolve, collapse)
+
+        sql_from = self.build_from(group, set(resolve) | self.features, join_type)
         
-        sql_where = self.build_where(hashes, group_by)
+        sql_where = self.build_where(hashes, group)
 
-        sql_groupby = "GROUP BY {}".format(self.db.faddr(group_by)) if collapse else ""
-        sql_orderby = "ORDER BY {}".format(self.db.faddr(group_by))
+        sql_groupby = "GROUP BY {}".format(self.db.faddr(group)) if collapse else ""
+        sql_orderby = "ORDER BY {}".format(self.db.faddr(group))
         
         return "{} {} WHERE {} {} {}".format(sql_select, sql_from, sql_where, sql_groupby, sql_orderby)
+    
 
+    def determine_group_by(self, resolve):
+        if len(resolve) == 0:
+            return self.db.dcontext(self.db.find("hash").database) + ":hash"
+        else:
+            return self.db.dcontext(self.db.find(resolve[0]).database) + ":hash"
+        
 
     def build_select(self, group_by, resolve, collapse=None):
         result = [ self.db.faddr(f) for f in [group_by] + resolve ]
         if collapse and collapse != "none":
             result = [ "{}(DISTINCT {})".format(collapse, r) for r in result ]
         return "SELECT DISTINCT " + ", ".join(result)
```

### Comparing `gbd_tools-4.6.2/gbd_core/schema.py` & `gbd_tools-4.6.3/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_core/util.py` & `gbd_tools-4.6.3/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_core/util_argparse.py` & `gbd_tools-4.6.3/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_init/benchmark_transformers.py` & `gbd_tools-4.6.3/gbd_init/benchmark_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_init/feature_extractors.py` & `gbd_tools-4.6.3/gbd_init/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_init/gbdhash.py` & `gbd_tools-4.6.3/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_init/initializer.py` & `gbd_tools-4.6.3/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.6.3/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.6.3/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.6.3/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_server/static/main.css` & `gbd_tools-4.6.3/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_server/static/w3.js` & `gbd_tools-4.6.3/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_server/templates/index.html` & `gbd_tools-4.6.3/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.6.3/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.6.2
+Version: 4.6.3
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.6.2/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.6.3/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/server.py` & `gbd_tools-4.6.3/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.6.2/setup.py` & `gbd_tools-4.6.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.6.2',
+  version='4.6.3',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

