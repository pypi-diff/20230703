# Comparing `tmp/pythonic-dbm-0.4.0.tar.gz` & `tmp/pythonic-dbm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonic-dbm-0.4.0.tar", last modified: Thu Dec 22 21:41:50 2022, max compression
+gzip compressed data, was "pythonic-dbm-0.5.0.tar", last modified: Mon Jul  3 18:12:27 2023, max compression
```

## Comparing `pythonic-dbm-0.4.0.tar` & `pythonic-dbm-0.5.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.490036 pythonic-dbm-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      282 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2022-12-22 21:41:50.490036 pythonic-dbm-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/docs/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.478035 pythonic-dbm-0.4.0/docs/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/docs/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18280 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/overrides/assets/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/tutorial/field-types.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/tutorial/model-config.md
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/tutorial/models.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/docs/tutorial/validators.md
--rw-r--r--   0 runner    (1001) docker     (123)      667 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2022-12-22 21:41:50.490036 pythonic-dbm-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.478035 pythonic-dbm-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/src/pydbm/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/src/pydbm/database/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/src/pydbm/database/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/database/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/database/data_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/database/data_types/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/inspect_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.482035 pythonic-dbm-0.4.0/src/pydbm/models/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.486035 pythonic-dbm-0.4.0/src/pydbm/models/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/fields/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.486035 pythonic-dbm-0.4.0/src/pydbm/models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/validators/builtin_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/models/validators/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/src/pydbm/typing_extra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.486035 pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2022-12-22 21:41:50.000000 pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2022-12-22 21:41:50.000000 pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 21:41:50.000000 pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-22 21:41:50.000000 pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-22 21:41:50.000000 pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 21:41:50.000000 pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.486035 pythonic-dbm-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.486035 pythonic-dbm-0.4.0/tests/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/database/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.486035 pythonic-dbm-0.4.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.490036 pythonic-dbm-0.4.0/tests/models/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/fields/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/fields/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/fields/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/fields/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/fields/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:50.490036 pythonic-dbm-0.4.0/tests/models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/validators/test_builtin_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/models/validators/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/test_inspect_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-22 21:41:39.000000 pythonic-dbm-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.723841 pythonic-dbm-0.5.0/docs/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/overrides/assets/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/field-types.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/model-config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/docs/tutorial/validators.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.723841 pythonic-dbm-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/database/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/data_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/data_types/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/inspect_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/fields/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.727841 pythonic-dbm-0.5.0/src/pydbm/models/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/validators/builtin_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/models/validators/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/src/pydbm/typing_extra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:12:27.000000 pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/database/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/fields/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:27.731841 pythonic-dbm-0.5.0/tests/models/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/validators/test_builtin_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/models/validators/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/test_inspect_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 18:12:16.000000 pythonic-dbm-0.5.0/tox.ini
```

### Comparing `pythonic-dbm-0.4.0/.gitignore` & `pythonic-dbm-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/.pre-commit-config.yaml` & `pythonic-dbm-0.5.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Install the git hook scripts, run `$ pre-commit install` to set up the git hook scripts
 # Run against all the files, `$ pre-commit run --all-files`
 # Updating hooks automatically: `$ pre-commit autoupdate`
 
 repos:
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/hakancelikdev/unimport
-    rev: 0.12.2
+    rev: 0.16.0
     hooks:
       - id: unimport
         args:
           - --remove
           - --include-star-import
           - --gitignore
 
@@ -22,21 +22,21 @@
     hooks:
       - id: unexport
         exclude: "tests/|__init__.py"
         args:
           - --refactor
 
   - repo: https://github.com/myint/docformatter
-    rev: v1.5.0
+    rev: v1.6.5
     hooks:
       - id: docformatter
         args: [--in-place]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.3.0
     hooks:
       - id: mypy
         args: [--no-strict-optional, --ignore-missing-imports, --show-error-codes]
         additional_dependencies: [types-toml==0.1.3]
         exclude: "tests/"
 
   - repo: https://github.com/pycqa/flake8
