# Comparing `tmp/yaecs-4.0.2.tar.gz` & `tmp/yaecs-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-4.0.2.tar", last modified: Fri Jun 30 12:12:49 2023, max compression
+gzip compressed data, was "yaecs-4.1.0.tar", last modified: Mon Jul  3 09:21:42 2023, max compression
```

## Comparing `yaecs-4.0.2.tar` & `yaecs-4.1.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.962137 yaecs-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 12:12:34.000000 yaecs-4.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.950137 yaecs-4.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.954137 yaecs-4.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 12:12:34.000000 yaecs-4.0.2/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-30 12:12:34.000000 yaecs-4.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-30 12:12:34.000000 yaecs-4.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-30 12:12:34.000000 yaecs-4.0.2/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-06-30 12:12:34.000000 yaecs-4.0.2/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-06-30 12:12:34.000000 yaecs-4.0.2/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-06-30 12:12:34.000000 yaecs-4.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 12:12:34.000000 yaecs-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-30 12:12:49.962137 yaecs-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-30 12:12:34.000000 yaecs-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/yaecs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/yaecs_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-30 12:12:34.000000 yaecs-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 12:12:34.000000 yaecs-4.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 12:12:34.000000 yaecs-4.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-06-30 12:12:34.000000 yaecs-4.0.2/resources/yaecs_constructor_overview.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/scipts/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 12:12:34.000000 yaecs-4.0.2/scipts/build_docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 12:12:34.000000 yaecs-4.0.2/scipts/tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:12:49.962137 yaecs-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 12:12:34.000000 yaecs-4.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 12:12:34.000000 yaecs-4.0.2/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    37943 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.962137 yaecs-4.0.2/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24885 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33849 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.962137 yaecs-4.0.2/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.092118 yaecs-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 09:21:24.000000 yaecs-4.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.084117 yaecs-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 09:21:24.000000 yaecs-4.1.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-03 09:21:24.000000 yaecs-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-07-03 09:21:24.000000 yaecs-4.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-03 09:21:24.000000 yaecs-4.1.0/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-07-03 09:21:24.000000 yaecs-4.1.0/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    78342 2023-07-03 09:21:24.000000 yaecs-4.1.0/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-07-03 09:21:24.000000 yaecs-4.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 09:21:24.000000 yaecs-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-03 09:21:42.092118 yaecs-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-03 09:21:24.000000 yaecs-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/yaecs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-03 09:21:24.000000 yaecs-4.1.0/docs/yaecs_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-03 09:21:24.000000 yaecs-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 09:21:24.000000 yaecs-4.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 09:21:24.000000 yaecs-4.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-07-03 09:21:24.000000 yaecs-4.1.0/resources/yaecs_constructor_overview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/scipts/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 09:21:24.000000 yaecs-4.1.0/scipts/build_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 09:21:24.000000 yaecs-4.1.0/scipts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:21:42.092118 yaecs-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 09:21:24.000000 yaecs-4.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-03 09:21:24.000000 yaecs-4.1.0/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:24.000000 yaecs-4.1.0/unittests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:24.000000 yaecs-4.1.0/unittests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-03 09:21:24.000000 yaecs-4.1.0/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37690 2023-07-03 09:21:24.000000 yaecs-4.1.0/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 09:21:24.000000 yaecs-4.1.0/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.088118 yaecs-4.1.0/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.092118 yaecs-4.1.0/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.092118 yaecs-4.1.0/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-03 09:21:24.000000 yaecs-4.1.0/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.092118 yaecs-4.1.0/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 09:21:41.000000 yaecs-4.1.0/yaecs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.092118 yaecs-4.1.0/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24885 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/config_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33849 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27670 2023-07-03 09:21:24.000000 yaecs-4.1.0/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:21:42.092118 yaecs-4.1.0/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-03 09:21:42.000000 yaecs-4.1.0/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-03 09:21:42.000000 yaecs-4.1.0/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:21:42.000000 yaecs-4.1.0/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 09:21:42.000000 yaecs-4.1.0/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 09:21:42.000000 yaecs-4.1.0/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-4.0.2/.github/workflows/pipy_deployment.yaml` & `yaecs-4.1.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/.gitignore` & `yaecs-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/.pylintrc` & `yaecs-4.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/COPYING.LESSER.md` & `yaecs-4.1.0/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/COPYING.md` & `yaecs-4.1.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/DOCUMENTATION_WIP.md` & `yaecs-4.1.0/DOCUMENTATION_WIP.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,127 @@
 # YAECS (Yet Another Experiment Config System) : documentation
 
 ---
 
-This documentation page describes our take on config systems : YAECS. It is mainly comprised of the Configuration object, which is meant to make some operations more practical, including :
+This documentation page describes our take on config systems : YAECS. It is mainly comprised of the Configuration
+object, which is meant to make some operations more practical, including :
 
 - printing, saving and loading configurations easily and in a flexible way
 - flexibility to adapt to the size of a project (simple configs for small
 projects, multi-file and/or nested configs for large projects)
-- making it easy to change the config between two experiments, to implement hyper-parameter searches, or to visualise the differences between past experiments
-- increasing the overall readability of the config files and introducing safeguards against bad practices for projects with several contributors/use cases
-- allowing for every single parameter in a project to be grouped in a single place (the default config) for easy access, without making the config hard to manipulate and use due to its size
+- making it easy to change the config between two experiments, to implement hyper-parameter searches, or to visualise
+the differences between past experiments
+- increasing the overall readability of the config files and introducing safeguards against bad practices for projects
+with several contributors/use cases
+- allowing for every single parameter in a project to be grouped in a single place (the default config) for easy access,
+without making the config hard to manipulate and use due to its size
 
 ## 0) Our philosophy
 
-Before heading right into the nitty gritty of things, we'd like to take a moment to tell you our thoughts about experiments and the research process. This will let us define the terms we use throughout this documentation, and if you realise that we think alike, maybe this config system is for you ;)
+Before heading right into the nitty gritty of things, we'd like to take a moment to tell you our thoughts about
+experiments and the research process. This will let us define the terms we use throughout this documentation, and if you
+realise that we think alike, maybe this config system is for you ;)
 
 ### What we call experiments
 
-A research project has many phases. Some are very wild and exploratory, using notebooks or third-party tools to quickly iterate and visualise. Some others involve debugging or refactoring. What we call **experiments** are the following situations :
+A research project has many phases. Some are very wild and exploratory, using notebooks or third-party tools to quickly
+iterate and visualise. Some others involve debugging or refactoring. What we call **experiments** are the following
+situations :
+
+- you run a part of your code to gain **trustworthy knowledge** about a certain component or process in your project.
+*This includes for example evaluating a metric to report it in a paper or take an impactful decision for the future of*
+*your paper* (rule of importance)
+- you run a part of your code **for a long time**, or using a **large amount of data**, or needing **significant**
+**computational resources**. *This includes for example training a neural network, evaluating on more than 10 samples,*
+*or having to package your code to run it on another machine* (rule of cost)
+- the effect you are studying is **complex**, involves **significant portions of code**, or involves interactions
+between **several different modules** with distinct purposes that you investigate at the same time. *This includes*
+*evaluating a specific function in the context of your entire pipeline, exploring possibilities for more than a day,*
+*or changing the behaviour of several components simultaneously* (rule of complexity)
 
-- you run a part of your code to gain **trustworthy knowledge** about a certain component or process in your project. *This includes for example evaluating a metric to report it in a paper or take an impactful decision for the future of your paper* (rule of importance)
-- you run a part of your code **for a long time**, or using a **large amount of data**, or needing **significant computational resources**. *This includes for example training a neural network, evaluating on more than 10 samples, or having to package your code to run it on another machine* (rule of cost)
-- the effect you are studying is **complex**, involves **significant portions of code**, or involves interactions between **several different modules** with distinct purposes that you investigate at the same time. *This includes evaluating a specific function in the context of your entire pipeline, exploring possibilities for more than a day, or changing the behaviour of several components simultaneously* (rule of complexity)
-
-**In those cases, we argue that your action should be regarded as an experiment, and performed under a number of safeguards.**
-This is the core of our philosophy, and the purpose which this library intends to serve.
+**In those cases, we argue that your action should be regarded as an experiment, and performed under a number of**
+**safeguards.** This is the core of our philosophy, and the purpose which this library intends to serve.
 
 ### Properties of the ideal experiment
 
-Now that we have outlined the scope of what we consider "experiments", here we describe how we think a good experiment should be.
+Now that we have outlined the scope of what we consider "experiments", here we describe how we think a good experiment
+should be.
 
-- **clear** : understanding your experiment, its purpose, setup and results, should be as simple as possible, be it for coworkers, the scientific community, or most of the time future you :)
-- **reproducible** : running your experiment again, to witness the same behaviour or continue investigating from that previous state, should be reliable and effortless
-- **responsible** : an experiment is an investment of precious resources and a step towards a result with an impact on our world. For efficiency and accountability, its outcome and context should be logged
-- **simple** : we are all human, and projects can be long and taxing. Starting a new experiment should be simple, enjoyable and exciting
+- **clear** : understanding your experiment, its purpose, setup and results, should be as simple as possible, be it for
+coworkers, the scientific community, or most of the time future you :)
+- **reproducible** : running your experiment again, to witness the same behaviour or continue investigating from that
+previous state, should be reliable and effortless
+- **responsible** : an experiment is an investment of precious resources and a step towards a result with an impact on
+our world. For efficiency and accountability, its outcome and context should be logged
+- **simple** : we are all human, and projects can be long and taxing. Starting a new experiment should be simple,
+enjoyable and exciting
 
 ### What we call configs
 
-A very abstract way of viewing experiments is to consider them "processes that use resources to produce outcomes". In our case, resources are as diverse as the code, the hardware, the data... but for the purpose of this explanation, we can simplify them in 2 categories : the support and the configuration (config). The support is comprised of all the resources needed to reproduce all the experiments in your project. All the hardware. All versions of your code and data. And the config is simply how to configure your support to reproduce a given experiment. Each experiment has its own config, and the project has a single support which suffices to reproduce any experiment.
-
-In this library, we tackle the config side of things. Other tools such as git, remote deployment to specific hardware or dataset version control can help setting up and maintaining the support throughout the project.
-
-So then, back to the config. The config generally assumes a certain knowledge of the support, which makes sense in that it is a configuration *of that support*. Therefore, appropriate naming and organisation should make it obvious, with that knowledge, which element of the support each part of the config controls. The config is an object which contains key-value pairs as would a dictionary. When running an experiment, instead of resorting to hard-coded values which present many issues, the support queries the corresponding config for its values using the keys. Such key-value pairs are commonly referred to as "parameters" (though from a Machine Learning perspective they are ususally called hyper-parameters to disambiguate them from learnable parameters).
+A very abstract way of viewing experiments is to consider them "processes that use resources to produce outcomes". In
+our case, resources are as diverse as the code, the hardware, the data... but for the purpose of this explanation, we
+can simplify them in 2 categories : the support and the configuration (config). The support is comprised of all the
+resources needed to reproduce all the experiments in your project. All the hardware. All versions of your code and data.
+And the config is simply how to configure your support to reproduce a given experiment. Each experiment has its own
+config, and the project has a single support which suffices to reproduce any experiment.
+
+In this library, we tackle the config side of things. Other tools such as git, remote deployment to specific hardware or
+dataset version control can help setting up and maintaining the support throughout the project.
+
+So then, back to the config. The config generally assumes a certain knowledge of the support, which makes sense in that
+it is a configuration *of that support*. Therefore, appropriate naming and organisation should make it obvious, with
+that knowledge, which element of the support each part of the config controls. The config is an object which contains
+key-value pairs as would a dictionary. When running an experiment, instead of resorting to hard-coded values which
+present many issues, the support queries the corresponding config for its values using the keys. Such key-value pairs
+are commonly referred to as "parameters" (though from a Machine Learning perspective they are ususally called
+hyper-parameters to disambiguate them from learnable parameters).
 
 ### How proper configs save the day
 
