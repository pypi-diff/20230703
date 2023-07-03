# Comparing `tmp/bomf-0.5.9.tar.gz` & `tmp/bomf-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.5.9.tar", last modified: Fri Jun  9 13:21:33 2023, max compression
+gzip compressed data, was "bomf-0.6.0.tar", last modified: Mon Jul  3 13:11:25 2023, max compression
```

## Comparing `bomf-0.5.9.tar` & `bomf-0.6.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-09 13:21:25.000000 bomf-0.5.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-09 13:21:25.000000 bomf-0.5.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-09 13:21:25.000000 bomf-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-09 13:21:33.478128 bomf-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-09 13:21:25.000000 bomf-0.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-09 13:21:25.000000 bomf-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 13:21:25.000000 bomf-0.5.9/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-09 13:21:25.000000 bomf-0.5.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 13:21:33.482128 bomf-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 13:21:25.000000 bomf-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-09 13:21:25.000000 bomf-0.5.9/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_list_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-03 13:11:17.000000 bomf-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-03 13:11:17.000000 bomf-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 13:11:17.000000 bomf-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-03 13:11:25.608066 bomf-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-03 13:11:17.000000 bomf-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 13:11:17.000000 bomf-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 13:11:17.000000 bomf-0.6.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-03 13:11:17.000000 bomf-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-03 13:11:25.608066 bomf-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 13:11:17.000000 bomf-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-03 13:11:17.000000 bomf-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_list_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21270 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_validation.py
```

### Comparing `bomf-0.5.9/.github/dependabot.yml` & `bomf-0.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.github/workflows/black.yml` & `bomf-0.6.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.github/workflows/codeql-analysis.yml` & `bomf-0.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.github/workflows/coverage.yml` & `bomf-0.6.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.github/workflows/packaging_test.yml` & `bomf-0.6.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.github/workflows/python-publish.yml` & `bomf-0.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.github/workflows/pythonlint.yml` & `bomf-0.6.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.github/workflows/unittests.yml` & `bomf-0.6.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.gitignore` & `bomf-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/.pre-commit-config.yaml` & `bomf-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/LICENSE` & `bomf-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/PKG-INFO` & `bomf-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.9
+Version: 0.6.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.9/README.md` & `bomf-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/pyproject.toml` & `bomf-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/setup.cfg` & `bomf-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 packages = find:
 zip_safe = False
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	attrs
 	bo4e
-	pydantic
+	pydantic>=2.0.0
 	typeguard==2.13.3
 	frozendict
 	bidict
 	networkx
 	injector
 
 [options.packages.find]
```

### Comparing `bomf-0.5.9/src/bomf/__init__.py` & `bomf-0.6.0/src/bomf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Generic, Optional
 
 import attrs
 from injector import inject
 
 from bomf.filter import Filter
 from bomf.loader.entityloader import EntityLoader, LoadingSummary
+from bomf.logging import logger
 from bomf.mapper import (
     Bo4eDataSetToTargetMapper,
     IntermediateDataSet,
     PaginationNotSupportedException,
     SourceToBo4eDataSetMapper,
     TargetDataModel,
 )
@@ -56,58 +57,57 @@
         """
         a mapper that transforms bo4e data sets to a structure that suits the target system
         """
         self.target_loader: EntityLoader[TargetDataModel] = target_loader
         """
         The target loader moves the target entities into the actual target system.
         """
-        self.logger = logging.getLogger(self.__class__.__name__)
-        """
-        Class logger
-        """
 
     async def _map_to_target_validate_and_load(self, bo4e_datasets: list[IntermediateDataSet]) -> list[LoadingSummary]:
         """
         This method encapsulates the steps:
         1. validation
         2. mapping intermediate models to target
         3. load to target system.
         They have been encapsulated because they're used by both the migrate and migrate_paginated methods.
         """
+        _logger = logger.get()
         if self.validation_manager is not None:
-            self.logger.info("Applying validation rules to %i bo4e data sets", len(bo4e_datasets))
+            _logger.info("Applying validation rules to %i bo4e data sets", len(bo4e_datasets))
             validation_result = await self.validation_manager.validate(*bo4e_datasets)
