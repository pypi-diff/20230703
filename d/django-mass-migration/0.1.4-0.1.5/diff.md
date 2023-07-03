# Comparing `tmp/django-mass-migration-0.1.4.tar.gz` & `tmp/django-mass-migration-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mass-migration-0.1.4.tar", last modified: Mon Jul  3 10:01:38 2023, max compression
+gzip compressed data, was "django-mass-migration-0.1.5.tar", last modified: Mon Jul  3 15:10:40 2023, max compression
```

## Comparing `django-mass-migration-0.1.4.tar` & `django-mass-migration-0.1.5.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/django_mass_migration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/backends/djangae.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/management/commands/makemassmigration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.615184 django-mass-migration-0.1.4/massmigration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.615184 django-mass-migration-0.1.4/massmigration/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.615184 django-mass-migration-0.1.4/massmigration/templates/admin/massmigration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/templates/admin/massmigration/migrationrecord/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/templates/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/delete_migration.html
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/manage_migrations.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/run_migration.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/templates/migration_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/migration_templates/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/migration_templates/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/migration_templates/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-03 10:01:37.000000 django-mass-migration-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.356444 django-mass-migration-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-03 15:10:40.356444 django-mass-migration-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.352445 django-mass-migration-0.1.5/django_mass_migration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-03 15:10:40.000000 django-mass-migration-0.1.5/django_mass_migration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-03 15:10:40.000000 django-mass-migration-0.1.5/django_mass_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:10:40.000000 django-mass-migration-0.1.5/django_mass_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 15:10:40.000000 django-mass-migration-0.1.5/django_mass_migration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 15:10:40.000000 django-mass-migration-0.1.5/django_mass_migration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.352445 django-mass-migration-0.1.5/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.352445 django-mass-migration-0.1.5/massmigration/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/backends/djangae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.352445 django-mass-migration-0.1.5/massmigration/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.352445 django-mass-migration-0.1.5/massmigration/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/management/commands/makemassmigration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.348444 django-mass-migration-0.1.5/massmigration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.348444 django-mass-migration-0.1.5/massmigration/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.348444 django-mass-migration-0.1.5/massmigration/templates/admin/massmigration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.352445 django-mass-migration-0.1.5/massmigration/templates/admin/massmigration/migrationrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.356444 django-mass-migration-0.1.5/massmigration/templates/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/massmigration/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/massmigration/delete_migration.html
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/massmigration/manage_migrations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/massmigration/migration_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/massmigration/run_migration.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.356444 django-mass-migration-0.1.5/massmigration/templates/migration_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/migration_templates/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/migration_templates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/templates/migration_templates/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.356444 django-mass-migration-0.1.5/massmigration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/utils/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/massmigration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:10:40.356444 django-mass-migration-0.1.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-07-03 15:10:37.000000 django-mass-migration-0.1.5/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:10:40.356444 django-mass-migration-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-03 15:10:39.000000 django-mass-migration-0.1.5/setup.py
```

### Comparing `django-mass-migration-0.1.4/LICENSE` & `django-mass-migration-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/PKG-INFO` & `django-mass-migration-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-mass-migration-0.1.4/README.md` & `django-mass-migration-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/django_mass_migration.egg-info/PKG-INFO` & `django-mass-migration-0.1.5/django_mass_migration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-mass-migration-0.1.4/django_mass_migration.egg-info/SOURCES.txt` & `django-mass-migration-0.1.5/django_mass_migration.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 massmigration/management/__init__.py
 massmigration/management/commands/__init__.py
 massmigration/management/commands/makemassmigration.py
 massmigration/templates/admin/massmigration/migrationrecord/change_list.html
 massmigration/templates/massmigration/base.html
 massmigration/templates/massmigration/delete_migration.html
 massmigration/templates/massmigration/manage_migrations.html
+massmigration/templates/massmigration/migration_detail.html
 massmigration/templates/massmigration/run_migration.html
 massmigration/templates/migration_templates/custom.py
 massmigration/templates/migration_templates/mapper.py
 massmigration/templates/migration_templates/simple.py
 massmigration/utils/__init__.py
 massmigration/utils/apps.py
 massmigration/utils/functional.py
