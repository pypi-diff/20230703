# Comparing `tmp/gazouilloire-1.4.0.tar.gz` & `tmp/gazouilloire-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gazouilloire-1.4.0.tar", last modified: Thu Dec  8 09:28:13 2022, max compression
+gzip compressed data, was "gazouilloire-1.5.0.tar", last modified: Mon Jul  3 11:36:23 2023, max compression
```

## Comparing `gazouilloire-1.4.0.tar` & `gazouilloire-1.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.379700 gazouilloire-1.4.0/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    35150 2020-09-02 16:04:35.000000 gazouilloire-1.4.0/LICENSE
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      151 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/MANIFEST.in
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    26349 2022-12-08 09:28:13.379700 gazouilloire-1.4.0/PKG-INFO
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    26030 2022-12-07 17:34:43.000000 gazouilloire-1.4.0/README.md
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.371700 gazouilloire-1.4.0/gazouilloire/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2020-09-29 12:30:22.000000 gazouilloire-1.4.0/gazouilloire/__init__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       22 2022-12-08 09:26:07.000000 gazouilloire-1.4.0/gazouilloire/__version__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     2365 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/api_wrapper.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.375700 gazouilloire-1.4.0/gazouilloire/cli/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/cli/__init__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    27704 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/cli/__main__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      937 2022-11-02 16:01:16.000000 gazouilloire-1.4.0/gazouilloire/config.json.example
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5952 2022-12-07 17:30:12.000000 gazouilloire-1.4.0/gazouilloire/config_format.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     4867 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/daemon.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.375700 gazouilloire-1.4.0/gazouilloire/database/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/database/__init__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5902 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/database/db_mappings.json
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    22547 2022-08-16 09:57:32.000000 gazouilloire-1.4.0/gazouilloire/database/elasticmanager.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.375700 gazouilloire-1.4.0/gazouilloire/exports/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/exports/__init__.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    15670 2022-11-02 16:05:54.000000 gazouilloire-1.4.0/gazouilloire/exports/export_csv.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     5949 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/exports/tweet_fields.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1825 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/manage_scripts.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     2796 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/multiprocessing.py
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     1064 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/resolving_script.py
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)    39527 2022-12-07 17:25:12.000000 gazouilloire-1.4.0/gazouilloire/run.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.375700 gazouilloire-1.4.0/gazouilloire/scripts/
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     1199 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/scripts/add_bearer_token_to_conf.sh
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     2347 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/scripts/backup_corpus_ids.sh
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     2668 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/scripts/daily_mail_export.sh
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     3283 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/scripts/elasticdump.sh
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     1885 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/scripts/monthly_archive.sh
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     3483 2022-09-05 12:22:54.000000 gazouilloire-1.4.0/gazouilloire/scripts/restart.sh
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     1526 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/test_metas.py
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     1257 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/test_search.py
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     1443 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/test_stream.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1271 2022-12-07 12:55:34.000000 gazouilloire-1.4.0/gazouilloire/twitter_connexion.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     6928 2022-11-02 16:01:16.000000 gazouilloire-1.4.0/gazouilloire/url_resolve.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.375700 gazouilloire-1.4.0/gazouilloire/web/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        0 2020-09-02 16:04:35.000000 gazouilloire-1.4.0/gazouilloire/web/__init__.py
--rwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)     3992 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/web/app.py
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    15886 2022-07-28 15:17:56.000000 gazouilloire-1.4.0/gazouilloire/web/export.py
-drwxrwxr-x   0 bmazoyer  (1000) bmazoyer  (1000)        0 2022-12-08 09:28:13.375700 gazouilloire-1.4.0/gazouilloire.egg-info/
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)    26349 2022-12-08 09:28:13.000000 gazouilloire-1.4.0/gazouilloire.egg-info/PKG-INFO
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1281 2022-12-08 09:28:13.000000 gazouilloire-1.4.0/gazouilloire.egg-info/SOURCES.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)        1 2022-12-08 09:28:13.000000 gazouilloire-1.4.0/gazouilloire.egg-info/dependency_links.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)      103 2022-12-08 09:28:13.000000 gazouilloire-1.4.0/gazouilloire.egg-info/entry_points.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       75 2022-12-08 09:28:13.000000 gazouilloire-1.4.0/gazouilloire.egg-info/requires.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       13 2022-12-08 09:28:13.000000 gazouilloire-1.4.0/gazouilloire.egg-info/top_level.txt
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)       38 2022-12-08 09:28:13.379700 gazouilloire-1.4.0/setup.cfg
--rw-rw-r--   0 bmazoyer  (1000) bmazoyer  (1000)     1327 2022-11-02 16:01:16.000000 gazouilloire-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.934278 gazouilloire-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35150 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    26349 2023-07-03 11:36:23.934278 gazouilloire-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    26030 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.930278 gazouilloire-1.5.0/gazouilloire/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/api_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.930278 gazouilloire-1.5.0/gazouilloire/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27966 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/config.json.example
+-rw-r--r--   0 runner    (1001) docker     (122)     6050 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/config_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4867 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.930278 gazouilloire-1.5.0/gazouilloire/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/database/db_mappings.json
+-rw-r--r--   0 runner    (1001) docker     (122)    22547 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/database/elasticmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.930278 gazouilloire-1.5.0/gazouilloire/exports/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16206 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/exports/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/exports/tweet_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/manage_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2796 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/multiprocessing.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1064 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/resolving_script.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    39527 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.930278 gazouilloire-1.5.0/gazouilloire/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1199 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/scripts/add_bearer_token_to_conf.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2347 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/scripts/backup_corpus_ids.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2668 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/scripts/daily_mail_export.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3283 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/scripts/elasticdump.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1945 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/scripts/monthly_archive.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/scripts/restart.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1526 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/test_metas.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1257 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/test_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1443 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/twitter_connexion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6928 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/url_resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.934278 gazouilloire-1.5.0/gazouilloire/web/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/web/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3992 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/web/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15886 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/gazouilloire/web/export.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 11:36:23.930278 gazouilloire-1.5.0/gazouilloire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    26349 2023-07-03 11:36:23.000000 gazouilloire-1.5.0/gazouilloire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-03 11:36:23.000000 gazouilloire-1.5.0/gazouilloire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 11:36:23.000000 gazouilloire-1.5.0/gazouilloire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-03 11:36:23.000000 gazouilloire-1.5.0/gazouilloire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-03 11:36:23.000000 gazouilloire-1.5.0/gazouilloire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-03 11:36:23.000000 gazouilloire-1.5.0/gazouilloire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 11:36:23.934278 gazouilloire-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-07-03 11:36:13.000000 gazouilloire-1.5.0/setup.py
```

### Comparing `gazouilloire-1.4.0/LICENSE` & `gazouilloire-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/PKG-INFO` & `gazouilloire-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gazouilloire
-Version: 1.4.0
+Version: 1.5.0
 Summary: Twitter stream & search API grabber
 Home-page: http://github.com/medialab/gazouilloire
 Author: Benjamin Ooghe-Tabanou
 Author-email: 
 License: GPL-3.0
 Keywords: twitter
 Requires-Python: >=3.7