-            self.logger.info(
+            _logger.info(
                 "Creating target models from those %i datasets that passed the validation",
                 len(validation_result.succeeded_data_sets),
             )
             target_data_models = await self.bo4e_to_target_mapper.create_target_models(
                 validation_result.succeeded_data_sets
             )
         else:
-            self.logger.warning("No validation set; skipping validation")
-            self.logger.info("Creating target models from all %i datasets", len(bo4e_datasets))
+            _logger.warning("No validation set; skipping validation")
+            _logger.info("Creating target models from all %i datasets", len(bo4e_datasets))
             target_data_models = await self.bo4e_to_target_mapper.create_target_models(bo4e_datasets)
-        self.logger.info("Loading %i target models into target system", len(target_data_models))
+        _logger.info("Loading %i target models into target system", len(target_data_models))
         loading_summaries = await self.target_loader.load_entities(target_data_models)
         await self.target_loader.close()
+        del target_data_models
         success_count, failure_count = _get_success_failure_count(loading_summaries)
-        self.logger.info("Loaded %i entities successfully, %i failed", success_count, failure_count)
+        _logger.info("Loaded %i entities successfully, %i failed", success_count, failure_count)
         return loading_summaries
 
     async def migrate(self) -> list[LoadingSummary]:
         """
         run the entire migration flow from source to target which includes:
         1. create bo4e data source using the source_data_set_to_bo4e_mapper
         2. checking that all the bo4e data sets obey the validation rules
         3. mapping from bo4e to the target data model
         4. loading the target data models into the target system.
         """
+        _logger = logger.get()
         # todo: here we should add some logging and statistics stuff
-        self.logger.info("Starting migration %s (w/o pagination)", self.__class__.__name__)
+        _logger.info("Starting migration %s (w/o pagination)", self.__class__.__name__)
         bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets()
         loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
         return loading_summaries
 
     async def migrate_paginated(
         self, chunk_size: int, initial_offset: int = 0, upper_bound: Optional[int] = None
     ) -> list[LoadingSummary]:
@@ -116,49 +116,51 @@
         Therefore, the source_data_to_bo4e_mapper must support pagination.
         You can specify an offset on where to start (initial_offset).
         The upper_bound does not cap the number of entries you want to migrate but instead is a number up to which the
         offset will definitely be incremented. This allows you to paginate over empty pages (because there's no matching
         entry within the range covered by one page). If you don't specify an upper_bound, the migration will stop on the
         first empty page.
         """
-        self.logger.info(
+        _logger = logger.get()
+        _logger.info(
             "Starting migration %s (with page size %i and initial offset %i)",
             self.__class__.__name__,
             chunk_size,
             initial_offset,
         )
         offset = initial_offset
         loading_summaries = []
         while True:
-            self.logger.info("Processing offset=%i, limit=%i", offset, chunk_size)
+            _logger.info("Processing offset=%i, limit=%i", offset, chunk_size)
             try:
                 bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets(
                     limit=chunk_size, offset=offset
                 )  # this might raise an PaginationNotSupportedException
             except TypeError as type_error:
                 error_message = str(type_error)
                 if (
                     "got an unexpected keyword argument 'limit'" in error_message
                     or "got an unexpected keyword argument 'offset'" in error_message
                 ):
                     # this case should be prevented by the type checker already
                     raise PaginationNotSupportedException() from type_error
                 raise
-            self.logger.debug("Received %i datasets (limit was %i)", len(bo4e_datasets), chunk_size)
+            _logger.debug("Received %i datasets (limit was %i)", len(bo4e_datasets), chunk_size)
             if (upper_bound is None or offset > upper_bound) and len(bo4e_datasets) == 0:
                 if upper_bound is not None:
-                    self.logger.info("Reached first empty page after upper bound %i; Stopping", upper_bound)
+                    _logger.info("Reached first empty page after upper bound %i; Stopping", upper_bound)
                 else:
-                    self.logger.info("Received no more datasets (first empty page; no upper bound defined); Stopping")
+                    _logger.info("Received no more datasets (first empty page; no upper bound defined); Stopping")
                 break
             chunk_loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
+            del bo4e_datasets
             loading_summaries.extend(chunk_loading_summaries)
             await asyncio.sleep(1)  # give the system 1s some time to breathe
             offset += chunk_size
         success_count, failure_count = _get_success_failure_count(loading_summaries)
-        self.logger.info(
+        _logger.info(
             "Finished paginated migration. In total we loaded %i entities out of which %i succeeded and %i failed",
             len(loading_summaries),
             success_count,
             failure_count,
         )
         return loading_summaries
```

### Comparing `bomf-0.5.9/src/bomf/filter/__init__.py` & `bomf-0.6.0/src/bomf/filter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 # pylint:disable=too-few-public-methods
 
 import asyncio
 import logging
 from abc import ABC, abstractmethod
 from typing import Awaitable, Callable, Generic, TypeVar
 
+from bomf.logging import logger
+
 Candidate = TypeVar("Candidate")  #: an arbitrary but fixed type on which the filter operates
 
 
 class Filter(ABC, Generic[Candidate]):
     """
     A filter takes objects from candidates and returns only those that are relevant for its use case.
     The advantage over inlining the filtering is that we can easily test these and log in the well-defined filters.
     """
 
     def __init__(self):
-        self._logger = logging.getLogger(self.__module__)
+        self._logger = logger.get()
 
     @abstractmethod
     async def predicate(self, candidate: Candidate) -> bool:
         """
         Returns true iff the candidate shall pass the filter.
 
         You might wonder why this method is async: The plan is that this allows for building filters that do not only
@@ -67,15 +69,15 @@
     the filter.
     """
 
     def __init__(self, base_filter: Filter[Aggregate]):
         """
         Instantiate by providing a filter that is applied on the aggregate
         """
-        self._logger = logging.getLogger(self.__module__)
+        self._logger = logger.get()
         self._base_filter = base_filter
 
     @abstractmethod
     async def aggregate(self, candidates: list[Candidate]) -> list[Aggregate]:
         """
         Create aggregates which are then passed to the base filter that works on the aggregate.
         The method is async so that you can do complex (and e.g. network based) aggregations.
```

### Comparing `bomf-0.5.9/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.6.0/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf/loader/entityloader.py` & `bomf-0.6.0/src/bomf/loader/entityloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 from abc import ABC, abstractmethod
 from datetime import datetime
 from pathlib import Path
 from typing import Awaitable, Callable, Generic, Optional, TypeVar
 
 import attrs
-from pydantic import BaseModel  # pylint:disable=no-name-in-module
+from pydantic import BaseModel, RootModel  # pylint:disable=no-name-in-module
 
 _TargetEntity = TypeVar("_TargetEntity")
 
 
 @attrs.define(auto_attribs=True, kw_only=True)
 class EntityLoadingResult:  # pylint:disable=too-few-public-methods
     """
@@ -153,43 +153,53 @@
 
     async def verify(self, entity: _TargetEntity, id_in_target_system: Optional[str] = None) -> bool:
         return True
 
     def __init__(self, file_path: Path, list_encoder: Callable[[list[_TargetEntity]], list[dict]]):
         """provide a path to a json file (will be created if not exists and overwritten if exists)"""
         self._file_path = file_path
+        self._file_lock = asyncio.Lock()
         self._list_encoder = list_encoder
-        self._entities: list[_TargetEntity] = []
 
     async def load_entity(self, entity: _TargetEntity) -> Optional[EntityLoadingResult]:
-        self._entities.append(entity)
+        async with self._file_lock:
+            existing_entries: list[dict]  # untyped entries
+            if self._file_path.exists():
+                with open(self._file_path, "r", encoding="utf-8") as json_file:
+                    json_body = json.load(json_file)
+                    existing_entries = json_body
+                existing_entries.extend(self._list_encoder([entity]))
+            else:
+                existing_entries = self._list_encoder([entity])
+            with open(self._file_path, "w+", encoding="utf-8") as outfile:
+                json.dump(existing_entries, outfile, ensure_ascii=False, indent=2)
+
         return None
 
     async def load_entities(self, entities: list[_TargetEntity]) -> list[LoadingSummary]:
         base_result = await super().load_entities(entities)
-        dict_list = self._list_encoder(self._entities)
-        with open(self._file_path, "w+", encoding="utf-8") as outfile:
-            json.dump(dict_list, outfile, ensure_ascii=False, indent=2)
+        dict_list = self._list_encoder(entities)
+        async with self._file_lock:
+            with open(self._file_path, "w+", encoding="utf-8") as outfile:
+                json.dump(dict_list, outfile, ensure_ascii=False, indent=2)
         return base_result
 
 
 _PydanticTargetModel = TypeVar("_PydanticTargetModel", bound=BaseModel)
 
 
 # pylint:disable=too-few-public-methods
-class _ListOfPydanticModels(BaseModel, Generic[_PydanticTargetModel]):
-    # https://stackoverflow.com/a/58641115/10009545
-    # for the instantiation see the serialization unit test
-    __root__: list[_PydanticTargetModel]
+class _ListOfPydanticModels(RootModel[list[_PydanticTargetModel]], Generic[_PydanticTargetModel]):
+    pass
 
 
 class PydanticJsonFileEntityLoader(JsonFileEntityLoader[_PydanticTargetModel], Generic[_PydanticTargetModel]):
     """
     A json file entity loader specifically for pydantic models
     """
 
     def __init__(self, file_path: Path):
         """provide a file path"""
         super().__init__(
             file_path=file_path,
-            list_encoder=lambda x: json.loads(_ListOfPydanticModels(__root__=x).json(by_alias=True)),
+            list_encoder=lambda x: [y.model_dump() for y in _ListOfPydanticModels(root=x).root],
         )
```

### Comparing `bomf-0.5.9/src/bomf/mapper/__init__.py` & `bomf-0.6.0/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf/model/__init__.py` & `bomf-0.6.0/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf/provider/__init__.py` & `bomf-0.6.0/src/bomf/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 from abc import ABC, abstractmethod
 from itertools import groupby
 from pathlib import Path
 from typing import Callable, Generic, Mapping, TypeVar, Union
 
 from bomf import PaginationNotSupportedException
+from bomf.logging import logger
 
 SourceDataModel = TypeVar("SourceDataModel")
 """
 Source data model is the data model of the source (meaning: the data model of the system from which the data originate).
 """
 
 KeyTyp = TypeVar("KeyTyp")
@@ -62,27 +63,24 @@
     """
 
     def __init__(self, source_data_models: list[SourceDataModel], key_selector: Callable[[SourceDataModel], KeyTyp]):
         """
         instantiate it by providing a list of source data models
         """
         self._models: list[SourceDataModel] = source_data_models
-        logger = logging.getLogger(self.__module__)
         for key, key_models in groupby(source_data_models, key=key_selector):
             affected_entries_count = len(list(key_models))
             if affected_entries_count > 1:
-                logger.warning(
+                logger.get().warning(
                     "There are %i>1 entries for the key '%s'. You might miss entries because the key is not unique.",
                     affected_entries_count,
                     str(key),
                 )
         self._models_dict: Mapping[KeyTyp, SourceDataModel] = {key_selector(m): m for m in source_data_models}
-        logging.getLogger(self.__module__).info(
-            "Read %i records from %s", len(self._models_dict), str(source_data_models)
-        )
+        logger.get().info("Read %i records from %s", len(self._models_dict), str(source_data_models))
         self.key_selector = key_selector
 
     async def get_entry(self, key: KeyTyp) -> SourceDataModel:
         return self._models_dict[key]
 
     async def get_data(self) -> list[SourceDataModel]:
         return self._models
```

### Comparing `bomf-0.5.9/src/bomf/validation/core/analysis.py` & `bomf-0.6.0/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf/validation/core/errors.py` & `bomf-0.6.0/src/bomf/validation/core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import random
 from contextlib import asynccontextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, AsyncGenerator, Generic, Optional, TypeAlias
 
 from bidict import bidict
 
-from bomf.validation.core.types import DataSetT, MappedValidatorT, ValidatorT, validation_logger
+from bomf.logging import logger
+from bomf.validation.core.types import DataSetT, MappedValidatorT, ValidatorT
 from bomf.validation.core.validator import Parameters
 
 if TYPE_CHECKING:
     from bomf.validation.core.execution import ValidationManager
 
 
 def format_parameter_infos(
@@ -67,15 +68,15 @@
 
 
 def _generate_new_id(identifier: _IdentifierType, last_id: Optional[_IDType] = None) -> _IDType:
     """
     Generate a new random id with taking the identifier as seed. If last_id is provided it will be used as seed instead.
     """
     if last_id is not None:
-        validation_logger.debug(
+        logger.get().debug(
             "Duplicated ID for %s and %s. Generating new ID...", identifier, _ERROR_ID_MAP.inverse[last_id]
         )
         random.seed(last_id)
     else:
         module_name_hash = int(hashlib.blake2s((identifier[0] + identifier[1]).encode(), digest_size=4).hexdigest(), 16)
         random.seed(module_name_hash + identifier[2])
     # This range has no further meaning, but you have to define it.
@@ -166,15 +167,15 @@
             msg,
             error,
             self.data_set,
             mapped_validator,
             validation_manager,
             error_id,
         )
-        validation_logger.exception(
+        logger.get().exception(
             str(error_nested),
             exc_info=error_nested,
         )
         async with asyncio.Lock():
             if mapped_validator not in self.excs:
                 self.excs[mapped_validator] = []
             self.excs[mapped_validator].append(error_nested)
```

### Comparing `bomf-0.5.9/src/bomf/validation/core/execution.py` & `bomf-0.6.0/src/bomf/validation/core/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from datetime import timedelta
 from enum import IntEnum, StrEnum
 from typing import Generic, Iterator, Optional
 
 import networkx as nx
 from typeguard import check_type
 
+from bomf.logging import logger
 from bomf.validation.core.analysis import ValidationResult
 from bomf.validation.core.errors import ErrorHandler, ValidationError
-from bomf.validation.core.types import DataSetT, MappedValidatorSyncAsync, SyncValidatorFunction, validation_logger
+from bomf.validation.core.types import DataSetT, MappedValidatorSyncAsync, SyncValidatorFunction
 from bomf.validation.core.validator import MappedValidator, Parameters, is_async, is_sync
 
 
 class _CustomErrorIDS(IntEnum):
     PARAM_TYPE_MISMATCH = 5
     ABANDON_EXEC = 2
     PARAM_PROVIDER_ERRORED = 1
@@ -166,15 +167,15 @@
         """
         dependency_graph_edges = self._dependency_graph_edges(mapped_validator, depends_on)
         self.validators[mapped_validator] = _ExecutionInfo(
             depends_on=depends_on if depends_on is not None else set(), timeout=timeout
         )
         self.dependency_graph.add_node(mapped_validator)
         self.dependency_graph.add_edges_from(dependency_graph_edges)
-        validation_logger.debug("Registered validator: %s", repr(mapped_validator))
+        logger.get().debug("Registered validator: %s", repr(mapped_validator))
 
     async def _dependency_errored(self, current_mapped_validator: MappedValidatorSyncAsync) -> bool:
         """
         Checks if a dependency has completed with errors. If so, this function returns True which will cause the
         current validator to be cancelled.
         """
         dep_exceptions: dict[MappedValidatorSyncAsync, list[ValidationError]] = {
@@ -352,15 +353,15 @@
                 async with asyncio.TaskGroup() as task_group:
                     await self._execute_validators(validator_execution_order, task_group=task_group)
             else:
                 await self._execute_validators(validator_execution_order)
 
         validation_result = ValidationResult(self, error_handlers)
         if log_summary:
-            validation_logger.info(
+            logger.get().info(
                 "Validation Summary: %i succeeded, %i failed, %i errors. %s",
                 validation_result.num_succeeds,
                 validation_result.num_fails,
                 validation_result.num_errors_total,
                 str(validation_result.num_errors_per_id),
             )
         return validation_result
```

### Comparing `bomf-0.5.9/src/bomf/validation/core/types.py` & `bomf-0.6.0/src/bomf/validation/core/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Contains the types used in the validation framework
 """
-import logging
 from typing import TYPE_CHECKING, Any, Callable, Coroutine, TypeAlias, TypeVar
 
 from bomf.model import Bo4eDataSet
 
 if TYPE_CHECKING:
     from bomf.validation.core.validator import MappedValidator, Validator
 
-validation_logger = logging.getLogger(__name__)
 DataSetT = TypeVar("DataSetT", bound=Bo4eDataSet)
 AsyncValidatorFunction: TypeAlias = Callable[..., Coroutine[Any, Any, None]]
 SyncValidatorFunction: TypeAlias = Callable[..., None]
 ValidatorFunction: TypeAlias = AsyncValidatorFunction | SyncValidatorFunction
 ValidatorFunctionT = TypeVar("ValidatorFunctionT", SyncValidatorFunction, AsyncValidatorFunction)
 ValidatorT: TypeAlias = "Validator[DataSetT, ValidatorFunctionT]"  # pylint: disable=invalid-name
 MappedValidatorT: TypeAlias = "MappedValidator[DataSetT, ValidatorFunctionT]"  # pylint: disable=invalid-name
```

### Comparing `bomf-0.5.9/src/bomf/validation/core/utils.py` & `bomf-0.6.0/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf/validation/core/validator.py` & `bomf-0.6.0/src/bomf/validation/core/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import inspect
 import types
 from abc import ABC, abstractmethod
 from typing import Any, Generator, Generic, TypeGuard, Union, overload
 
 from frozendict import frozendict
 
+from bomf.logging import logger
 from bomf.validation.core.types import (
     AsyncValidatorFunction,
     DataSetT,
     MappedValidatorT,
     SyncValidatorFunction,
     ValidatorFunctionT,
     ValidatorT,
-    validation_logger,
 )
 
 
 class Validator(Generic[DataSetT, ValidatorFunctionT]):
     """
     Holds the actual validator function:
         - The parameter list must contain at least one element
@@ -40,15 +40,15 @@
     def __init__(self, validator_func: ValidatorFunctionT):
         validator_signature = inspect.signature(validator_func)
         if len(validator_signature.parameters) == 0:
             raise ValueError("The validator function must take at least one argument")
         if any(param.kind == param.POSITIONAL_ONLY for param in validator_signature.parameters.values()):
             raise ValueError("The function parameters must not contain positional only parameters")
         if validator_signature.return_annotation not in (None, validator_signature.empty):
-            validation_logger.warning(
+            logger.get().warning(
                 "Annotated return type is not None (the return value will be ignored): %s(...) -> %s",
                 validator_func.__name__,
                 validator_signature.return_annotation,
             )
         param: inspect.Parameter
         for param in validator_signature.parameters.values():
             if param.annotation == param.empty:
@@ -65,15 +65,15 @@
             param_name
             for param_name in self.param_names
             if validator_signature.parameters[param_name].default == validator_signature.parameters[param_name].empty
         }
         self.optional_param_names = self.param_names - self.required_param_names
         self.name = validator_func.__name__
         self.is_async: bool = asyncio.iscoroutinefunction(validator_func)
-        validation_logger.debug("Created validator: %s", self.name)
+        logger.get().debug("Created validator: %s", self.name)
 
     def __hash__(self):
         return hash(self.func)
 
     def __eq__(self, other):
         return isinstance(other, Validator) and self.func == other.func
 
@@ -131,15 +131,15 @@
     """
     A validator which is capable to fill the parameter list by querying a data set instance.
     """
 
     def __init__(self, validator: ValidatorT):
         self.validator: ValidatorT = validator
         self.name = validator.name
-        validation_logger.debug("Created ParameterProvider: %s, %s", self.__class__.__name__, self.validator.name)
+        logger.get().debug("Created ParameterProvider: %s, %s", self.__class__.__name__, self.validator.name)
 
     @abstractmethod
     def provide(self, data_set: DataSetT) -> Generator[Parameters[DataSetT] | Exception, None, None]:
         """
         A generator function to return on each yield a parameter list to fill the validator function with it.
         If a parameter list could not be built you should yield an exception instead but your generator should not
         raise any exceptions because this will cause the generator to be destroyed (because python does not know where
```

### Comparing `bomf-0.5.9/src/bomf/validation/path_map.py` & `bomf-0.6.0/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf/validation/query_map.py` & `bomf-0.6.0/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf/validation/utils.py` & `bomf-0.6.0/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/src/bomf.egg-info/PKG-INFO` & `bomf-0.6.0/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.9
+Version: 0.6.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.9/src/bomf.egg-info/SOURCES.txt` & `bomf-0.6.0/src/bomf.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/bomf.egg-info/not-zip-safe
 src/bomf.egg-info/requires.txt
 src/bomf.egg-info/top_level.txt
 src/bomf/filter/__init__.py
 src/bomf/filter/sourcedataproviderfilter.py
 src/bomf/loader/__init__.py
 src/bomf/loader/entityloader.py
+src/bomf/logging/__init__.py
 src/bomf/mapper/__init__.py
 src/bomf/model/__init__.py
 src/bomf/provider/__init__.py
 src/bomf/validation/__init__.py
 src/bomf/validation/path_map.py
 src/bomf/validation/query_map.py
 src/bomf/validation/utils.py
@@ -40,14 +41,15 @@
 src/bomf/validation/core/analysis.py
 src/bomf/validation/core/errors.py
 src/bomf/validation/core/execution.py
 src/bomf/validation/core/types.py
 src/bomf/validation/core/utils.py
 src/bomf/validation/core/validator.py
 unittests/__init__.py
+unittests/conftest.py
 unittests/example_source_data.json
 unittests/test_bo4e_data_set.py
 unittests/test_entity_loader.py
 unittests/test_filter.py
 unittests/test_list_conversion.py
 unittests/test_mapper.py
 unittests/test_migration.py
```

### Comparing `bomf-0.5.9/tox.ini` & `bomf-0.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/unittests/test_bo4e_data_set.py` & `bomf-0.6.0/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/unittests/test_entity_loader.py` & `bomf-0.6.0/unittests/test_entity_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 from pathlib import Path
 from typing import Optional
 
 from pydantic import BaseModel
 
 from bomf.loader.entityloader import EntityLoader, EntityLoadingResult, PydanticJsonFileEntityLoader
@@ -125,7 +126,19 @@
         my_loader = MyLoader(file_path)
         await my_loader.load_entities(my_entities)
         del my_loader
         with open(file_path, "r", encoding="utf-8") as infile:
             json_body = json.load(infile)
         assert len(json_body) == 2
         assert json_body == [{"foo": "asd", "bar": 123}, {"foo": "qwe", "bar": 456}]
+
+    async def test_dumping_to_file_via_load_entity(self, tmp_path):
+        my_entity_a = MyPydanticClass(foo="asd", bar=123)
+        my_entity_b = MyPydanticClass(foo="qwe", bar=456)
+        file_path = Path(tmp_path) / Path("foo.json")
+        my_loader = MyLoader(file_path)
+        await asyncio.gather(my_loader.load_entity(my_entity_a), my_loader.load_entity(my_entity_b))
+        del my_loader
+        with open(file_path, "r", encoding="utf-8") as infile:
+            json_body = json.load(infile)
+        assert len(json_body) == 2
+        # we cannot guarantee the order of the entities
```

### Comparing `bomf-0.5.9/unittests/test_filter.py` & `bomf-0.6.0/unittests/test_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 _FooFilter(),
                 [{"foo": "baz"}, {"foo": "bar"}],
                 [{"foo": "bar"}],
             ),
         ],
     )
     async def test_filter(self, filter_under_test: Filter, candidates: list[dict], survivors: list[dict], caplog):
-        caplog.set_level(logging.DEBUG, logger=self.__module__)
+        caplog.set_level(logging.DEBUG, logger="")
         actual = await filter_under_test.apply(candidates)
         assert actual == survivors
         assert "1 out of 2 candidates have been removed by the filter" in caplog.messages
 
 
 @dataclasses.dataclass
 class _MyCandidate:
@@ -90,15 +90,15 @@
                 [_MyCandidate(number=19, string="bar"), _MyCandidate(number=2, string="foo")],
             ),
         ],
     )
     async def test_aggregate_filter(
         self, filter_under_test: AggregateFilter, candidates: list[dict], survivors: list[dict], caplog
     ):