```

### Comparing `django-mass-migration-0.1.4/massmigration/admin.py` & `django-mass-migration-0.1.5/massmigration/admin.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/backends/base.py` & `django-mass-migration-0.1.5/massmigration/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/backends/djangae.py` & `django-mass-migration-0.1.5/massmigration/backends/djangae.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/enforcement.py` & `django-mass-migration-0.1.5/massmigration/enforcement.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/exceptions.py` & `django-mass-migration-0.1.5/massmigration/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/loader.py` & `django-mass-migration-0.1.5/massmigration/loader.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/management/commands/makemassmigration.py` & `django-mass-migration-0.1.5/massmigration/management/commands/makemassmigration.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/migrations.py` & `django-mass-migration-0.1.5/massmigration/migrations.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/models.py` & `django-mass-migration-0.1.5/massmigration/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 from .utils.apps import get_app_label_choices
 from .utils.functional import MemoizedLazyList
 
 
 class MigrationRecord(models.Model):
     """ Stores a record of a particular migration being applied to the database. """
 
+    class Status(models.TextField):
+        APPLIED = "APPLIED"
+        ERRORED = "ERRORED"
+        RUNNING = "RUNNING"
+        NOT_RUN = "NOT_RUN"  # Can't be returned by this object, as this object won't exist
+
     # I'm still not sure whether the key should be computed from the app_label and name or the
     # other way round. The app_label at least is good for filtering in the Django admin though.
     key = models.CharField(max_length=250, primary_key=True)
     app_label = ComputedCharField(
         "_app_label", max_length=100, choices=MemoizedLazyList(get_app_label_choices)
     )
     name = ComputedCharField("_name", max_length=150)
@@ -59,7 +65,14 @@
     @staticmethod
     def key_from_name_tuple(name_tuple):
         """ Given a 2-part migration identifier, return the single string object which we use as
             the `key` field value.
         """
         assert len(name_tuple) == 2
         return ":".join(name_tuple)
+
+    def status(self):
+        if self.is_applied:
+            return self.Status.APPLIED
+        if self.has_error:
+            return self.Status.ERRORED
+        return self.Status.RUNNING
```

### Comparing `django-mass-migration-0.1.4/massmigration/record_cache.py` & `django-mass-migration-0.1.5/massmigration/record_cache.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/templates/massmigration/base.html` & `django-mass-migration-0.1.5/massmigration/templates/massmigration/base.html`

 * *Files 15% similar despite different names*

```diff
@@ -35,25 +35,28 @@
 		}
 		.messages .info {
 			background: #bbbbff;
 		}
 		.messages .error {
 			background: #ffbbbb;
 		}