-The support is usually huge, changes often and is worked on by several people at the same time. For that reason, reaching our goal of having simple, reproductible, clear experiments can be a daunting task. But is it really ? Thinking about it, what *distinguishes* experiments, the config, is on the contrary quite simple. Experiments that make too many factors vary at once are usually a bad practice which users will try to avoid, which means most of the time only a few differences separate two experiments.
-
-This means at least in principle that setting up your configs, logging them, reading them and sharing them with other people familiar with the support should be simple, and what is simple is usually also clear and enjoyable. A quick glance should be sufficient to remind you what this specific experiment was about, and then you can go on to checking the results. To reproduce an experiment, you simply use the same config, and you can then modify it as you wish.
-
-Of course, not everything is that simple. Complex projects can require hundreds or even thousands of config parameters to support all existing and potential future experiments. Moreover, two experiments close in time are easy to compare, but months later, the config may look very different. This is where YAECS comes in.
+The support is usually huge, changes often and is worked on by several people at the same time. For that reason,
+reaching our goal of having simple, reproductible, clear experiments can be a daunting task. But is it really ? Thinking
+about it, what *distinguishes* experiments, the config, is on the contrary quite simple. Experiments that make too many
+factors vary at once are usually a bad practice which users will try to avoid, which means most of the time only a few
+differences separate two experiments.
+
+This means at least in principle that setting up your configs, logging them, reading them and sharing them with other
+people familiar with the support should be simple, and what is simple is usually also clear and enjoyable. A quick
+glance should be sufficient to remind you what this specific experiment was about, and then you can go on to checking
+the results. To reproduce an experiment, you simply use the same config, and you can then modify it as you wish.
+
+Of course, not everything is that simple. Complex projects can require hundreds or even thousands of config parameters
+to support all existing and potential future experiments. Moreover, two experiments close in time are easy to compare,
+but months later, the config may look very different. This is where YAECS comes in.
 
 ### The guiding principles of YAECS
 
 YAECS learns from other existing config systems such as YACS or hydra to make it so that :
 
 - integrating the YAECS config system in small projects takes almost no effort at all ;
 - the amount of overhead in your main code is minimal ;
-- it seemlessly grows and adapts as your project does, accepting an ever-increasing number of parameters and features while maintaining a similar ease of use ;
-- it provides all the flexibility needed to hide away complex parameter processing behind simple APIs. Features that could be useful to handle configs should be available, and once the relevant feature has been set up in your project, the ease of use for following experiments should remain unchanged or be improved ;
-- it simplifies backward and forward reproducibility and, coupled with a certain rigor when implementing new features, allows you to reproduce experiments without even checking out another code version. That way, previous experiments can be reproduced while still benefitting from new codebase improvements ;
+- it seemlessly grows and adapts as your project does, accepting an ever-increasing number of parameters and features
+while maintaining a similar ease of use ;
+- it provides all the flexibility needed to hide away complex parameter processing behind simple APIs. Features that
+could be useful to handle configs should be available, and once the relevant feature has been set up in your project,
+the ease of use for following experiments should remain unchanged or be improved ;
+- it simplifies backward and forward reproducibility and, coupled with a certain rigor when implementing new features,
+allows you to reproduce experiments without even checking out another code version. That way, previous experiments can
+be reproduced while still benefitting from new codebase improvements ;
 - it provides integration with common trackers to log and visualise its configs and the resulting outcome ;
-- and it prints warnings or raises errors as a safeguard against bad practices... because we all have those days don't we ;)
+- and it prints warnings or raises errors as a safeguard against bad practices... because we all have those days don't
+we ;)
 
-Did we meet all our goals ? Well... that is for you to judge :) if you think we haven't, do leave us gitlab issues for us to do better.
+Did we meet all our goals ? Well... that is for you to judge :) if you think we haven't, do leave us gitlab issues for
+us to do better.
 We hope you enjoy your YAECS experience !
 
 ## I) Getting started
 
-Getting started with using YAECS requires a single thing : creating a Configuration object containing your parameters. There are many ways to create this config object, but let us focus on the easiest one.
+Getting started with using YAECS requires a single thing : creating a Configuration object containing your parameters.
+There are many ways to create this config object, but let us focus on the easiest one.
 
 ```python
 from yaecs import make_config
 
 dictionary = {
     "batch_size": 32,
     "experiment_name": "overfit",
@@ -85,19 +134,25 @@
 
 ```python
 print(config.batch_size)  # 32
 print(config["experiment_name"])  # overfit
 print(config.get("learning_rate", None))  # 0.001
 ```
 
-At this point you might think that this is nothing more than a more fancy dictionary... and you'd be right, that's actually a very good way to think about your config. In fact, because it mostly behaves like a dictionary, it is much easier to integrate into existing code or libraries which expect dictionaries.
+At this point you might think that this is nothing more than a more fancy dictionary... and you'd be right, that's
+actually a very good way to think about your config. In fact, because it mostly behaves like a dictionary, it is much
+easier to integrate into existing code or libraries which expect dictionaries.
+
+Of course, in many situations, it is much more than a simple dictionary, as we will demonstrate thoughout this
+documentation. In this first introduction, we will cover two more things : loading a config from a **yaml file**, and
+some basic **command line interaction**. If you want more, we encourage you to keep reading our other tutorials TODO in
+which we give **practical tips** and **best practices** for the management of your config over the course of a project.
 
-Of course, in many situations, it is much more than a simple dictionary, as we will demonstrate thoughout this documentation. In this first introduction, we will cover two more things : loading a config from a **yaml file**, and some basic **command line interaction**. If you want more, we encourage you to keep reading our other tutorials TODO in which we give **practical tips** and **best practices** for the management of your config over the course of a project.
-
-The main purpose of using a config system is to manage your parameters more easily by **getting them out of your code**. So let's do just that :)
+The main purpose of using a config system is to manage your parameters more easily by **getting them out of your code**.
+So let's do just that :)
 
 We will create a file called `config.yaml` in the root of our project, next to our `main.py` :
 
 ```yaml
 batch_size: 32
 experiment_name: overfit
 learning_rate: 0.001
@@ -121,15 +176,16 @@
 $ python main.py
 [CONFIG] Building config from default : config
 32
 overfit
 0.001
 ```
 
-One way the YAECS config system provides to manage parameters is to edit them from the command line, which is performed automatically when you create your config. See for yourself :
+One way the YAECS config system provides to manage parameters is to edit them from the command line, which is performed
+automatically when you create your config. See for yourself :
 
 ```bash
 $ python main.py --batch_size 16
 [CONFIG] Building config from default : config
 [CONFIG] Merging from command line : {'batch_size': 16}
 16
 overfit
@@ -138,44 +194,58 @@
 [CONFIG] Building config from default : config
 [CONFIG] Merging from command line : {'experiment_name': 'production', 'batch_size': 16}
 16
 production
 0.001
 ```
 
-The YAECS command line parser, one of YAECS' many ways of **preparing your experiment's config**, is very flexible and fast when you want to change only a handful of parameters.
+The YAECS command line parser, one of YAECS' many ways of **preparing your experiment's config**, is very flexible and
+fast when you want to change only a handful of parameters.
 
-This is as far as we go for this short introduction. If you're already used to config systems and managing config files, this might be enough to get you started. However, if you've always just used hardcoded values in your code, and maybe argparse, you might not really know where to start. We advise you to look at our tutorial TODO, which will walk you through config management using YAECS from early set-up to advanced usage.
+This is as far as we go for this short introduction. If you're already used to config systems and managing config files,
+this might be enough to get you started. However, if you've always just used hardcoded values in your code, and maybe
+argparse, you might not really know where to start. We advise you to look at our tutorial TODO, which will walk you
+through config management using YAECS from early set-up to advanced usage.
 
 Happy experimenting !
 
 ## II) Tutorial to a clean config management
 
 ### Basic setup for small projects
 
-You have never used a config system, and you just found out about YAECS ? You've come to the right place ! In this first part of our tutorial, we will walk you through the basics of setting up your project for easy and safe experiments.
+You have never used a config system, and you just found out about YAECS ? You've come to the right place ! In this first
+part of our tutorial, we will walk you through the basics of setting up your project for easy and safe experiments.
 
 In this first "basic" part of our tutorial, we will :
 
 1) set up the default config for your project
 2) explain how to load the config in your code and conduct experiments
 3) see our first management tool : sub-configs
 4) explain how to access parameters and perform basic actions
 
 Let's start !
 
 #### 1) Creating the default config
 
-To use YAECS in a project, the very first thing to always do is to prepare the default config. The default config needs to be a YAML file, which will contain **all the parameters for your project** and their default values. We have decided to enforce the requirement that every single param be in the defaults, because it is both safer and desirable for you.
-
-It is **safer** because if you want to change a parameter and miss-spell its name, YAECS will know that the parameter name is wrong because it is not in the default config. Therefore instead of starting your experiment with incorrect values, YAECS will throw an error.
-
-It is **desirable** because it gives you a centralised place where you can look up all the values, all the hyper-parameters, all the magic numbers, without going through dozens of source files. YAECS is designed so that having a very large default config never becomes a burden for clarity. Therefore, no need to shy away from having **a lot** of parameters in there.
-
-YAML is a very intuitive config format. We chose it for its elegance, flexibility and the fact that it supports comments (which is not the case in JSON for example). If you need, you can find the YAML documentation here : TODO. Here is the config example we choose to use in this tutorial :
+To use YAECS in a project, the very first thing to always do is to prepare the default config. The default config needs
+to be a YAML file, which will contain **all the parameters for your project** and their default values. We have decided
+to enforce the requirement that every single param be in the defaults, because it is both safer and desirable for you.
+
+It is **safer** because if you want to change a parameter and miss-spell its name, YAECS will know that the parameter
+name is wrong because it is not in the default config. Therefore instead of starting your experiment with incorrect
+values, YAECS will throw an error.
+
+It is **desirable** because it gives you a centralised place where you can look up all the values, all the
+hyper-parameters, all the magic numbers, without going through dozens of source files. YAECS is designed so that having
+a very large default config never becomes a burden for clarity. Therefore, no need to shy away from having **a lot** of
+parameters in there.
+
+YAML is a very intuitive config format. We chose it for its elegance, flexibility and the fact that it supports comments
+(which is not the case in JSON for example). If you need, you can find the YAML documentation here : TODO. Here is the
+config example we choose to use in this tutorial :
 
 ```yaml
 ---  # Default config - configs/default.yaml
 
 experiment_path: null
 use_gpu: true
 do_train: true