-        caplog.set_level(logging.DEBUG, logger=self.__module__)
+        caplog.set_level(logging.DEBUG, logger="")
         actual = await filter_under_test.apply(candidates)
         assert actual == survivors
         assert "There are 4 candidates and 4 aggregates" in caplog.messages
         assert "There are 2 filtered aggregates left" in caplog.messages
 
 
 class TestBlockAndAllowlistFilter:
@@ -140,15 +140,15 @@
         survivors: list[_MyCandidate],
         caplog,
     ):
         my_provider: ListBasedSourceDataProvider[_MyCandidate, int] = ListBasedSourceDataProvider(
             candidates, key_selector=lambda mc: mc.number
         )
         sdp_filter: SourceDataProviderFilter[_MyCandidate, int] = SourceDataProviderFilter(candidate_filter)
-        caplog.set_level(logging.DEBUG, logger=self.__module__)
+        caplog.set_level(logging.DEBUG, logger="")
         filtered_provider = await sdp_filter.apply(my_provider)
         assert isinstance(filtered_provider, SourceDataProvider)
         actual = await filtered_provider.get_data()
         assert actual == survivors
         assert "There are 4 candidates and 4 aggregates" in caplog.messages
         assert "There are 2 filtered aggregates left" in caplog.messages
```

### Comparing `bomf-0.5.9/unittests/test_list_conversion.py` & `bomf-0.6.0/unittests/test_list_conversion.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/unittests/test_mapper.py` & `bomf-0.6.0/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/unittests/test_migration.py` & `bomf-0.6.0/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.9/unittests/test_source_data_provider.py` & `bomf-0.6.0/unittests/test_source_data_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         assert await example_json_data_provider.get_entry("world") == {"myKey": "world", "qwe": "rtz"}
         with pytest.raises(KeyError):
             _ = await example_json_data_provider.get_entry("something unknown")
 
 
 class TestListBasedSourceDataProvider:
     async def test_list_based_provider(self, caplog):
