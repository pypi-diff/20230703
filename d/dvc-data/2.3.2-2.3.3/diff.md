# Comparing `tmp/dvc-data-2.3.2.tar.gz` & `tmp/dvc-data-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-data-2.3.2.tar", last modified: Sun Jul  2 19:32:36 2023, max compression
+gzip compressed data, was "dvc-data-2.3.3.tar", last modified: Mon Jul  3 01:13:39 2023, max compression
```

## Comparing `dvc-data-2.3.2.tar` & `dvc-data-2.3.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.337136 dvc-data-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.317136 dvc-data-2.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.317136 dvc-data-2.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-02 19:32:11.000000 dvc-data-2.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-02 19:32:11.000000 dvc-data-2.3.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-02 19:32:11.000000 dvc-data-2.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-02 19:32:11.000000 dvc-data-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-02 19:32:36.337136 dvc-data-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 19:32:11.000000 dvc-data-2.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-02 19:32:11.000000 dvc-data-2.3.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-02 19:32:11.000000 dvc-data-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-02 19:32:36.337136 dvc-data-2.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.313136 dvc-data-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.317136 dvc-data-2.3.2/src/dvc_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.325136 dvc-data-2.3.2/src/dvc_data/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.325136 dvc-data-2.3.2/src/dvc_data/hashfile/db/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/db/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/db/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/db/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/db/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/hash_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/hashfile/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.329136 dvc-data-2.3.2/src/dvc_data/index/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/index/view.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-02 19:32:11.000000 dvc-data-2.3.2/src/dvc_data/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.321136 dvc-data-2.3.2/src/dvc_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-02 19:32:36.000000 dvc-data-2.3.2/src/dvc_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-02 19:32:36.000000 dvc-data-2.3.2/src/dvc_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:32:36.000000 dvc-data-2.3.2/src/dvc_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-02 19:32:36.000000 dvc-data-2.3.2/src/dvc_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:32:36.000000 dvc-data-2.3.2/src/dvc_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-02 19:32:36.000000 dvc-data-2.3.2/src/dvc_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 19:32:36.000000 dvc-data-2.3.2/src/dvc_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.329136 dvc-data-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.329136 dvc-data-2.3.2/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/benchmarks/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.333136 dvc-data-2.3.2/tests/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_db_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_hash_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/hashfile/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:36.337136 dvc-data-2.3.2/tests/index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/index/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/index/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/index/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/index/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/index/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-02 19:32:11.000000 dvc-data-2.3.2/tests/test_dvc_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.903480 dvc-data-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.891479 dvc-data-2.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.891479 dvc-data-2.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-03 01:13:00.000000 dvc-data-2.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-03 01:13:00.000000 dvc-data-2.3.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-03 01:13:00.000000 dvc-data-2.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-03 01:13:00.000000 dvc-data-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-03 01:13:39.903480 dvc-data-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 01:13:00.000000 dvc-data-2.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-03 01:13:00.000000 dvc-data-2.3.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-03 01:13:00.000000 dvc-data-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-03 01:13:39.903480 dvc-data-2.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.891479 dvc-data-2.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.895480 dvc-data-2.3.3/src/dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.895480 dvc-data-2.3.3/src/dvc_data/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.899479 dvc-data-2.3.3/src/dvc_data/hashfile/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/db/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/db/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/db/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/db/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/hash_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/hashfile/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.899479 dvc-data-2.3.3/src/dvc_data/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/index/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-03 01:13:00.000000 dvc-data-2.3.3/src/dvc_data/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.895480 dvc-data-2.3.3/src/dvc_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-03 01:13:39.000000 dvc-data-2.3.3/src/dvc_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-03 01:13:39.000000 dvc-data-2.3.3/src/dvc_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:13:39.000000 dvc-data-2.3.3/src/dvc_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 01:13:39.000000 dvc-data-2.3.3/src/dvc_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:13:39.000000 dvc-data-2.3.3/src/dvc_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-03 01:13:39.000000 dvc-data-2.3.3/src/dvc_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 01:13:39.000000 dvc-data-2.3.3/src/dvc_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.899479 dvc-data-2.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.899479 dvc-data-2.3.3/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/benchmarks/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.903480 dvc-data-2.3.3/tests/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_db_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_hash_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/hashfile/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:39.903480 dvc-data-2.3.3/tests/index/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/index/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/index/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/index/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/index/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/index/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-03 01:13:00.000000 dvc-data-2.3.3/tests/test_dvc_data.py
```

### Comparing `dvc-data-2.3.2/.cruft.json` & `dvc-data-2.3.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/.github/dependabot.yml` & `dvc-data-2.3.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/.github/workflows/benchmark.yml` & `dvc-data-2.3.3/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/.github/workflows/release.yml` & `dvc-data-2.3.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/.github/workflows/tests.yml` & `dvc-data-2.3.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/.gitignore` & `dvc-data-2.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/.pre-commit-config.yaml` & `dvc-data-2.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/CODE_OF_CONDUCT.rst` & `dvc-data-2.3.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/CONTRIBUTING.rst` & `dvc-data-2.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/LICENSE` & `dvc-data-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/PKG-INFO` & `dvc-data-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 2.3.2
+Version: 2.3.3
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-2.3.2/README.rst` & `dvc-data-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/noxfile.py` & `dvc-data-2.3.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/pyproject.toml` & `dvc-data-2.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/setup.cfg` & `dvc-data-2.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/cli.py` & `dvc-data-2.3.3/src/dvc_data/cli.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/fs.py` & `dvc-data-2.3.3/src/dvc_data/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/__init__.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/_progress.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/build.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/cache.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/checkout.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/db/__init__.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/db/index.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/db/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/db/local.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/db/local.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/db/migrate.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/db/migrate.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/db/reference.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/db/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/diff.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/gc.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/hash.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/hash_info.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/hash_info.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/istextfile.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/meta.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/meta.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/state.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/state.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/status.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/status.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/transfer.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,18 @@
         dir_obj = find_tree_by_obj_id([cache_odb, src], dir_hash)
         assert dir_obj
 
         entry_ids = {oid for _, _, oid in dir_obj}
         bound_file_ids = all_file_ids & entry_ids
         all_file_ids -= entry_ids
 