@@ -200,29 +270,41 @@
    optimiser:
       type: Adam
       learning_rate: .001
       betas: [0.9, 0.999]
       weight_decay: 0
 ```
 
-Let us save this under `configs/default.yaml`. We created this config file to give you an example of what it could look like (and also to show you some nice features later), but yours will most likely be bigger. Here is what we advise you to store in this default config :
-
-- variables you intend to change later, or you think you might change later (for example up there `do_test`, `experiment_path`, `train.epochs`, ...)
-- variables you don't necessarily want to change, but for which you might want to be able to find the value easily (for example `use_gpu` or `model.activation`)
+Let us save this under `configs/default.yaml`. We created this config file to give you an example of what it could look
+like (and also to show you some nice features later), but yours will most likely be bigger. Here is what we advise you
+to store in this default config :
+
+- variables you intend to change later, or you think you might change later (for example up there `do_test`,
+`experiment_path`, `train.epochs`, ...)
+- variables you don't necessarily want to change, but for which you might want to be able to find the value easily
+(for example `use_gpu` or `model.activation`)
 - generally any hardcoded value in your code that has an understandable meaning
 
-So yeah... that's gonna be a lot of parameters. Much more than in our simple example here. But fear not, don't be shy, put them all in. This is by far the most time-consuming part of the process, but you will not regret the time you invest here. Even if you decide later that YAECS is not for you after all, you will be glad to have it whichever other tool you decide to go for.
-
-As for the values to use for the parameters you put in there, well, it's a default config, so use default values. Values which make sense in general, which will be used "by default" if the user does not specify their own. As you can see with `experiment_path`, sometimes no value really makes sense for a parameter, for example when this parameter should always be set by the user in all experiments. In those cases you can use `null`, which is YAML's equivalent for python's `None`.
+So yeah... that's gonna be a lot of parameters. Much more than in our simple example here. But fear not, don't be shy,
+put them all in. This is by far the most time-consuming part of the process, but you will not regret the time you invest
+here. Even if you decide later that YAECS is not for you after all, you will be glad to have it whichever other tool you
+decide to go for.
+
+As for the values to use for the parameters you put in there, well, it's a default config, so use default values. Values
+which make sense in general, which will be used "by default" if the user does not specify their own. As you can see with
+`experiment_path`, sometimes no value really makes sense for a parameter, for example when this parameter should always
+be set by the user in all experiments. In those cases you can use `null`, which is YAML's equivalent for python's
+`None`.
 
 And here you go, that's your first (and longest) step out of the way.
 
 #### 2) Loading your config and starting an experiment
 
-Imagine you want to start a new experiment, for example an overfitting experiment. Let us prepare a config file for this experiment, which we will store in `configs/overfit.yaml`.
+Imagine you want to start a new experiment, for example an overfitting experiment. Let us prepare a config file for this
+experiment, which we will store in `configs/overfit.yaml`.
 
 ```yaml
 ---  # Experiment config - configs/overfit.yaml
 
 experiment_path: "logs/overfit"
 data:
    number_of_samples: 2
@@ -231,26 +313,28 @@
 ```
 
 In the example above, many if the characteristics of an "experiment config" can already be seen.
 In contrast to the default config, it :
 
 - is short and contains only the values that are modified ;
 - cannot add new parameter, only update existing ones.
-In this config file, what is being done in this specific experiment is clear at a glance, regardless of the complexity of the default config. For now, your project's folder should look something like this :
+In this config file, what is being done in this specific experiment is clear at a glance, regardless of the complexity
+of the default config. For now, your project's folder should look something like this :
 
 ```markdown
 project_root
 ├── configs
 │   ├── default.yaml
 │   └── overfit.yaml
 ├── main.py
 └── ...
 ```
 
-And now, let's get down to business and see what the code part of things will look like. Before using YAECS, your `main.py` might have looked like this :
+And now, let's get down to business and see what the code part of things will look like. Before using YAECS, your
+`main.py` might have looked like this :
 
 ```python
 # import some stuff
 
 def main():
     # runs the project's code
     ...
@@ -273,106 +357,74 @@
 if __name__ == "__main__":
     # load the config
     config = make_config("configs/overfit.yaml",
                          default_config="configs/default.yaml")
     main(config)
 ```
 
-Two very important notes here :
-
-- **the code above will not work**, because up to now I ommited an important point to avoid confusion. To see how to fix our current setup, please read the next section about sub-configs ;
-- here we use make_config to simplify things, but it will not allow us to leverage all of YAECS' features. In the "intermediate" section of this guide, we will learn how to load configs with other, more powerful functions.
+And there you go ! You have a working example !
 
-At this point, you probably have many questions... so let's head on to the next sections to answer them !
+Important note : here we use make_config to simplify things, but it will not allow us to leverage all of YAECS'
+features.
+In the "intermediate" section of this guide, we will learn how to create configs with other, more powerful constructors.
 
 #### 3) An omnipresent feature for config organisation : sub-configs
 
-The only change we have to do to make everything work is in the configs. I'll first show you the working version, then I'll explain the difference and why it's important.
+At this point, we should explain the important aspect of a "sub-config". As you can see from our example above, there 
+are parameters in our config that contain other parameters (for example `model`, or `data`). They are defined as YAML
+dictionaries, but don't be fooled : they will not be parsed as python `dict` by YAECS, but as sub-configs. It *is*
+possible to declare a parameter in the YAML file that will take as value a python `dict`, but to do that, you need to 
+*tag* it.
+
+A YAML tag, in YAML, is a small statement starting with a `!` used to "tag" the following value. In YAECS, we use those 
+tags to differentiate sub-configs from simple dictionaries. Indeed, in YAML, declaring `dict: a: 1` or its equivalent 
+`dict: {a: 1}` will result in YAECS creating a sub-config called `dict`, which contains a param called `a` with value 1.
+To instead define a param called `dict` containing a python dict `{"a": 1}`, you need to *tag* this dictionary using a
+type-hint : `dict: !type:dict {a: 1}`. You can learn more about type hints in the corresponding part of this tutorial TODO.
+
+Dictionaries **are not** sub-configs. Sub-configs can check and process their parameters, and they can be accessed using
+the `config.subconfig.parameter` syntax. They are also restricted to only the parameters which have been defined in the
+defaut config. In an experiment config, you can access and modify a single parameter of a subconfig, and the others will
+take their default values. When you replace the value of a dict in the experiment config, on the contrary, you have to
+write the complete dict, because dict keys have no default values.
 
-In the default config :
+Knowing when you want a sub-config and when you want a dict can be tricky and requires experience, but most of the time
+you can't go much wrong by simply sub-configs, which is why this was chosen as the default behaviour.
 
-```yaml
----  # Default config - configs/default.yaml
+Sub-configs allow you to organise your parameters into categories and sub-categories, which will come in handy in
+basically all your projects.
 
-experiment_path: null
-use_gpu: true
-do_train: true
-do_val: true
-do_test: false
-
-model: !model
-   type: ResNet
-   layers: 10
-   activations: ReLU
-
-data: !data
-   size: [64, 64]
-   number_of_samples: null
-   flip_probability: 0.5
-   rotate_probability: 0
-
-train: !train
-   epochs: 100
-   batch_size: 32
-   optimiser: !optimiser
-      type: Adam
-      learning_rate: .001
-      betas: [0.9, 0.999]
-      weight_decay: 0
-```
-
-... and in the experiment config :
-
-```yaml
----  # Experiment config - configs/overfit.yaml
-
-experiment_path: "logs/overfit"
-data: !data
-   number_of_samples: 2
-   flip_probability: 0
-train.batch_size: 2
-```
-
-What we did is rather simple : for every parameter which contains other parameters (referred to as "sub-configs"), we added a so-called YAML tag. A YAML tag, in YAML, is a small statement starting with a `!` used to "tag" the following value. In YAECS, we use those tags to differentiate sub-configs from simple dictionaries.
-
-Indeed, in YAML, declaring `dict: a: 1` or its equivalent `dict: {a: 1}` defines a python `dict` by default. To define a YAECS sub-config instead, you need to *tag* this dictionary using a tag that is **exactly the parameter's name**, for example `subconfig: !subconfig {a: 1}`.
-
-Dictionaries **are not** sub-configs. Sub-configs can check and process their parameters, and they can be accessed using the `config.subconfig.parameter` syntax. They are also restricted to only the parameters which have been defined in the defaut config. In an experiment config, you can access and modify a single parameter of a subconfig, and the others will take their default values. When you replace the value of a dict in the experiment config, on the contrary, you have to write the complete dict, because dict keys have no default values.
-
-Knowing when you want a sub-config and when you want a dict can be tricky and requires experience, but most of the time you can't go much wrong by simply declaring **all** your dicts as sub-configs instead.
-
-Sub-configs allow you to organise your parameters into categories and sub-categories, which will come in handy in basically all your projects.
-
-In the following, we re-write the previous experiment config using **3 ways** to declare parameters in sub-configs. All three of them will work both in default or experiment configs.
+There are **3 ways** to declare parameters in sub-configs in your YAML files. All three of them will work both in
+default or experiment configs, and they have the same behaviour. We demonstrate all three of them below :
 
 Using the dot convention (optimal when there is one or two parameters in the sub-config) :
 
 ```yaml
 ---  # Experiment config with dot convention only
 
 experiment_path: "logs/overfit"
 data.number_of_samples: 2
 data.flip_probability: 0
 train.batch_size: 2
 ```
 
-Using tagged dictionnaries (optimal when there are two parameters or more) :
+Using **untagged** dictionnaries (optimal when there are two parameters or more) :
 
 ```yaml
 ---  # Experiment config with tagged dictionnaries only
 
 experiment_path: "logs/overfit"
-data: !data
+data:
    number_of_samples: 2
    flip_probability: 0
-train: !train
+train:
    batch_size: 2
 ```
 
-Using tagged documents (optimal when the sub-config is complex and/or contains other sub-configs) :
+Using **tagged** documents (optimal when the sub-config is complex and/or contains other sub-configs) :
 
 ```yaml
 ---  # Start of a first document, without any tag, therefore within the main config's scope
 
 experiment_path: "logs/overfit"
 
 
