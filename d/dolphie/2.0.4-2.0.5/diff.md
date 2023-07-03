# Comparing `tmp/dolphie-2.0.4.tar.gz` & `tmp/dolphie-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-2.0.4.tar", max compression
+gzip compressed data, was "dolphie-2.0.5.tar", max compression
```

## Comparing `dolphie-2.0.4.tar` & `dolphie-2.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.4/LICENSE
--rw-r--r--   0        0        0     7199 2023-07-03 09:15:41.538676 dolphie-2.0.4/README.md
--rw-r--r--   0        0        0     1347 2023-07-03 06:44:11.377308 dolphie-2.0.4/dolphie/Database.py
--rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.4/dolphie/Functions.py
--rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.4/dolphie/KBHit.py
--rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.4/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.4/dolphie/Panels/innodb_io_panel.py
--rw-r--r--   0        0        0     5323 2023-07-03 01:29:41.157031 dolphie-2.0.4/dolphie/Panels/innodb_locks_panel.py
--rw-r--r--   0        0        0    10063 2023-07-03 01:37:34.898441 dolphie-2.0.4/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0    11947 2023-07-03 06:53:31.927002 dolphie-2.0.4/dolphie/Panels/replica_panel.py
--rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.4/dolphie/Queries.py
--rw-r--r--   0        0        0    51459 2023-07-03 08:29:44.341857 dolphie-2.0.4/dolphie/__init__.py
--rwxr-xr-x   0        0        0    16038 2023-07-03 08:34:51.161992 dolphie-2.0.4/dolphie/app.py
--rw-r--r--   0        0        0      521 2023-07-03 09:16:00.033175 dolphie-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 dolphie-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.5/LICENSE
+-rw-r--r--   0        0        0     7199 2023-07-03 09:15:41.538676 dolphie-2.0.5/README.md
+-rw-r--r--   0        0        0     1347 2023-07-03 06:44:11.377308 dolphie-2.0.5/dolphie/Database.py
+-rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.5/dolphie/Functions.py
+-rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.5/dolphie/KBHit.py
+-rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.5/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.5/dolphie/Panels/innodb_io_panel.py
+-rw-r--r--   0        0        0     5323 2023-07-03 01:29:41.157031 dolphie-2.0.5/dolphie/Panels/innodb_locks_panel.py
+-rw-r--r--   0        0        0    10063 2023-07-03 01:37:34.898441 dolphie-2.0.5/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0    11947 2023-07-03 06:53:31.927002 dolphie-2.0.5/dolphie/Panels/replica_panel.py
+-rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.5/dolphie/Queries.py
+-rw-r--r--   0        0        0    51459 2023-07-03 10:22:51.305863 dolphie-2.0.5/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    16046 2023-07-03 10:23:55.259836 dolphie-2.0.5/dolphie/app.py
+-rw-r--r--   0        0        0      521 2023-07-03 10:24:46.555236 dolphie-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 dolphie-2.0.5/PKG-INFO
```

### Comparing `dolphie-2.0.4/LICENSE` & `dolphie-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/README.md` & `dolphie-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Database.py` & `dolphie-2.0.5/dolphie/Database.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Functions.py` & `dolphie-2.0.5/dolphie/Functions.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/KBHit.py` & `dolphie-2.0.5/dolphie/KBHit.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Panels/dashboard_panel.py` & `dolphie-2.0.5/dolphie/Panels/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Panels/innodb_io_panel.py` & `dolphie-2.0.5/dolphie/Panels/innodb_io_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Panels/innodb_locks_panel.py` & `dolphie-2.0.5/dolphie/Panels/innodb_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Panels/processlist_panel.py` & `dolphie-2.0.5/dolphie/Panels/processlist_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Panels/replica_panel.py` & `dolphie-2.0.5/dolphie/Panels/replica_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/Queries.py` & `dolphie-2.0.5/dolphie/Queries.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/__init__.py` & `dolphie-2.0.5/dolphie/__init__.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.4/dolphie/app.py` & `dolphie-2.0.5/dolphie/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,44 +110,45 @@
     parser.add_argument(
         "-f",
         "--host-cache-file",
         dest="host_cache_file",
         type=str,
         help=(
             "Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line "
-            "using format: ip=hostname [default: %s/host_cache]"
-        )
-        % os.path.dirname(os.path.abspath(__file__)),
+            "using format: ip=hostname [default: %(default)s]"
+        ),
     )
     parser.add_argument(
         "-l",
         "--login-path",
         dest="login_path",
         default="client",
         type=str,
         help=(
             "Specify login path to use mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. "
-            "Supercedes config file [default: client]"
+            "Supercedes config file [default: %(default)s]"
         ),
     )
     parser.add_argument(
         "-r",
         "--refresh_interval",
         dest="refresh_interval",
+        default=1,
         type=int,
-        help="How much time to wait in seconds between each refresh [default: 1]",
+        help="How much time to wait in seconds between each refresh [default: %(default)s]",
     )
     parser.add_argument(
         "-R",
         "--refresh_interval_innodb_status",
         dest="refresh_interval_innodb_status",
+        default=1,
         type=int,
         help=(
             "How much time to wait in seconds to execute SHOW ENGINE INNODB STATUS to refresh data its responsible "
-            "for [default: 1]"
+            "for [default: %(default)s]"
         ),
     )
     parser.add_argument(
         "-H",
         "--heartbeat-table",
         dest="heartbeat_table",
         type=str,
```

### Comparing `dolphie-2.0.4/pyproject.toml` & `dolphie-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolphie"
-version = "2.0.4"
+version = "2.0.5"
 description = "An intuitive feature-rich top tool for monitoring MySQL in real time"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.4.2"
```

### Comparing `dolphie-2.0.4/PKG-INFO` & `dolphie-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 2.0.4
+Version: 2.0.5
 Summary: An intuitive feature-rich top tool for monitoring MySQL in real time
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