```

### Comparing `gazouilloire-1.4.0/README.md` & `gazouilloire-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/api_wrapper.py` & `gazouilloire-1.5.0/gazouilloire/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/cli/__main__.py` & `gazouilloire-1.5.0/gazouilloire/cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import click
 import os
 from gazouilloire.__version__ import __version__
 from gazouilloire.run import STOP_TIMEOUT, find_running_processes, get_pids, stop as main_stop
 from gazouilloire.config_format import create_conf_example, load_conf, log
 from gazouilloire.daemon import Daemon
 from gazouilloire.resolving_script import resolve_script
-from gazouilloire.exports.export_csv import export_csv, count_by_step, call_database
+from gazouilloire.exports.export import export_from_db, count_by_step, call_database
 from gazouilloire.database.elasticmanager import ElasticManager, INDEX_QUERIES
 from gazouilloire.manage_scripts import list_scripts, spawn_script, get_script_infos
 from elasticsearch import exceptions
 from twitwi.constants import TWEET_FIELDS
 import shutil
 import sys
 
@@ -288,47 +288,53 @@
 @click.option("--list-fields", is_flag=True, help="Print the full list of available fields to export then quit.")
 @click.option("--resume", "-r", is_flag=True, help="Restart the export from the last id specified in --output file")
 @click.option("--lucene", is_flag=True, help="""Use lucene query syntax.
                 Usage: 'gazou export --lucene "user_location:('Sao Paulo' OR Tokyo)'\n 'gazou export --lucene
                 "NOT(mentioned_names:*)"'
                 """
               )