@@ -380,87 +432,121 @@
 number_of_samples: 2
 flip_probability: 0
 
 --- !train  # end of the data document's scope, start of a new document tagged as train
 batch_size: 2
 ```
 
-Those 3 options will result in the exact same behaviour ! Combining them will allow you to adapt your config to complex situations while keeping things clean.
+Notice how, in this last case, you do need to tag the document to indicate the name of the create sub-configs. This tag
+will create a sub-config and place all parameters in the document in this sub-config. You can see this as some sort of
+scope. 
+
+Those 3 options will result in the exact same behaviour ! Combining them will allow you to adapt your config to complex
+situations while keeping things clean.
 
-Now that we have seen how to declare configs and sub-configs, and how to load them into the code, let's wrap up this first part of our beginner tutorial with the printing, saving and reproducing of configs.
+Now that we have seen how to declare configs and sub-configs, and how to load them into the code, let's wrap up this
+first part of our beginner tutorial with the printing, saving and reproducing of configs.
 
 #### 4) Using, printing, saving, reproducing
 
-To wrap up this first part of our tutorial, let's go over four basic operations that you will need over the course of your experiments : accessing your parameters, printing your config details, saving your config and using it to reproduce an experiment.
+To wrap up this first part of our tutorial, let's go over four basic operations that you will need over the course of
+your experiments : accessing your parameters, printing your config details, saving your config and using it to reproduce
+an experiment.
 
 ##### Accessing params
 
-Accessing parameters can be done either using standard object operations (such as `config.param` or `getattr(config, "param"`) or dictionnary operations (such as `config["param"]` or `config.get("param")`). Actually, many dict methods are implemented for configs, such as `items`, `keys` or `values`. Nevertheless, `Configuration` does not inherit from `dict`, therefore we also provide the `get_dict` method in case you need your config to be a dict (for example to pass it to a third-party library which explicitly checks for a `dict` object).
+Accessing parameters can be done either using standard object operations (such as `config.param` or
+`getattr(config, "param"`) or dictionnary operations (such as `config["param"]` or `config.get("param")`). Actually,
+many dict methods are implemented for configs, such as `items`, `keys` or `values`. Nevertheless, `Configuration` does
+not inherit from `dict`, therefore we also provide the `get_dict` method in case you need your config to be a dict (for
+example to pass it to a third-party library which explicitly checks for a `dict` object).
 
 ##### Printing configs
 
-You can use `config.details()` to generate a string that describes your config. If you use `print(config.details())` with our previous config, here is what you get : TODO
+You can use `config.details()` to generate a string that describes your config. If you use `print(config.details())`
+with our previous config, here is what you get : TODO
 
-Let's discuss in more details the first thing displayed : the config hierarchy. It is a list of path and dicts which indicates the order in which different sources were used to create this config. The first one in the list is always the default config. It is also the only one in the list which is allowed to set new parameters. All the other sources in the list can only modify parameters which have been set by the default config. This list is quite practical to get a condensed gist of the idea behind your experiment. For example, if you read :
+Let's discuss in more details the first thing displayed : the config hierarchy. It is a list of path and dicts which
+indicates the order in which different sources were used to create this config. The first one in the list is always the
+default config. It is also the only one in the list which is allowed to set new parameters. All the other sources in the
+list can only modify parameters which have been set by the default config. This list is quite practical to get a
+condensed gist of the idea behind your experiment. For example, if you read :
 
 ```bash
 - configs/default.yaml
 - configs/overfit.yaml
 - {data.flip_probability: 0.5}
 ```
 
-... you might already be able to figure out most parameters, and also the intent behind the experiment, before having seen any of the parameters at all ! Here the experimenter simply wanted to do an overfitting experiment, and they activated the flip augmentation (perhaps using the command line interface) to see if this would affect the model's capability to overfit.
+... you might already be able to figure out most parameters, and also the intent behind the experiment, before having
+seen any of the parameters at all ! Here the experimenter simply wanted to do an overfitting experiment, and they
+activated the flip augmentation (perhaps using the command line interface) to see if this would affect the model's
+capability to overfit.
 
 ##### Saving configs
 
-Saving a config is as simple as calling `config.save("save_path.yaml")`. This will save two files : `path.yaml` which contains the full list of all parameters as well as some metadata, and `save_path_hierarchy.yaml` which contains the config hierarchy we talked about before. The latter is saved in a separate file for easy access because of how practical it is.
+Saving a config is as simple as calling `config.save("save_path.yaml")`. This will save two files : `path.yaml` which
+contains the full list of all parameters as well as some metadata, and `save_path_hierarchy.yaml` which contains the
+config hierarchy we talked about before. The latter is saved in a separate file for easy access because of how practical
+it is.
 
 ##### Reproducing experiments
 
 Finally, to reproduce an experiment, all you have to do is load the config you saved when running it :
 
 ```python
 reproduced_config = make_config("save_path.yaml",
                                 default_config="configs/default.yaml")
 ```
 
-The saved config will be used as an experiment config and overwrite the values of the default config with the values of the experiment to reproduce.
+The saved config will be used as an experiment config and overwrite the values of the default config with the values of
+the experiment to reproduce.
 
-The most certain way to achieve perfect reproducility regardless of the coding practices of the experimenter is to go back to the git commit where the experiment was performed and use the saved config file. However, by design YAECS makes it simpler to achieve perfect reproductibility *without* leaving your current branch. This requires additional rigor to be observed by the experimenter, which we summarise as a set of good practices which you can find here TODO.
-
-This ends the first part of our tutorial, which aimed at teaching you the basics required to integrate YAECS in a small project and introduce you to its most fundamental features. As of now though, nothing distinguishes it from its alternatives like Hydra or YACS. If you want to know more, follow us into the second part of our tutorial : TODO
+The most certain way to achieve perfect reproducility regardless of the coding practices of the experimenter is to go
+back to the git commit where the experiment was performed and use the saved config file. However, by design YAECS makes
+it simpler to achieve perfect reproductibility *without* leaving your current branch. This requires additional rigor to
+be observed by the experimenter, which we summarise as a set of good practices which you can find here TODO.
+
+This ends the first part of our tutorial, which aimed at teaching you the basics required to integrate YAECS in a small
+project and introduce you to its most fundamental features. As of now though, nothing distinguishes it from its
+alternatives like Hydra or YACS. If you want to know more, follow us into the second part of our tutorial : TODO
 
 ### Intermediate features for more scalability
 
-Now that you understand the basics of setting up config files for your projects and loading them, let us see how you can make your life easier with a few more very practical features.
+Now that you understand the basics of setting up config files for your projects and loading them, let us see how you can
+make your life easier with a few more very practical features.
 
 In this second "intermediate" part of this tutorial, we will :
 
 1) go over different ways to create configs
 2) explain how to use our command line interface
 3) introduce one of our most interesting features : parameter processing
 4) suggest a workflow to experiment while taking advantage of YAECS' features
 5) explain how to split your config across multiple files
 Let us get started.
 
 #### 1) Sub-classing Configuration and using constructors
 
-For now, we have only created configs by passing a dict or a path to our convenient `make_config` utility function. But in most projects, this won't be the most flexible way to proceed. In any project that you intend to be working on for a while, we suggest you create your own subclass for the Configuration class. This is slightly more cumbersome, but also much more scalable and will keep your `main.py` cleaner. Let's create a new file, for example called `config.py`.
+For now, we have only created configs by passing a dict or a path to our convenient `make_config` utility function. But
+in most projects, this won't be the most flexible way to proceed. In any project that you intend to be working on for a
+while, we suggest you create your own subclass for the Configuration class. This is slightly more cumbersome, but also
+much more scalable and will keep your `main.py` cleaner. Let's create a new file, for example called `config.py`.
 
 ```markdown
 project_root
 ├── configs
 │   ├── default.yaml
 │   └── overfit.yaml
 ├── main.py
 ├── config.py
 └── ...
 ```
 
-This file should be seen as a part of your codebase and commited to the project's repository. To re-use the vocabulary introduced in section 0 (TODO), it is part of the support. In this file, let's create a basic sub-class.
+This file should be seen as a part of your codebase and commited to the project's repository. To re-use the vocabulary
+introduced in section 0 (TODO), it is part of the support. In this file, let's create a basic sub-class.
 
 ```python
 from yaecs import Configuration
 
 class MyProjectConfig(Configuration):
     @staticmethod
     def get_default_config_path():
@@ -469,19 +555,23 @@
     def parameters_pre_processing(self):
         return {}
 
     def parameters_post_processing(self):
         return {}
 ```
 
-Because the default config can also be seen as a part of the support (because there is one and only one default config per project and it should be the same for all users), it is required to hard-code it in the subclass definition. There should never be a use case for using a different default config than this one.
+Because the default config can also be seen as a part of the support (because there is one and only one default config
+per project and it should be the same for all users), it is required to hard-code it in the subclass definition. There
+should never be a use case for using a different default config than this one.
 
-The `parameters_pre_processing` and `parameters_post_processing` methods are not required, but they'll come in handy, though we'll leave them empty for now. You will learn more about them in a future section (TODO).
+The `parameters_pre_processing` and `parameters_post_processing` methods are not required, but they'll come in handy,
+though we'll leave them empty for now. You will learn more about them in a future section (TODO).
 
-Now that our subclass is ready, let's come back to our `main.py` and present its 3 constructors, starting with the simplest : `load_config`.
+Now that our subclass is ready, let's come back to our `main.py` and present its 3 constructors, starting with the
+simplest : `load_config`.
 
 ```python
 # import some stuff
 from config import MyProjectConfig
 
 def main(config):
     # runs the project's code
@@ -489,25 +579,43 @@
 
 if __name__ == "__main__":
     # load the config
     config = MyProjectConfig.load_config("configs/overfit.yaml")
     main(config)
 ```
 
-This constructor takes as argument one or several paths or dictionaries, and merges them one after the other into the default config. Then, it merges the command line arguments (TODO), and finally, it performs post-processing operations (TODO).  The default config path does not need to be specified because it is hardcoded into the subclass.
-
-The fact that the default config path is not clearly written in the `main.py` can be seen as unclear. In particular, if a user unfamiliar with YAECS reviews the project, they might not expect the default values to be initialised based on a path hardcoded in a different file. To avoid this issue, you can choose to still pass the default config explicitly using the `default_config_path` keyword argument, or you can use the `build_from_configs` constructor.
-
-`build_from_configs` also expects one or several config paths or dictionaries as argument, but contrary to `load_config` it will not use the hard-coded default config, instead using the first provided path or dictionary as the default config. Otherwise, it behaves like `load_config`. Under the hood, this is what `make_config` uses : it generates a template sub-class and calls its `build_from_configs` constructor with its arguments. This is why `make_config` will also implicitly merge command line parameters (TODO) and perform post-processing (TODO).
-
-Finally, a most useful constructor is the `build_from_argv`. Its base usage is to call it without argument : `MyProjectConfig.build_from_argv()`. As its name implies, it expects to receive the config to merge from the command line interface. When using this constructor, the command will be parsed for a pattern of the form `--config path/to/config.yaml`, and the provided path will be used as experiment config. You can also provide several paths separated by comas : `--config path1,path2`.
-
-By default, `build_from_argv` will raise an error if no such pattern is detected. This is a safety measure against oversights. However, you can also configure a fallback to be used everytime the `config` flag is not set : `MyProjectConfig.build_from_argv(fallback="path/to/fallback/config.yaml")`.
-
-`build_from_argv` also accepts config paths or dictionaries as positional arguments. Those configs are merged into the default config first, followed by the one given in the command line, followed by the command line params (TODO). Those features make it the most convenient and flexible constructor to use in general, thus we will henceforth consider that your `main.py` looks like this :
+This constructor takes as argument one or several paths or dictionaries, and merges them one after the other into the
+default config. Then, it merges the command line arguments (TODO), and finally, it performs post-processing operations
+(TODO).  The default config path does not need to be specified because it is hardcoded into the subclass.
+
+The fact that the default config path is not clearly written in the `main.py` can be seen as unclear. In particular, if
+a user unfamiliar with YAECS reviews the project, they might not expect the default values to be initialised based on a
+path hardcoded in a different file. To avoid this issue, you can choose to still pass the default config explicitly
+using the `default_config_path` keyword argument, or you can use the `build_from_configs` constructor.
+
+`build_from_configs` also expects one or several config paths or dictionaries as argument, but contrary to `load_config`
+it will not use the hard-coded default config, instead using the first provided path or dictionary as the default
+config. Otherwise, it behaves like `load_config`. Under the hood, this is what `make_config` uses : it generates a
+template sub-class and calls its `build_from_configs` constructor with its arguments. This is why `make_config` will
+also implicitly merge command line parameters (TODO) and perform post-processing (TODO).
+
+Finally, a most useful constructor is the `build_from_argv`. Its base usage is to call it without argument :
+`MyProjectConfig.build_from_argv()`. As its name implies, it expects to receive the config to merge from the command
+line interface. When using this constructor, the command will be parsed for a pattern of the form
+`--config path/to/config.yaml`, and the provided path will be used as experiment config. You can also provide several
+paths separated by comas : `--config path1,path2`.
+
+By default, `build_from_argv` will raise an error if no such pattern is detected. This is a safety measure against
+oversights. However, you can also configure a fallback to be used everytime the `config` flag is not set :
+`MyProjectConfig.build_from_argv(fallback="path/to/fallback/config.yaml")`.
+
+`build_from_argv` also accepts config paths or dictionaries as positional arguments. Those configs are merged into the
+default config first, followed by the one given in the command line, followed by the command line params (TODO). Those
+features make it the most convenient and flexible constructor to use in general, thus we will henceforth consider that
+your `main.py` looks like this :
 
 ```python
 # import some stuff
 from config import MyProjectConfig
 
 def main(config):
     # runs the project's code
@@ -517,53 +625,80 @@
     # load the config
     config = MyProjectConfig.build_from_argv(fallback="configs/overfit.yaml")
     main(config)
 ```
 
 #### 2) Using the command line interface
 
-In this section, you will learn to control your config from the command line interface (CLI). There are two aspects to this : modifying parameters from the CLI, and choosing your experiment config file from the CLI. We saw how to do the latter in the previous section already with the `build_from_argv` constructor (TODO), so here we focus on the former.
+In this section, you will learn to control your config from the command line interface (CLI). There are two aspects to
+this : modifying parameters from the CLI, and choosing your experiment config file from the CLI. We saw how to do the
+latter in the previous section already with the `build_from_argv` constructor (TODO), so here we focus on the former.
 
 Let's assume you usually start your python code using something like :
 
 ```bash
 python main.py
 ```
 
-If your config is a YAECS config, then any parameter you pass as an argument to your script will be merged at the end of the config creation, if it corresponds to a parameter. Continuing with the example from the previous tutorial section, here's what you would do to start a new experiment, still with our overfit experiment config but this time with some flip probability.
+If your config is a YAECS config, then any parameter you pass as an argument to your script will be merged at the end of
+the config creation, if it corresponds to a parameter. Continuing with the example from the previous tutorial section,
+here's what you would do to start a new experiment, still with our overfit experiment config but this time with some
+flip probability.
 
 ```bash
 python main.py --experiment_path logs/overfit_with_flip --data.flip_probability 0.5
 ```
 
-Here we of course change the name of the experiment, and then also our flip probability. The YAECS parser is quite flexible, and supports expressions such as `--name value`, `--name=value`, the "\*" wildcard in a param name to match several params at once (although in shells it needs to be escaped) and of course the dot-convention to access params of sub-configs.
-
-Most of the time, changing parameters from the CLI is just that simple. It only gets a bit more tricky if you want to change the type of a parameter (ie. replace a param that was a float with a string for instance), or replace entire lists or dicts from the CLI. For those operations, please refer to our dedicated section : TODO.
-
-*Note :* if you want to replace a param with the boolean value `True`, you don't need to write it explicitly. If you don't provide a new value, the CLI parser will assume you want to set the parameter to `True`. For example, to perform the test in our earlier example :
+Here we of course change the name of the experiment, and then also our flip probability. The YAECS parser is quite
+flexible, and supports expressions such as `--name value`, `--name=value`, the "\*" wildcard in a param name to match
+several params at once (although in shells it needs to be escaped) and of course the dot-convention to access params of
+sub-configs.
+
+Most of the time, changing parameters from the CLI is just that simple. It only gets a bit more tricky if you want to
+change the type of a parameter (ie. replace a param that was a float with a string for instance), or replace entire
+lists or dicts from the CLI. For those operations, please refer to our dedicated section : TODO.
+
+*Note :* if you want to replace a param with the boolean value `True`, you don't need to write it explicitly. If you
+don't provide a new value, the CLI parser will assume you want to set the parameter to `True`. For example, to perform
+the test in our earlier example :
 
 ```bash
 python main.py --do_test
 ```
 
 #### 3) Parameter processing is awesome
 
-Here we present what we believe to be one of YAECS' main improvement over its competitors : parameters processing.  The idea is quite simple : most of the time, it is really useful to be able to perform some kind of processing on your parameters before using them, and it only makes sense that these operations should be performed by the config system. Here is why. The config should be prepared such that the code can access it in a simple, reliable and well-organised well. But at the same time, the config should be prepared by a human in a clear interface using the YAML language. In many cases, those two conditions do not fully align, and therefore it makes sense that the config system should be tasked with translating the config as seen by the human operator into the config as used by the code.
+Here we present what we believe to be one of YAECS' main improvement over its competitors : parameters processing.  The
+idea is quite simple : most of the time, it is really useful to be able to perform some kind of processing on your
+parameters before using them, and it only makes sense that these operations should be performed by the config system.
+Here is why. The config should be prepared such that the code can access it in a simple, reliable and well-organised
+well. But at the same time, the config should be prepared by a human in a clear interface using the YAML language. In
+many cases, those two conditions do not fully align, and therefore it makes sense that the config system should be
+tasked with translating the config as seen by the human operator into the config as used by the code.
 
 Here are a few example use cases :
 
 - if you want to check the value of a param for safety (see `check` in example below)
-- if you want to convert a param to another format (degrees to radians, human-readable to machine-readable etc.) (see `convert`)
+- if you want to convert a param to another format (degrees to radians, human-readable to machine-readable etc.)
+(see `convert`)
 - if you want to use the info in your YAML-supported values to create custom objects (see `instanciate`)
 - if you want to control how the config is created via parameters in the config itself (see next section TODO)
-- if you want to prepare or initialise stuff based on the content of the config (for example by creating folders for your logs) (see `register_as_experiment_path`)
+- if you want to prepare or initialise stuff based on the content of the config (for example by creating folders for
+your logs) (see `register_as_experiment_path`)
 
-All these use cases are covered by either using parameters **pre-processing**, or parameters **post-processing**. In this part, we won't go in too much details about the difference between those. Instead, we'll simply provide a few examples, to make things clearer. We perform a deeper dive into this mecanism here (TODO).
-
-Processing is very simple : all you have to do is associate the names of your parameters with functions. Those functions are required to accept exactly one argument (the previous value of the param), and return exactly one value (the processed value of the param). Then, during the config creation operations, the specified function will be used when the specified name is encountered. This mapping between name and function is configured using the dictionary returned by the `parameters_pre_processing` and `parameters_post_processing` methods in your subclass. Here is an example modified config.py to implement the above-mentioned processing functions :
+All these use cases are covered by either using parameters **pre-processing**, or parameters **post-processing**. In
+this part, we won't go in too much details about the difference between those. Instead, we'll simply provide a few
+examples, to make things clearer. We perform a deeper dive into this mecanism here (TODO).
+
+Processing is very simple : all you have to do is associate the names of your parameters with functions. Those functions
+are required to accept exactly one argument (the previous value of the param), and return exactly one value (the
+processed value of the param). Then, during the config creation operations, the specified function will be used when the
+specified name is encountered. This mapping between name and function is configured using the dictionary returned by the
+`parameters_pre_processing` and `parameters_post_processing` methods in your subclass. Here is an example modified
+config.py to implement the above-mentioned processing functions :
 
 ```python
 from pathlib import Path
 from yaecs import Configuration
 
 def check(param_to_check):
     if param_to_check < 0:
@@ -591,46 +726,77 @@
     def parameters_post_processing(self):
         return {
             "experiment_path": self.register_as_experiment_path,
             "*_path": instanciate,
         }
 ```
 
-As you can see, processing is a flexible feature that can enable very complex behaviours depending on your needs. Use the provided library of pre-built processing functions TODO, or build your own ! 
+As you can see, processing is a flexible feature that can enable very complex behaviours depending on your needs. Use
+the provided library of pre-built processing functions TODO, or build your own ! 
 
 #### 4) Our proposed workflow to use YAECS efficiently
 
-As an experimenter, your goal should be to easily start any experiment you want and enrich your code with new innovative features without losing reproducibility for older experiments. In this section, we propose a workflow that satisfies these conditions and address some common issues and concerns.
-
-**STEP 1 : Preparing your project.** At the start of your project, you want to populate a basic default config with parameters you think you might need. After one or two projects, you will probably have a template or strongly established habits to help you do that. Those parameters include for example learning rates, numbers of epochs, batch sizes, data processing parameters, a path where to save your experiment results etc.. Sometimes, you might use existing research code as a basis for your work. In this case, if said codebase does not have a config, you can simply browse the code and extract all values from it to the config.
-
-**STEP 2 : Starting an experiment.** To start your first experiment, you might have an idea of something you'd like to try. Often, this might be for example reproducing the results of a paper. To do this, prepare an experiment config file that reproduces the values you want to use, then use this file as your experiment config (for example by using build_from_argv and calling your code with the `--config` flag TODO).
-
-**STEP 3 : Improvising from there.** Very often, an idea sparking an experiment doesn't work right from the start. You might need to tweak the learning rate, or train slightly longer. We find that, instead of creating a new YAML file for each small change or changing your experiment configs, it is easier and better practice to make those changes from the CLI TODO. So long as your experiment does not deviate from the experiment config file, it makes sense to iteratively tweak things from the CLI. This encourages experiment config files to actually take the role of configuring not experiments but *series* of experiments. Therefore : 
+As an experimenter, your goal should be to easily start any experiment you want and enrich your code with new innovative
+features without losing reproducibility for older experiments. In this section, we propose a workflow that satisfies
+these conditions and address some common issues and concerns.
+
+**STEP 1 : Preparing your project.** At the start of your project, you want to populate a basic default config with
+parameters you think you might need. After one or two projects, you will probably have a template or strongly
+established habits to help you do that. Those parameters include for example learning rates, numbers of epochs, batch
+sizes, data processing parameters, a path where to save your experiment results etc.. Sometimes, you might use existing
+research code as a basis for your work. In this case, if said codebase does not have a config, you can simply browse the
+code and extract all values from it to the config.
+
+**STEP 2 : Starting an experiment.** To start your first experiment, you might have an idea of something you'd like to
+try. Often, this might be for example reproducing the results of a paper. To do this, prepare an experiment config file
+that reproduces the values you want to use, then use this file as your experiment config (for example by using
+`build_from_argv` and calling your code with the `--config` flag TODO).
+
+**STEP 3 : Improvising from there.** Very often, an idea sparking an experiment doesn't work right from the start. You
+might need to tweak the learning rate, or train slightly longer. We find that, instead of creating a new YAML file for
+each small change or changing your experiment configs, it is easier and better practice to make those changes from the
+CLI TODO. So long as your experiment does not deviate from the experiment config file, it makes sense to iteratively
+tweak things from the CLI. This encourages experiment config files to actually take the role of configuring not
+experiments but *series* of experiments. Therefore : 
 - the default config contains the information relative to the project
 - the experiment config contains the information relative to the series of experiment
 - the CLI contains the information relative to a specific iteration
 
-**STEP 4 : Adding features and parameters.** It is naive to think you can build your code once and then find the best solution simply by interacting with the config. You will always need to make changes to the code, to solve bugs, add features and refactor. It is however possible, by being rigorous, to ensure perfect *forward reproducibility*. Forward reproducibility means that at any point during development, you can still load old saved configs from past experiments and they will be perfectly reproduced. To achieve this, you should apply the following rules :
+**STEP 4 : Adding features and parameters.** It is naive to think you can build your code once and then find the best
+solution simply by interacting with the config. You will always need to make changes to the code, to solve bugs, add
+features and refactor. It is however possible, by being rigorous, to ensure perfect *forward reproducibility*. Forward
+reproducibility means that at any point during development, you can still load old saved configs from past experiments
+and they will be perfectly reproduced. To achieve this, you should apply the following rules :
 - never rename a parameter or change its default value : always change values from experiment configs ;
-- when adding a new feature controled by a new parameter, always make sure that the default value disactivates the new feature. For example, if you want to add a new data augmentation function, the new parameter "use_new_augmentation" should be False by default ;
-- if you change your post-processing functions TODO, make sure that they still have the same behaviour for values used previously for your parameters.
-
-For a while, following these rules might be simple. For long projects however, maintaining full forward reproducibility might be challenging. In our advanced tips for larger projects TODO, we provide more advice to scale up to massive projects.
+- when adding a new feature controled by a new parameter, always make sure that the default value disactivates the new
+feature. For example, if you want to add a new data augmentation function, the new parameter "use_new_augmentation"
+should be False by default ;
+- if you change your post-processing functions TODO, make sure that they still have the same behaviour for values used
+previously for your parameters.
+
+For a while, following these rules might be simple. For long projects however, maintaining full forward reproducibility
+might be challenging. In our advanced tips for larger projects TODO, we provide more advice to scale up to massive
+projects.
 
 
 #### 5) Splitting a config across multiple files
 
-To wrap up with our intermediate features, we would like to present how to split a config across multiple files. This is useful to organise large configs containing hundreds of parameters, which can make your config file really long. Usually, we recommend splitting across a config across 4 files :
-- a base file that contains the most general parameters (debug mode, is the experiment a training, a test or an inference, path to the experiment results, cpu/gpu etc.) ;
+To wrap up with our intermediate features, we would like to present how to split a config across multiple files. This is
+useful to organise large configs containing hundreds of parameters, which can make your config file really long.
+Usually, we recommend splitting across a config across 4 files :
+- a base file that contains the most general parameters (debug mode, is the experiment a training, a test or an
+inference, path to the experiment results, cpu/gpu etc.) ;
 - a file for data-related parameters (data paths, sample descriptions, processing parameters etc.) ;
 - a file for model-related parameters (architecture, layers, normalisation etc.) ;
-- a file for run-related parameters (training params such as epochs, optimiser or batch sizes ; validation params ; inference parms).
+- a file for run-related parameters (training params such as epochs, optimiser or batch sizes ; validation params ;
+inference parms).
 
-Generally speaking, to build a config you only give your Configuration object one path. Therefore, how can you let your config system know where to look for other files for other parameters ? The answer lie in a feature we've already seen : parameters processing :). Let us assume the 4 following configs :
+Generally speaking, to build a config you only give your Configuration object one path. Therefore, how can you let your
+config system know where to look for other files for other parameters ? The answer lie in a feature we've already seen :
+parameters processing :). Let us assume the 4 following configs :
 
 ```
 project_root
 ├── configs
 │   ├── default
 │   │   ├── base.yaml
 │   │   ├── data.yaml
@@ -667,24 +833,27 @@
 ...
 normalisation: BatchNorm
 ```
 
 ```yaml
 ---  # Run file (configs/default/run.yaml)
 
-train: !train
+train:
     batch_size: 8
     epochs: 100
     ...
 val.batch_size: 32
 test.batch_size: 32
 infer.batch_size: 1
 ```
 
-You might have noticed that the base file - ie. the file we will give to the config system - contains paths to the other files. All we need to do is tell the config system that those are not just any parameter : they are actually paths that the config system should use to find the rest of the config. To do this, you can simply assign them the `register_as_additional_config_file` pre-processing function, for example like this :
+You might have noticed that the base file - ie. the file we will give to the config system - contains paths to the other
+files. All we need to do is tell the config system that those are not just any parameter : they are actually paths that
+the config system should use to find the rest of the config. To do this, you can simply assign them the
+`register_as_additional_config_file` pre-processing function, for example like this :
 ```python
 from yaecs import Configuration
 
 class MyProjectConfig(Configuration):
     @staticmethod
     def get_default_config_path():
         return "configs/default/base.yaml"
@@ -693,21 +862,24 @@
         return {
             "*_config_file": self.register_as_additional_config_file,
         }
 
     def parameters_post_processing(self):
         return {}
 ```
-And there you go ! Now all parameters that end with `_config_file` will be recognised as you trying to add the corresponding paths to the config.
+And there you go ! Now all parameters that end with `_config_file` will be recognised as you trying to add the
+corresponding paths to the config.
 
-This ends the Intermediate section of our tutorial. By now, you already know most of what you need to work efficiently with YAECS. To become a real pro, there is only one section left !
+This ends the Intermediate section of our tutorial. By now, you already know most of what you need to work efficiently
+with YAECS. To become a real pro, there is only one section left !
 
 ### Advanced tips for larger projects
 
-Now that you might feel better acquainted with the core features of YAECS we can give you more details about a couple of very nice features which can save you a lot of time in certain particular situations.
+Now that you might feel better acquainted with the core features of YAECS we can give you more details about a couple of
+very nice features which can save you a lot of time in certain particular situations.
 
 In this third "advanced" part we will :
 
 1) tell you more about parameters processing, as well as type-checking
 2) give examples to easily configure complex elements such as dataset versions or machine-specific configs
 3) present config variations, which is useful to run sweeps over values of a parameter for example
 4) showcase our WIP new feature : tracking integration
@@ -1186,15 +1358,15 @@
         "*_config_path": self.register_as_additional_config_file
     }
 ```
 
 This way, any param ending with “_config_path” anywhere in the config would be
 interpreted as a path to a new config file.
 
-### Defining nested configs
+### Defining nested configs (DEPRECATED)
 
 Another desirable property of our configuration is the ability to nest
 configurations inside other configurations. Reusing the example of section 2.
 of the previous advanced feature, it is easy to see that as the number of
 parameters grows, it would be nice to not only organise those parameters in
 different files on the disk, but also organise them in different “sub-configs”
 in our Configuration object. That way, a function that requires access to
```

### Comparing `yaecs-4.0.2/LICENSE.md` & `yaecs-4.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/PKG-INFO` & `yaecs-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 4.0.2
+Version: 4.1.0
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-4.0.2/README.md` & `yaecs-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/Makefile` & `yaecs-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/conf.py` & `yaecs-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/getting_started.md` & `yaecs-4.1.0/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/index.rst` & `yaecs-4.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/license.md` & `yaecs-4.1.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/make.bat` & `yaecs-4.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/yaecs.rst` & `yaecs-4.1.0/docs/yaecs.rst`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/docs/yaecs_config.rst` & `yaecs-4.1.0/docs/yaecs_config.rst`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/pyproject.toml` & `yaecs-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/resources/yaecs_constructor_overview.png` & `yaecs-4.1.0/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/setup.py` & `yaecs-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/short-readme.md` & `yaecs-4.1.0/short-readme.md`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/unittests/config/conftest.py` & `yaecs-4.1.0/unittests/config/conftest.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/unittests/config/test_config.py` & `yaecs-4.1.0/unittests/config/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     ]
 
 
 def test_merge_from_command_line(caplog, yaml_default, yaml_experiment):
 
     def mcl(cfg, string):
         # pylint: disable=protected-access
-        to_merge = cfg._gather_command_line_dict(string_to_merge=string)
+        to_merge = cfg._gather_command_line_dict(to_merge=string)
         if to_merge:
             logging.getLogger("yaecs.config").info(f"Merging from command line : {to_merge}")
             cfg._merge(to_merge)
 
     caplog.clear()
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
@@ -262,49 +262,42 @@
         config_2 = load_config(yaml_experiment, default_config=yaml_default)
         mcl(config_2, config.get_command_line_argument(do_return_string=True))
     assert caplog.text.count("WARNING") == 0
     caplog.clear()
     check_integrity(config_2, 1, 0.6, p_4="test test")
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
-        mcl(config_2, "--param1 2 --*param2=none --*param3=none !str "
-                      "--*param4= '[ 1!int  ,0.5 !float, {string:\\'"
-                      "[as !str}!dict]' !list")
+        mcl(config_2, "--param1 2 --*param2=null --*param3=\\\"null\\\" "
+                      "--*param4= [ 1  ,0.5 , {string: \\\"\\'[as \\!a \\\"}] ")
     assert caplog.text.count("WARNING") == 0
     caplog.clear()
-    check_integrity(config_2, 2, None, "none",
-                    p_4=[1, 0.5, {
-                        "string": "'[as"
-                    }])
+    check_integrity(config_2, 2, None, "null", p_4=[1, 0.5, {"string": "'[as !a "}])
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
         mcl(config, config_2.get_command_line_argument(do_return_string=True))
     assert caplog.text.count("WARNING") == 0
     caplog.clear()
-    check_integrity(config, 2, None, "none", p_4=[1, 0.5, {"string": "'[as"}])
+    check_integrity(config_2, 2, None, "null", p_4=[1, 0.5, {"string": "'[as !a "}])
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
         mcl(config, "--subconfig1.param2")
     assert caplog.text.count("WARNING") == 0
     assert config.subconfig1.param2 is True
     caplog.clear()
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
         mcl(config, "--subconfig1.param2=False")
     assert caplog.text.count("WARNING") == 0
     assert config.subconfig1.param2 is False
     caplog.clear()
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
-        mcl(config, "--subconfig1.param2=1")
+        mcl(config, "--subconfig1.param2=yes")
     assert caplog.text.count("WARNING") == 0
     assert config.subconfig1.param2 is True
-    with pytest.raises(Exception, match="could not convert string to float: "
-                       "'False'"):
-        mcl(config, "--param1=False")
 
 
 def test_method_name(caplog):
     caplog.clear()
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
         config = make_config({"save": "test"}, do_not_merge_command_line=True)
```

### Comparing `yaecs-4.0.2/unittests/config/utils.py` & `yaecs-4.1.0/unittests/config/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/usage_example/configs/project_config.py` & `yaecs-4.1.0/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/usage_example/main.py` & `yaecs-4.1.0/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/usage_example/project_utils/utils.py` & `yaecs-4.1.0/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/__init__.py` & `yaecs-4.1.0/yaecs/__init__.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/config/config.py` & `yaecs-4.1.0/yaecs/config/config.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/config/config_base.py` & `yaecs-4.1.0/yaecs/config/config_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from typing import (TYPE_CHECKING,
                     Any, Callable, Dict, List, Optional, Tuple, Type, Union)
 
 import yaml
 
 from ..yaecs_utils import (YAML_EXPRESSIONS,
                            ConfigDeclarator, TypeHint,
-                           adapt_to_type, compare_string_pattern, compose, format_str, get_order, is_type_valid,
-                           parse_type, recursive_set_attribute, set_function_attribute, update_state)
+                           compare_string_pattern, compose, format_str, get_quasi_bash_sys_argv, get_order,
+                           is_type_valid, parse_type, recursive_set_attribute, set_function_attribute, update_state)
 from .config_convenience import ConfigConvenienceMixin
 from .config_getters import ConfigGettersMixin
 from .config_hooks import ConfigHooksMixin
 from .config_processing_functions import ConfigProcessingFunctionsMixin
 from .config_setters import ConfigSettersMixin
 
 if TYPE_CHECKING:
@@ -241,30 +241,30 @@
         :param config_path_or_dictionary: path or dictionary for the config to merge
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         """
         self._manual_merge(config_path_or_dictionary=config_path_or_dictionary, do_not_pre_process=do_not_pre_process,
                            do_not_post_process=do_not_post_process)
 
-    def merge_from_command_line(self, string_to_merge: Optional[str] = None,
+    def merge_from_command_line(self, to_merge: Optional[Union[List[str], str]] = None,
                                 do_not_pre_process: bool = False, do_not_post_process: bool = False) -> None:
         """
         Formerly used to manually merge the command line arguments into the config, which is now done automatically and
         thus should no longer be done manually. Can still be used to manually merge a string emulating command line
         arguments.
 
-        :param string_to_merge: if specified, merges this string instead of the sys.argv string
+        :param to_merge: if specified, merges this string or list of strings instead of the sys.argv list of strings
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         """
-        if self._verbose and string_to_merge is None:
+        if self._verbose and to_merge is None:
             YAECS_LOGGER.warning("WARNING : merge_from_command_line is now deprecated and will automatically start "
                                  "after using any constructor.\nYou can remove the 'config.merge_from_command_line()' "
                                  "line from your code now :) it's redundant.")
-        to_merge = self._gather_command_line_dict(string_to_merge)
+        to_merge = self._gather_command_line_dict(to_merge)
         if to_merge:
             self._manual_merge(to_merge, do_not_pre_process=do_not_pre_process, do_not_post_process=do_not_post_process,
                                source='command line')
 
     @staticmethod
     def _added_pre_processing():
         """ Will contain pre-processing function added via self.add_processing_function_all. """
@@ -679,37 +679,22 @@
         if type_hints is not None:
             for key, value in type_hints.items():
                 self[name].add_type_hint(key, value)
         self[name].init_from_config(content)
         self[name].config_metadata["config_hierarchy"] += [content]
         self.set_sub_config(self[name])
 
-    def _gather_command_line_dict(self, string_to_merge: Optional[str] = None) -> Dict[str, Any]:
+    def _gather_command_line_dict(self, to_merge: Optional[Union[List[str], str]] = None) -> Dict[str, Any]:
         """ Method called automatically at the end of each constructor to gather all parameters from the command line
         into a dictionary. This dictionary is then merged. """
-        # If a string is passed as input, process it as sys.argv would
-        if string_to_merge is not None:
-            list_to_merge = [""]
-            in_quotes = []
-            escaped = False
-            for char in string_to_merge:
-                if char == "\\" and not escaped:
-                    escaped = True
-                elif char in ['"', "'"] and not escaped:
-                    if not in_quotes or in_quotes[-1] != char:
-                        in_quotes.append(char)
-                    else:
-                        in_quotes.pop(-1)
-                elif char == " " and not in_quotes and list_to_merge[-1] and not escaped:
-                    list_to_merge.append("")
-                else:
-                    escaped = False
-                    list_to_merge[-1] += char
-            if in_quotes:
-                raise ValueError(f"Could not parse args : open quotations were left unclosed : {in_quotes}.")
+
+        if to_merge is not None:
+            if isinstance(to_merge, list):
+                to_merge = " ".join(to_merge)
+            list_to_merge = get_quasi_bash_sys_argv(to_merge)
         else:
             list_to_merge = sys.argv
 
         # Setting the config to operational mode in case this
         # is called manually
         object.__setattr__(self, "_operating_creation_or_merging", True)
 
@@ -725,40 +710,33 @@
                     value = value if value != "" else None
                 else:
                     pattern, value = element[2:], None
                 in_param = []
                 for parameter in self.get_parameter_names(deep=True):
                     if compare_string_pattern(parameter, pattern):
                         in_param.append(parameter)
-                        to_merge[parameter] = [self[parameter], value, None]
+                        to_merge[parameter] = value
                 if not in_param:
                     un_matched_params.append(pattern)
             elif element.startswith("--"):
                 in_param = []
                 found_config_path = True
-            elif in_param and to_merge[in_param[0]][1] is None:
+            elif in_param and to_merge[in_param[0]] is None:
                 for parameter in in_param:
-                    to_merge[parameter][1] = element
-            elif in_param and element[0] == "!":
-                if element[1:] in ["int", "float", "str", "bool", "list", "dict"]:
-                    for parameter in in_param:
-                        to_merge[parameter][2] = element[1:]
-                    in_param = []
-                else:
-                    raise TypeError(f"Unknown type '{element[1:]}', should be in [int, float, str, bool, list, dict].")
+                    to_merge[parameter] = element
             elif in_param:
                 for parameter in in_param:
-                    to_merge[parameter][1] += f" {element}"
+                    to_merge[parameter] = f"{to_merge[parameter]} {element}"
 
         if un_matched_params and self._verbose:
             YAECS_LOGGER.warning(f"WARNING : parameters {un_matched_params}, encountered while merging params from the "
                                  f"command line, do not match any param in the config. They will not be merged.")
 
         # Infer types, then return
-        return {key: adapt_to_type(val[0], val[1], val[2], key) for key, val in to_merge.items()}
+        return {key: yaml.safe_load("true" if val is None else val) for key, val in to_merge.items()}
 
     def _post_process_modified_parameters(self) -> None:
         """ This method is called at the end of a config creation or merging operation. It applies post-processing to
         all parameters modified by this operation. If a parameter is converted into a non-native YAML type, also keeps
         its former value in memory for saving purposes. """
         modified = [
             self._get_full_path(self._modified_buffer.pop(0))
```

### Comparing `yaecs-4.0.2/yaecs/config/config_convenience.py` & `yaecs-4.1.0/yaecs/config/config_convenience.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/config/config_getters.py` & `yaecs-4.1.0/yaecs/config/config_getters.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import logging
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
-from ..yaecs_utils import TypeHint, escape_symbols, get_param_as_parsable_string
+from ..yaecs_utils import TypeHint, get_param_as_parsable_string
 
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
@@ -84,42 +84,32 @@
 
         :return: list corresponding to the sub-configs
         """
         if self._are_same_sub_configs(self, self._main_config):
             return list(self._sub_configs_list)
         return self._main_config.get_all_sub_configs()
 