```

### Comparing `pythonic-dbm-0.4.0/LICENSE` & `pythonic-dbm-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/PKG-INFO` & `pythonic-dbm-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonic-dbm
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pydbm is a more pythonic way to use dbm.
 Home-page: https://pydbm.hakancelik.dev/
 Author: Hakan Celik
 Author-email: hakancelikdev@gmail.com
 License: GPL-3.0
 Project-URL: Documentation, https://pydbm.hakancelik.dev/
 Project-URL: Issues, https://github.com/hakancelikdev/pydbm/issues/
```

### Comparing `pythonic-dbm-0.4.0/README.md` & `pythonic-dbm-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/docs/CONTRIBUTING.md` & `pythonic-dbm-0.5.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/docs/index.md` & `pythonic-dbm-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/docs/overrides/assets/images/logo.png` & `pythonic-dbm-0.5.0/docs/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/docs/overrides/main.html` & `pythonic-dbm-0.5.0/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/docs/tutorial/field-types.md` & `pythonic-dbm-0.5.0/docs/tutorial/field-types.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/docs/tutorial/models.md` & `pythonic-dbm-0.5.0/docs/tutorial/models.md`

 * *Files 5% similar despite different names*

```diff
@@ -133,16 +133,27 @@
 ### Save
 Save method is used to save the valid data to the database.
 
 ```python
 user = UserModel(username="hakancelik")
 user.save()
 ```
-That's it, now we have saved our user to the database.
+That's it, now we have saved our user to the database. In addition If you wish, you can update any field belonging
+to the instance and then have it updated in your database.
 
+```python
+user = UserModel(username="hakan")
+user.save()  # save user to database for the first time
+
+user.username="hakancelik"
+user.save()  # update username field
+```
+
+UserModel.objects.get(pk=user.pk) == UserModel(username="hakancelik")
+```
 
 ### Get
 Get method is used to get the data from the database and return it as a model instance.
 
 ```python
 try:
     user = UserModel.objects.get(user.id)
```

### Comparing `pythonic-dbm-0.4.0/docs/tutorial/validators.md` & `pythonic-dbm-0.5.0/docs/tutorial/validators.md`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/pyproject.toml` & `pythonic-dbm-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
 
 [tool.unimport]
 remove = true
-include_start_import = true
+include_star_import = true
 ignore_init = true
 
 [tool.docformatter]
 recursive = true
 wrap-summaries = 79
 wrap-descriptions = 79
 blank = true
```

### Comparing `pythonic-dbm-0.4.0/setup.cfg` & `pythonic-dbm-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pythonic-dbm
-version = 0.4.0
+version = 0.5.0
 url = https://pydbm.hakancelik.dev/
 author = Hakan Celik
 author_email = hakancelikdev@gmail.com
 description = Pydbm is a more pythonic way to use dbm.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPL-3.0
```

### Comparing `pythonic-dbm-0.4.0/src/pydbm/__init__.py` & `pythonic-dbm-0.5.0/src/pydbm/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/database/data_types/base.py` & `pythonic-dbm-0.5.0/src/pydbm/database/data_types/base.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/database/data_types/types.py` & `pythonic-dbm-0.5.0/src/pydbm/database/data_types/types.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/database/manager.py` & `pythonic-dbm-0.5.0/src/pydbm/database/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,79 +11,80 @@
 
 if typing.TYPE_CHECKING:
     from pydbm import DbmModel
     from pydbm.typing_extra import SupportedClassT
 
 
 __all__ = (
+    "DATABASE_EXTENSION",
+    "DATABASE_HEADER_MAPPING",
+    "DATABASE_HEADER_NAME",
+    "DATABASE_PATH",
     "DatabaseManager",
 )
 
 Self = typing.TypeVar("Self", bound="DatabaseManager")  # unexport: not-public
 