+@click.option("--json", is_flag=True, help="""Export in json format (instead of csv by default)."""
+              )
 @click.option('--index', '-i',
               help="In case of multi-index, monthly indices to export in format YYYY-MM, or relative positions such as "
                    "'last', 'first', 'inactive', separated by comma. Use `--index inactive` to export all inactive"
                    "indices (i. e. not used any more for indexing). By default, export from all opened indices.")
 @click.option('--sort', default="timestamp_utc",
               help="Names of fields who should serve as sorting key, separated by comma. Choose 'no' to reduce export "
                    "time. Defaults to 'timestamp_utc'. 'id' is not a valid option. Run 'gazou export --list-fields' "
                    "to see the full list of available fields.")
 def export(path, query, exclude_threads, exclude_retweets, verbose, export_threads_from_file, export_tweets_from_file,
-           columns, format, list_fields, output, resume, since, until, lucene, step, index, sort):
+           columns, format, list_fields, output, resume, since, until, lucene, step, index, sort, json):
     if output == "-":
         output = None
     if resume and not output:
         log.error("The --resume option requires to set a file name with --output")
         sys.exit(1)
 
-    if resume and not os.path.isfile(output):
-        log.error("The file {} could not be found".format(output))
-        sys.exit(1)
+    if resume:
+        if json:
+            log.error("--resume flag is not supported with json format")
+            sys.exit(1)
+        if not os.path.isfile(output):
+            log.error("The file {} could not be found".format(output))
+            sys.exit(1)
 
     if format == "tcat" and columns:
         log.error("The tcat format is not compatible with the --columns / --select option")
         sys.exit(1)
 
     if list_fields:
         for field in TWEET_FIELDS:
             print(field)
 
     else:
         conf = load_conf(path)
-        export_csv(conf, query, exclude_threads, exclude_retweets, since, until,
+        export_from_db(conf, query, exclude_threads, exclude_retweets, since, until,
                    verbose, export_threads_from_file, export_tweets_from_file, columns, format, output, resume, lucene,
-                   step, index, sort)
+                   step, index, sort, json)
 
 
 @main.command(help="Get a report about the number of tweets. Type 'gazou count' to get the number of collected tweets "
                    "or 'gazou count médialab' to get the number of tweets that contain médialab")
 @click.argument('query', nargs=-1)
 @click.option('--until', type=click.DateTime(), help="Count tweets published strictly before the given "
                                                                    "date, in isoformat")
```

### Comparing `gazouilloire-1.4.0/gazouilloire/config.json.example` & `gazouilloire-1.5.0/gazouilloire/config.json.example`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/config_format.py` & `gazouilloire-1.5.0/gazouilloire/config_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,33 +63,36 @@
         copyfile(os.path.join(os.path.dirname(__file__), "config.json.example"), file_path)
         return True
     else:
         log.warning('A file named config.json already exists in %s' % os.path.realpath(dir_path))
         return False
 
 
-def api_keys_support_stream(conf):
-    try:
-        oauth, oauth2 = get_oauth(conf)
-    except Exception as e:
-        log.error('Could not initiate connections to Twitter API: %s %s' % (type(e), e))
-        sys.exit(1)
-    _, _, streamco = instantiate_clients(oauth, oauth2)
-    args = {'filter_level': 'none', 'stall_warnings': 'true', 'track': ['the']}
-    try:
-        streamiter = streamco.statuses.filter(**args)
-        return True
-    except TwitterHTTPError as e:
-        if "Please use V2 filtered and sample volume stream as alternatives" in str(e):
-            log.warning("Your Twitter API keys were probably created after April 29, 2022. "
-                      "Gazouilloire will only use the 'search' Twitter API, and not the 'stream'.")
-            return False
-        else:
-            log.error("Error while accessing the Twitter API, please retry: {}".format(e))
-            sys.exit(1)
+# def api_keys_support_stream(conf):
+#     """
+#     v1.1 streaming statuses/filter endpoint is now deprecated
+#     """
+#     try:
+#         oauth, oauth2 = get_oauth(conf)
+#     except Exception as e:
+#         log.error('Could not initiate connections to Twitter API: %s %s' % (type(e), e))
+#         sys.exit(1)
+#     _, _, streamco = instantiate_clients(oauth, oauth2)
+#     args = {'filter_level': 'none', 'stall_warnings': 'true', 'track': ['the']}
+#     try:
+#         streamiter = streamco.statuses.filter(**args)
+#         return True
+#     except TwitterHTTPError as e:
+#         if "Please use V2 filtered and sample volume stream as alternatives" in str(e):
+#             log.warning("Your Twitter API keys were probably created after April 29, 2022. "
+#                       "Gazouilloire will only use the 'search' Twitter API, and not the 'stream'.")
+#             return False
+#         else:
+#             log.error("Error while accessing the Twitter API, please retry: {}".format(e))
+#             sys.exit(1)
 
 
 def required_format(conf):
     subfields = {
         "twitter": ["key", "secret", "oauth_token", "oauth_secret"],
         "database": ["host", "port", "db_name"],
         "timezone": []
@@ -132,15 +135,15 @@
         if conf["database"]["nb_past_months"] > 12:
             log.error(
                 'When using "multi_index", "nb_past_months" is limited to 12 months max. '
                 'Please set "nb_past_months" to 12 or less in the config file.'
             )
             sys.exit(1)
 
-    conf["start_stream"] = api_keys_support_stream(conf)
+    conf["start_stream"] = False
 
 
     if "download_media" in conf:
         for subfield in ["photos", "videos", "animated_gifs"]:
             if type(conf["download_media"][subfield]) != bool:
                 log.error(
                     "The '{}' parameter in config.json should be set to either true or false".format(subfield)
```