-    def get_command_line_argument(self, deep: bool = True, do_return_string: bool = False,
-                                  ignore_unknown_types: bool = False,
-                                  ) -> Union[List[str], str]:
+    def get_command_line_argument(self, deep: bool = True, do_return_string: bool = False) -> Union[List[str], str]:
         """
         Returns a list of command line parameters that can be used in a bash shell to re-create this exact config
         from the default. Can alternatively return the string itself with do_return_string=True.
 
         :param deep: whether to also take the sub-config parameters into account
         :param do_return_string: whether to return a string (True) or a list of strings (False, default)
-        :param ignore_unknown_types: if False (default), types that cannot be parsed in YAML raise an error. Else, they
-            are skipped when creating the list.
         :return: list or string containing the parameters
         """
         to_return = []
         for param in self.get_parameter_names(deep=deep):
             if not isinstance(self[param], ConfigGettersMixin):
                 full_name = self._get_full_path(param)
-                pair = get_param_as_parsable_string(
+                value = get_param_as_parsable_string(
                     self[param] if full_name not in self.get_main_config().get_pre_post_processing_values() else
                     self.get_main_config().get_pre_post_processing_values()[full_name],
-                    ignore_unknown_types=ignore_unknown_types,
                 )
-                if pair.count(" !"):
-                    pair_as_list = pair.split(" !")
-                    param_value, param_force = (" !".join(pair_as_list[:-1]), pair_as_list[-1],)
-                    to_return.append(escape_symbols(f"--{param} '{param_value}' \\!{param_force}", ["{", "}", "*"]))
-                else:
-                    to_return.append(escape_symbols(f"--{param} {pair}", ["{", "}", "*"]))
+                to_return.append(f"--{param} {value}")
 
         return " ".join(to_return) if do_return_string else to_return
 
     def get_dict(self, deep: bool = True) -> dict:
         """
         Returns a dictionary corresponding to the config.
```

### Comparing `yaecs-4.0.2/yaecs/config/config_hooks.py` & `yaecs-4.1.0/yaecs/config/config_hooks.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/config/config_processing_functions.py` & `yaecs-4.1.0/yaecs/config/config_processing_functions.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/config/config_setters.py` & `yaecs-4.1.0/yaecs/config/config_setters.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/config_history.py` & `yaecs-4.1.0/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/experiment.py` & `yaecs-4.1.0/yaecs/experiment.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/pytorch_lightning_utils.py` & `yaecs-4.1.0/yaecs/pytorch_lightning_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/user_utils.py` & `yaecs-4.1.0/yaecs/user_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-4.0.2/yaecs/yaecs_utils.py` & `yaecs-4.1.0/yaecs/yaecs_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
+from decimal import Context
 import functools
 import importlib.util
 import io
 import logging
 import os
 import re
 import sys
@@ -33,183 +34,14 @@
 ConfigDeclarator = Union[str, dict]
 ConfigInput = Union[List[ConfigDeclarator], ConfigDeclarator]
 Hooks = Union[Dict[str, List[str]], List[str]]
 TypeHint = Union[type, tuple, list, dict, set, int]
 VariationDeclarator = Union[List[ConfigDeclarator], Dict[str, ConfigDeclarator]]
 
 
-def adapt_to_type(previous_value: Any, value_to_adapt: str, force: str, param: str) -> Any:
-    """
-    Uses the previous value (more specifically, its type) of a parameter
-    to parse a string containing its new value. Takes into account
-    attempts from the user to force the new value to take a new type.
-
-    :param previous_value: previous value taken by the parameter
-    :param value_to_adapt: string corresponding to the new value of the
-        parameter
-    :param force: previously-detected type-forcing tag
-    :param param: name of the param for error logging
-    :raises TypeError: if the new value type cannot be adapted
-    :raises ValueError: the boolean value cannot be interpreted
-    :return: new value for the param
-    """
-
-    def _parse_scalar(raw_string, force_):
-        if force_ is None:
-            for forced_type in ["int", "float", "str", "bool", "list", "dict"]:
-                if raw_string.endswith(f"!{forced_type}") and raw_string[raw_string.rindex("!") - 1] != "\\":
-                    force_ = forced_type
-                    raw_string = raw_string[:-1 - len(forced_type)]
-        raw_string.lstrip(" ")
-        while raw_string[-1] == " " and raw_string[-2] != "\\":
-            raw_string = raw_string[:-1]
-        to_return = ""
-        esc = False
-        for character in raw_string:
-            if esc or character != "\\":
-                esc = False
-                to_return += character
-            else:
-                esc = True
-        return raw_string, force_
-
-    def _parse_container(container_string):
-        new_list = [""]
-        in_brackets = []
-        esc = False
-        for character in container_string:
-            if esc:
-                esc = False
-                if character == " ":
-                    new_list[-1] += "\\" + character
-                else:
-                    new_list[-1] += character
-            else:
-                if character == "\\":
-                    esc = True
-                elif character == "," and not in_brackets:
-                    new_list.append("")
-                elif character != " " or new_list[-1]:
-                    new_list[-1] += character
-                    if character in ["[", "{"]:
-                        in_brackets.append(character)
-                    if character == "]" and in_brackets[-1] == "[":
-                        in_brackets.pop(-1)
-                    if character == "}" and in_brackets[-1] == "{":
-                        in_brackets.pop(-1)
-        for i in range(len(new_list)):  # pylint: disable=consider-using-enumerate
-            while new_list[i][-1] == " " and new_list[i][-2] != "\\":
-                new_list[i] = new_list[i][:-1]
-            new_list[i] = new_list[i].replace("\\ ", " ")
-            forced = False
-            for forced_type in ["int", "float", "str", "bool", "list", "dict"]:
-                if (not forced and new_list[i].endswith(f"!{forced_type}")
-                        and new_list[i][-2 - len(forced_type)] != "\\"):
-                    forced = True
-                    new_list[i] = [new_list[i][:new_list[i].rindex("!")], forced_type]
-                    while new_list[i][0][-1] == " " and new_list[0][-2] != "\\":
-                        new_list[i][0] = new_list[i][0][:-1]
-            if not forced:
-                new_list[i] = [new_list[i], None]
-        return new_list
-
-    if value_to_adapt is None:
-        return True
-
-    if value_to_adapt.lower() in ["none", "null"] and force is None:
-        return None
-
-    scalar_parsed, force = _parse_scalar(value_to_adapt, force)
-
-    if previous_value is None and force is None:
-        if scalar_parsed.lower() not in ["none", "null"]:
-            raise TypeError(f"Type of param '{param}' cannot be inferred because its "
-                            "previous value was None.\n. To overwrite None values from "
-                            "command line, please force their type :\n\nExample : \t\t "
-                            "python main.py --none_param=0.001 !float")
-        return None
-
-    if (isinstance(previous_value, str) and force is None) or force == "str":
-        return scalar_parsed
-
-    if (isinstance(previous_value, list) and force is None) or force == "list":
-        if value_to_adapt[0] == "[" and value_to_adapt[-1] == "]":
-            value_to_adapt = value_to_adapt[1:-1]
-        value_to_adapt = (_parse_container(value_to_adapt) if value_to_adapt else [])
-        if isinstance(previous_value, list):
-            if all(isinstance(i, type(previous_value[-1])) for i in previous_value[:-1]):
-                return [adapt_to_type(previous_value[0], v[0], v[1], param) for v in value_to_adapt]
-            if len(previous_value) == len(value_to_adapt):
-                return [
-                    adapt_to_type(previous_value[index], value_to_adapt[index][0], value_to_adapt[index][1], param,
-                                  ) for index in range(len(value_to_adapt))
-                ]
-            if all(v[1] is not None or v[0].lower() in ["none", "null"] for v in value_to_adapt):
-                return [adapt_to_type(None, v[0], v[1], param) for v in value_to_adapt]
-            raise TypeError(f"New value for list in '{param}' is inconsistent with "
-                            f"old value '{previous_value}'. If the new value is "
-                            "correct, please force the type of the elements in the "
-                            "list so type inference can be done.")
-        if all(v[1] is not None or v[0].lower() in ["none", "null"] for v in value_to_adapt):
-            return [adapt_to_type(None, v[0], v[1], param) for v in value_to_adapt]
-        raise TypeError(f"Since the previous value for '{param}' was not a list, none of "
-                        "its items' values can be inferred. Please force the type of all "
-                        "elements in the new value's list.")
-
-    if (isinstance(previous_value, dict) and force is None) or force == "dict":
-        if value_to_adapt[0] == "{" and value_to_adapt[-1] == "}":
-            value_to_adapt = value_to_adapt[1:-1]
-        value_to_adapt = (_parse_container(value_to_adapt) if value_to_adapt else [])
-        if any(value_to_adapt):
-            value_to_adapt = {v[0].split(":", 1)[0]: (v[0].split(":", 1)[1], v[1]) for v in value_to_adapt}
-        else:
-            value_to_adapt = {}
-        if isinstance(previous_value, dict):
-            if all(key in previous_value or value_to_adapt[key][1] is not None
-                   or value_to_adapt[key][0].lstrip(" ").lower() in ["none", "null"] for key in value_to_adapt):
-                return {
-                    k.rstrip(" "): adapt_to_type(previous_value.get(k, None), v[0].lstrip(" "), v[1], param,
-                                                 )
-                    for k, v in value_to_adapt.items()
-                }
-            raise TypeError(f"New value for dict in '{param}' is inconsistent with old "
-                            f"value '{previous_value}'. If the new value is correct, "
-                            "please force the type of the new elements in the dict so "
-                            "type inference can be done.")
-        if all(value_to_adapt[key][1] is not None or value_to_adapt[key][0].lstrip(" ").lower() in ["none", "null"]
-               for key in value_to_adapt):
-            return {
-                k.rstrip(" "): adapt_to_type(None, v[0].lstrip(" "), v[1], param)
-                for k, v in value_to_adapt.items()
-            }
-        raise TypeError(f"Since the previous value for '{param}' was not a dict, "
-                        "none of its keys' values can be inferred. Please force the "
-                        "type of all elements in the new value's dict.")
-
-    if (isinstance(previous_value, int) and not isinstance(previous_value, bool) and force is None) or force == "int":
-        try:
-            parsed = int(scalar_parsed)
-        except ValueError:
-            parsed = float(scalar_parsed)
-        return int(parsed) if force == "int" else parsed
-
-    if (isinstance(previous_value, float) and force is None) or force == "float":
-        return float(scalar_parsed)
-
-    if (isinstance(previous_value, bool) and force is None) or force == "bool":
-        if scalar_parsed.strip(" ").lower() in ["y", "yes", "true", "1"]:
-            return True
-        if scalar_parsed.strip(" ").lower() in ["n", "no", "false", "0"]:
-            return False
-        raise ValueError("Boolean parameters can only be replaced with (non case sensitive)"
-                         " : \n"
-                         "- to get a True value : y, yes, true, 1\n"
-                         "- to get a False value : n, no, false, 0")
-
-
 def add_to_csv(csv_path: str, name: str, value: Any, step: int) -> None:
     """
     Adds a logged value to the csv containing previously logged values
 
     :param csv_path: path to the csv containing the logged values
     :param name: name of the value to log
     :param value: value of the value to log
@@ -382,67 +214,86 @@
     if pattern in sys.argv:
         fallback = [cfg.strip(" ") for cfg in sys.argv[sys.argv.index(pattern) + 1].strip("[]").split(",")]
     if not isinstance(fallback, list):
         fallback = [fallback]
     return fallback
 
 
+def get_quasi_bash_sys_argv(string_to_convert: str) -> List[str]:
+    """
+    If a string is passed as input, process it as sys.argv would in a bash shell
+    It gives exactly what sys.argv would if the script was used in a bash terminal, except that escaped '!' in quotes
+    are properly escaped and the escape symbol is removed, contrary to bash (which would keep the escape for some
+    obscure reason).
+
+    :param string_to_convert: string to process
+    :return: the list of strings that sys.argv would give
+    """
+    converted_list = [""]
+    in_quotes = ""
+    escaped = False
+    for index, char in enumerate(string_to_convert):
+        if char == "\\" and not escaped and (not in_quotes or string_to_convert[index+1] == "!"):
+            escaped = True
+        elif char in ['"', "'"] and not escaped:
+            if not in_quotes:
+                in_quotes = char
+            elif in_quotes == char:
+                in_quotes = ""
+            else:
+                converted_list[-1] += char
+        elif char == " " and not in_quotes and converted_list[-1] and not escaped:
+            converted_list.append("")
+        elif char == "!" and not escaped:
+            raise ValueError("Bash would say 'event not found', please escape the '!' character.")
+        else:
+            escaped = False
+            converted_list[-1] += char
+    if in_quotes:
+        raise ValueError(f"Could not parse args : open quotations were left unclosed : {in_quotes}.")
+    return converted_list
+
+
 def get_order(func: Callable) -> Union[Real, 'Priority']:
     """
     If input function has an "order" attribute, returns it. Otherwise, returns Priority.INDIFFERENT.
 
     :param func: function to get the order of
     :return: the order value
     """
     return getattr(func, "order", Priority.INDIFFERENT)
 
 
-def get_param_as_parsable_string(param: Any, in_iterable: bool = False, ignore_unknown_types: bool = False) -> str:
+def get_param_as_parsable_string(param: Any) -> str:
     """
-    Gets given value as a string that can be parsed by
-    the Configuration.
+    Gets given value as a string that can be parsed by the Configuration. The string is formatted so as to be either
+    used as is in a bash shell (ie., python main.py --param_name string), or with merge_from_command_line (ie.,
+    config.merge_from_command_line(f"--param_name {string}")
 
-    :param param:
-    :param in_iterable: used only for bookkeeping in recursive calls
-    :param ignore_unknown_types: how to treat types that cannot be
-        parsed by the Configuration
+    :param param: parameter value to be returned as a valid string
     :raises TypeError: if the type of 'param' cannot be enforced
-    :return: string usable in the command line to reproduce the value
-        of param
+    :return: string usable in the command line to reproduce the value of param
     """
+    container_separator = ",\\ "
     if param is None:
-        return "none"
+        return "null"
     if isinstance(param, list):
-        to_ret = [get_param_as_parsable_string(i, True) for i in param]
-        return f"[{','.join(to_ret)}] !list"
+        parsable_strings = [get_param_as_parsable_string(i) for i in param]
+        return f"[{container_separator.join(parsable_strings)}]"
     if isinstance(param, dict):
-        to_ret = [f"{k}:{get_param_as_parsable_string(v, True)}" for k, v in param.items()]
-        return "{" + ",".join(to_ret) + "} !dict"
+        parsable_strings = [f"{key}:\\ {get_param_as_parsable_string(value)}" for key, value in param.items()]
+        return "{" + container_separator.join(parsable_strings) + "}"
     if isinstance(param, (int, float)) and not isinstance(param, bool):
-        type_forcing = "float"
-    elif isinstance(param, str):
-        type_forcing = "str"
-    elif isinstance(param, bool):
-        type_forcing = "bool"
-    elif ignore_unknown_types:
-        YAECS_LOGGER.warning(f"WARNING: parameter value '{param}' will not have its type enforced because it is not in "
-                             f"[int, float, str, bool].")
-        type_forcing = ""
-    else:
-        raise TypeError(f"Parameter value '{param}' will not have its type enforced "
-                        "because it is not in [int, float, str, bool]. Pass "
-                        "ignore_unknown_types=True to avoid enforcing type when type "
-                        "is unknown.")
-    value = str(param)
-    value = escape_symbols(value, ["\\"])
-    if in_iterable:
-        value = escape_symbols(value, ["{", "}", "[", "]", ","])
-        value = escape_symbols(value, ["{", "}", "[", "]", ","])
-    value = escape_symbols(value, ["'", '"', " "])
-    return value + (f" !{type_forcing}" if type_forcing else "")
+        return format(Context(prec=20).create_decimal(repr(param)), 'f')
+    if isinstance(param, str):
+        string = escape_symbols(param, ['"', "'", "!", " "])
+        return escape_symbols(f'"{string}"', ['"'])
+    if isinstance(param, bool):
+        return str(param).lower()
+    raise TypeError("Provided value's type is not YAML-compatible (None, str, bool, int, float, list and dict work).")
 
 
 def hook(hook_name: str) -> Callable[[Callable], Callable]:
     """
     Decorator used to keep track of registered params.
 
     :param hook_name: name of the hook to store
```

### Comparing `yaecs-4.0.2/yaecs.egg-info/PKG-INFO` & `yaecs-4.1.0/yaecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 4.0.2
+Version: 4.1.0
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-4.0.2/yaecs.egg-info/SOURCES.txt` & `yaecs-4.1.0/yaecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

