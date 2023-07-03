# Comparing `tmp/swh.loader.git-2.5.1.tar.gz` & `tmp/swh.loader.git-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.loader.git-2.5.1.tar", last modified: Wed Jun 28 08:50:28 2023, max compression
+gzip compressed data, was "swh.loader.git-2.5.2.tar", last modified: Mon Jul  3 12:55:17 2023, max compression
```

## Comparing `swh.loader.git-2.5.1.tar` & `swh.loader.git-2.5.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.299480 swh.loader.git-2.5.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2953 2023-06-28 08:50:28.299480 swh.loader.git-2.5.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2026 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/bin/dir-git-repo-meta.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/docs/attic/
--rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/attic/api-backend-protocol.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/attic/git-loading-design.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      115 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       33 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/resources/
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/resources/local-loader-git.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/resources/remote-loader-git.ini
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/resources/test/
--rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/resources/test/back.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/resources/test/db-manager.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/resources/updater.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-28 08:50:28.299480 swh.loader.git-2.5.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2448 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.299480 swh.loader.git-2.5.1/swh/loader/git/
--rw-r--r--   0 jenkins    (115) docker     (999)      842 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9923 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2730 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8150 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/dumb.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15174 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    27520 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     1900 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.299480 swh.loader.git-2.5.1/swh/loader/git/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1331 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.299480 swh.loader.git-2.5.1/swh/loader/git/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.299480 swh.loader.git-2.5.1/swh/loader/git/tests/data/git-repos/
--rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/data/git-repos/example-submodule.bundle
--rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/data/testrepo.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5871 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/test_from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    40371 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2602 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1259 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/test_tasks_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2799 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5449 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/swh/loader/git/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-28 08:50:28.295480 swh.loader.git-2.5.1/swh.loader.git.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2953 2023-06-28 08:50:28.000000 swh.loader.git-2.5.1/swh.loader.git.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1576 2023-06-28 08:50:28.000000 swh.loader.git-2.5.1/swh.loader.git.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-28 08:50:28.000000 swh.loader.git-2.5.1/swh.loader.git.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      158 2023-06-28 08:50:28.000000 swh.loader.git-2.5.1/swh.loader.git.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      254 2023-06-28 08:50:28.000000 swh.loader.git-2.5.1/swh.loader.git.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-28 08:50:28.000000 swh.loader.git-2.5.1/swh.loader.git.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-06-28 08:50:22.000000 swh.loader.git-2.5.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.922072 swh.loader.git-2.5.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2953 2023-07-03 12:55:17.922072 swh.loader.git-2.5.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2026 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.914072 swh.loader.git-2.5.2/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/bin/dir-git-repo-meta.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.914072 swh.loader.git-2.5.2/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.914072 swh.loader.git-2.5.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.914072 swh.loader.git-2.5.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.914072 swh.loader.git-2.5.2/docs/attic/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/attic/api-backend-protocol.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/attic/git-loading-design.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      115 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       33 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.914072 swh.loader.git-2.5.2/resources/
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/resources/local-loader-git.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/resources/remote-loader-git.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.918072 swh.loader.git-2.5.2/resources/test/
+-rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/resources/test/back.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/resources/test/db-manager.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/resources/updater.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-03 12:55:17.922072 swh.loader.git-2.5.2/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2448 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.918072 swh.loader.git-2.5.2/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.918072 swh.loader.git-2.5.2/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.918072 swh.loader.git-2.5.2/swh/loader/git/
+-rw-r--r--   0 jenkins    (115) docker     (999)      842 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9923 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2730 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8150 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/dumb.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15174 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    27722 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     1900 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.922072 swh.loader.git-2.5.2/swh/loader/git/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1331 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.922072 swh.loader.git-2.5.2/swh/loader/git/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.922072 swh.loader.git-2.5.2/swh/loader/git/tests/data/git-repos/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/data/git-repos/example-submodule.bundle
+-rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/data/testrepo.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5871 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/test_from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    40517 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2602 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1259 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/test_tasks_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2799 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5449 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/swh/loader/git/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-03 12:55:17.918072 swh.loader.git-2.5.2/swh.loader.git.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2953 2023-07-03 12:55:17.000000 swh.loader.git-2.5.2/swh.loader.git.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1576 2023-07-03 12:55:17.000000 swh.loader.git-2.5.2/swh.loader.git.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-03 12:55:17.000000 swh.loader.git-2.5.2/swh.loader.git.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      158 2023-07-03 12:55:17.000000 swh.loader.git-2.5.2/swh.loader.git.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      254 2023-07-03 12:55:17.000000 swh.loader.git-2.5.2/swh.loader.git.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-03 12:55:17.000000 swh.loader.git-2.5.2/swh.loader.git.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-07-03 12:55:12.000000 swh.loader.git-2.5.2/tox.ini
```

### Comparing `swh.loader.git-2.5.1/.pre-commit-config.yaml` & `swh.loader.git-2.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/CODE_OF_CONDUCT.md` & `swh.loader.git-2.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/LICENSE` & `swh.loader.git-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/PKG-INFO` & `swh.loader.git-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.5.1
+Version: 2.5.2
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
```

### Comparing `swh.loader.git-2.5.1/README.md` & `swh.loader.git-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/bin/dir-git-repo-meta.sh` & `swh.loader.git-2.5.2/bin/dir-git-repo-meta.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/conftest.py` & `swh.loader.git-2.5.2/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/docs/attic/api-backend-protocol.txt` & `swh.loader.git-2.5.2/docs/attic/api-backend-protocol.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/docs/attic/git-loading-design.txt` & `swh.loader.git-2.5.2/docs/attic/git-loading-design.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/setup.py` & `swh.loader.git-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/__init__.py` & `swh.loader.git-2.5.2/swh/loader/git/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/base.py` & `swh.loader.git-2.5.2/swh/loader/git/base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/converters.py` & `swh.loader.git-2.5.2/swh/loader/git/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/directory.py` & `swh.loader.git-2.5.2/swh/loader/git/directory.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/dumb.py` & `swh.loader.git-2.5.2/swh/loader/git/dumb.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/from_disk.py` & `swh.loader.git-2.5.2/swh/loader/git/from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/loader.py` & `swh.loader.git-2.5.2/swh/loader/git/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 import dulwich.client
 from dulwich.object_store import ObjectStoreGraphWalker
 from dulwich.objects import Blob, Commit, ShaFile, Tag, Tree
 from dulwich.pack import PackData, PackInflater
 
 from swh.core.statsd import Statsd
