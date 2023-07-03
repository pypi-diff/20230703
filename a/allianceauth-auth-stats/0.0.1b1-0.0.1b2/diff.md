# Comparing `tmp/allianceauth-auth-stats-0.0.1b1.tar.gz` & `tmp/allianceauth-auth-stats-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-auth-stats-0.0.1b1.tar", last modified: Sun Jun 25 02:44:03 2023, max compression
+gzip compressed data, was "allianceauth-auth-stats-0.0.1b2.tar", last modified: Mon Jul  3 12:11:05 2023, max compression
```

## Comparing `allianceauth-auth-stats-0.0.1b1.tar` & `allianceauth-auth-stats-0.0.1b2.tar`

### file list

```diff
@@ -1,60 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.918209 allianceauth-auth-stats-0.0.1b1/allianceauth_auth_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-25 02:44:03.000000 allianceauth-auth-stats-0.0.1b1/allianceauth_auth_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-25 02:44:03.000000 allianceauth-auth-stats-0.0.1b1/allianceauth_auth_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 02:44:03.000000 allianceauth-auth-stats-0.0.1b1/allianceauth_auth_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 02:44:03.000000 allianceauth-auth-stats-0.0.1b1/allianceauth_auth_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 02:44:03.000000 allianceauth-auth-stats-0.0.1b1/allianceauth_auth_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.918209 allianceauth-auth-stats-0.0.1b1/authstats/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.914209 allianceauth-auth-stats-0.0.1b1/authstats/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.918209 allianceauth-auth-stats-0.0.1b1/authstats/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/management/commands/__init.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/management/commands/reports_refresh_all_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/management/commands/reports_run_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/management/commands/reports_sync_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/authstats/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0002_reportdatathrough_checkbox_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0003_authreportsconfiguration_states_to_include.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0004_alter_authreportsconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0005_alter_authreportsconfiguration_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0006_report_show_character_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0007_reportdatathrough_allow_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/0008_alter_reportdatathrough_long_descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/authstats/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/authstats/templates/authstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/templates/authstats/react_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/authstats/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/templatetags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/authstats/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/authstats/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 02:44:03.922209 allianceauth-auth-stats-0.0.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/tests/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-25 02:43:16.000000 allianceauth-auth-stats-0.0.1b1/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.697862 allianceauth-auth-stats-0.0.1b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-03 12:11:05.697862 allianceauth-auth-stats-0.0.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.685860 allianceauth-auth-stats-0.0.1b2/allianceauth_auth_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/allianceauth_auth_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/allianceauth_auth_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/allianceauth_auth_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/allianceauth_auth_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/allianceauth_auth_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.689861 allianceauth-auth-stats-0.0.1b2/authstats/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.685860 allianceauth-auth-stats-0.0.1b2/authstats/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.689861 allianceauth-auth-stats-0.0.1b2/authstats/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/management/commands/__init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/management/commands/reports_refresh_all_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/management/commands/reports_run_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/management/commands/reports_sync_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.689861 allianceauth-auth-stats-0.0.1b2/authstats/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0002_reportdatathrough_checkbox_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0003_authreportsconfiguration_states_to_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0004_alter_authreportsconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0005_alter_authreportsconfiguration_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0006_report_show_character_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0007_reportdatathrough_allow_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/0008_alter_reportdatathrough_long_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.685860 allianceauth-auth-stats-0.0.1b2/authstats/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.689861 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/asset-manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.685860 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.689861 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/css/main.ec2c1bf0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/css/main.ec2c1bf0.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.689861 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   565427 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/js/main.12f25e42.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/js/main.12f25e42.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2146268 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/authstats/static/authstats/static/js/main.12f25e42.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.693861 allianceauth-auth-stats-0.0.1b2/authstats/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.693861 allianceauth-auth-stats-0.0.1b2/authstats/templates/authstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/templates/authstats/react_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.693861 allianceauth-auth-stats-0.0.1b2/authstats/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/templatetags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.693861 allianceauth-auth-stats-0.0.1b2/authstats/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/authstats/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.685860 allianceauth-auth-stats-0.0.1b2/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.693861 allianceauth-auth-stats-0.0.1b2/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/frontend/build/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.685860 allianceauth-auth-stats-0.0.1b2/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.693861 allianceauth-auth-stats-0.0.1b2/frontend/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/frontend/build/static/css/main.ec2c1bf0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/frontend/build/static/css/main.ec2c1bf0.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.693861 allianceauth-auth-stats-0.0.1b2/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   565427 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/frontend/build/static/js/main.12f25e42.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/frontend/build/static/js/main.12f25e42.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2146268 2023-07-03 12:11:05.000000 allianceauth-auth-stats-0.0.1b2/frontend/build/static/js/main.12f25e42.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:11:05.697862 allianceauth-auth-stats-0.0.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:05.697862 allianceauth-auth-stats-0.0.1b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/tests/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 12:09:35.000000 allianceauth-auth-stats-0.0.1b2/tests/views.py
```

### Comparing `allianceauth-auth-stats-0.0.1b1/LICENCE` & `allianceauth-auth-stats-0.0.1b2/LICENCE`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/PKG-INFO` & `allianceauth-auth-stats-0.0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-auth-stats
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-corp-tools
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -54,15 +54,15 @@
 
 ## Installation
 
 **BETA INSTALL** This will be updated with QOL in later releases but this is still BETA software
 
 ### Bare Metal
 
-1. `pip install allianceauth-auth-stats==0.0.1b1`
+1. `pip install allianceauth-auth-stats==0.0.1b2`
 1. add `'authstats',` to your local.py
 1. migrate `python manage.py migrate`
 1. collectstatic `python manage.py collectstatic --noinput`
 1. sync commands `python manage.py reports_sync_filters`
 1. restart auth
 1. continue to the common section
```

