# Comparing `tmp/dbt-glue-1.5.0.tar.gz` & `tmp/dbt-glue-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.5.0.tar", last modified: Thu Jun 29 09:30:25 2023, max compression
+gzip compressed data, was "dbt-glue-1.5.1.tar", last modified: Mon Jul  3 08:14:25 2023, max compression
```

## Comparing `dbt-glue-1.5.0.tar` & `dbt-glue-1.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.782446 dbt-glue-1.5.0/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-06-29 09:30:25.782269 dbt-glue-1.5.0/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.5.0/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774231 dbt-glue-1.5.0/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774051 dbt-glue-1.5.0/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.776975 dbt-glue-1.5.0/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.0/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-06-29 08:43:24.000000 dbt-glue-1.5.0/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.0/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2524 2023-06-29 08:38:08.000000 dbt-glue-1.5.0/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.777791 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     9699 2023-06-29 08:34:49.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    36786 2023-06-29 09:26:37.000000 dbt-glue-1.5.0/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.0/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774293 dbt-glue-1.5.0/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.778503 dbt-glue-1.5.0/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.778880 dbt-glue-1.5.0/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.0/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.779355 dbt-glue-1.5.0/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.779960 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.780469 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/snapshot.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.780677 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/table/
--rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.0/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774866 dbt-glue-1.5.0/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.780863 dbt-glue-1.5.0/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.781904 dbt-glue-1.5.0/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.0/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-06-29 09:30:25.782505 dbt-glue-1.5.0/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.0/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.201209 dbt-glue-1.5.1/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-03 08:14:25.201053 dbt-glue-1.5.1/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.5.1/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.194167 dbt-glue-1.5.1/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.193998 dbt-glue-1.5.1/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.196665 dbt-glue-1.5.1/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.1/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-07-03 08:13:38.000000 dbt-glue-1.5.1/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.1/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2524 2023-06-29 08:38:08.000000 dbt-glue-1.5.1/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.197480 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     9695 2023-07-03 08:12:14.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    36786 2023-06-29 09:26:37.000000 dbt-glue-1.5.1/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.1/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.194221 dbt-glue-1.5.1/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.198192 dbt-glue-1.5.1/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.198349 dbt-glue-1.5.1/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.1/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.198687 dbt-glue-1.5.1/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199159 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199493 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/snapshot.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199670 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/table/
+-rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.1/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.194783 dbt-glue-1.5.1/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199847 dbt-glue-1.5.1/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.200782 dbt-glue-1.5.1/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.1/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-07-03 08:14:25.201255 dbt-glue-1.5.1/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.1/setup.py
```

### Comparing `dbt-glue-1.5.0/LICENSE` & `dbt-glue-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/PKG-INFO` & `dbt-glue-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.5.0
+Version: 1.5.1
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.5.0/README.md` & `dbt-glue-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/adapters/glue/connections.py` & `dbt-glue-1.5.1/dbt/adapters/glue/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/adapters/glue/credentials.py` & `dbt-glue-1.5.1/dbt/adapters/glue/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,17 +183,17 @@
         if not self._session:
             return
 
         for elapsed in wait(1):
             if self.state not in [GlueSessionState.PROVISIONING, GlueSessionState.READY, GlueSessionState.RUNNING]:
                 return
             
-            logger.debug(f"[elapsed {elapsed}s - calling delete_session for {self.session_id} in {self.state} state")
+            logger.debug(f"[elapsed {elapsed}s - calling stop_session for {self.session_id} in {self.state} state")
             try:
-                self.client.delete_session(Id=self.session_id)
+                self.client.stop_session(Id=self.session_id)
             except Exception as e:
                 if "Session is in PROVISIONING status" in str(e):
                     logger.debug(f"session is not yet initialised - retrying to close")
                 else:
                     raise e
```

### Comparing `dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/adapters/glue/impl.py` & `dbt-glue-1.5.1/dbt/adapters/glue/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/adapters/glue/relation.py` & `dbt-glue-1.5.1/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.5.1/dbt/include/glue/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql` & `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.5.1/dbt/include/glue/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.5.1/dbt_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.5.0
+Version: 1.5.1
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.5.0/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.5.1/dbt_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.0/setup.py` & `dbt-glue-1.5.1/setup.py`

 * *Files identical despite different names*

