# Comparing `tmp/ez-a-sync-0.5.2.tar.gz` & `tmp/ez-a-sync-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.5.2.tar", last modified: Mon Jul  3 19:35:15 2023, max compression
+gzip compressed data, was "ez-a-sync-0.5.3.tar", last modified: Mon Jul  3 20:37:48 2023, max compression
```

## Comparing `ez-a-sync-0.5.2.tar` & `ez-a-sync-0.5.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.328940 ez-a-sync-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.328940 ez-a-sync-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.328940 ez-a-sync-0.5.2/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7695 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 19:35:15.000000 ez-a-sync-0.5.2/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-03 19:35:15.000000 ez-a-sync-0.5.2/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 19:35:15.000000 ez-a-sync-0.5.2/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-03 19:35:15.000000 ez-a-sync-0.5.2/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-03 19:35:15.000000 ez-a-sync-0.5.2/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:15.332940 ez-a-sync-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-03 19:35:04.000000 ez-a-sync-0.5.2/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.940776 ez-a-sync-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.932776 ez-a-sync-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.932776 ez-a-sync-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 20:37:48.940776 ez-a-sync-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/TODO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.936776 ez-a-sync-0.5.3/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.936776 ez-a-sync-0.5.3/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.936776 ez-a-sync-0.5.3/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.936776 ez-a-sync-0.5.3/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7363 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.936776 ez-a-sync-0.5.3/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.940776 ez-a-sync-0.5.3/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-03 20:37:48.000000 ez-a-sync-0.5.3/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-03 20:37:48.000000 ez-a-sync-0.5.3/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 20:37:48.000000 ez-a-sync-0.5.3/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-03 20:37:48.000000 ez-a-sync-0.5.3/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-03 20:37:48.000000 ez-a-sync-0.5.3/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-03 20:37:48.940776 ez-a-sync-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:48.940776 ez-a-sync-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-03 20:37:35.000000 ez-a-sync-0.5.3/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.5.2/.github/workflows/codeql.yaml` & `ez-a-sync-0.5.3/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/.github/workflows/mypy.yaml` & `ez-a-sync-0.5.3/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/.github/workflows/pytest.yaml` & `ez-a-sync-0.5.3/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/.github/workflows/release.yaml` & `ez-a-sync-0.5.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/LICENSE.txt` & `ez-a-sync-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/README.md` & `ez-a-sync-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/__init__.py` & `ez-a-sync-0.5.3/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/_bound.py` & `ez-a-sync-0.5.3/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/_flags.py` & `ez-a-sync-0.5.3/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/_helpers.py` & `ez-a-sync-0.5.3/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/_kwargs.py` & `ez-a-sync-0.5.3/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/_meta.py` & `ez-a-sync-0.5.3/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/_typing.py` & `ez-a-sync-0.5.3/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/abstract.py` & `ez-a-sync-0.5.3/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/base.py` & `ez-a-sync-0.5.3/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/config.py` & `ez-a-sync-0.5.3/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/decorator.py` & `ez-a-sync-0.5.3/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/exceptions.py` & `ez-a-sync-0.5.3/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/modified.py` & `ez-a-sync-0.5.3/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/modifiers/__init__.py` & `ez-a-sync-0.5.3/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.5.3/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.5.3/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/modifiers/limiter.py` & `ez-a-sync-0.5.3/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/modifiers/manager.py` & `ez-a-sync-0.5.3/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.5.3/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/primitives/executor.py` & `ez-a-sync-0.5.3/a_sync/primitives/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 
 import asyncio
 import concurrent.futures as cf
+import logging
 import queue
 import threading
 import weakref
 from concurrent.futures import _base, thread
 from functools import cached_property
-from typing import Callable, TypeVar
+from typing import Callable, NoReturn, TypeVar
 
 from typing_extensions import ParamSpec
 
 TEN_MINUTES = 60 * 10
 
 T = TypeVar('T')
 P = ParamSpec('P')
 