-		.massmigrations {
+		.table {
 			border: 1px solid #3333aa;
 			border-collapse: collapse;
 		}
-		.massmigrations th, .massmigrations td {
+		.table th, .table td {
 			border: 1px solid #3333aa;
 			padding: 0.4em;
 		}
 		.pt {
 			padding-top: 1rem;
 		}
+		.mt {
+			margin-top: 1.5rem;
+		}
 	</style>
 </head>
 <body>
 	<div class="main">
 		<nav class="nav">
 			<div><a href="{% url 'massmigration_manage' %}">Migrations</a></div>
 		</nav>
```

### Comparing `django-mass-migration-0.1.4/massmigration/templates/massmigration/delete_migration.html` & `django-mass-migration-0.1.5/massmigration/templates/massmigration/delete_migration.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "massmigration/base.html" %}
 
 {% block content %}
 
-<h1>Run Migration</h1>
+<h1>Cancel/Delete Migration</h1>
 <h2>{{migration.key}}</h2>
 <p>{{migration.description}}</p>
 <p class="pt">
 	This will delete the <em>record</em> for the migration in the database.
 </p>
 <p>
 	Once you have delete the record, you will be able to run the migration again.
```

### Comparing `django-mass-migration-0.1.4/massmigration/templates/massmigration/manage_migrations.html` & `django-mass-migration-0.1.5/massmigration/templates/massmigration/manage_migrations.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 {% extends "massmigration/base.html" %}
 
 {% block content %}
 
 <h1>Migrations</h1>
-<table class="massmigrations">
+<table class="table">
 	<thead>
 		<tr>
 			<th>App</th>
 			<th>Migration</th>
 			<th>Status</th>
 			<th>Actions</th>
 		</tr>
 	</thead>
 	<tbody>
 	{% for migration in migrations %}
 		<tr>
 			<td>{{migration.app_label}}</td>
-			<td>{{migration.name}}</td>
+			<td><a href="{% url 'massmigration_detail' key=migration.key %}">{{migration.name}}</a></td>
 			<td>{% if migration.record.is_applied %}APPLIED{% elif migration.record.has_error %}ERRORED{% elif migration.record %}RUNNING{% else %}NOT RUN{% endif %}</td>
 			<td>
 				{% if not migration.record %}<a href="{% url 'massmigration_run' key=migration.key %}">Run...</a>
-				{% elif migration.record.has_error %}<a href="{% url 'massmigration_delete' key=migration.key %}">Delete...</a>
-				{% else %}-
+				{% else %}<a href="{% url 'massmigration_delete' key=migration.key %}">Delete...</a>
 				{% endif %}
 			</td>
 		</tr>
 	{% endfor %}
 	</tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends "massmigration/base.html" %} {% block content %}
 ****** Migrations ******
 App                    Migration         Status                      Actions
                                          {% if
-                                         migration.record.is_applied {% if not migration.record
-                                         %}APPLIED{% elif            %}Run... {% elif
-{                      {                 migration.record.has_error  migration.record.has_error
-{migration.app_label}} {migration.name}} %}ERRORED{% elif            %}Delete... {% else %}- {%
+                                         migration.record.is_applied {% if not
+                                         %}APPLIED{% elif            migration.record
+{                      {                 migration.record.has_error  %}Run... {% else
+{migration.app_label}} {migration.name}} %}ERRORED{% elif            %}Delete... {%
                                          migration.record %}RUNNING  endif %}
                                          {% else %}NOT RUN{% endif
                                          %}
 {% endblock %}
```

### Comparing `django-mass-migration-0.1.4/massmigration/templates/migration_templates/custom.py` & `django-mass-migration-0.1.5/massmigration/templates/migration_templates/custom.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/templates/migration_templates/mapper.py` & `django-mass-migration-0.1.5/massmigration/templates/migration_templates/mapper.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/templates/migration_templates/simple.py` & `django-mass-migration-0.1.5/massmigration/templates/migration_templates/simple.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/utils/functional.py` & `django-mass-migration-0.1.5/massmigration/utils/functional.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/utils/transaction.py` & `django-mass-migration-0.1.5/massmigration/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/massmigration/views.py` & `django-mass-migration-0.1.5/massmigration/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,35 @@
     # else...
     context = {
         "migration": migration,
     }
     return render(request, "massmigration/run_migration.html", context)
 
 
+@superuser_required()
+def migration_detail(request, key):
+    """ View the details of a single migration. """
+    migration = store.by_key.get(key)
+    record = MigrationRecord.objects.filter(key=key).first()
+    dependencies = []
+    dependency_keys = [MigrationRecord.key_from_name_tuple(x) for x in migration.dependencies]
+    dependency_records_by_key = MigrationRecord.objects.in_bulk(dependency_keys)
+    for dep_key in dependency_keys:
+        dependencies.append({
+            "key": dep_key,
+            "record": dependency_records_by_key.get(dep_key),
+        })
+    context = {
+        "migration": migration,
+        "record": record,
+        "dependencies": dependencies,
+    }
+    return render(request, "massmigration/migration_detail.html", context)
+
+
 
 @superuser_required()
 def delete_migration(request, key):
     """ Delete a migration which has already started or has errored. """
     migration = store.by_key.get(key)
     record = MigrationRecord.objects.filter(key=key).first()
     if not migration:
```

### Comparing `django-mass-migration-0.1.4/scripts/release.py` & `django-mass-migration-0.1.5/scripts/release.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.4/setup.py` & `django-mass-migration-0.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # TODO: possibly make the dependency on djangae optional
 EXTRAS = {}
 
 
 setup(
     name=NAME,
-    version="v0.1.4",
+    version="v0.1.5",
     packages=PACKAGES,
     author=AUTHOR,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     keywords=["django", "djangae", "django-gcloud-connectors", "Google App Engine"],
     url=URL,
```

