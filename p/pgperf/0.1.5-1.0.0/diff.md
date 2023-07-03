# Comparing `tmp/pgperf-0.1.5.tar.gz` & `tmp/pgperf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgperf-0.1.5.tar", max compression
+gzip compressed data, was "pgperf-1.0.0.tar", max compression
```

## Comparing `pgperf-0.1.5.tar` & `pgperf-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,82 @@
--rw-r--r--   0        0        0    35148 2022-06-24 18:09:22.195604 pgperf-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0    21356 2022-06-23 08:52:18.893142 pgperf-0.1.5/README.rst
--rw-r--r--   0        0        0     1118 2022-06-24 18:18:57.237141 pgperf-0.1.5/long_description.md
--rw-r--r--   0        0        0     1102 2022-06-24 17:49:35.302884 pgperf-0.1.5/pgperf/__init__.py
--rw-r--r--   0        0        0     4097 2022-06-21 14:27:24.470130 pgperf-0.1.5/pgperf/db.py
--rw-r--r--   0        0        0    13932 2022-06-21 14:27:47.266586 pgperf-0.1.5/pgperf/main.py
--rw-r--r--   0        0        0      233 2022-06-21 14:26:49.783784 pgperf-0.1.5/pgperf/templates/active_conection.sql
--rw-r--r--   0        0        0      200 2022-06-21 14:26:49.783784 pgperf-0.1.5/pgperf/templates/add_extensions.sql
--rw-r--r--   0        0        0      527 2022-06-21 14:26:49.783784 pgperf-0.1.5/pgperf/templates/all_locks.sql
--rw-r--r--   0        0        0     4124 2022-06-21 14:26:49.783784 pgperf-0.1.5/pgperf/templates/bloat.sql
--rw-r--r--   0        0        0      553 2022-06-21 14:26:49.783784 pgperf-0.1.5/pgperf/templates/blocking.sql
--rw-r--r--   0        0        0      691 2022-06-21 14:26:49.783784 pgperf-0.1.5/pgperf/templates/buffercache_stats.sql
--rw-r--r--   0        0        0      350 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/buffercache_usage.sql
--rw-r--r--   0        0        0      328 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/cache_hit.sql
--rw-r--r--   0        0        0      564 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/calls.sql
--rw-r--r--   0        0        0      549 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/calls_legacy.sql
--rw-r--r--   0        0        0      483 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/db_settings.sql
--rw-r--r--   0        0        0      656 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/duplicate_indexes.sql
--rw-r--r--   0        0        0      106 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/extensions.sql
--rw-r--r--   0        0        0      499 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/index_cache_hit.sql
--rw-r--r--   0        0        0      434 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/index_scans.sql
--rw-r--r--   0        0        0      378 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/index_size.sql
--rw-r--r--   0        0        0      319 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/index_usage.sql
--rw-r--r--   0        0        0      278 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/indexes.sql
--rw-r--r--   0        0        0      213 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/kill_all.sql
--rw-r--r--   0        0        0      653 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/locks.sql
--rw-r--r--   0        0        0      357 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/long_running_queries.sql
--rw-r--r--   0        0        0     1120 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/null_indexes.sql
--rw-r--r--   0        0        0      591 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/outliers.sql
--rw-r--r--   0        0        0      123 2022-06-21 14:26:49.787117 pgperf-0.1.5/pgperf/templates/pg_stat_statements_reset.sql
--rw-r--r--   0        0        0      193 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/records_rank.sql
--rw-r--r--   0        0        0      155 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/seq_scans.sql
--rw-r--r--   0        0        0       59 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/ssl_used.sql
--rw-r--r--   0        0        0      510 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/table_cache_hit.sql
--rw-r--r--   0        0        0      179 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/table_index_scans.sql
--rw-r--r--   0        0        0      389 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/table_index_size.sql
--rw-r--r--   0        0        0      373 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/table_size.sql
--rw-r--r--   0        0        0      298 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/total_index_size.sql
--rw-r--r--   0        0        0      391 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/total_table_size.sql
--rw-r--r--   0        0        0      734 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/unused_indexes.sql
--rw-r--r--   0        0        0     1918 2022-06-21 14:26:49.790451 pgperf-0.1.5/pgperf/templates/vacuum_stats.sql
--rw-r--r--   0        0        0      932 2022-06-24 18:17:37.308318 pgperf-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2157 2022-06-24 18:19:09.385006 pgperf-0.1.5/setup.py
--rw-r--r--   0        0        0     2317 2022-06-24 18:19:09.385215 pgperf-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-06-24 18:09:22.195604 pgperf-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0    21356 2022-06-23 08:52:18.893142 pgperf-1.0.0/README.rst
+-rw-r--r--   0        0        0     1118 2022-06-24 18:18:57.237141 pgperf-1.0.0/long_description.md
+-rw-r--r--   0        0        0     1013 2023-06-30 22:48:00.639829 pgperf-1.0.0/pgperf/__init__.py
+-rw-r--r--   0        0        0     5321 2023-07-03 08:23:57.167777 pgperf-1.0.0/pgperf/db.py
+-rw-r--r--   0        0        0     9691 2023-06-30 22:50:27.211093 pgperf-1.0.0/pgperf/main.py
+-rw-r--r--   0        0        0     1983 2023-07-01 20:51:52.024862 pgperf-1.0.0/pgperf/server/__init__.py
+-rw-r--r--   0        0        0      877 2023-06-30 22:48:00.639829 pgperf-1.0.0/pgperf/server/additional/__init__.py
+-rw-r--r--   0        0        0     4810 2023-07-03 09:07:08.404802 pgperf-1.0.0/pgperf/server/configuration/__init__.py
+-rw-r--r--   0        0        0     2300 2023-07-03 09:05:48.962231 pgperf-1.0.0/pgperf/server/configuration/replication.py
+-rw-r--r--   0        0        0      659 2023-06-30 22:48:00.639829 pgperf-1.0.0/pgperf/server/stats/__init__.py
+-rw-r--r--   0        0        0     8395 2023-06-30 22:05:26.233029 pgperf-1.0.0/pgperf/server/stats/collected.py
+-rw-r--r--   0        0        0     2956 2023-06-30 22:11:39.798751 pgperf-1.0.0/pgperf/server/stats/dinamic.py
+-rw-r--r--   0        0        0      527 2022-06-21 14:26:49.783784 pgperf-1.0.0/pgperf/templates/all_locks.sql
+-rw-r--r--   0        0        0     4124 2022-06-21 14:26:49.783784 pgperf-1.0.0/pgperf/templates/bloat.sql
+-rw-r--r--   0        0        0      553 2022-06-21 14:26:49.783784 pgperf-1.0.0/pgperf/templates/blocking.sql
+-rw-r--r--   0        0        0      691 2022-06-21 14:26:49.783784 pgperf-1.0.0/pgperf/templates/buffercache_stats.sql
+-rw-r--r--   0        0        0      350 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/buffercache_usage.sql
+-rw-r--r--   0        0        0      328 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/cache_hit.sql
+-rw-r--r--   0        0        0      564 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/calls.sql
+-rw-r--r--   0        0        0      549 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/calls_legacy.sql
+-rw-r--r--   0        0        0      656 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/duplicate_indexes.sql
+-rw-r--r--   0        0        0      499 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/index_cache_hit.sql
+-rw-r--r--   0        0        0      434 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/index_scans.sql
+-rw-r--r--   0        0        0      378 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/index_size.sql
+-rw-r--r--   0        0        0      319 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/index_usage.sql
+-rw-r--r--   0        0        0      278 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/indexes.sql
+-rw-r--r--   0        0        0      653 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/locks.sql
+-rw-r--r--   0        0        0      357 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/long_running_queries.sql
+-rw-r--r--   0        0        0     1120 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/null_indexes.sql
+-rw-r--r--   0        0        0      591 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/outliers.sql
+-rw-r--r--   0        0        0      123 2023-06-30 09:09:21.620176 pgperf-1.0.0/pgperf/templates/pg_stat_statements_reset.sql
+-rw-r--r--   0        0        0      193 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/records_rank.sql
+-rw-r--r--   0        0        0      155 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/seq_scans.sql
+-rw-r--r--   0        0        0      233 2022-06-21 14:26:49.783784 pgperf-1.0.0/pgperf/templates/server/active_conection.sql
+-rw-r--r--   0        0        0      200 2023-06-30 22:33:18.023676 pgperf-1.0.0/pgperf/templates/server/additional/add_all_recommended_extensions.sql
+-rw-r--r--   0        0        0      106 2023-06-30 22:33:28.616938 pgperf-1.0.0/pgperf/templates/server/additional/extensions.sql
+-rw-r--r--   0        0        0        9 2023-07-01 20:52:32.207657 pgperf-1.0.0/pgperf/templates/server/config/show_all.sql
+-rw-r--r--   0        0        0       20 2023-07-03 08:22:50.138713 pgperf-1.0.0/pgperf/templates/server/config/show_variable.sql
+-rw-r--r--   0        0        0      483 2023-07-01 20:54:10.413036 pgperf-1.0.0/pgperf/templates/server/db_settings.sql
+-rw-r--r--   0        0        0      213 2022-06-21 14:26:49.787117 pgperf-1.0.0/pgperf/templates/server/kill_all.sql
+-rw-r--r--   0        0        0       59 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/server/ssl_used.sql
+-rw-r--r--   0        0        0       34 2023-06-30 21:31:28.179266 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_all_indexes.sql
+-rw-r--r--   0        0        0       33 2023-06-30 21:30:05.484644 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_all_tables.sql
+-rw-r--r--   0        0        0       31 2023-06-30 21:25:48.657476 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_archiver.sql
+-rw-r--r--   0        0        0       31 2023-06-30 21:29:11.240477 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_bgwriter.sql
+-rw-r--r--   0        0        0       30 2023-06-30 21:29:31.820792 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_database.sql
+-rw-r--r--   0        0        0       41 2023-06-30 21:29:52.481110 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_database_conflicts.sql
+-rw-r--r--   0        0        0       34 2023-06-30 21:31:54.886353 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_sys_indexes.sql
+-rw-r--r--   0        0        0       33 2023-06-30 21:30:21.371556 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_sys_tables.sql
+-rw-r--r--   0        0        0       37 2023-06-30 21:35:31.171649 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_user_functions.sql
+-rw-r--r--   0        0        0       35 2023-06-30 21:32:12.206627 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_user_indexes.sql
+-rw-r--r--   0        0        0       34 2023-06-30 21:30:35.798447 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_user_tables.sql
+-rw-r--r--   0        0        0       38 2023-06-30 21:30:46.171942 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_xact_all_tables.sql
+-rw-r--r--   0        0        0       38 2023-06-30 21:31:00.458831 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_xact_sys_tables.sql
+-rw-r--r--   0        0        0       42 2023-06-30 21:35:46.177137 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_xact_user_functions.sql
+-rw-r--r--   0        0        0       39 2023-06-30 21:31:14.405717 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_stat_xact_user_tables.sql
+-rw-r--r--   0        0        0       36 2023-06-30 21:33:36.688508 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_all_indexes.sql
+-rw-r--r--   0        0        0       38 2023-06-30 21:34:47.728590 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_all_sequences.sql
+-rw-r--r--   0        0        0       35 2023-06-30 21:32:24.903495 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_all_tables.sql
+-rw-r--r--   0        0        0       36 2023-06-30 21:33:31.978977 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_sys_indexes.sql
+-rw-r--r--   0        0        0       38 2023-06-30 21:35:02.374007 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_sys_sequences.sql
+-rw-r--r--   0        0        0       37 2023-06-30 21:33:38.654980 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_sys_tables.sql
+-rw-r--r--   0        0        0       37 2023-06-30 21:34:28.086988 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_user_indexes.sql
+-rw-r--r--   0        0        0       39 2023-06-30 21:35:17.672738 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_user_sequences.sql
+-rw-r--r--   0        0        0       36 2023-06-30 21:32:56.180660 pgperf-1.0.0/pgperf/templates/server/stats/collected/pg_statio_user_tables.sql
+-rw-r--r--   0        0        0       31 2023-06-30 09:09:41.996661 pgperf-1.0.0/pgperf/templates/server/stats/dinamic/pg_stat_activity.sql
+-rw-r--r--   0        0        0       38 2023-06-30 10:05:58.057835 pgperf-1.0.0/pgperf/templates/server/stats/dinamic/pg_stat_progress_vacuum.sql
+-rw-r--r--   0        0        0       34 2023-06-30 09:26:54.710612 pgperf-1.0.0/pgperf/templates/server/stats/dinamic/pg_stat_replication.sql
+-rw-r--r--   0        0        0       26 2023-06-30 09:55:36.786742 pgperf-1.0.0/pgperf/templates/server/stats/dinamic/pg_stat_ssl.sql
+-rw-r--r--   0        0        0       34 2023-06-30 09:52:44.191723 pgperf-1.0.0/pgperf/templates/server/stats/dinamic/pg_stat_subscription.sql
+-rw-r--r--   0        0        0       34 2023-06-30 09:47:04.234986 pgperf-1.0.0/pgperf/templates/server/stats/dinamic/pg_stat_wal_receiver.sql
+-rw-r--r--   0        0        0     1918 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/server/vacuum_stats.sql
+-rw-r--r--   0        0        0      510 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/table_cache_hit.sql
+-rw-r--r--   0        0        0      179 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/table_index_scans.sql
+-rw-r--r--   0        0        0      389 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/table_index_size.sql
+-rw-r--r--   0        0        0      373 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/table_size.sql
+-rw-r--r--   0        0        0      298 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/total_index_size.sql
+-rw-r--r--   0        0        0      391 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/total_table_size.sql
+-rw-r--r--   0        0        0      734 2022-06-21 14:26:49.790451 pgperf-1.0.0/pgperf/templates/unused_indexes.sql
+-rw-r--r--   0        0        0     1118 2023-06-30 09:51:51.685558 pgperf-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 pgperf-1.0.0/PKG-INFO
```

### Comparing `pgperf-0.1.5/LICENSE.txt` & `pgperf-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/README.rst` & `pgperf-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/long_description.md` & `pgperf-1.0.0/long_description.md`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/__init__.py` & `pgperf-1.0.0/pgperf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-__version__ = '0.1.5'
+__version__ = '1.0.0'
 
-import fire
 import os
 from rich.console import Console
 from omegaconf import OmegaConf
 from jinja2 import Environment, PackageLoader
 
 console = Console()
 user_home = os.path.expanduser('~')
 default_config = user_home + '/.pgperf.yml'
 try:
     OmegaConf.load(default_config)
 except Exception:
-    console.print(f"[white] Creating default config...")
+    console.print("[white] Creating default config...")
     conf_yaml = """
 prod:
   db:
     server: 127.0.0.1
     port: 5432
     db: prod_db_name
     user: prod_db_user
@@ -32,11 +31,7 @@
     input()
 config = OmegaConf.load(default_config)
 file_loader = PackageLoader('pgperf', 'templates')
 env = Environment(loader=file_loader)
 env.trim_blocks = True
 env.lstrip_blocks = True
 env.rstrip_blocks = True
-
-debug = os.getenv('DEBUG')
-log = os.getenv('LOG')
-conn = os.getenv('CONN')
```