+from swh.loader.exception import NotFound
 from swh.loader.git.utils import raise_not_found_repository
 from swh.model import hashutil
 from swh.model.git_objects import (
     content_git_object,
     directory_git_object,
     release_git_object,
     revision_git_object,
@@ -344,14 +345,18 @@
             sys.stderr.flush()
 
         try:
             with raise_not_found_repository():
                 fetch_info = self.fetch_pack_from_origin(
                     self.origin.url, base_repo, do_progress
                 )
+        except NotFound:
+            # NotFound inherits from ValueError and should not be caught
+            # by the next exception handler
+            raise
         except (AttributeError, NotImplementedError, ValueError):
             # with old dulwich versions, those exceptions types can be raised
             # by the fetch_pack operation when encountering a repository with
             # dumb transfer protocol so we check if the repository supports it
             # here to continue the loading if it is the case
             self.dumb = dumb.check_protocol(self.origin.url)
             if not self.dumb:
```

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tasks.py` & `swh.loader.git-2.5.2/swh/loader/git/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/conftest.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/data/git-repos/example-submodule.bundle` & `swh.loader.git-2.5.2/swh/loader/git/tests/data/git-repos/example-submodule.bundle`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/data/testrepo.tgz` & `swh.loader.git-2.5.2/swh/loader/git/tests/data/testrepo.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/test_converters.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/test_directory.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/test_from_disk.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/test_from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/test_loader.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/test_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import attr
 from dulwich.errors import GitProtocolError, NotGitRepository, ObjectFormatException
 from dulwich.pack import REF_DELTA
 from dulwich.porcelain import push
 import dulwich.repo
 from dulwich.tests.utils import build_pack
 import pytest
+from requests import HTTPError
 
 from swh.loader.git import converters, dumb
 from swh.loader.git.loader import FetchPackReturn, GitLoader
 from swh.loader.git.tests.test_from_disk import SNAPSHOT1, FullGitLoaderTests
 from swh.loader.tests import (
     assert_last_visit_matches,
     get_stats,
@@ -61,18 +62,21 @@
             GitProtocolError("unexpected http resp 410"),
             NotGitRepository("not a git repo"),
         ],
     )
     def test_load_visit_not_found(self, failure_exception):
         """Ingesting an unknown url result in a visit with not_found status"""
         # simulate an initial communication error (e.g no repository found, ...)
-        mock = self.mocker.patch(
+        self.mocker.patch(
             "swh.loader.git.loader.GitLoader.fetch_pack_from_origin"
-        )
-        mock.side_effect = failure_exception
+        ).side_effect = failure_exception
+
+        self.mocker.patch(
+            "swh.loader.git.loader.dumb.check_protocol"
+        ).side_effect = HTTPError("404 not found")
 
         res = self.loader.load()
         assert res == {"status": "uneventful"}
 
         assert_last_visit_matches(
             self.loader.storage,
             self.repo_url,
```

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/test_tasks.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/test_tasks_directory.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/test_tasks_directory.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/tests/test_utils.py` & `swh.loader.git-2.5.2/swh/loader/git/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh/loader/git/utils.py` & `swh.loader.git-2.5.2/swh/loader/git/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/swh.loader.git.egg-info/PKG-INFO` & `swh.loader.git-2.5.2/swh.loader.git.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.5.1
+Version: 2.5.2
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
```

### Comparing `swh.loader.git-2.5.1/swh.loader.git.egg-info/SOURCES.txt` & `swh.loader.git-2.5.2/swh.loader.git.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.5.1/tox.ini` & `swh.loader.git-2.5.2/tox.ini`

 * *Files identical despite different names*