### Comparing `gazouilloire-1.4.0/gazouilloire/daemon.py` & `gazouilloire-1.5.0/gazouilloire/daemon.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/database/db_mappings.json` & `gazouilloire-1.5.0/gazouilloire/database/db_mappings.json`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/database/elasticmanager.py` & `gazouilloire-1.5.0/gazouilloire/database/elasticmanager.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/exports/export_csv.py` & `gazouilloire-1.5.0/gazouilloire/exports/export.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,37 +29,47 @@
             "proper_links", source.get("links", "")
         )
     ]
     source["domains"] = domains
     return source
 
 
-def yield_csv(queryiterator, fmt, last_ids=set(), export_list=False, query_fields=None):
+def filter_iterator(queryiterator, last_ids, export_list=False, query_fields=None):
     for t in queryiterator:
         try:
             source = t["_source"]
         except KeyError:
             log.error(t)
             if not t["found"]:
                 log.warning(t["_id"] + " not found in database")
                 source = {"_id": t["_id"]}
 
         # ignore tweets only caught on deletion missing most fields
         # if export_list or (len(source) >= 10 and t["_id"] not in last_ids):
         if export_list or t["_id"] not in last_ids:
+            source["id"] = t["_id"]
+            yield post_process_tweet_from_elastic(source)
+
+
+def yield_formatted(queryiterator, fmt, last_ids=set(), export_list=False, query_fields=None, json_fmt=False):
+
+    filtered = filter_iterator(queryiterator, last_ids, export_list, query_fields)
+    if json_fmt:
+        for tweet in filtered:
+            yield tweet
+    else:
+        for tweet in filtered:
             if fmt == "tcat":
-                source = apply_tcat_format(post_process_tweet_from_elastic(source))
-            else:
-                source = post_process_tweet_from_elastic(source)
+                tweet = apply_tcat_format(tweet)
             transform_tweet_into_csv_dict(
-                source,
-                item_id=t["_id"],
+                tweet,
+                item_id=tweet["id"],
                 allow_erroneous_plurals=True
             )