+DATABASE_HEADER_NAME: str = "__database_headers__"
+DATABASE_HEADER_MAPPING: dict[SupportedClassT, str] = {
+    bool: "bool",
+    bytes: "bytes",
+    datetime.date: "date",
+    datetime.datetime: "datetime",
+    float: "float",
+    int: "int",
+    None: "null",
+    str: "str",
+}
+DATABASE_EXTENSION: str = "pydbm"
+DATABASE_PATH: Path = Path("pydbm")  # TODO: take from env
+
 
 class DatabaseManager:
     if typing.TYPE_CHECKING:
         __database_headers__: dict[str, SupportedClassT]  # TODO: make this more generic
 
-    __header_name__: typing.ClassVar[str] = "__database_headers__"
-    __header_mapping__: dict[SupportedClassT, str] = {
-        bool: "bool",
-        bytes: "bytes",
-        datetime.date: "date",
-        datetime.datetime: "datetime",
-        float: "float",
-        int: "int",
-        None: "null",
-        str: "str",
-    }
-
     __slots__ = (
         "model",
         "table_name",
         "db_path",
-
         "db",
-        __header_name__,
-
+        DATABASE_HEADER_NAME,
         "__key",
     )
 
-    database_path: typing.ClassVar[Path] = Path("pydbm")  # TODO: take from env
-
     def __init__(self, *, model: typing.Type[DbmModel], table_name: str) -> None:  # TODO: table_name -> db_name
         self.model = model
         self.table_name = table_name
 
-        self.db_path = self.database_path / f"{self.table_name}.db"
+        self.db_path = DATABASE_PATH / f"{self.table_name}.{DATABASE_EXTENSION}"
 
         ann = get_obj_annotations(obj=model)
-        db_headers = bytes(str({key: self.__class__.__header_mapping__[value] for key, value in ann.items()}), "utf-8")
+        db_headers = bytes(str({key: DATABASE_HEADER_MAPPING[value] for key, value in ann.items()}), "utf-8")
 
         db = self.open()
-        first_key: bytes | None = db.firstkey()
-        if first_key is None:
-            db[self.__class__.__header_name__] = db_headers
+        database_header: bytes | None
+        if (database_header := db.get(DATABASE_HEADER_NAME, None)) is None:
+            db[DATABASE_HEADER_NAME] = db_headers
         else:
-            assert first_key == self.__class__.__header_name__.encode(), f"First key is not {self.__class__.__header_name__}"  # noqa: E501
             # TODO: migrations
-            assert db[first_key] == db_headers, f"Database headers are not equal: '{db[self.__class__.__header_name__]}' != '{db_headers}'"  # type: ignore[str-bytes-safe]  # noqa: E501
+            assert database_header == db_headers, f"Database headers are not equal: '{database_header}' != '{db_headers}'"  # type: ignore[str-bytes-safe]  # noqa: E501
         db.close()
 
-        setattr(self, self.__class__.__header_name__, ann)
+        setattr(self, DATABASE_HEADER_NAME, ann)
 
     def __enter__(self, *args, **kwargs):
         return self.open()
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
     def __len__(self) -> int:
         with self as db:
-            return len(db)
+            return len(db) - 1  # NOTE: subtract 1 for the database header
 
     def __getitem__(self, pk: str) -> DbmModel:
         return self.get(pk=pk)
 
     def __setitem__(self, pk: str, fields: dict[str, typing.Any]) -> None:
         self.save(pk=pk, fields=fields)
 
@@ -91,15 +92,15 @@
         self.delete(pk=pk)
 
     def __contains__(self, pk: str) -> bool:
         with self as db:
             return pk in db
 
     def __iter__(self: Self) -> Self:
-        self.__key: bytes = self.__class__.__header_name__.encode()  # NOTE: this is the first key in the database
+        self.__key: bytes = DATABASE_HEADER_NAME.encode()  # NOTE: this is the first key in the database
         return self
 
     def __next__(self) -> str:
         with self as db:
             self.__key: bytes | None = db.nextkey(self.__key)  # type: ignore
 
         if self.__key is not None:
@@ -108,15 +109,15 @@
             del self.__key
             raise StopIteration
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(model={self.model!r}, table_name={self.table_name!r})"
 
     def open(self):