-        caplog.set_level(logging.DEBUG, logger=ListBasedSourceDataProvider.__module__)
+        caplog.set_level(logging.DEBUG, logger="")
         my_provider = ListBasedSourceDataProvider(["foo", "bar", "baz"], key_selector=lambda x: x)
         assert len(await my_provider.get_data()) == 3
         assert len(await my_provider.get_paginated_data(offset=0, limit=0)) == 0
         assert len(await my_provider.get_paginated_data(offset=0, limit=3)) == 3
         assert len(await my_provider.get_paginated_data(offset=0, limit=30)) == 3
         assert len(await my_provider.get_paginated_data(offset=1, limit=30)) == 2
         assert len(await my_provider.get_paginated_data(offset=3, limit=30)) == 0
```

### Comparing `bomf-0.5.9/unittests/test_validation.py` & `bomf-0.6.0/unittests/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import re
 from datetime import timedelta
 from typing import Any, Iterator, Optional
 
 import pytest
-from pydantic import BaseModel, Required
+from pydantic import BaseModel
 
 from bomf import ValidationManager
 from bomf.model import Bo4eDataSet
 from bomf.validation import Query, QueryMappedValidator, Validator, optional_field, param, required_field
 from bomf.validation.core import ValidationError, ValidatorFunctionT
 from bomf.validation.core.types import (
     AsyncValidatorFunction,
@@ -17,15 +17,15 @@
     ValidatorFunction,
 )
 from bomf.validation.path_map import PathMappedValidator
 
 
 class Wrapper(BaseModel):
     x: str
-    z: Optional[str] = Required
+    z: Optional[str]
 
 
 class DataSetTest(Bo4eDataSet):
     x: str
     y: int
     z: Wrapper
     a: int = -1
```

