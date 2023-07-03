# Comparing `tmp/django-mass-migration-0.1.3.tar.gz` & `tmp/django-mass-migration-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mass-migration-0.1.3.tar", last modified: Wed Jun 28 16:57:26 2023, max compression
+gzip compressed data, was "django-mass-migration-0.1.4.tar", last modified: Mon Jul  3 10:01:38 2023, max compression
```

## Comparing `django-mass-migration-0.1.3.tar` & `django-mass-migration-0.1.4.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.803449 django-mass-migration-0.1.3/django_mass_migration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-06-28 16:57:26.000000 django-mass-migration-0.1.3/django_mass_migration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-28 16:57:26.000000 django-mass-migration-0.1.3/django_mass_migration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 16:57:26.000000 django-mass-migration-0.1.3/django_mass_migration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-28 16:57:26.000000 django-mass-migration-0.1.3/django_mass_migration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 16:57:26.000000 django-mass-migration-0.1.3/django_mass_migration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/backends/djangae.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/management/commands/makemassmigration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.803449 django-mass-migration-0.1.3/massmigration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.803449 django-mass-migration-0.1.3/massmigration/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.803449 django-mass-migration-0.1.3/massmigration/templates/admin/massmigration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/templates/admin/massmigration/migrationrecord/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/templates/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/massmigration/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/massmigration/delete_migration.html
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/massmigration/manage_migrations.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/massmigration/run_migration.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/templates/migration_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/migration_templates/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/migration_templates/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/templates/migration_templates/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/massmigration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-28 16:57:18.000000 django-mass-migration-0.1.3/massmigration/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 16:57:26.807449 django-mass-migration-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-28 16:57:23.000000 django-mass-migration-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/django_mass_migration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 10:01:38.000000 django-mass-migration-0.1.4/django_mass_migration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/backends/djangae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/management/commands/makemassmigration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.615184 django-mass-migration-0.1.4/massmigration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.615184 django-mass-migration-0.1.4/massmigration/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.615184 django-mass-migration-0.1.4/massmigration/templates/admin/massmigration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/templates/admin/massmigration/migrationrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/templates/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/delete_migration.html
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/manage_migrations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/massmigration/run_migration.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/templates/migration_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/migration_templates/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/migration_templates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/templates/migration_templates/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/massmigration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/utils/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/massmigration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-07-03 10:01:33.000000 django-mass-migration-0.1.4/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:01:38.619184 django-mass-migration-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-03 10:01:37.000000 django-mass-migration-0.1.4/setup.py
```

### Comparing `django-mass-migration-0.1.3/LICENSE` & `django-mass-migration-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/PKG-INFO` & `django-mass-migration-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -37,15 +37,15 @@
 
 
 Installation
 ------------
 
 1. Install the package: `pip install django-mass-migration`
 2. Add `massmigration` to `settings.INSTALLED_APPS`.
-3. Add  `path("migrations/, include("massmigration.urls")` to your root urlconf.
+3. Add  `path("migrations/", include("massmigration.urls"))` to your root urlconf.
 4. If you're using the bundled backend, set `settings.MASSMIGRATION_TASK_QUEUE` to a Google Cloud Tasks queue name.
 
 
 Creating A Migration
 --------------------
 
 To create a new migration, run the `makemassmigration` management command:
@@ -167,15 +167,16 @@
 --------
 
 The following settings can be used:
 
 #### `MASSMIGRATION_BACKEND`
 
 This should be a dotted path string to the backend class that you want to use.
-The default is `"massmigration.backends.djangae.DjangaeBackend"`.
+The default is `"massmigration.backends.djangae.DjangaeBackend"`,
+which works with SQL, Google Cloud Datastore and Firestore databases.
 
 
 #### `MASSMIGRATION_TASK_QUEUE`
 
 Used by the `DjangaeBackend`, this sets the Google Cloud Tasks queue name to be used for running migration tasks.
```

### Comparing `django-mass-migration-0.1.3/README.md` & `django-mass-migration-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 Installation
 ------------
 
 1. Install the package: `pip install django-mass-migration`
 2. Add `massmigration` to `settings.INSTALLED_APPS`.
-3. Add  `path("migrations/, include("massmigration.urls")` to your root urlconf.
+3. Add  `path("migrations/", include("massmigration.urls"))` to your root urlconf.
 4. If you're using the bundled backend, set `settings.MASSMIGRATION_TASK_QUEUE` to a Google Cloud Tasks queue name.
 
 
 Creating A Migration
 --------------------
 
 To create a new migration, run the `makemassmigration` management command:
@@ -148,15 +148,16 @@
 --------
 
 The following settings can be used:
 
 #### `MASSMIGRATION_BACKEND`
 
 This should be a dotted path string to the backend class that you want to use.
-The default is `"massmigration.backends.djangae.DjangaeBackend"`.
+The default is `"massmigration.backends.djangae.DjangaeBackend"`,
+which works with SQL, Google Cloud Datastore and Firestore databases.
 
 
 #### `MASSMIGRATION_TASK_QUEUE`
 
 Used by the `DjangaeBackend`, this sets the Google Cloud Tasks queue name to be used for running migration tasks.
```

### Comparing `django-mass-migration-0.1.3/django_mass_migration.egg-info/PKG-INFO` & `django-mass-migration-0.1.4/django_mass_migration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -37,15 +37,15 @@
 
 
 Installation
 ------------
 
 1. Install the package: `pip install django-mass-migration`
 2. Add `massmigration` to `settings.INSTALLED_APPS`.