-        Path(self.database_path).mkdir(parents=True, exist_ok=True)
+        Path(DATABASE_PATH).mkdir(parents=True, exist_ok=True)
 
         self.db = dbm.open(self.db_path.as_posix(), "c")
         return self.db
 
     def close(self):
         self.db.close()
         del self.db
@@ -171,7 +172,10 @@
             yield self.get(pk=key)
 
     def filter(self, **kwargs) -> typing.Iterable[DbmModel]:
         def check(model: DbmModel) -> bool:
             return all(model.fields[key] == value for key, value in kwargs.items())
 
         yield from filter(check, self.all())
+
+    def count(self):
+        return len(self)
```

### Comparing `pythonic-dbm-0.4.0/src/pydbm/exceptions.py` & `pythonic-dbm-0.5.0/src/pydbm/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# TODO: Add to docs.
 import typing
 
 __all__ = (
     "PydbmBaseException",
     "PydbmTypeError",
     "ValidationError",
+    "EmptyModelError",
+    "UnnecessaryParamsError",
 )
 
 
 class PydbmBaseException(Exception):
     """Base exception for pydbm models."""
 
     pass
@@ -15,17 +18,29 @@
 
 class PydbmTypeError(PydbmBaseException, TypeError):
     """Exception for not valid type of value."""
 
     pass
 
 
-class ValidationError(PydbmBaseException):
+class ValidationError(PydbmBaseException, ValueError):
     """Exception for not valid value."""
 
     def __init__(self, field_name: str, field_value: typing.Any, error: ValueError) -> None:
         self.field_name = field_name
         self.field_value = field_value
         self.error = error
 
     def __str__(self) -> str:
         return f"Invalid value for {self.field_name}={self.field_value!r}; {self.error}."
+
+
+class EmptyModelError(PydbmBaseException):
+    """Exception for empty model."""
+
+    pass
+
+
+class UnnecessaryParamsError(PydbmBaseException, ValueError):
+    """Exception for invalid params."""
+
+    pass
```

### Comparing `pythonic-dbm-0.4.0/src/pydbm/inspect_extra.py` & `pythonic-dbm-0.5.0/src/pydbm/inspect_extra.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/logging.py` & `pythonic-dbm-0.5.0/src/pydbm/logging.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/__init__.py` & `pythonic-dbm-0.5.0/src/pydbm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/base.py` & `pythonic-dbm-0.5.0/src/pydbm/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,46 +10,49 @@
 )
 
 
 class DbmModel(metaclass=Meta):
     if typing.TYPE_CHECKING:
         required_fields: typing.ClassVar[list[str]]
         objects: typing.ClassVar[DatabaseManager]
-        pk: str
+        pk: typing.ClassVar[str]
         id: str
+        empty_model: typing.ClassVar[bool]
 
     def __init__(self, **fields: typing.Any) -> None:
         self.id = fields.pop("pk")
-
         self.fields: dict[str, typing.Any] = fields
 
         for key, value in fields.items():
             setattr(self, key, value)
 
+    def __repr__(self):
+        kwargs = ", ".join(f"{key}={getattr(self, key)!r}" for key in self.fields)
+        return f"{type(self).__name__}({kwargs})"
+
+    def __eq__(self, other):
+        if isinstance(other, type(self)):
+            return self.fields == other.fields and self.pk == other.pk
+        return False
+
+    def __hash__(self):
+        if self.pk is None:
+            raise TypeError("Model instances without primary key value are unhashable")
+        return hash(self.pk)
+
+    def __len__(self):
+        return self.objects.count()  # type: ignore
+
     def save(self) -> None:
         self.objects.save(pk=self.pk, fields=self.fields)
 
     def update(self, **updated_fields) -> None:
         for field_name, field_value in updated_fields.items():
             setattr(self, field_name, field_value)
 
         self.objects.update(pk=self.pk, **updated_fields)
 
     def delete(self) -> None:
         self.objects.delete(pk=self.pk)
 
     def as_dict(self) -> dict[str, typing.Any]:
         return self.fields