### Comparing `pgperf-0.1.5/pgperf/templates/all_locks.sql` & `pgperf-1.0.0/pgperf/templates/all_locks.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/bloat.sql` & `pgperf-1.0.0/pgperf/templates/bloat.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/blocking.sql` & `pgperf-1.0.0/pgperf/templates/blocking.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/buffercache_stats.sql` & `pgperf-1.0.0/pgperf/templates/buffercache_stats.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/calls.sql` & `pgperf-1.0.0/pgperf/templates/calls.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/calls_legacy.sql` & `pgperf-1.0.0/pgperf/templates/calls_legacy.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/duplicate_indexes.sql` & `pgperf-1.0.0/pgperf/templates/duplicate_indexes.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/locks.sql` & `pgperf-1.0.0/pgperf/templates/locks.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/null_indexes.sql` & `pgperf-1.0.0/pgperf/templates/null_indexes.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/outliers.sql` & `pgperf-1.0.0/pgperf/templates/outliers.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/unused_indexes.sql` & `pgperf-1.0.0/pgperf/templates/unused_indexes.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pgperf/templates/vacuum_stats.sql` & `pgperf-1.0.0/pgperf/templates/server/vacuum_stats.sql`

 * *Files identical despite different names*

### Comparing `pgperf-0.1.5/pyproject.toml` & `pgperf-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 [tool.poetry]
 name = "pgperf"
