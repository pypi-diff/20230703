# Comparing `tmp/lamindb_setup-0.48.1.tar.gz` & `tmp/lamindb_setup-0.48.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.48.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.48.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.48.1.tar` & `lamindb_setup-0.48.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0     4010 2023-06-21 19:39:29.494297 lamindb_setup-0.48.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.48.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.48.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.48.1/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.48.1/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.48.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.48.1/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.48.1/README.md
--rw-r--r--   0        0        0    56567 2023-07-02 09:51:05.743941 lamindb_setup-0.48.1/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.48.1/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.48.1/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.48.1/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.48.1/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.48.1/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4418 2023-06-20 11:14:24.334197 lamindb_setup-0.48.1/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.48.1/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.48.1/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.48.1/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.48.1/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.48.1/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.48.1/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.48.1/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.48.1/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.48.1/lamin-project.yaml
--rw-r--r--   0        0        0     2757 2023-07-02 09:51:00.353981 lamindb_setup-0.48.1/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.48.1/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1413 2023-07-02 09:09:44.106951 lamindb_setup-0.48.1/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.48.1/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.48.1/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.48.1/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.48.1/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7053 2023-07-02 09:27:47.960491 lamindb_setup-0.48.1/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6276 2023-07-02 09:27:47.961713 lamindb_setup-0.48.1/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1118 2023-06-15 00:10:45.075143 lamindb_setup-0.48.1/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.48.1/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.48.1/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.48.1/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.48.1/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.48.1/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.48.1/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.48.1/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.48.1/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.48.1/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.48.1/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.48.1/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.48.1/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10748 2023-06-29 15:11:20.989570 lamindb_setup-0.48.1/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.48.1/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     3456 2023-06-18 07:46:49.405332 lamindb_setup-0.48.1/lamindb_setup/dev/_hub_client.py
--rw-r--r--   0        0        0     9074 2023-06-20 11:14:24.335109 lamindb_setup-0.48.1/lamindb_setup/dev/_hub_core.py
--rw-r--r--   0        0        0     3310 2023-06-18 07:46:49.405673 lamindb_setup-0.48.1/lamindb_setup/dev/_hub_crud.py
--rw-r--r--   0        0        0     4129 2023-06-27 14:15:46.405828 lamindb_setup-0.48.1/lamindb_setup/dev/_hub_utils.py
--rw-r--r--   0        0        0     9365 2023-06-28 12:32:26.045930 lamindb_setup-0.48.1/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.48.1/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.48.1/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.48.1/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.48.1/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.48.1/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.48.1/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4812 2023-06-15 12:55:29.508183 lamindb_setup-0.48.1/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.48.1/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.48.1/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.48.1/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.48.1/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.48.1/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.48.1/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    29416 2023-06-29 19:17:30.194449 lamindb_setup-0.48.1/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.48.1/lnschema-core/LICENSE
--rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.48.1/lnschema-core/README.md
--rw-r--r--   0        0        0      617 2023-06-30 11:14:16.252662 lamindb_setup-0.48.1/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.48.1/lnschema-core/lnschema_core/_queryset.py
--rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.48.1/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
--rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
--rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
--rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
--rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    23909 2023-06-29 19:17:30.196117 lamindb_setup-0.48.1/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      951 2023-06-29 19:17:30.196374 lamindb_setup-0.48.1/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.48.1/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.48.1/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.48.1/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.48.1/lnschema-core/tests/test_integrity.py
--rw-r--r--   0        0        0     1821 2023-06-27 14:15:46.405994 lamindb_setup-0.48.1/noxfile.py
--rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.48.1/pyproject.toml
--rw-r--r--   0        0        0     1169 2023-06-27 14:15:46.406331 lamindb_setup-0.48.1/tests/hub/test_instance.py
--rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.48.1/tests/hub/test_signup_signin.py
--rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.48.1/tests/hub/test_storage.py
--rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.48.1/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-19 15:23:54.026893 lamindb_setup-0.48.1/tests/test_init_instance.py
--rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.48.1/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.48.1/tests/test_login.py
--rw-r--r--   0        0        0      420 2023-06-15 00:10:45.075855 lamindb_setup-0.48.1/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.48.1/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.48.1/tests/test_signup.py
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.48.1/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-21 19:39:29.494297 lamindb_setup-0.48.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.48.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.48.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.48.2/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.48.2/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.48.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.48.2/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.48.2/README.md
+-rw-r--r--   0        0        0    56753 2023-07-03 13:12:20.573226 lamindb_setup-0.48.2/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.48.2/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.48.2/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.48.2/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.48.2/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.48.2/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4418 2023-06-20 11:14:24.334197 lamindb_setup-0.48.2/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.48.2/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.48.2/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.48.2/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.48.2/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.48.2/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.48.2/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.48.2/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.48.2/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.48.2/lamin-project.yaml
+-rw-r--r--   0        0        0     2757 2023-07-03 13:12:31.506061 lamindb_setup-0.48.2/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.48.2/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1413 2023-07-02 09:09:44.106951 lamindb_setup-0.48.2/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      714 2023-07-03 13:01:58.204697 lamindb_setup-0.48.2/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.48.2/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.48.2/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.48.2/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7196 2023-07-03 13:01:58.205108 lamindb_setup-0.48.2/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6419 2023-07-03 13:01:58.205472 lamindb_setup-0.48.2/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1118 2023-06-15 00:10:45.075143 lamindb_setup-0.48.2/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.48.2/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.48.2/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.48.2/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.48.2/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.48.2/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.48.2/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.48.2/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.48.2/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.48.2/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.48.2/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.48.2/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.48.2/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10748 2023-06-29 15:11:20.989570 lamindb_setup-0.48.2/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.48.2/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3456 2023-06-18 07:46:49.405332 lamindb_setup-0.48.2/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0     9074 2023-06-20 11:14:24.335109 lamindb_setup-0.48.2/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     3310 2023-06-18 07:46:49.405673 lamindb_setup-0.48.2/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     4129 2023-06-27 14:15:46.405828 lamindb_setup-0.48.2/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9365 2023-06-28 12:32:26.045930 lamindb_setup-0.48.2/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.48.2/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.48.2/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.48.2/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.48.2/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.48.2/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.48.2/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4812 2023-06-15 12:55:29.508183 lamindb_setup-0.48.2/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.48.2/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.48.2/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.48.2/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.48.2/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.48.2/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.48.2/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29416 2023-06-29 19:17:30.194449 lamindb_setup-0.48.2/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.48.2/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.48.2/lnschema-core/README.md
+-rw-r--r--   0        0        0      617 2023-06-30 11:14:16.252662 lamindb_setup-0.48.2/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.48.2/lnschema-core/lnschema_core/_queryset.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.48.2/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    23909 2023-06-29 19:17:30.196117 lamindb_setup-0.48.2/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      951 2023-06-29 19:17:30.196374 lamindb_setup-0.48.2/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.48.2/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.48.2/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.48.2/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.48.2/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     1821 2023-06-27 14:15:46.405994 lamindb_setup-0.48.2/noxfile.py
+-rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.48.2/pyproject.toml
+-rw-r--r--   0        0        0     1169 2023-06-27 14:15:46.406331 lamindb_setup-0.48.2/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.48.2/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.48.2/tests/hub/test_storage.py
+-rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.48.2/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-19 15:23:54.026893 lamindb_setup-0.48.2/tests/test_init_instance.py
+-rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.48.2/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.48.2/tests/test_login.py
+-rw-r--r--   0        0        0      420 2023-06-15 00:10:45.075855 lamindb_setup-0.48.2/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.48.2/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.48.2/tests/test_signup.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.48.2/PKG-INFO
```

### Comparing `lamindb_setup-0.48.1/.github/workflows/build.yml` & `lamindb_setup-0.48.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/.github/workflows/latest-changes.yml` & `lamindb_setup-0.48.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/.gitignore` & `lamindb_setup-0.48.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/.pre-commit-config.yaml` & `lamindb_setup-0.48.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/LICENSE` & `lamindb_setup-0.48.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/changelog.md` & `lamindb_setup-0.48.2/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚸 Silence loggers and close instance during init & load | [433](https://github.com/laminlabs/lamindb-setup/pull/433) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 | 0.48.2
 🐛 Fix sqlite file not existing in the bucket error | [432](https://github.com/laminlabs/lamindb-setup/pull/432) | [Koncopd](https://github.com/Koncopd) | 2023-06-28 | 0.48.1
 🩹 Do not register storage through `set.storage` on the hub | [430](https://github.com/laminlabs/lamindb-setup/pull/430) | [falexwolf](https://github.com/falexwolf) | 2023-06-28 |
 🐛 Lock cloud sqlite instances on init | [429](https://github.com/laminlabs/lamindb-setup/pull/429) | [Koncopd](https://github.com/Koncopd) | 2023-06-27 |
 👷 Add local hub tests | [427](https://github.com/laminlabs/lamindb-setup/pull/427) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 |
 ✨ Set s3 region in set.storage | [428](https://github.com/laminlabs/lamindb-setup/pull/428) | [Koncopd](https://github.com/Koncopd) | 2023-06-26 |
 ➖ Simplify deps | [426](https://github.com/laminlabs/lamindb-setup/pull/426) | [falexwolf](https://github.com/falexwolf) | 2023-06-21 |
 ✅ Try to trigger error | [424](https://github.com/laminlabs/lamindb-setup/pull/424) | [falexwolf](https://github.com/falexwolf) | 2023-06-20 | 0.47.11
```

### Comparing `lamindb_setup-0.48.1/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.48.2/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.48.2/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.48.2/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.48.2/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.48.2/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.48.2/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.48.2/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/docs/guide/setup-user.md` & `lamindb_setup-0.48.2/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/__init__.py` & `lamindb_setup-0.48.2/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.48.1"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.48.2"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.48.1/lamindb_setup/__main__.py` & `lamindb_setup-0.48.2/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.48.2/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_close.py` & `lamindb_setup-0.48.2/lamindb_setup/_close.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from lamin_logger import logger
 
 from ._settings import settings
 from .dev._settings_store import current_instance_settings_file
 from .dev._setup_bionty_sources import delete_bionty_sources_yaml
 
 
-def close() -> None:
+def close(mute: bool = False) -> None:
     """Close existing instance.
 
     Returns `None` if succeeds, otherwise an exception is raised.
     """
     if current_instance_settings_file().exists():
         instance = settings.instance.identifier
         settings.instance._update_cloud_sqlite_file()
         current_instance_settings_file().unlink()
         delete_bionty_sources_yaml()
-        logger.success(f"Closed {instance}")
+        logger.success(f"Closed instance: {instance}")
     else:
-        logger.info("No instance loaded")
+        if not mute:
+            logger.info("No instance loaded")
```

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_delete.py` & `lamindb_setup-0.48.2/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_docstrings.py` & `lamindb_setup-0.48.2/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_init_instance.py` & `lamindb_setup-0.48.2/lamindb_setup/_init_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from typing import Optional, Union
 
 from lamin_logger import logger
 from pydantic import PostgresDsn
 
 from lamindb_setup.dev.upath import UPath
 
+from ._close import close as close_instance
 from ._docstrings import instance_description as description
 from ._settings import settings
+from ._silence_loggers import silence_loggers
 from .dev import InstanceSettings
 from .dev._docs import doc_args
 from .dev._setup_schema import get_schema_module_name, load_schema
 from .dev._storage import Storage
 
 
 def register_user_and_storage(isettings: InstanceSettings, usettings):
@@ -94,14 +96,15 @@
 
     Args:
         storage: {}
         name: {}
         db: {}
         schema: {}
     """
+    close_instance(mute=True)
     from ._check_instance_setup import check_instance_setup
 
     if "lamindb" in sys.modules and check_instance_setup():
         raise RuntimeError(
             "Currently don't support init or load of multiple instances in the same"
             " Python sessionWe will bring this feature back at some point"
         )
@@ -165,14 +168,16 @@
             f"Registered instance on hub: https://lamin.ai/{owner}/{name_str}"
         )
 
     if _test:
         isettings._persist()
         return None
 
+    silence_loggers()
+
     if isettings._is_db_setup(mute=True)[0]:
         raise RuntimeError(
             "Your instance DB is already set up but couldn't be loaded, something"
             " is off"
         )
     load_from_isettings(isettings, init=True)
     if isettings._is_cloud_sqlite:
```

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_load_instance.py` & `lamindb_setup-0.48.2/lamindb_setup/_load_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
 
 from lamindb_setup.dev.upath import UPath
 
+from ._close import close as close_instance
 from ._init_instance import load_from_isettings
 from ._settings import InstanceSettings, settings
+from ._silence_loggers import silence_loggers
 from .dev._django import setup_django
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
 from .dev._storage import StorageSettings
 
 
 def load(
@@ -26,14 +28,15 @@
 
     Args:
         identifier: `str` - The instance identifier can the instance name (owner is
             current user), handle/name, or the URL: https://lamin.ai/handle/name.
         storage: `Optional[PathLike] = None` - Load the instance with an
             updated default storage.
     """
+    close_instance(mute=True)
     from ._check_instance_setup import check_instance_setup
 
     if "lamindb" in sys.modules and check_instance_setup():
         raise RuntimeError(
             "Currently don't support init or load of multiple instances in the same"
             " Python sessionWe will bring this feature back at some point"
         )
@@ -72,14 +75,16 @@
 
     if storage is not None:
         update_isettings_with_storage(isettings, storage)
     if _test:
         isettings._persist()  # this is to test the settings
         return None
 
+    silence_loggers()
+
     check, msg = isettings._is_db_setup()  # this also updates local SQLite
     if not check:
         local_db = isettings._is_cloud_sqlite and isettings._sqlite_file_local.exists()
         if local_db:
             logger.warning(
                 "SQLite file does not exist in the cloud, but exists locally. To push"
                 " the file to the cloud, call: lamin close"
```

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_migrate.py` & `lamindb_setup-0.48.2/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_notebook.py` & `lamindb_setup-0.48.2/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_register_instance.py` & `lamindb_setup-0.48.2/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_schema.py` & `lamindb_setup-0.48.2/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_set.py` & `lamindb_setup-0.48.2/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_settings.py` & `lamindb_setup-0.48.2/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_setup_user.py` & `lamindb_setup-0.48.2/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.48.2/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_django.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_hub_client.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_hub_core.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_hub_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_hub_crud.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_hub_utils.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lamindb_setup/dev/upath.py` & `lamindb_setup-0.48.2/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.48.2/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.48.2/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/.gitignore` & `lamindb_setup-0.48.2/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.48.2/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.48.2/lnschema-core/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/LICENSE` & `lamindb_setup-0.48.2/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/__init__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/_queryset.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/_queryset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/models.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.48.2/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/lnschema-core/pyproject.toml` & `lamindb_setup-0.48.2/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/noxfile.py` & `lamindb_setup-0.48.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/pyproject.toml` & `lamindb_setup-0.48.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/tests/hub/test_instance.py` & `lamindb_setup-0.48.2/tests/hub/test_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/tests/hub/test_storage.py` & `lamindb_setup-0.48.2/tests/hub/test_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/tests/test_init_instance.py` & `lamindb_setup-0.48.2/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/tests/test_load_instance.py` & `lamindb_setup-0.48.2/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.1/PKG-INFO` & `lamindb_setup-0.48.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.48.1
+Version: 0.48.2
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
 Requires-Dist: django
 Requires-Dist: dj_database_url
```