-
-    def __repr__(self):
-        kwargs = ", ".join(f"{key}={getattr(self, key)!r}" for key in self.fields)
-        return f"{type(self).__name__}({kwargs})"
-
-    def __eq__(self, other):
-        if isinstance(other, type(self)):
-            return self.fields == other.fields and self.pk == other.pk
-        return False
-
-    def __hash__(self):
-        if self.pk is None:
-            raise TypeError("Model instances without primary key value are unhashable")
-        return hash(self.pk)
```

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/fields/auto.py` & `pythonic-dbm-0.5.0/src/pydbm/models/fields/auto.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,18 +36,24 @@
     def __get__(self, instance: Meta, owner: DbmModel) -> typing.Any:
         return self.get_default_value()
 
     def __set__(self, instance: DbmModel, value: typing.Any) -> None:
         raise AttributeError("AutoField is read-only")
 
     def __call__(self: Self, fields: dict[str, typing.Any] | None = None, *args, **kwargs) -> Self:  # type: ignore[valid-type, override]  # noqa: E501
-        if self.unique_together and not fields:
+        if fields is not None:
+            _fields = fields.copy()
+            _fields.pop("pk", None)
+        else:
+            _fields = None
+
+        if self.unique_together and not _fields:
             raise ValueError("unique_together ise set, fields must be passed")
 
-        self.fields = fields
+        self.fields = _fields
         return super().__call__(self.field_name, self.field_type, *args, **kwargs)  # type: ignore
 
     def generate_pk(self) -> str:
         if self.unique_together and self._is_call_run:
             text = "*".join(map(str, (attr for name in self.unique_together if (attr := self.fields.get(name, None)))))
             return hashlib.md5(bytes(text, "utf-8")).hexdigest()
         else:
```

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/fields/base.py` & `pythonic-dbm-0.5.0/src/pydbm/models/fields/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,18 @@
         else:
             if self.min_value or self.max_value:
                 logger.warning(
                     "min_value and max_value are only valid for int type. "
                     f"They are ignored for {value.__class__.__name__} type."
                 )
 
-        normalize_and_validate_value = self.before_set(value)
-        setattr(instance, self.private_name, normalize_and_validate_value)
+        eligible_value = self.before_set(value)
+
+        setattr(instance, self.private_name, eligible_value)
+        instance.fields[self.field_name] = eligible_value
 
     def __call__(self: Self, field_name: str, field_type: SupportedClassT, *args, **kwargs) -> Self:  # type: ignore[valid-type]  # noqa: E501
         self._is_call_run = True
 
         self.field_name = field_name
         self.field_type = field_type
