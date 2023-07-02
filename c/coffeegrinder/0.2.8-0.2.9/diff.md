# Comparing `tmp/coffeegrinder-0.2.8.tar.gz` & `tmp/coffeegrinder-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeegrinder-0.2.8.tar", last modified: Sun Jul  2 10:31:50 2023, max compression
+gzip compressed data, was "coffeegrinder-0.2.9.tar", last modified: Sun Jul  2 23:26:56 2023, max compression
```

## Comparing `coffeegrinder-0.2.8.tar` & `coffeegrinder-0.2.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.605457 coffeegrinder-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/scripts/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.605457 coffeegrinder-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/DEPENDENCIES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/gp_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/hdf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/mpl_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/diffop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/fd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/diffop/sbp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation.py
--rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation_testing.nb
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/sbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/free_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/grid/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/ibvp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32830 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/io/simulation_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/mpi/mpiinterfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/solvers/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/tslices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/tslices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/tslices/tslices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/systems/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvection/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvection_fd/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.333356 coffeegrinder-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.333356 coffeegrinder-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/scripts/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-02 23:26:56.345357 coffeegrinder-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.333356 coffeegrinder-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/DEPENDENCIES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/actions/gp_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/actions/hdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/actions/mpl_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/diffop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/diffop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/diffop/fd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/diffop/sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/diffop/sbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/diffop/sbp/dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/diffop/sbp/dissipation_testing.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/diffop/sbp/sbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/free_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/ibvp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32830 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/io/simulation_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/mpi/mpiinterfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.337356 coffeegrinder-0.2.9/src/coffee/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/solvers/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/src/coffee/tslices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/tslices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/src/coffee/tslices/tslices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/src/coffeegrinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-02 23:26:56.000000 coffeegrinder-0.2.9/src/coffeegrinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-02 23:26:56.000000 coffeegrinder-0.2.9/src/coffeegrinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:26:56.000000 coffeegrinder-0.2.9/src/coffeegrinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:26:56.000000 coffeegrinder-0.2.9/src/coffeegrinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-02 23:26:56.000000 coffeegrinder-0.2.9/src/coffeegrinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 23:26:56.000000 coffeegrinder-0.2.9/src/coffeegrinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.333356 coffeegrinder-0.2.9/systems/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/systems/OneDAdvection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection/OneDAdvection_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/systems/OneDAdvection_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/systems/OneDAdvection_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/systems/OneDAdvection_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:26:56.341357 coffeegrinder-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 23:26:46.000000 coffeegrinder-0.2.9/tox.ini
```

### Comparing `coffeegrinder-0.2.8/.coveragerc` & `coffeegrinder-0.2.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/.github/workflows/python-publish.yml` & `coffeegrinder-0.2.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/.gitignore` & `coffeegrinder-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/.readthedocs.yml` & `coffeegrinder-0.2.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/CONTRIBUTING.rst` & `coffeegrinder-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/LICENSE.txt` & `coffeegrinder-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/PKG-INFO` & `coffeegrinder-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.2.8
+Version: 0.2.9
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `coffeegrinder-0.2.8/README.rst` & `coffeegrinder-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/docs/Makefile` & `coffeegrinder-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/docs/conf.py` & `coffeegrinder-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/docs/index.rst` & `coffeegrinder-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/scripts/compare.py` & `coffeegrinder-0.2.9/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/setup.cfg` & `coffeegrinder-0.2.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	numpy
 	h5py
 	scipy
 	PyGnuplot
 	matplotlib
-	mpi4py
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `coffeegrinder-0.2.8/setup.py` & `coffeegrinder-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/__init__.py` & `coffeegrinder-0.2.9/src/coffee/__init__.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/actions/actions.py` & `coffeegrinder-0.2.9/src/coffee/actions/actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/actions/gp_plotter.py` & `coffeegrinder-0.2.9/src/coffee/actions/gp_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/actions/hdf_output.py` & `coffeegrinder-0.2.9/src/coffee/actions/hdf_output.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/actions/mpl_plotter.py` & `coffeegrinder-0.2.9/src/coffee/actions/mpl_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/backend/backend.py` & `coffeegrinder-0.2.9/src/coffee/backend/backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/diffop/fd.py` & `coffeegrinder-0.2.9/src/coffee/diffop/fd.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation.py` & `coffeegrinder-0.2.9/src/coffee/diffop/sbp/dissipation.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation_testing.nb` & `coffeegrinder-0.2.9/src/coffee/diffop/sbp/dissipation_testing.nb`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/diffop/sbp/sbp.py` & `coffeegrinder-0.2.9/src/coffee/diffop/sbp/sbp.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/free_data.py` & `coffeegrinder-0.2.9/src/coffee/free_data.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/grid/grid.py` & `coffeegrinder-0.2.9/src/coffee/grid/grid.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/ibvp.py` & `coffeegrinder-0.2.9/src/coffee/ibvp.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/io/simulation_data.py` & `coffeegrinder-0.2.9/src/coffee/io/simulation_data.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/mpi/mpiinterfaces.py` & `coffeegrinder-0.2.9/src/coffee/mpi/mpiinterfaces.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/solvers/solvers.py` & `coffeegrinder-0.2.9/src/coffee/solvers/solvers.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/system.py` & `coffeegrinder-0.2.9/src/coffee/system.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffee/tslices/tslices.py` & `coffeegrinder-0.2.9/src/coffee/tslices/tslices.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/src/coffeegrinder.egg-info/PKG-INFO` & `coffeegrinder-0.2.9/src/coffeegrinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.2.8
+Version: 0.2.9
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `coffeegrinder-0.2.8/src/coffeegrinder.egg-info/SOURCES.txt` & `coffeegrinder-0.2.9/src/coffeegrinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection.py` & `coffeegrinder-0.2.9/systems/OneDAdvection/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_plotter.py` & `coffeegrinder-0.2.9/systems/OneDAdvection/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_setup.py` & `coffeegrinder-0.2.9/systems/OneDAdvection/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection.py` & `coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py` & `coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py` & `coffeegrinder-0.2.9/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection.py` & `coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py` & `coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py` & `coffeegrinder-0.2.9/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection.py` & `coffeegrinder-0.2.9/systems/OneDAdvection_fd/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection_plotter.py` & `coffeegrinder-0.2.9/systems/OneDAdvection_fd/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection_setup.py` & `coffeegrinder-0.2.9/systems/OneDAdvection_fd/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection.py` & `coffeegrinder-0.2.9/systems/OneDAdvection_sbp/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection_plotter.py` & `coffeegrinder-0.2.9/systems/OneDAdvection_sbp/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection_setup.py` & `coffeegrinder-0.2.9/systems/OneDAdvection_sbp/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/tests/test_actions.py` & `coffeegrinder-0.2.9/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/tests/test_backend.py` & `coffeegrinder-0.2.9/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.8/tox.ini` & `coffeegrinder-0.2.9/tox.ini`

 * *Files identical despite different names*