+        logger.debug(
+            "transfer dir: %s with %d files", dir_hash, len(bound_file_ids)
+        )
+
         dir_fails = _add(src, dest, bound_file_ids, **kwargs)
         if dir_fails:
             logger.debug(
                 "failed to upload full contents of '%s', "
                 "aborting .dir file upload",
                 dir_hash,
             )
```

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/tree.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/hashfile/utils.py` & `dvc-data-2.3.3/src/dvc_data/hashfile/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/__init__.py` & `dvc-data-2.3.3/src/dvc_data/index/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/add.py` & `dvc-data-2.3.3/src/dvc_data/index/add.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/build.py` & `dvc-data-2.3.3/src/dvc_data/index/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/checkout.py` & `dvc-data-2.3.3/src/dvc_data/index/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/diff.py` & `dvc-data-2.3.3/src/dvc_data/index/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/fetch.py` & `dvc-data-2.3.3/src/dvc_data/index/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/index.py` & `dvc-data-2.3.3/src/dvc_data/index/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/save.py` & `dvc-data-2.3.3/src/dvc_data/index/save.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/serialize.py` & `dvc-data-2.3.3/src/dvc_data/index/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/index/view.py` & `dvc-data-2.3.3/src/dvc_data/index/view.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data/repo.py` & `dvc-data-2.3.3/src/dvc_data/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data.egg-info/PKG-INFO` & `dvc-data-2.3.3/src/dvc_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 2.3.2
+Version: 2.3.3
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-2.3.2/src/dvc_data.egg-info/SOURCES.txt` & `dvc-data-2.3.3/src/dvc_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/src/dvc_data.egg-info/requires.txt` & `dvc-data-2.3.3/src/dvc_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/benchmarks/test_checkout.py` & `dvc-data-2.3.3/tests/benchmarks/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_cache.py` & `dvc-data-2.3.3/tests/hashfile/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_db_index.py` & `dvc-data-2.3.3/tests/hashfile/test_db_index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_diff.py` & `dvc-data-2.3.3/tests/hashfile/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_hash.py` & `dvc-data-2.3.3/tests/hashfile/test_hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_hash_stream.py` & `dvc-data-2.3.3/tests/hashfile/test_hash_stream.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_istextfile.py` & `dvc-data-2.3.3/tests/hashfile/test_istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_tree.py` & `dvc-data-2.3.3/tests/hashfile/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/hashfile/test_utils.py` & `dvc-data-2.3.3/tests/hashfile/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/index/conftest.py` & `dvc-data-2.3.3/tests/index/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/index/test_build.py` & `dvc-data-2.3.3/tests/index/test_build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/index/test_checkout.py` & `dvc-data-2.3.3/tests/index/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/index/test_diff.py` & `dvc-data-2.3.3/tests/index/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-2.3.2/tests/index/test_index.py` & `dvc-data-2.3.3/tests/index/test_index.py`

 * *Files identical despite different names*