```

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/meta.py` & `pythonic-dbm-0.5.0/src/pydbm/models/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing
 
 from pydbm import typing_extra
 from pydbm.database import DatabaseManager
-from pydbm.exceptions import PydbmBaseException
+from pydbm.exceptions import EmptyModelError, PydbmBaseException, UnnecessaryParamsError
 from pydbm.inspect_extra import get_obj_annotations
 from pydbm.models.fields import AutoField, Field, Undefined
 
 __all__ = (
     "Meta",
 )
 
@@ -24,41 +24,50 @@
 
 
 @typing_extra.dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
 class Meta(type):
     if typing.TYPE_CHECKING:
         not_required_fields: list[Field | AutoField]
         required_fields: list[str]
-        database: DatabaseManager
+        objects: DatabaseManager
+        DoesNotExists: typing.Type[PydbmBaseException]
 
     @staticmethod
     def __new__(mcs, cls_name: str, bases: tuple[Meta, ...], namespace: dict[str, typing.Any], **kwargs: typing.Any) -> type:  # noqa: E501
         if not [b for b in bases if isinstance(b, mcs)]:
             namespace["__slots__"] = mcs.generate_slots(namespace) + ("fields", "id")
             return super().__new__(mcs, cls_name, bases, namespace)
-
-        namespace["__slots__"] = mcs.generate_slots(namespace) + ("database",)
-        return super().__new__(mcs, cls_name, bases, namespace)
+        else:
+            if "__annotations__" in namespace:
+                namespace["__annotations__"]["pk"] = str
+            namespace["__slots__"] = mcs.generate_slots(namespace) + ("database",)
+            return super().__new__(mcs, cls_name, bases, namespace)
 
     def __init__(cls, cls_name: str, bases: tuple[Meta, ...], namespace: dict[str, typing.Any], **kwargs: typing.Any) -> None:  # noqa: E501
         super().__init__(cls_name, bases, namespace, **kwargs)
         if [b for b in bases if isinstance(b, type(cls))]:
+            if not namespace.get("__annotations__", {}):
+                raise EmptyModelError("Empty model is not allowed.")
+
             mcs = type(cls)
 
             config = mcs.get_config(cls_name, namespace)
             fields = mcs.generate_fields(cls, cls_name, namespace)
 
             cls.required_fields, cls.not_required_fields = mcs.split_fields(list(fields.values()))
             cls.objects = DatabaseManager(model=cls, table_name=config.table_name)  # type: ignore
-            cls.DoesNotExists = type("DoesNotExists", (PydbmBaseException,), {"__doc__": "Exception for not found id in the models."})  # noqa: E501
+            cls.DoesNotExists = type("DoesNotExists", (PydbmBaseException,), {"__doc__": "Exception for not found id in the models."})  # type: ignore # noqa: E501
 
             for key, value in fields.items():
                 setattr(cls, key, value)
 
     def __call__(cls, **kwargs):
+        for extra_field_name in (set(kwargs.keys()) - set(cls.__annotations__.keys())):
+            raise UnnecessaryParamsError(f"{extra_field_name} is not defined in {cls.__name__}")
+
         for field in cls.not_required_fields:
             if field.public_name not in kwargs and field.public_name != PRIMARY_KEY:
                 kwargs[field.public_name] = field.get_default_value()  # type: ignore[attr-defined]  # noqa: E501
 
         for field in cls.required_fields:  # type: ignore[assignment]
             if field not in kwargs:
                 raise ValueError(f"{field} is required")
```

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/validators/__init__.py` & `pythonic-dbm-0.5.0/src/pydbm/models/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/validators/builtin_types.py` & `pythonic-dbm-0.5.0/src/pydbm/models/validators/builtin_types.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/models/validators/compare.py` & `pythonic-dbm-0.5.0/src/pydbm/models/validators/compare.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pydbm/typing_extra.py` & `pythonic-dbm-0.5.0/src/pydbm/typing_extra.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/PKG-INFO` & `pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonic-dbm
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pydbm is a more pythonic way to use dbm.
 Home-page: https://pydbm.hakancelik.dev/
 Author: Hakan Celik
 Author-email: hakancelikdev@gmail.com
 License: GPL-3.0
 Project-URL: Documentation, https://pydbm.hakancelik.dev/
 Project-URL: Issues, https://github.com/hakancelikdev/pydbm/issues/
```

### Comparing `pythonic-dbm-0.4.0/src/pythonic_dbm.egg-info/SOURCES.txt` & `pythonic-dbm-0.5.0/src/pythonic_dbm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/database/test_manager.py` & `pythonic-dbm-0.5.0/tests/database/test_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         },
     )
     return minimum_manager.objects
 
 
 def test_init(minimum_manager):
     assert minimum_manager.table_name == "minimum_managers"
-    assert minimum_manager.db_path.as_posix() == "pydbm/minimum_managers.db"
+    assert minimum_manager.db_path.as_posix() == "pydbm/minimum_managers.pydbm"
 
 
 def test_context_manager(minimum_manager):
     assert hasattr(minimum_manager, "__enter__")
     assert hasattr(minimum_manager, "__exit__")
 
 
@@ -35,20 +35,20 @@
 
     with pytest.raises(dbm.error) as cm:
         db["test"] = {}
     assert str(cm.value) == "GDBM object has already been closed"
 
 
 def test__database_headers__minimum_manager(minimum_manager):