+logger = logging.getLogger(__name__)
+
 """
 With ASync executors, you can simply run sync fns in your executor with `await executor.run(fn, *args)`
 """
 
 class _ASyncExecutorBase:
     _max_workers: int
     _workers: str
     async def run(self, fn: Callable[P, T], *args: P.args, **_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work: P.kwargs) -> T:
         """
         A shorthand way to call `await asyncio.get_event_loop().run_in_executor(this_executor, fn, *args)`
         Doesn't `await this_executor.run(fn, *args)` look so much better?
         """
         self._check_kwargs(_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work)
-        if not hasattr(self, '_work'):
-            self._work = []
-        self._work.append((fn, args))
-        self._ensure_debug_daemon()
+        t = self._start_debug_daemon(fn, *args)
         retval = await self._aioloop_run_in_executor(self, fn, *args)
-        self._work.remove((fn, args))
+        t.cancel()
+        return retval
     def submit(self, fn: Callable[P, T], *args: P.args, **_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work: P.kwargs) -> "asyncio.Task[T]":
         """Submits a job to the executor and returns an `asyncio.Task` that can be awaited for the result."""
         return asyncio.ensure_future(self.run(fn, *args, **_kwargs_dont_work_but_i_need_this_here_to_make_type_hints_work))
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} object at {hex(id(self))} [{len(self)}/{self._max_workers} {self._workers}]>"
+        return f"<{self.__class__.__name__} object at {hex(id(self))} [{len(self)}/{self._max_workers} {self._workers}  {len(self._work_queue)}]>"
     def __len__(self) -> int:
         return len(getattr(self, f"_{self._workers}"))
     @cached_property
     def _aioloop_run_in_executor(self) -> asyncio.BaseEventLoop:
         return asyncio.get_event_loop().run_in_executor
     def _check_kwargs(self, kwargs: dict):
         if kwargs: 
             raise ValueError("You can't use kwargs here, sorry. Pass them as positional args if you can.")
-    async def _debug_daemon(self) -> None:
-        while self._work:
+    async def _debug_daemon(self, fn, *args) -> NoReturn:
+        """Runs until manually cancelled by the finished work item"""
+        while True:
             await asyncio.sleep(15)
-            if self._work:
-                logger.debug(f'{self} processing {[self._work[i] for i in range(min(len(self._work), 10))]}{" and more" if len(self._work)>10 else ""}')
-    def _ensure_debug_daemon(self) -> None:
-        if not hasattr(self, '_daemon'):
-            self._daemon = None
-        if not self._daemon:
-            self._daemon = asyncio.create_task(self._debug_daemon())
-            def done_callback(t):
-                self._daemon = None
-                if e := t.exception():
-                    logger.info(e, exc_info=True)
-            self._daemon.add_done_callback(done_callback)
+            logger.debug(f'{self} processing {fn}{args}')
+    def _start_debug_daemon(self, fn, *args) -> "asyncio.Task[NoReturn]":
+        return asyncio.create_task(self._debug_daemon(fn, *args))
+    
 # Process
 
 class ProcessPoolExecutor(cf.ProcessPoolExecutor, _ASyncExecutorBase):
     _workers = "processes"
 
 # Thread
```

### Comparing `ez-a-sync-0.5.2/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.5.3/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/primitives/locks/event.py` & `ez-a-sync-0.5.3/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.5.3/a_sync/primitives/locks/semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/a_sync/property.py` & `ez-a-sync-0.5.3/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.5.3/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/setup.py` & `ez-a-sync-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/tests/fixtures.py` & `ez-a-sync-0.5.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/tests/test_base.py` & `ez-a-sync-0.5.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/tests/test_cache.py` & `ez-a-sync-0.5.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/tests/test_decorator.py` & `ez-a-sync-0.5.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/tests/test_limiter.py` & `ez-a-sync-0.5.3/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/tests/test_meta.py` & `ez-a-sync-0.5.3/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.5.2/tests/test_semaphore.py` & `ez-a-sync-0.5.3/tests/test_semaphore.py`

 * *Files identical despite different names*