-            yield source
+            yield tweet
 
 
 def build_body(query, exclude_threads, exclude_retweets, query_fields=None, since=None, until=None, resume=False,
                lucene=False):
     if len(query) == 0 and not exclude_threads and not exclude_retweets and not since and not until and not resume:
         body = {
             "query": {
@@ -166,25 +176,26 @@
         rev_reader = reverse_reader(f, ignore_null_bytes=True)
         for row in rev_reader:
             if row[rev_reader.headers.local_time] == last_time:
                 last_ids.add(row[rev_reader.headers.id])
             else:
                 return last_time, last_ids
 
-
-def export_csv(conf, query, exclude_threads, exclude_retweets, since, until,
+def export_from_db(conf, query, exclude_threads, exclude_retweets, since, until,
                verbose, export_threads_from_file, export_tweets_from_file, selection, fmt, outputfile, resume,
                lucene,
                step=None,
                index=None,
-               sort_key="timestamp_utc"
+               sort_key="timestamp_utc",
+               json_fmt=False
                ):
     threads = conf.get('grab_conversations', False)
 
     sort_key = check_elastic_fields(sort_key, sort=True) if sort_key != "no" else ["_doc"]
+
     if "id" in sort_key:
         log.error("Sorting by id is not a valid option.")
         sys.exit(1)
 
     query_fields = None
     if selection:
         headers = check_elastic_fields(selection)
@@ -229,14 +240,15 @@
             sys.exit(1)
         with open(export_tweets_from_file) as f:
             body = sorted([t.get("id", t.get("_id")) for t in csv.DictReader(f)])
 
     if export_threads_from_file or export_tweets_from_file:
         count = len(body)
         iterator = yield_csv(db.multi_get(body, index), fmt, export_list=True)
+
     else:
         last_ids = set()
         if resume:
             last_timestamp, last_ids = find_potential_duplicate_ids(outputfile)
             since = datetime.fromisoformat(last_timestamp)
         body = build_body(query, exclude_threads, exclude_retweets, query_fields, since, until, lucene=lucene)
         try:
@@ -245,40 +257,49 @@
             log.error("Query wrongly formatted. {}".format(str(e)))
             if lucene:
                 log.error(
                     "Please read ElasticSearch's documentation regarding Lucene queries: "
                     "https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-query-string-query.html")
             sys.exit(1)
         if step:
-            iterator = yield_csv(
+            iterator = yield_formatted(
                 yield_step_scans(db, step, since, until, query, exclude_threads, exclude_retweets, query_fields, index,
                                  lucene, sort_key),
                 fmt,
-                last_ids=last_ids
+                last_ids=last_ids,
+                json_fmt=json_fmt
             )
         else:
             body["sort"] = sort_key
-            iterator = yield_csv(
+            iterator = yield_formatted(
                 yield_scans(db, body, since, until, index, sort_key),
                 fmt,
-                last_ids=last_ids
+                last_ids=last_ids,
+                json_fmt=json_fmt
             )
+
     if verbose:
         from tqdm import tqdm
         iterator = tqdm(iterator, total=count)
 
     if resume:
         file = open_file(outputfile, 'a')
     else:
         file = open_file(outputfile, 'w') if outputfile else sys.stdout
-    writer = csv.DictWriter(file, fieldnames=headers, restval='', quoting=csv.QUOTE_MINIMAL, extrasaction='ignore')
-    if not resume:
-        writer.writeheader()
-    for t in iterator:
-        writer.writerow(t)
+
+    if json_fmt:
+        for t in iterator:
+            json.dump(t, file)
+            file.write('\n')
+    else:
+        writer = csv.DictWriter(file, fieldnames=headers, restval='', quoting=csv.QUOTE_MINIMAL, extrasaction='ignore')
+        if not resume:
+            writer.writeheader()
+        for t in iterator:
+            writer.writerow(t)
     file.close()
     iterator.close()
 
 
 def increment_steps(start_date, step):
     return start_date + relativedelta.relativedelta(**{step: 1})
```

### Comparing `gazouilloire-1.4.0/gazouilloire/exports/tweet_fields.py` & `gazouilloire-1.5.0/gazouilloire/exports/tweet_fields.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/manage_scripts.py` & `gazouilloire-1.5.0/gazouilloire/manage_scripts.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/multiprocessing.py` & `gazouilloire-1.5.0/gazouilloire/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/resolving_script.py` & `gazouilloire-1.5.0/gazouilloire/resolving_script.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/run.py` & `gazouilloire-1.5.0/gazouilloire/run.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/scripts/add_bearer_token_to_conf.sh` & `gazouilloire-1.5.0/gazouilloire/scripts/add_bearer_token_to_conf.sh`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/scripts/backup_corpus_ids.sh` & `gazouilloire-1.5.0/gazouilloire/scripts/backup_corpus_ids.sh`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/scripts/daily_mail_export.sh` & `gazouilloire-1.5.0/gazouilloire/scripts/daily_mail_export.sh`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/scripts/elasticdump.sh` & `gazouilloire-1.5.0/gazouilloire/scripts/elasticdump.sh`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/scripts/monthly_archive.sh` & `gazouilloire-1.5.0/gazouilloire/scripts/monthly_archive.sh`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # So a typical crontab would look something like the following:
 #
 # m  h dom mon dow   command
 # 00 4  1   *   *    bash /data/gazouilloire/monthly_export.sh MYENV delete
 
 
 TODAY=$(date --iso)
+TIMESTAMP=`date +%s`
 
 # Corpus directory assumed to be the same as the script's
 CORPUSDIR=$(dirname "$0")
 cd $CORPUSDIR
 
 # Corpus python environment
 CORPUSENV=$1
@@ -46,19 +47,19 @@
 export PATH="$PYENV_ROOT/bin:$PATH"
 export PYENV_VIRTUALENV_DISABLE_PROMPT=1
 eval "$(pyenv init -)"
 eval "$(pyenv virtualenv-init -)"
 pyenv activate "$CORPUSENV"
 
 # Export inactive indices (older than the value of nb_past_months set in config.json)
-gazou count --index inactive --step days > "collected_tweets_per_day_${TODAY}.csv"
-gazou export --index inactive --step hours > "monthly_export_${TODAY}.csv"
+gazou count --index inactive --step days > "collected_tweets_per_day_${TODAY}_${TIMESTAMP}.csv"
+gazou export --index inactive --step hours > "monthly_export_${TODAY}_${TIMESTAMP}.csv"
 
 # Compress the monthly export
-gzip "monthly_export_${TODAY}.csv"
+gzip "monthly_export_${TODAY}_${TIMESTAMP}.csv"
 
 if [ "$?" = 0 ]; then
   # Close or delete inactive indices
   if [[ $CLOSE == "close" ]]; then
     gazou close --index inactive
   elif [[ $CLOSE == "delete" ]]; then
     gazou close --index inactive --delete
```

### Comparing `gazouilloire-1.4.0/gazouilloire/scripts/restart.sh` & `gazouilloire-1.5.0/gazouilloire/scripts/restart.sh`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/test_metas.py` & `gazouilloire-1.5.0/gazouilloire/test_metas.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/test_search.py` & `gazouilloire-1.5.0/gazouilloire/test_search.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/test_stream.py` & `gazouilloire-1.5.0/gazouilloire/test_stream.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/twitter_connexion.py` & `gazouilloire-1.5.0/gazouilloire/twitter_connexion.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/url_resolve.py` & `gazouilloire-1.5.0/gazouilloire/url_resolve.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/web/app.py` & `gazouilloire-1.5.0/gazouilloire/web/app.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire/web/export.py` & `gazouilloire-1.5.0/gazouilloire/web/export.py`

 * *Files identical despite different names*

### Comparing `gazouilloire-1.4.0/gazouilloire.egg-info/PKG-INFO` & `gazouilloire-1.5.0/gazouilloire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gazouilloire
-Version: 1.4.0
+Version: 1.5.0
 Summary: Twitter stream & search API grabber
 Home-page: http://github.com/medialab/gazouilloire
 Author: Benjamin Ooghe-Tabanou
 Author-email: 
 License: GPL-3.0
 Keywords: twitter
 Requires-Python: >=3.7
```

### Comparing `gazouilloire-1.4.0/gazouilloire.egg-info/SOURCES.txt` & `gazouilloire-1.5.0/gazouilloire.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 gazouilloire.egg-info/top_level.txt
 gazouilloire/cli/__init__.py
 gazouilloire/cli/__main__.py
 gazouilloire/database/__init__.py
 gazouilloire/database/db_mappings.json
 gazouilloire/database/elasticmanager.py
 gazouilloire/exports/__init__.py
-gazouilloire/exports/export_csv.py
+gazouilloire/exports/export.py
 gazouilloire/exports/tweet_fields.py
 gazouilloire/scripts/add_bearer_token_to_conf.sh
 gazouilloire/scripts/backup_corpus_ids.sh
 gazouilloire/scripts/daily_mail_export.sh
 gazouilloire/scripts/elasticdump.sh
 gazouilloire/scripts/monthly_archive.sh
 gazouilloire/scripts/restart.sh
```

### Comparing `gazouilloire-1.4.0/setup.py` & `gazouilloire-1.5.0/setup.py`

 * *Files identical despite different names*