-3. Add  `path("migrations/, include("massmigration.urls")` to your root urlconf.
+3. Add  `path("migrations/", include("massmigration.urls"))` to your root urlconf.
 4. If you're using the bundled backend, set `settings.MASSMIGRATION_TASK_QUEUE` to a Google Cloud Tasks queue name.
 
 
 Creating A Migration
 --------------------
 
 To create a new migration, run the `makemassmigration` management command:
@@ -167,15 +167,16 @@
 --------
 
 The following settings can be used:
 
 #### `MASSMIGRATION_BACKEND`
 
 This should be a dotted path string to the backend class that you want to use.
-The default is `"massmigration.backends.djangae.DjangaeBackend"`.
+The default is `"massmigration.backends.djangae.DjangaeBackend"`,
+which works with SQL, Google Cloud Datastore and Firestore databases.
 
 
 #### `MASSMIGRATION_TASK_QUEUE`
 
 Used by the `DjangaeBackend`, this sets the Google Cloud Tasks queue name to be used for running migration tasks.
```

### Comparing `django-mass-migration-0.1.3/django_mass_migration.egg-info/SOURCES.txt` & `django-mass-migration-0.1.4/django_mass_migration.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,10 @@
 massmigration/templates/massmigration/run_migration.html
 massmigration/templates/migration_templates/custom.py
 massmigration/templates/migration_templates/mapper.py
 massmigration/templates/migration_templates/simple.py
 massmigration/utils/__init__.py
 massmigration/utils/apps.py
 massmigration/utils/functional.py
-massmigration/utils/permissions.py
+massmigration/utils/permissions.py
+massmigration/utils/transaction.py
+scripts/release.py
```

### Comparing `django-mass-migration-0.1.3/massmigration/admin.py` & `django-mass-migration-0.1.4/massmigration/admin.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/backends/base.py` & `django-mass-migration-0.1.4/massmigration/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/enforcement.py` & `django-mass-migration-0.1.4/massmigration/enforcement.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/exceptions.py` & `django-mass-migration-0.1.4/massmigration/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/loader.py` & `django-mass-migration-0.1.4/massmigration/loader.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/management/commands/makemassmigration.py` & `django-mass-migration-0.1.4/massmigration/management/commands/makemassmigration.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/migrations.py` & `django-mass-migration-0.1.4/massmigration/migrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Standard library
 from uuid import UUID
 import logging
 
 # Third party
-from gcloudc.db import transaction
 from djangae.utils import retry_on_error
 from django.conf import settings
 from django.db import models
 from django.utils.module_loading import import_string
 
-# Djangae Migrations
+# Mass Migration
 from . import record_cache
 from .constants import DEFAULT_BACKEND
 from .exceptions import DependentMigrationNotApplied, MigrationAlreadyStarted
 from .models import MigrationRecord
+from .utils.transaction import get_transaction
 
 
 logger = logging.getLogger(__name__)
 
 
 class BaseMigration:
     """ An operation to be performed on the database. """
@@ -70,15 +70,15 @@
         logger.info("Launched migration %s on backend %s", self.key, backend.__class__)
 
     def can_be_started(self) -> bool:
         return not MigrationRecord.objects.filter(key=self.key).exists()
 
     def mark_as_started(self) -> UUID:
         """ Mark the migration as started in the database. Return the attempt UUID. """
-        with transaction.atomic():
+        with get_transaction().atomic():
             if not self.can_be_started():
                 raise MigrationAlreadyStarted(
                     f"Migration {self.__class__.__name__} has already been initiated."
                 )
             migration = MigrationRecord.objects.create(key=self.key)
             return migration.attempt_uuid
 
@@ -88,15 +88,15 @@
         # TODO: Generate a proper traceback here
         error_str = f"{error.__class__.__name__}: {error}"
         MigrationRecord.objects.filter(key=self.key).update(has_error=True, last_error=error_str)
 
     @retry_on_error()
     def mark_as_finished(self):
         """ Mark the migration as applied/finalized in the database. """
-        with transaction.atomic():
+        with get_transaction().atomic():
             migration = MigrationRecord.objects.get(key=self.key)
             if migration.is_applied:
                 logger.warning("Migration %s is already marked as applied.", self.key)
             else:
                 migration.is_applied = True
                 migration.save()
                 logger.info("Migration %s finished. Marked it as applied.", self.key)
```

### Comparing `django-mass-migration-0.1.3/massmigration/models.py` & `django-mass-migration-0.1.4/massmigration/models.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/record_cache.py` & `django-mass-migration-0.1.4/massmigration/record_cache.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/templates/massmigration/base.html` & `django-mass-migration-0.1.4/massmigration/templates/massmigration/base.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/templates/massmigration/delete_migration.html` & `django-mass-migration-0.1.4/massmigration/templates/massmigration/delete_migration.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/templates/massmigration/manage_migrations.html` & `django-mass-migration-0.1.4/massmigration/templates/massmigration/manage_migrations.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/templates/migration_templates/custom.py` & `django-mass-migration-0.1.4/massmigration/templates/migration_templates/custom.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/templates/migration_templates/mapper.py` & `django-mass-migration-0.1.4/massmigration/templates/migration_templates/mapper.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/templates/migration_templates/simple.py` & `django-mass-migration-0.1.4/massmigration/templates/migration_templates/simple.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/utils/functional.py` & `django-mass-migration-0.1.4/massmigration/utils/functional.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/massmigration/views.py` & `django-mass-migration-0.1.4/massmigration/views.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.3/setup.py` & `django-mass-migration-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # TODO: possibly make the dependency on djangae optional
 EXTRAS = {}
 
 
 setup(
     name=NAME,
-    version="v0.1.3",
+    version="v0.1.4",
     packages=PACKAGES,
     author=AUTHOR,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     keywords=["django", "djangae", "django-gcloud-connectors", "Google App Engine"],
     url=URL,
```