-version = "0.1.5"
+version = "1.0.0"
 description = "PostgreSQL Performance Tools"
 authors = ["Aldo A. Villagra B. <aldovillagra@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "long_description.md"
 homepage = "https://github.com/aldovillagra/pgperf"
 repository = "https://github.com/aldovillagra/pgperf"
 documentation = "https://github.com/aldovillagra/pgperf#readme"
 include = ["README.rst", "LICENSE.txt"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/aldovillagra/pgperf/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-rich = "^12.4.4"
-fire = "^0.4.0"
 omegaconf = "^2.2.1"
 pandas = "^1.4.2"
 SQLAlchemy = "^1.4.36"
 numpy = "^1.22.4"
 psycopg2 = "^2.9.3"
 tabulate = "^0.8.9"
 Jinja2 = "^3.1.2"
 XlsxWriter = "^3.0.3"
+typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
+[tool.poetry.group.dev.dependencies]
+mkdocs = "^1.4.3"
+ruff = "^0.0.275"
+ipdb = "^0.13.13"
+deptry = "^0.12.0"
+poethepoet = "^0.20.0"
+autopep8 = "^2.0.2"
+bpython = "^0.24"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-pgperf = 'pgperf.main:run'
+pgperf = 'pgperf.main:app'
```

### Comparing `pgperf-0.1.5/PKG-INFO` & `pgperf-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pgperf
-Version: 0.1.5
+Version: 1.0.0
 Summary: PostgreSQL Performance Tools
 Home-page: https://github.com/aldovillagra/pgperf
 License: GPL-3.0-or-later
 Author: Aldo A. Villagra B.
 Author-email: aldovillagra@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.36,<2.0.0)
 Requires-Dist: XlsxWriter (>=3.0.3,<4.0.0)
-Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: omegaconf (>=2.2.1,<3.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
-Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/aldovillagra/pgperf/issues
 Project-URL: Documentation, https://github.com/aldovillagra/pgperf#readme
 Project-URL: Repository, https://github.com/aldovillagra/pgperf
 Description-Content-Type: text/markdown
 
 # Python PostgreSQL Performance Tools
```