### Comparing `allianceauth-auth-stats-0.0.1b1/README.md` & `allianceauth-auth-stats-0.0.1b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 ## Installation
 
 **BETA INSTALL** This will be updated with QOL in later releases but this is still BETA software
 
 ### Bare Metal
 
-1. `pip install allianceauth-auth-stats==0.0.1b1`
+1. `pip install allianceauth-auth-stats==0.0.1b2`
 1. add `'authstats',` to your local.py
 1. migrate `python manage.py migrate`
 1. collectstatic `python manage.py collectstatic --noinput`
 1. sync commands `python manage.py reports_sync_filters`
 1. restart auth
 1. continue to the common section
```

### Comparing `allianceauth-auth-stats-0.0.1b1/allianceauth_auth_stats.egg-info/PKG-INFO` & `allianceauth-auth-stats-0.0.1b2/allianceauth_auth_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-auth-stats
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-corp-tools
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -54,15 +54,15 @@
 
 ## Installation
 
 **BETA INSTALL** This will be updated with QOL in later releases but this is still BETA software
 
 ### Bare Metal
 
-1. `pip install allianceauth-auth-stats==0.0.1b1`
+1. `pip install allianceauth-auth-stats==0.0.1b2`
 1. add `'authstats',` to your local.py
 1. migrate `python manage.py migrate`
 1. collectstatic `python manage.py collectstatic --noinput`
 1. sync commands `python manage.py reports_sync_filters`
 1. restart auth
 1. continue to the common section
```

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/admin.py` & `allianceauth-auth-stats-0.0.1b2/authstats/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/api.py` & `allianceauth-auth-stats-0.0.1b2/authstats/api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/auth_hooks.py` & `allianceauth-auth-stats-0.0.1b2/authstats/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/management/commands/reports_refresh_all_reports.py` & `allianceauth-auth-stats-0.0.1b2/authstats/management/commands/reports_refresh_all_reports.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/management/commands/reports_run_report.py` & `allianceauth-auth-stats-0.0.1b2/authstats/management/commands/reports_run_report.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/management/commands/reports_sync_filters.py` & `allianceauth-auth-stats-0.0.1b2/authstats/management/commands/reports_sync_filters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/migrations/0001_initial.py` & `allianceauth-auth-stats-0.0.1b2/authstats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/migrations/0003_authreportsconfiguration_states_to_include.py` & `allianceauth-auth-stats-0.0.1b2/authstats/migrations/0003_authreportsconfiguration_states_to_include.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/migrations/0004_alter_authreportsconfiguration_options.py` & `allianceauth-auth-stats-0.0.1b2/authstats/migrations/0004_alter_authreportsconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/migrations/0005_alter_authreportsconfiguration_options_and_more.py` & `allianceauth-auth-stats-0.0.1b2/authstats/migrations/0005_alter_authreportsconfiguration_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/migrations/0008_alter_reportdatathrough_long_descriptions.py` & `allianceauth-auth-stats-0.0.1b2/authstats/migrations/0008_alter_reportdatathrough_long_descriptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/models.py` & `allianceauth-auth-stats-0.0.1b2/authstats/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/schema.py` & `allianceauth-auth-stats-0.0.1b2/authstats/schema.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/signals.py` & `allianceauth-auth-stats-0.0.1b2/authstats/signals.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,7 +52,18 @@
     except:
         logger.error("Bah Humbug")  # we failed! do something here
 
 
 for _filter in filters.get_hooks():
     post_save.connect(new_filter, sender=_filter)
     pre_delete.connect(rem_filter, sender=_filter)
+
+
+def purge_cached_reports(sender, instance, created, **kwargs):
+    """
+    Clear any cached data if a report gets updated/changed/what ever...
+    """
+    if not created:
+        models.ReportResults.objects.filter(report_id=instance.id).delete()
+
+
+post_save.connect(purge_cached_reports, sender=models.Report)
```

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/tasks.py` & `allianceauth-auth-stats-0.0.1b2/authstats/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/templates/authstats/react_base.html` & `allianceauth-auth-stats-0.0.1b2/authstats/templates/authstats/react_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/tests/__init__.py` & `allianceauth-auth-stats-0.0.1b2/authstats/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/tests/test_access.py` & `allianceauth-auth-stats-0.0.1b2/authstats/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/authstats/views.py` & `allianceauth-auth-stats-0.0.1b2/authstats/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/setup.py` & `allianceauth-auth-stats-0.0.1b2/setup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/tests/celery.py` & `allianceauth-auth-stats-0.0.1b2/tests/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-auth-stats-0.0.1b1/tests/test_settings.py` & `allianceauth-auth-stats-0.0.1b2/tests/test_settings.py`

 * *Files identical despite different names*