-    assert len(minimum_manager) == 1
-    assert minimum_manager.__database_headers__ == {"str": str}
+    assert len(minimum_manager) == 0
+    assert minimum_manager.__database_headers__ == {"pk": str, "str": str}
 
     with minimum_manager as db:
         assert "__database_headers__" in db
-        assert db["__database_headers__"] == b"{'str': 'str'}"
+        assert db["__database_headers__"] == b"{'str': 'str', 'pk': 'str'}"
 
 
 @pytest.mark.parametrize("annotations", [
     {
         "bool": bool,
         "bytes": bytes,
         "date": datetime.date,
@@ -70,31 +70,31 @@
     },
 ])
 def test__database_headers__maximum_manager(annotations):
     class MaximumManager(DbmModel):
         __annotations__ = annotations
 
     objects = MaximumManager.objects
-
-    assert len(objects) == 1
+    assert len(objects) == 0
     assert objects.__database_headers__ == {
+        "pk": str,
         "bool": bool,
         "bytes": bytes,
         "date": datetime.date,
         "datetime": datetime.datetime,
         "float": float,
         "int": int,
         "none": None,
         "str": str,
     }
 
     with objects as db:
         assert "__database_headers__" in db
         assert (
-            b"{'bool': 'bool', 'bytes': 'bytes', 'date': 'date', 'datetime': 'datetime', 'float': 'float', 'int': 'int', 'none': 'null', 'str': 'str'}"  # noqa: E501
+            b"{'bool': 'bool', 'bytes': 'bytes', 'date': 'date', 'datetime': 'datetime', 'float': 'float', 'int': 'int', 'none': 'null', 'str': 'str', 'pk': 'str'}"  # noqa: E501
             == db["__database_headers__"]
         )
 
 
 @pytest.mark.parametrize(
     "field_type, expected_field_type, field_value",
     [
@@ -118,31 +118,34 @@
         ("str", str, "test"),
     ],
 )
 def test_save_get_delete(teardown_db, field_type, expected_field_type, field_value):
     class SaveGetDeleteTestModel(DbmModel):
         __annotations__ = {"field": field_type}
 
-    assert SaveGetDeleteTestModel.objects.__database_headers__ == {"field": expected_field_type}
+    assert SaveGetDeleteTestModel.objects.__database_headers__ == {
+        "pk": str,
+        "field": expected_field_type
+    }
 
     # save
-    assert len(SaveGetDeleteTestModel.objects) == 1
+    assert len(SaveGetDeleteTestModel.objects) == 0
     pk = SaveGetDeleteTestModel(field=field_value).pk
     SaveGetDeleteTestModel.objects.save(pk=pk, fields={"field": field_value})
-    assert len(SaveGetDeleteTestModel.objects) == 2
+    assert len(SaveGetDeleteTestModel.objects) == 1
 
     # get
     _model = SaveGetDeleteTestModel.objects.get(pk=pk)
     assert _model.field == field_value
     assert _model.pk == pk
     assert _model.id == pk
 
     # delete
     SaveGetDeleteTestModel.objects.delete(pk=pk)
-    assert len(SaveGetDeleteTestModel.objects) == 1
+    assert len(SaveGetDeleteTestModel.objects) == 0
 
 
 @pytest.mark.parametrize(
     "field_type, expected_field_type, field_value, updated_value",
     [
         (bool, bool, True, False),
         (bool, bool, False, True),
@@ -164,30 +167,30 @@
         ("str", str, "test", "new-value"),
     ],
 )
 def test_create_update(teardown_db, field_type, expected_field_type, field_value, updated_value):
     class CreateUpdateTestModel(DbmModel):
         __annotations__ = {"field": field_type}
 
-    assert CreateUpdateTestModel.objects.__database_headers__ == {"field": expected_field_type}
+    assert CreateUpdateTestModel.objects.__database_headers__ == {"pk": str, "field": expected_field_type}
 
     # create
