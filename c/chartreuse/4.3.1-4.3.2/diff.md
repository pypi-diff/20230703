# Comparing `tmp/chartreuse-4.3.1.tar.gz` & `tmp/chartreuse-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartreuse-4.3.1.tar", last modified: Tue Nov 22 11:19:28 2022, max compression
+gzip compressed data, was "chartreuse-4.3.2.tar", last modified: Mon Jul  3 06:48:47 2023, max compression
```

## Comparing `chartreuse-4.3.1.tar` & `chartreuse-4.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 11:19:28.118967 chartreuse-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     7642 2022-11-22 11:19:12.000000 chartreuse-4.3.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-22 11:19:12.000000 chartreuse-4.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      404 2022-11-22 11:19:28.118967 chartreuse-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2022-11-22 11:19:12.000000 chartreuse-4.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-11-22 11:19:12.000000 chartreuse-4.3.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-22 11:19:12.000000 chartreuse-4.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      596 2022-11-22 11:19:28.118967 chartreuse-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2022-11-22 11:19:12.000000 chartreuse-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 11:19:28.114967 chartreuse-4.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 11:19:28.118967 chartreuse-4.3.1/src/chartreuse/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-11-22 11:19:12.000000 chartreuse-4.3.1/src/chartreuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2022-11-22 11:19:12.000000 chartreuse-4.3.1/src/chartreuse/chartreuse.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4101 2022-11-22 11:19:12.000000 chartreuse-4.3.1/src/chartreuse/chartreuse_upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 11:19:28.118967 chartreuse-4.3.1/src/chartreuse/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2022-11-22 11:19:12.000000 chartreuse-4.3.1/src/chartreuse/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6310 2022-11-22 11:19:12.000000 chartreuse-4.3.1/src/chartreuse/utils/alembic_migration_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 11:19:28.118967 chartreuse-4.3.1/src/chartreuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2022-11-22 11:19:28.000000 chartreuse-4.3.1/src/chartreuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      512 2022-11-22 11:19:28.000000 chartreuse-4.3.1/src/chartreuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 11:19:28.000000 chartreuse-4.3.1/src/chartreuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       74 2022-11-22 11:19:28.000000 chartreuse-4.3.1/src/chartreuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      161 2022-11-22 11:19:28.000000 chartreuse-4.3.1/src/chartreuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-22 11:19:28.000000 chartreuse-4.3.1/src/chartreuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 11:19:27.000000 chartreuse-4.3.1/src/chartreuse.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-03 06:48:37.000000 chartreuse-4.3.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 06:48:37.000000 chartreuse-4.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 06:48:47.191141 chartreuse-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-03 06:48:37.000000 chartreuse-4.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 06:48:37.000000 chartreuse-4.3.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 06:48:37.000000 chartreuse-4.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 06:48:47.195141 chartreuse-4.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 06:48:37.000000 chartreuse-4.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/chartreuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/chartreuse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4101 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/chartreuse_upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/chartreuse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6307 2023-07-03 06:48:37.000000 chartreuse-4.3.2/src/chartreuse/utils/alembic_migration_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:48:47.191141 chartreuse-4.3.2/src/chartreuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 06:48:47.000000 chartreuse-4.3.2/src/chartreuse.egg-info/zip-safe
```

### Comparing `chartreuse-4.3.1/LICENCE.md` & `chartreuse-4.3.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.1/README.md` & `chartreuse-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.1/setup.cfg` & `chartreuse-4.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.1/setup.py` & `chartreuse-4.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.1/src/chartreuse/chartreuse.py` & `chartreuse-4.3.2/src/chartreuse/chartreuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         alembic_config_file_path: str,
         postgresql_url: str,
         release_name: str,
         alembic_allow_migration_for_empty_database: bool,
         alembic_additional_parameters: str = "",
         kubernetes_helper: wiremind_kubernetes.kubernetes_helper.KubernetesDeploymentManager = None,
     ):
-
         configure_logging()
 
         self.alembic_migration_helper = AlembicMigrationHelper(
             alembic_directory_path=alembic_directory_path,
             alembic_config_file_path=alembic_config_file_path,
             database_url=postgresql_url,
             allow_migration_for_empty_database=alembic_allow_migration_for_empty_database,
```

### Comparing `chartreuse-4.3.1/src/chartreuse/chartreuse_upgrade.py` & `chartreuse-4.3.2/src/chartreuse/chartreuse_upgrade.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.1/src/chartreuse/utils/alembic_migration_helper.py` & `chartreuse-4.3.2/src/chartreuse/utils/alembic_migration_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,24 +40,23 @@
 
         if configure:
             self._configure()
 
         self.is_migration_needed = self._check_migration_needed()
 
     def _configure(self) -> None:
-        cleaned_url = self.database_url.replace("/", r"\/")
-        command_sq: str = (
-            f"sed -i -e 's/sqlalchemy.url.*=.*/sqlalchemy.url={cleaned_url}/' {self.alembic_config_file_path}"
-        )
-        stdout, _, returncode = run_command(command_sq, cwd=self.alembic_directory_path, return_result=True)
-        if returncode == 0:
+        with open("%s/%s" % (self.alembic_directory_path, self.alembic_config_file_path), "r") as f:
+            content = f.read()
+            content_new = re.sub("(sqlalchemy.url.*=.*){1}", r"sqlalchemy.url=%s" % self.database_url, content, flags=re.M)
+        if content != content_new:
+            with open("%s/%s" % (self.alembic_directory_path, self.alembic_config_file_path), "w") as f:
+                f.write(content_new)
             logger.info("alembic.ini was configured.")
         else:
-            # To avoid displaying the password. sed can still display a part of the URL
-            raise SubprocessError(f"{command_sq.format(sqlalchemy_url='REDACTED')} has failed: {stdout}")
+            raise SubprocessError("configuration of alembic.ini has failed (alembic.ini is unchanged)")
 
     def _wait_postgres_is_configured(self) -> None:
         """
         Make sure the user `wiremind_owner_user` was created by the postgres-operator
         and that default privileges were configured.
         # TODO: Maybe make this a readinessProbe on Patroni PG Pods
         """
```

### Comparing `chartreuse-4.3.1/src/chartreuse.egg-info/SOURCES.txt` & `chartreuse-4.3.2/src/chartreuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