-    assert len(CreateUpdateTestModel.objects) == 1
+    assert len(CreateUpdateTestModel.objects) == 0
     _model = CreateUpdateTestModel.objects.create(field=field_value)
-    assert len(CreateUpdateTestModel.objects) == 2
+    assert len(CreateUpdateTestModel.objects) == 1
     assert _model.field == field_value
 
     pk = _model.pk
 
     # get
     assert CreateUpdateTestModel.objects.get(pk=pk).field == field_value
 
     # update
     CreateUpdateTestModel.objects.update(pk=pk, field=updated_value)
-    assert len(CreateUpdateTestModel.objects) == 2
+    assert len(CreateUpdateTestModel.objects) == 1
 
     # get
     assert CreateUpdateTestModel.objects.get(pk=pk).field == updated_value
 
     # delete
     CreateUpdateTestModel.objects.delete(pk=pk)
-    assert len(CreateUpdateTestModel.objects) == 1
+    assert len(CreateUpdateTestModel.objects) == 0
```

### Comparing `pythonic-dbm-0.4.0/tests/models/fields/test_auto.py` & `pythonic-dbm-0.5.0/tests/models/fields/test_auto.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/models/fields/test_base.py` & `pythonic-dbm-0.5.0/tests/models/fields/test_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     assert field.validators == []
 
 
 def test_base_set_attr():
     class Model:
         field = Field()("field", str)
 
+        def __init__(self):
+            self.fields = {}
+
     model = Model()
 
     model.field = "value"  # set
     assert model.field == "value"  # get
 
 
 def test_base_is_required():
```

### Comparing `pythonic-dbm-0.4.0/tests/models/fields/test_bool.py` & `pythonic-dbm-0.5.0/tests/models/fields/test_bool.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/models/fields/test_date.py` & `pythonic-dbm-0.5.0/tests/models/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/models/fields/test_numeric.py` & `pythonic-dbm-0.5.0/tests/models/fields/test_numeric.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/models/fields/test_sequence.py` & `pythonic-dbm-0.5.0/tests/models/fields/test_sequence.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/models/test_meta.py` & `pythonic-dbm-0.5.0/tests/models/test_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import datetime
 
 import pytest
 
-from pydbm import exceptions
+from pydbm import DbmModel, exceptions
 from pydbm.models import meta
 from pydbm.models.fields import AutoField
 
 
-class DbmModel(metaclass=meta.Meta):
-    def __init__(self, **kwargs):
-        kwargs.pop("pk")
-        for name, value in kwargs.items():
-            setattr(self, name, value)
-
-
 def test_generate_table_name():
     assert meta.Meta.generate_table_name("User") == "users"
     assert meta.Meta.generate_table_name("UserModel") == "usermodels"
 
 
 def test_config():
     config = meta.Config(table_name="users", unique_together=("email", "username"))
@@ -119,7 +112,18 @@
         "str": "str",
     }
     model_body.update(updated_fields)
 
     with pytest.raises(exceptions.ValidationError) as cm:
         Model(**model_body)
     assert str(cm.value) == expected_error_ms
+
+
+def test_meta_unnecessary_params_error():
+    class TestModel(DbmModel):
+        email: str
+        username: str
+
+    with pytest.raises(exceptions.UnnecessaryParamsError) as cm:
+        TestModel(email="email", username="username", extra_field="test")
+
+    assert cm.value.args == ("extra_field is not defined in TestModel",)
```

### Comparing `pythonic-dbm-0.4.0/tests/models/validators/test_builtin_types.py` & `pythonic-dbm-0.5.0/tests/models/validators/test_builtin_types.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/models/validators/test_compare.py` & `pythonic-dbm-0.5.0/tests/models/validators/test_compare.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/test_exception.py` & `pythonic-dbm-0.5.0/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/test_inspect_extra.py` & `pythonic-dbm-0.5.0/tests/test_inspect_extra.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tests/test_logging.py` & `pythonic-dbm-0.5.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pythonic-dbm-0.4.0/tox.ini` & `pythonic-dbm-0.5.0/tox.ini`

 * *Files identical despite different names*

