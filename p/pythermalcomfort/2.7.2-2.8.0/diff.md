# Comparing `tmp/pythermalcomfort-2.7.2.tar.gz` & `tmp/pythermalcomfort-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythermalcomfort-2.7.2.tar", last modified: Thu May 11 02:25:42 2023, max compression
+gzip compressed data, was "pythermalcomfort-2.8.0.tar", last modified: Mon Jul  3 01:32:48 2023, max compression
```

## Comparing `pythermalcomfort-2.7.2.tar` & `pythermalcomfort-2.8.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/appveyor-with-compiler.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/templates/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/templates/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/contact_us.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/reference/pythermalcomfort.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_adaptive_ASHRAE.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_adaptive_EN.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_jos3.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_phs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_pmv_ppd.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_set_tmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_utci.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.624899 pythermalcomfort-2.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/src/pythermalcomfort/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/construction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/thermoregulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   172325 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/optimized_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/psychrometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/shared_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tests/test_jos3.py
--rw-r--r--   0 runner    (1001) docker     (123)    41005 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tests/test_pythermalcomfort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/appveyor-with-compiler.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/templates/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/templates/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/contact_us.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/reference/pythermalcomfort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_adaptive_ASHRAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_adaptive_EN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_phs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_pmv_ppd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_set_tmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_utci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.810787 pythermalcomfort-2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/src/pythermalcomfort/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/thermoregulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171792 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/optimized_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/psychrometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/shared_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tests/test_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tests/test_pythermalcomfort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tox.ini
```

### Comparing `pythermalcomfort-2.7.2/.appveyor.yml` & `pythermalcomfort-2.8.0/.appveyor.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 version: '{branch}-{build}'
 build: off
 environment:
   matrix:
-    - TOXENV: py36,codecov
-      TOXPYTHON: C:\Python36-x64\python.exe
-      PYTHON_HOME: C:\Python36-x64
-      PYTHON_VERSION: '3.6'
-      PYTHON_ARCH: '64'
-    - TOXENV: py37,codecov
-      TOXPYTHON: C:\Python37-x64\python.exe
-      PYTHON_HOME: C:\Python37-x64
-      PYTHON_VERSION: '3.7'
-      PYTHON_ARCH: '64'
     - TOXENV: py38,codecov
       TOXPYTHON: C:\Python38-x64\python.exe
       PYTHON_HOME: C:\Python38-x64
       PYTHON_VERSION: '3.8'
       PYTHON_ARCH: '64'
     - TOXENV: py39,codecov
       TOXPYTHON: C:\Python39-x64\python.exe
```

### Comparing `pythermalcomfort-2.7.2/.cookiecutterrc` & `pythermalcomfort-2.8.0/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/.readthedocs.yml` & `pythermalcomfort-2.8.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/.travis.yml` & `pythermalcomfort-2.8.0/.travis.yml`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 env:
   global:
     - LD_PRELOAD=/lib/x86_64-linux-gnu/libSegFault.so
     - SEGFAULT_SIGNALS=all
 matrix:
   include:
     - env:
-        - TOXENV=py36,codecov
-      python: '3.6'
-    - env:
-        - TOXENV=py37,codecov
-      python: '3.7'
-    - env:
         - TOXENV=py38,codecov
       python: '3.8'
     - env:
         - TOXENV=py39,codecov
       python: '3.9'
+    - env:
+        - TOXENV=py39,codecov
+      python: '3.10'
 before_install:
   - python --version
   - uname -a
   - lsb_release -a || true
 install:
   - python -mpip install --progress-bar=off tox -rci/requirements.txt
   - virtualenv --version
```

### Comparing `pythermalcomfort-2.7.2/AUTHORS.rst` & `pythermalcomfort-2.8.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/CHANGELOG.rst` & `pythermalcomfort-2.8.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-
 Changelog
 =========
 
+2.8.0 (2023-07-03)
+-------------------
+
+* allowing the cooling effect to range from 0 to 40
+* fixed PHS documentation
+* improved JOS3 documentation
+
 2.7.0 (2023-02-16)
 -------------------
 
 * changed coefficient of vasodilation in set_tmp() to 120 to match ASHRAE 55 2020 code
 * slightly modified value in validation tables
 
 2.6.0 (2023-01-17)
```

### Comparing `pythermalcomfort-2.7.2/CONTRIBUTING.rst` & `pythermalcomfort-2.8.0/CONTRIBUTING.rst`

 * *Files 13% similar despite different names*

```diff
@@ -35,61 +35,78 @@
 Development
 ===========
 
 To set up `pythermalcomfort` for local development:
 
 1. Fork `pythermalcomfort <https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort>`_
    (look for the "Fork" button).
-2. Clone your fork locally::
+2. Clone your fork locally. Fetch and pull all the updates from the master branch before you do anything:
+
+.. code-block::
 
     git clone git@github.com:CenterForTheBuiltEnvironment/pythermalcomfort.git
 
-3. Create a branch for local development::
+3. Create a branch for local development. The naming rule for new branch are, as follows:
+
+    * If this update is for a new feature Feature/feature_name_here
+    * If this update is for bug fix Fix/bug_name_here
+    * If this update is for documentation Documentation/doc_name_here
+
+You can create a branch locally using the following command. Make sure you only push updates to this new branch only:
+
+.. code-block::
 
     git checkout -b name-of-your-bugfix-or-feature
 
-   Now you can make your changes locally.
+Now you can make your changes locally.
+
+4. When you're done making changes run all the checks and docs builder with tox one command:
 
-4. When you're done making changes run all the checks and docs builder with tox one command::
+.. code-block::
 
     tox
 
-5. Commit your changes and push your branch to GitHub::
+5. Commit your changes and push your branch to GitHub:
+
+.. code-block::
 
     git add .
     git commit -m "Your detailed description of your changes."
     git push origin name-of-your-bugfix-or-feature
 
-6. Submit a pull request through the GitHub website.
+6. Submit a pull request after you have done all your modifications and tested your work. The pull request should include a detailed description of your work:
+
+    * What this pull request is about
+    * Have you tested your work
+    * Will this work affect other component in the product
 
 Pull Request Guidelines
 -----------------------
 
 If you need some code review or feedback while you're developing the code just make the pull request.
 
 For merging, you should:
 
-1. Include passing tests (run ``tox``) [1]_.
+1. Include passing tests (run ``tox``).
 2. Update documentation when there's new API, functionality etc.
 3. Add a note to ``CHANGELOG.rst`` about the changes.
 4. Add yourself to ``AUTHORS.rst``.
 
-.. [1] If you don't have all the necessary python versions available locally you can rely on Travis - it will
-       `run the tests <https://travis-ci.org/CenterForTheBuiltEnvironment/pythermalcomfort/pull_requests>`_ for each change you add in the pull request.
-
-       It will be slower though ...
-
 Tips
 ----
 
-To run a subset of tests::
+To run a subset of tests:
+
+.. code-block::
 
     tox -e envname -- pytest -k test_myfeature
 
-To run all the test environments in *parallel* (you need to ``pip install detox``)::
+To run all the test environments in *parallel* (you need to ``pip install detox``):
+
+.. code-block::
 
     detox
 
 To add a function
 ^^^^^^^^^^^^^^^^^
 
 1. Add the function to the python file `src/pythermalcomfort/models.py` and document it.
```

### Comparing `pythermalcomfort-2.7.2/LICENSE` & `pythermalcomfort-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/README.rst` & `pythermalcomfort-2.8.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -101,9 +101,10 @@
 
 .. _here: https://pythermalcomfort.readthedocs.io/en/latest/contributing.html
 
 
 Deployment
 ==========
 
-I am using travis to test the code. In addition, I have enabled GitHub actions. Every time a commit containing the message `bump version` is pushed to master then the GitHub action tests the code and if the tests pass, a new version of the package is published automatically on PyPI. See file in `.github/workflows/` for more information.
-
+I am using travis to test the code. In addition, I have enabled GitHub actions.
+Every time the code is pushed or pulled to the `master` repository then the GitHub action tests the code and if the tests pass, a new version of the package is published automatically on PyPI.
+See file in `.github/workflows/` for more information.
```

### Comparing `pythermalcomfort-2.7.2/ci/appveyor-with-compiler.cmd` & `pythermalcomfort-2.8.0/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/ci/bootstrap.py` & `pythermalcomfort-2.8.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/ci/templates/.appveyor.yml` & `pythermalcomfort-2.8.0/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/ci/templates/.travis.yml` & `pythermalcomfort-2.8.0/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/docs/conf.py` & `pythermalcomfort-2.8.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "pythermalcomfort"
 year = "2019"
 author = "Federico Tartarini"
 copyright = "{0}, {1}".format(year, author)
-version = release = "2.7.2"
+version = release = "2.8.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": (
         "https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort/issues/%s",
         "#",
```

### Comparing `pythermalcomfort-2.7.2/docs/contact_us.rst` & `pythermalcomfort-2.8.0/docs/contact_us.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/docs/reference/pythermalcomfort.rst` & `pythermalcomfort-2.8.0/docs/reference/pythermalcomfort.rst`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 Joint system thermoregulation model (JOS-3)
 -------------------------------------------
 
 .. autoclass:: pythermalcomfort.models.JOS3
     :members:
     :undoc-members:
-    :show-inheritance:
+    :special-members: __init__
 
 Adaptive Thermal Heat Balance (ATHB)
 ------------------------------------
 
 .. autofunction:: pythermalcomfort.models.athb
 
 Adaptive ASHRAE
@@ -131,14 +131,19 @@
 .. autofunction:: pythermalcomfort.models.a_pmv
 
 Adjusted Predicted Mean Votes with Expectancy Factor (ePMV)
 -----------------------------------------------------------
 
 .. autofunction:: pythermalcomfort.models.e_pmv
 
+Discomfort Index (DI)
+---------------------
+
+.. autofunction:: pythermalcomfort.models.discomfort_index
+
 Psychrometrics functions
 ========================
 
 .. automodule:: pythermalcomfort.psychrometrics
     :members:
 
 Utilities functions
@@ -234,20 +239,20 @@
 .. [8] ISO, 2004. ISO 7933 - Ergonomics of the thermal environment — Analytical determination and interpretation of heat stress using calculation of the predicted heat strain.
 .. [9] Błażejczyk, K., Jendritzky, G., Bröde, P., Fiala, D., Havenith, G., Epstein, Y., Psikuta, A. and Kampmann, B., 2013. An introduction to the universal thermal climate index (UTCI). Geographia Polonica, 86(1), pp.5-10.
 .. [10] Gagge, A.P., Fobelets, A.P., and Berglund, L.G., 1986. A standard predictive Index of human reponse to thermal enviroment. Am. Soc. Heating, Refrig. Air-Conditioning Eng. 709–731.
 .. [11] ISO, 2017. ISO 7243 - Ergonomics of the thermal environment — Assessment of heat stress using the WBGT (wet bulb globe temperature) index.
 .. [12] Rothfusz LP (1990) The heat index equation. NWS Southern Region Technical Attachment, SR/SSD 90–23, Fort Worth, Texas
 .. [13] Steadman RG (1979) The assessment of sultriness. Part I: A temperature-humidity index based on human physiology and clothing science. J Appl Meteorol 18:861–873
 .. [14] Masterton JM, Richardson FA. Humidex, a method of quantifying human discomfort due to excessive heat and humidity. Downsview, Ontario: CLI 1-79, Environment Canada, Atmospheric Environment Service, 1979
-.. [15] Havenith, G., Fiala, D., 2016. Thermal indices and thermophysiological modeling for heat stress. Compr. Physiol. 6, 255–302. https://doi.org/10.1002/cphy.c140051
-.. [16] Blazejczyk, K., Epstein, Y., Jendritzky, G., Staiger, H., Tinz, B., 2012. Comparison of UTCI to selected thermal indices. Int. J. Biometeorol. 56, 515–535. https://doi.org/10.1007/s00484-011-0453-2
+.. [15] Havenith, G., Fiala, D., 2016. Thermal indices and thermophysiological modeling for heat stress. Compr. Physiol. 6, 255–302. DOI: doi.org/10.1002/cphy.c140051
+.. [16] Blazejczyk, K., Epstein, Y., Jendritzky, G., Staiger, H., Tinz, B., 2012. Comparison of UTCI to selected thermal indices. Int. J. Biometeorol. 56, 515–535. DOI: doi.org/10.1007/s00484-011-0453-2
 .. [17] Steadman RG (1984) A universal scale of apparent temperature. J Appl Meteorol Climatol 23:1674–1687
 .. [18] ASHRAE, 2017. 2017 ASHRAE Handbook Fundamentals. Atlanta.
 .. [20] Höppe P. The physiological equivalent temperature - a universal index for the biometeorological assessment of the thermal environment. Int J Biometeorol. 1999 Oct;43(2):71-5. doi: 10.1007/s004840050118. PMID: 10552310.
-.. [21] Walther, E. and Goestchel, Q., 2018. The PET comfort index: Questioning the model. Building and Environment, 137, pp.1-10. https://doi.org/10.1016/j.buildenv.2018.03.054
-.. [22] Teitelbaum, E., Alsaad, H., Aviv, D., Kim, A., Voelker, C., Meggers, F., & Pantelic, J. (2022). Addressing a systematic error correcting for free and mixed convection when measuring mean radiant temperature with globe thermometers. Scientific Reports, 12(1), 1–18. https://doi.org/10.1038/s41598-022-10172-5
-.. [23] Liu, S., Schiavon, S., Kabanshi, A., Nazaroff, W.W., 2017. Predicted percentage dissatisfied with ankle draft. Indoor Air 27, 852–862. https://doi.org/10.1111/ina.12364
+.. [21] Walther, E. and Goestchel, Q., 2018. The PET comfort index: Questioning the model. Building and Environment, 137, pp.1-10. DOI: doi.org/10.1016/j.buildenv.2018.03.054
+.. [22] Teitelbaum, E., Alsaad, H., Aviv, D., Kim, A., Voelker, C., Meggers, F., & Pantelic, J. (2022). Addressing a systematic error correcting for free and mixed convection when measuring mean radiant temperature with globe thermometers. Scientific Reports, 12(1), 1–18. DOI: doi.org/10.1038/s41598-022-10172-5
+.. [23] Liu, S., Schiavon, S., Kabanshi, A., Nazaroff, W.W., 2017. Predicted percentage dissatisfied with ankle draft. Indoor Air 27, 852–862. DOI: doi.org/10.1111/ina.12364
 .. [24] Polydoros, Anastasios & Cartalis, Constantinos. (2015). Use of Earth Observation based indices for the monitoring of built-up area features and dynamics in support of urban energy studies. Energy and Buildings. 98. 92-99. 10.1016/j.enbuild.2014.09.060.
 .. [25] Yao, Runming & Li, Baizhan & Liu, Jing. (2009). A theoretical adaptive model of thermal comfort – Adaptive Predicted Mean Vote (aPMV). Building and Environment. 44. 2089-2096. 10.1016/j.buildenv.2009.02.014.
 .. [26] Fanger, P. & Toftum, Jorn. (2002). Extension of the PMV model to non-air-conditioned buildings in warm climates. Energy and Buildings. 34. 533-536. 10.1016/S0378-7788(02)00003-8.
-.. [27] Schweiker, M., 2022. Combining adaptive and heat balance models for thermal sensation prediction: A new approach towards a theory and data‐driven adaptive thermal heat balance model. Indoor Air 32, 1–19. https://doi.org/10.1111/ina.13018
+.. [27] Schweiker, M., 2022. Combining adaptive and heat balance models for thermal sensation prediction: A new approach towards a theory and data‐driven adaptive thermal heat balance model. Indoor Air 32, 1–19. DOI: doi.org/10.1111/ina.13018
```

### Comparing `pythermalcomfort-2.7.2/docs/usage.rst` & `pythermalcomfort-2.8.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/examples/calc_adaptive_ASHRAE.py` & `pythermalcomfort-2.8.0/examples/calc_adaptive_ASHRAE.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/examples/calc_adaptive_EN.py` & `pythermalcomfort-2.8.0/examples/calc_adaptive_EN.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/examples/calc_jos3.py` & `pythermalcomfort-2.8.0/examples/calc_jos3.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/examples/calc_phs.py` & `pythermalcomfort-2.8.0/examples/calc_phs.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/examples/calc_pmv_ppd.py` & `pythermalcomfort-2.8.0/examples/calc_pmv_ppd.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/examples/calc_utci.py` & `pythermalcomfort-2.8.0/examples/calc_utci.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/setup.cfg` & `pythermalcomfort-2.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/setup.py` & `pythermalcomfort-2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="pythermalcomfort",
-    version="2.7.2",
+    version="2.8.0",
     license="MIT",
     description=(
         "Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET,"
         " adaptive) and convert physical variables. Please cite us if you use this"
         " package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python"
         " package for thermal comfort research. SoftwareX 12, 100578."
         " https://doi.org/10.1016/j.softx.2020.100578"
@@ -82,15 +82,15 @@
         "pmv",
         "ppd",
         "building design",
         "compliance",
         "thermal environment",
         "built environment",
     ],
-    python_requires=">=3.6.0",
+    python_requires=">=3.8.0",
     install_requires=[
         "scipy",
         "numba",
         "numpy",
     ],  # eg: 'aspectlib==1.1.1', 'six>=1.7',
     extras_require={
         # eg:
```

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/cli.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/cli.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/construction.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/construction.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,72 +75,72 @@
 
     return array.copy()
 
 
 def bsa_rate(
     height=1.72,
     weight=74.43,
-    formula="dubois",
+    bsa_equation="dubois",
 ):
     """Calculate the rate of bsa to standard body.
 
     Parameters
     ----------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    formula : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
 
     Returns
     -------
     bsa_rate : float
         The ratio of bsa to the standard body [-].
     """
     bsa_all = body_surface_area(
         height=height,
         weight=weight,
-        formula=formula,
+        formula=bsa_equation,
     )
     return bsa_all / _BSAst.sum()  # The bsa ratio to the standard body (1.87m2)
 
 
 def local_bsa(
     height=1.72,
     weight=74.43,
-    formula="dubois",
+    bsa_equation="dubois",
 ):
     """Calculate local body surface area (bsa) [m2].
 
     The local body surface area has been derived from 65MN.
     The head have been divided to head and neck based on Smith's model.
         head = 0.1396*0.1117/0.1414 (65MN_Head * Smith_Head / Smith_Head+neck)
         neck = 0.1396*0.0297/0.1414 (65MN_Head * Smith_Neck / Smith_Head+neck)
 
     Parameters
     ----------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    formula : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
 
     Returns
     -------
     local_bsa : ndarray(17,)
         Local body surface area (bsa) [m2].
     """
     _bsa_rate = bsa_rate(
         height=height,
         weight=weight,
-        formula=formula,
+        bsa_equation=bsa_equation,
     )  # The bsa ratio to the standard body (1.87m2)
     local_bsa = _BSAst * _bsa_rate
     return local_bsa
 
 
 def weight_rate(
     weight=74.43,
@@ -169,28 +169,28 @@
     """
     return weight / 74.43
 
 
 def bfb_rate(
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     age=20,
     ci=2.59,
 ):
     """Calculate the ratio of basal blood flow (BFB) of the standard body (290
     L/h).
 
     Parameters
     ----------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
     ci : float, optional
         Cardiac index [L/min/㎡]. The default is 2.59.
 
@@ -208,33 +208,33 @@
     elif age < 60:
         ci *= 0.85
     elif age < 70:
         ci *= 0.75
     else:  # age >= 70
         ci *= 0.7
 
-    bfb_all = ci * bsa_rate(height, weight, equation) * _BSAst.sum()  # [L/h]
+    bfb_all = ci * bsa_rate(height, weight, bsa_equation) * _BSAst.sum()  # [L/h]
     return bfb_all / 290
 
 
 def conductance(
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     fat=15,
 ):
     """Calculate thermal conductance between layers [W/K].
 
     Parameters
     ----------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     fat : float, optional
         Body fat rate [%]. The default is 15.
 
     Returns
     -------
@@ -439,15 +439,15 @@
             0.444,
             0.992,
         ]
     )
 
     # Changes values by body size based on the standard body.
     wr = weight_rate(weight)
-    bsar = bsa_rate(height, weight, equation)
+    bsar = bsa_rate(height, weight, bsa_equation)
     # head, neck (Sphere shape)
     cdt_cr_sk[:2] *= wr / bsar
     cdt_cr_ms[:2] *= wr / bsar
     cdt_ms_fat[:2] *= wr / bsar
     cdt_fat_sk[:2] *= wr / bsar
     cdt_ves_cr[:2] *= wr / bsar
     cdt_sfv_sk[:2] *= wr / bsar
@@ -487,28 +487,28 @@
 
     # Creates a symmetrical matrix
     cdt_whole = cdt_whole + cdt_whole.T
 
     return cdt_whole.copy()
 
 
-def capacity(height=1.72, weight=74.43, equation="dubois", age=20, ci=2.59):
+def capacity(height=1.72, weight=74.43, bsa_equation="dubois", age=20, ci=2.59):
     """Calculate the thermal capacity [J/K].
 
     The values of vascular and central blood capacity have been derived from
     Yokoyama's model.
     The specific heat of blood is assumed as 1.0 [kcal/L.K].
 
     Parameters
     ----------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
     ci : float, optional
         Cardiac index [L/min/㎡]. The default is 2.59.
 
@@ -679,15 +679,15 @@
             0.334,
             0.169,
             0.107,
         ]
     )
 
     # Changes the values based on the standard body
-    bfbr = bfb_rate(height, weight, equation, age, ci)
+    bfbr = bfb_rate(height, weight, bsa_equation, age, ci)
     wr = weight_rate(weight)
     cap_art *= bfbr
     cap_vein *= bfbr
     cap_sfv *= bfbr
     cap_cb *= bfbr
     cap_cr *= wr
     cap_ms *= wr
```

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/matrix.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/matrix.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/parameters.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,75 +99,75 @@
     },
     "clo": {
         "ex_output": True,
         "meaning": "clothing insulation (each body part)",
         "suffix": "Body name",
         "unit": "clo",
     },
-    "q_skin_latent": {
+    "q_skin2env_latent": {
         "ex_output": True,
         "meaning": "latent heat loss from the skin (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_bmr_core": {
+    "q_bmr_core": {
         "ex_output": True,
-        "meaning": "core heat production by basal metabolism (each body part)",
+        "meaning": "core thermogenesis by basal metabolism (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "met_base_fat": {
+    "q_bmr_fat": {
         "ex_output": True,
-        "meaning": "fat heat production by basal metabolism (each body part)",
+        "meaning": "fat thermogenesis by basal metabolism (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_bmr_muscle": {
+    "q_bmr_muscle": {
         "ex_output": True,
-        "meaning": "muscle heat production by basal metabolism (each body part)",
+        "meaning": "muscle thermogenesis by basal metabolism (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_bmr_skin": {
+    "q_bmr_skin": {
         "ex_output": True,
-        "meaning": "skin heat production by basal metabolism (each body part)",
+        "meaning": "skin thermogenesis by basal metabolism (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_total": {
+    "q_thermogenesis_total": {
         "ex_output": False,
-        "meaning": "total heat production of the whole body",
+        "meaning": "total thermogenesis of the whole body",
         "suffix": None,
         "unit": "W",
     },
-    "Q_nst": {
+    "q_nst": {
         "ex_output": True,
         "meaning": (
-            "core heat production by non-shivering thermogenesis (each body part)"
+            "core thermogenesis by non-shivering (each body part)"
         ),
         "suffix": "Body name",
         "unit": "W",
     },
     "simulation_time": {
         "ex_output": False,
         "meaning": "simulation times",
         "suffix": None,
         "unit": "sec",
     },
-    "Q_shiv": {
+    "q_shiv": {
         "ex_output": True,
         "meaning": (
-            "core or muscle heat production by shivering thermogenesis (each body part)"
+            "core or muscle thermogenesis by shivering (each body part)"
         ),
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_work": {
+    "q_work": {
         "ex_output": True,
-        "meaning": "core or muscle heat production by work (each body part)",
+        "meaning": "core or muscle thermogenesis by work (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
     "name": {
         "ex_output": True,
         "meaning": "name of the model",
         "suffix": None,
@@ -175,35 +175,35 @@
     },
     "par": {
         "ex_output": True,
         "meaning": "physical activity ratio",
         "suffix": None,
         "unit": "-",
     },
-    "Q_core": {
+    "q_thermogenesis_core": {
         "ex_output": True,
-        "meaning": "core total heat production (each body part)",
+        "meaning": "core total thermogenesis (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_fat": {
+    "q_thermogenesis_fat": {
         "ex_output": True,
-        "meaning": "fat total heat production (each body part)",
+        "meaning": "fat total thermogenesis (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_muscle": {
+    "q_thermogenesis_muscle": {
         "ex_output": True,
-        "meaning": "muscle total heat production (each body part)",
+        "meaning": "muscle total thermogenesis (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "Q_skin": {
+    "q_thermogenesis_skin": {
         "ex_output": True,
-        "meaning": "skin total heat production (each body part)",
+        "meaning": "skin total thermogenesis (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
     "q_res": {
         "ex_output": False,
         "meaning": "heat loss by respiration",
         "suffix": None,
@@ -223,51 +223,51 @@
     },
     "rh": {
         "ex_output": True,
         "meaning": "relative humidity (each body part)",
         "suffix": "Body name",
         "unit": "%",
     },
-    "Ret": {
+    "r_et": {
         "ex_output": True,
         "meaning": "total clothing evaporative heat resistance (each body part)",
         "suffix": "Body name",
         "unit": "(m2*kPa)/W",
     },
-    "Rt": {
+    "r_t": {
         "ex_output": True,
         "meaning": "total clothing heat resistance (each body part)",
         "suffix": "Body name",
         "unit": "(m2*K)/W",
     },
-    "q_skin_sensible": {
+    "q_skin2env_sensible": {
         "ex_output": True,
         "meaning": "sensible heat loss from the skin (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
-    "t_core_set": {
+    "t_skin_set": {
         "ex_output": True,
         "meaning": "skin set point temperature (each body part)",
         "suffix": "Body name",
         "unit": "°C",
     },
-    "t_skin_set": {
+    "t_core_set": {
         "ex_output": True,
         "meaning": "core set point temperature (each body part)",
         "suffix": "Body name",
         "unit": "°C",
     },
     "sex": {
         "ex_output": True,
         "meaning": "sex",
         "suffix": None,
         "unit": "-",
     },
-    "q_skin": {
+    "q_skin2env": {
         "ex_output": False,
         "meaning": "total heat loss from the skin (each body part)",
         "suffix": "Body name",
         "unit": "W",
     },
     "tdb": {
         "ex_output": True,
```

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/thermoregulation.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/thermoregulation.py`

 * *Files 13% similar despite different names*

```diff
@@ -427,15 +427,15 @@
     fcl = clo_area_factor(clo)
     r_cl = 0.155 * clo
     r_ea = 1 / (lewis_rate * hc)
     r_ecl = r_cl / (lewis_rate * i_clo)
     r_et = r_ea / fcl + r_ecl
     return r_et
 
-def error_signals(err_sk=0):
+def error_signals(err_sk=0.0):
     """Calculate WRMS and CLDS signals of thermoregulation.
 
     Parameters
     ----------
     err_sk : float or array, optional
         Difference between set-point and skin temperatures [°C].
         If array, its length should be 17.
@@ -444,14 +444,16 @@
     Returns
     -------
     wrms : array
         Warm signal (WRMS) [°C].
     clds : array
         Cold signal (CLDS) [°C].
     """
+    # Convert err_sk to float if it's not already
+    err_sk = np.array(err_sk, dtype=float)
 
     # SKINR (Distribution coefficients of thermal receptor) [-]
     receptor = np.array(
         [
             0.0549,
             0.0146,
             0.1492,
@@ -495,15 +497,15 @@
     err_sk,
     t_skin,
     tdb,
     rh,
     ret,
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     age=20,
 ):
     """Calculate evaporative heat loss.
 
     Parameters
     ----------
     err_cr, err_sk : array
@@ -516,15 +518,15 @@
         Relative humidity at local body segments [%].
     ret : array
         Total evaporative thermal resistances [m2.K/W].
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
 
     Returns
     -------
@@ -540,15 +542,15 @@
 
     wrms, clds = error_signals(
         err_sk,
     )  # Thermoregulation signals
     bsar = cons.bsa_rate(
         height,
         weight,
-        equation,
+        bsa_equation,
     )  # bsa rate
     bsa = _BSAst * bsar  # bsa
     p_a = antoine(tdb) * rh / 100  # Saturated vapor pressure of ambient [kPa]
     p_sk_s = antoine(t_skin)  # Saturated vapor pressure at the skin [kPa]
 
     e_max = (p_sk_s - p_a) / ret * bsa  # Maximum evaporative heat loss
 
@@ -614,29 +616,29 @@
 
 
 def skin_blood_flow(
     err_cr,
     err_sk,
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     age=20,
     ci=2.59,
 ):
     """Calculate skin blood flow rate (bf_skin) [L/h].
 
     Parameters
     ----------
     err_cr, err_sk : array
         Difference between set-point and body temperatures [°C].
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
     ci : float, optional
         Cardiac index [L/min/㎡]. The default is 2.59.
 
@@ -755,43 +757,43 @@
         * bfb_sk
         * 2 ** (err_sk / 6)
     )
     # Basal blood flow rate to the standard body [-]
     bfb_rate = cons.bfb_rate(
         height,
         weight,
-        equation,
+        bsa_equation,
         age,
         ci,
     )
     bf_skin *= bfb_rate
     return bf_skin
 
 
 def ava_blood_flow(
     err_cr,
     err_sk,
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     age=20,
     ci=2.59,
 ):
     """Calculate areteriovenous anastmoses (AVA) blood flow rate [L/h] based on
     Takemori's model, 1995.
 
     Parameters
     ----------
     err_cr, err_sk : array
         Difference between set-point and body temperatures [°C].
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
     ci : float, optional
         Cardiac index [L/min/m2]. The default is 2.59.
 
@@ -817,103 +819,103 @@
     sig_ava_foot = min(sig_ava_foot, 1)
     sig_ava_foot = max(sig_ava_foot, 0)
 
     # Basal blood flow rate to the standard body [-]
     bfb_rate = cons.bfb_rate(
         height,
         weight,
-        equation,
+        bsa_equation,
         age,
         ci,
     )
     # AVA blood flow rate [L/h]
     bf_ava_hand = 1.71 * bfb_rate * sig_ava_hand  # Hand
     bf_ava_foot = 2.16 * bfb_rate * sig_ava_foot  # Foot
     return bf_ava_hand, bf_ava_foot
 
 
 def basal_met(
-    height=1.72, weight=74.43, age=20, sex="male", equation="harris-benedict"
+    height=1.72, weight=74.43, age=20, sex="male", bmr_equation="harris-benedict"
 ):
     """Calculate basal metabolic rate [W].
 
     Parameters
     ----------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
     age : float, optional
         age [years]. The default is 20.
     sex : str, optional
         Choose male or female. The default is "male".
-    equation : str, optional
+    bmr_equation : str, optional
         Choose harris-benedict or ganpule. The default is "harris-benedict".
 
     Returns
     -------
      bmr: float
         Basal metabolic rate [W].
     """
 
-    if equation == "harris-benedict":
+    if bmr_equation == "harris-benedict":
         if sex == "male":
             bmr = 88.362 + 13.397 * weight + 500.3 * height - 5.677 * age
         else:
             bmr = 447.593 + 9.247 * weight + 479.9 * height - 4.330 * age
 
-    elif equation == "harris-benedict_origin":
+    elif bmr_equation == "harris-benedict_origin":
         if sex == "male":
             bmr = 66.4730 + 13.7516 * weight + 500.33 * height - 6.7550 * age
         else:
             bmr = 655.0955 + 9.5634 * weight + 184.96 * height - 4.6756 * age
 
-    elif equation == "japanese" or equation == "ganpule":
+    elif bmr_equation == "japanese" or bmr_equation == "ganpule":
         # Ganpule et al., 2007, https://doi.org/10.1038/sj.ejcn.1602645
         if sex == "male":
             bmr = 0.0481 * weight + 2.34 * height - 0.0138 * age - 0.4235
         else:
             bmr = 0.0481 * weight + 2.34 * height - 0.0138 * age - 0.9708
         bmr *= 1000 / 4.186
     else:
         valid_equations = ["harris-benedict", "harris-benedict_origin", "japanese", "ganpule"]
         raise ValueError(
-            f"Invalid equation: '{equation}'. Must be one of {valid_equations}"
+            f"Invalid equation: '{bmr_equation}'. Must be one of {valid_equations}"
         )
 
     bmr *= 0.048  # [kcal/day] to [W]
 
     return bmr
 
 
 def local_mbase(
-    height=1.72, weight=74.43, age=20, sex="male", equation="harris-benedict"
+    height=1.72, weight=74.43, age=20, sex="male", bmr_equation="harris-benedict"
 ):
     """Calculate local basal metabolic rate [W].
 
     Parameters
     ----------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
     age : float, optional
         age [years]. The default is 20.
     sex : str, optional
         Choose male or female. The default is "male".
-    equation : str, optional
+    bmr_equation : str, optional
         Choose harris-benedict or ganpule. The default is "harris-benedict".
 
     Returns
     -------
     mbase : array
         Local basal metabolic rate (Mbase) [W].
     """
 
-    mbase_all = basal_met(height, weight, age, sex, equation)
+    mbase_all = basal_met(height, weight, age, sex, bmr_equation)
     # Distribution coefficient of basal metabolic rate
     mbf_cr = np.array(
         [
             0.19551,
             0.00324,
             0.28689,
             0.25677,
@@ -1000,31 +1002,31 @@
     mbase_ms = mbf_ms * mbase_all
     mbase_fat = mbf_fat * mbase_all
     mbase_sk = mbf_sk * mbase_all
     return mbase_cr, mbase_ms, mbase_fat, mbase_sk
 
 
 def local_q_work(bmr, par):
-    """Calculate local heat production by work [W]
+    """Calculate local thermogenesis by work [W]
 
     Parameters
     ----------
     bmr : float
         Basal metabolic rate [W].
     par : float
         Physical activity ratio [-].
 
     Returns
     -------
-    Q_work : array
-        Local heat production by work [W].
+    q_work : array
+        Local thermogenesis by work [W].
     """
     q_work_all = (par - 1) * bmr
 
-    # Distribution coefficient of heat production by work
+    # Distribution coefficient of thermogenesis by work
     workf = np.array(
         [
             0,
             0,
             0.091,
             0.08,
             0.129,
@@ -1052,51 +1054,51 @@
 def shivering(
     err_cr,
     err_sk,
     t_core,
     t_skin,
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     age=20,
     sex="male",
     dtime=60,
     options={},
 ):
-    """Calculate local heat production by shivering [W].
+    """Calculate local thermogenesis by shivering [W].
 
     Parameters
     ----------
     err_cr, err_sk : array
         Difference between set-point and body temperatures [°C].
     t_core, t_skin : array
         Core and skin temperatures [°C].
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
     sex : str, optional
         Choose male or female. The default is "male".
     dtime : float, optional
         Interval of analysis time. The default is 60.
 
     Returns
     -------
-    Q_shiv : array
-        Local heat production by shivering [W].
+    q_shiv : array
+        Local thermogenesis by shivering [W].
     """
     # Integrated error signal in the warm and cold receptors
     wrms, clds = error_signals(err_sk)
 
-    # Distribution coefficient of heat production by shivering
+    # Distribution coefficient of thermogenesis by shivering
     shivf = np.array(
         [
             0.0339,
             0.0436,
             0.27394,
             0.24102,
             0.38754,
@@ -1161,54 +1163,54 @@
         sd_shiv = np.ones(17) * 0.90055
     elif age < 80:
         sd_shiv = np.ones(17) * 0.86188
     else:  # age >= 80
         sd_shiv = np.ones(17) * 0.82597
 
     # Ratio of body surface area to the standard body [-]
-    bsar = cons.bsa_rate(height, weight, equation)
+    bsar = cons.bsa_rate(height, weight, bsa_equation)
 
-    # Local heat production by shivering [W]
+    # Local thermogenesis by shivering [W]
     q_shiv = shivf * bsar * sd_shiv * sig_shiv
     return q_shiv
 
 def nonshivering(
     err_sk,
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     age=20,
     cold_acclimation=False,
     batpositive=True,
 ):
     """Calculate local metabolic rate by non-shivering [W]
 
     Parameters
     ----------
     err_sk : array
         Difference between set-point and body temperatures [°C].
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
     cold_acclimation : bool, optional
         Whether the subject acclimates cold environment or not.
         The default is False.
     batpositive : bool, optional
         Whether BAT activity is positive or not.
         The default is True.
 
     Returns
     -------
-    Q_nst : array
+    q_nst : array
         Local metabolic rate by non-shivering [W].
     """
     # NST (Non-Shivering Thermogenesis) model, Asaka, 2016
     wrms, clds = error_signals(err_sk)
 
     # BMI (Body Mass Index)
     bmi = weight / height**2
@@ -1242,15 +1244,15 @@
 
     # NST limit
     thres = (1.80 * bat + 2.43) + 5.62  # [W]
 
     sig_nst = 2.8 * clds  # [W]
     sig_nst = min(sig_nst, thres)
 
-    # Distribution coefficient of heat production by non-shivering
+    # Distribution coefficient of thermogenesis by non-shivering
     nstf = np.array(
         [
             0.000,
             0.190,
             0.000,
             0.190,
             0.190,
@@ -1266,62 +1268,62 @@
             0.000,
             0.000,
             0.000,
         ]
     )
 
     # Ratio of body surface area to the standard body [-]
-    bsar = cons.bsa_rate(height, weight, equation)
+    bsar = cons.bsa_rate(height, weight, bsa_equation)
 
-    # Local heat production by non-shivering [W]
+    # Local thermogenesis by non-shivering [W]
     q_nst = bsar * nstf * sig_nst
     return q_nst
 
 
 def sum_m(mbase, q_work, q_shiv, q_nst):
-    """Calculate total heat production in each layer [W].
+    """Calculate total thermogenesis in each layer [W].
 
     Parameters
     ----------
     mbase : array
         Local basal metabolic rate (Mbase) [W].
     q_work : array
-        Local heat production by work [W].
+        Local thermogenesis by work [W].
     q_shiv : array
-        Local heat production by shivering [W].
+        Local thermogenesis by shivering [W].
     q_nst : array
-        Local heat production by non-shivering [W].
+        Local thermogenesis by non-shivering [W].
 
     Returns
     -------
-    q_core, q_muscle, q_fat, q_skin : array
-        Total heat production in core, muscle, fat, skin layers [W].
+    q_thermogenesis_core, q_thermogenesis_muscle, q_thermogenesis_fat, q_thermogenesis_skin : array
+        Total thermogenesis in core, muscle, fat, skin layers [W].
     """
-    q_core = mbase[0].copy()
-    q_muscle = mbase[1].copy()
-    q_fat = mbase[2].copy()
-    q_skin = mbase[3].copy()
+    q_thermogenesis_core = mbase[0].copy()
+    q_thermogenesis_muscle = mbase[1].copy()
+    q_thermogenesis_fat = mbase[2].copy()
+    q_thermogenesis_skin = mbase[3].copy()
 
     for i, bn in enumerate(BODY_NAMES):
-        # If the segment has a muscle layer, muscle heat production increases by the activity.
+        # If the segment has a muscle layer, muscle thermogenesis increases by the activity.
         if IDICT[bn]["muscle"] is not None:
-            q_muscle[i] += q_work[i] + q_shiv[i]
-        # In other segments, core heat production increase, instead of muscle.
+            q_thermogenesis_muscle[i] += q_work[i] + q_shiv[i]
+        # In other segments, core thermogenesis increase, instead of muscle.
         else:
-            q_core[i] += q_work[i] + q_shiv[i]
-    q_core += q_nst  # Non-shivering thermogenesis occurs in core layers
-    return q_core, q_muscle, q_fat, q_skin
+            q_thermogenesis_core[i] += q_work[i] + q_shiv[i]
+    q_thermogenesis_core += q_nst  # Non-shivering thermogenesis occurs in core layers
+    return q_thermogenesis_core, q_thermogenesis_muscle, q_thermogenesis_fat, q_thermogenesis_skin
 
 
 def cr_ms_fat_blood_flow(
     q_work,
     q_shiv,
     height=1.72,
     weight=74.43,
-    equation="dubois",
+    bsa_equation="dubois",
     age=20,
     ci=2.59,
 ):
     """Calculate core, muscle and fat blood flow rate [L/h].
 
     Parameters
     ----------
@@ -1329,15 +1331,15 @@
         Heat production by work [W].
     q_shiv : array
         Heat production by shivering [W].
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
-    equation : str, optional
+    bsa_equation : str, optional
         The equation name (str) of bsa calculation. Choose a name from "dubois",
         "takahira", "fujimoto", or "kurazumi". The default is "dubois".
     age : float, optional
         age [years]. The default is 20.
     ci : float, optional
         Cardiac index [L/min/㎡]. The default is 2.59.
 
@@ -1410,15 +1412,15 @@
             0.0,
             0.0,
             0.0,
             0.0,
         ]
     )
 
-    bfb_rate = cons.bfb_rate(height, weight, equation, age, ci)
+    bfb_rate = cons.bfb_rate(height, weight, bsa_equation, age, ci)
     bf_core = bfb_core * bfb_rate
     bf_muscle = bfb_muscle * bfb_rate
     bf_fat = bfb_fat * bfb_rate
 
     for i, bn in enumerate(BODY_NAMES):
         # If the segment has a muscle layer, muscle blood flow increases.
         if IDICT[bn]["muscle"] is not None:
@@ -1460,28 +1462,28 @@
     co += bf_fat.sum()
     co += bf_skin.sum()
     co += 2 * bf_ava_hand
     co += 2 * bf_ava_foot
     return co
 
 
-def resp_heat_loss(tdb, p_a, q_total):
+def resp_heat_loss(tdb, p_a, q_thermogenesis_total):
     """
     Calculate heat loss by respiration [W].
 
     Parameters
     ----------
     tdb : float
         Dry bulb air temperature [oC].
     p_a : float
         Water vapor pressure in the ambient air  [kPa].
-    q_total: float
-        Total heat production [W].
+    q_thermogenesis_total: float
+        Total thermogenesis [W].
 
     Returns
     -------
     res_sh, res_lh : float
         Sensible and latent heat loss by respiration [W].
     """
-    res_sh = 0.0014 * q_total * (34 - tdb)  # sensible heat loss
-    res_lh = 0.0173 * q_total * (5.87 - p_a)  # latent heat loss
+    res_sh = 0.0014 * q_thermogenesis_total * (34 - tdb)  # sensible heat loss
+    res_lh = 0.0173 * q_thermogenesis_total * (5.87 - p_a)  # latent heat loss
     return res_sh, res_lh
```

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/utilities.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/utilities.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/models.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 calculate_ce=True,
                 limit_inputs=False,
             )
             - initial_set_tmp
         )
 
     try:
-        ce = optimize.brentq(function, 0.0, 15)
+        ce = optimize.brentq(function, 0.0, 40)
     except ValueError:
         ce = 0
 
     warnings.simplefilter("always")
 
     if ce == 0:
         warnings.warn(
@@ -276,15 +276,15 @@
         >>> # calculate relative air speed
         >>> v_r = v_relative(v=v, met=met)
         >>> # calculate dynamic clothing
         >>> clo_d = clo_dynamic(clo=clo, met=met)
         >>> results = pmv_ppd(tdb=tdb, tr=tr, vr=v_r, rh=rh, met=met, clo=clo_d)
         >>> print(results)
         {'pmv': 0.06, 'ppd': 5.1}
-        >>> print(results['pmv'])
+        >>> print(results["pmv"])
         -0.06
         >>> # you can also pass an array-like of inputs
         >>> results = pmv_ppd(tdb=[22, 25], tr=tr, vr=v_r, rh=rh, met=met, clo=clo_d)
         >>> print(results)
         {'pmv': array([-0.47,  0.06]), 'ppd': array([9.6, 5.1])}
 
     Raises
@@ -879,15 +879,15 @@
     Other Parameters
     ----------------
     max_sweating: float, [mL/h/m2] default 500
         max sweating
     round: boolean, default True
         if True rounds output value, if False it does not round it
     limit_inputs : boolean default True
-        By default, if the inputs are outsude the standard applicability limits the
+        By default, if the inputs are outside the standard applicability limits the
         function returns nan. If False returns pmv and ppd values even if input values are
         outside the applicability limits of the model.
 
         The applicability limits are 20 < tdb [°C] < 50, 20 < tr [°C] < 50,
         0.1 < v [m/s] < 4.5, 0.7 < met [met] < 2, and 0 < clo [clo] < 1.
 
     Returns
@@ -1918,15 +1918,15 @@
     height : float, default 1.8
         height, [m]
     walk_sp : float, default 0
         walking speed, [m/s]
     theta : float, default 0
         angle between walking direction and wind direction [degrees]
     acclimatized : float, default 100
-        100 if acclimatised subject, 0 otherwise
+        100 if acclimatized subject, 0 otherwise
     duration : float, default 480
         duration of the work sequence, [minutes]
     f_r : float, default 0.97
         emissivity of the reflective clothing, [dimensionless]
         Some reference values :py:meth:`pythermalcomfort.utilities.f_r_garments`.
     t_sk : float, default 34.1
         mean skin temperature when worker starts working, [°C]
@@ -1938,21 +1938,31 @@
         mean core temperature as a function of met when worker starts working, [°C]
     sweat_rate : float, default 0
 
     Returns
     -------
     t_re : float
         rectal temperature, [°C]
+    t_sk : float
+        skin temperature, [°C]
+    t_cr : float
+        core temperature, [°C]
+    t_cr_eq : float
+        core temperature as a function of the metabolic rate, [°C]
+    t_sk_t_cr_wg : float
+        fraction of the body mass at the skin temperature
     d_lim_loss_50 : float
         maximum allowable exposure time for water loss, mean subject, [minutes]
     d_lim_loss_95 : float
         maximum allowable exposure time for water loss, 95% of the working population,
         [minutes]
     d_lim_t_re : float
         maximum allowable exposure time for heat storage, [minutes]
+    water_loss_watt : float
+        maximum water loss in watts, [W]
     water_loss : float
         maximum water loss, [g]
 
     Examples
     --------
     .. code-block:: python
 
@@ -2053,24 +2063,24 @@
         t_cr_eq,
         t_sk_t_cr_wg,
         sweat_rate,
     )
 
     if kwargs["round"]:
         return {
-            "d_lim_loss_50": round(d_lim_loss_50, 1),
-            "d_lim_loss_95": round(d_lim_loss_95, 1),
-            "d_lim_t_re": round(d_lim_t_re, 1),
-            "water_loss": round(sw_tot_g, 1),
             "t_re": round(t_re, 1),
-            "t_cr": round(t_cr, 1),
             "t_sk": round(t_sk, 1),
+            "t_cr": round(t_cr, 1),
             "t_cr_eq": round(t_cr_eq, 1),
             "t_sk_t_cr_wg": round(t_sk_t_cr_wg, 2),
+            "d_lim_loss_50": round(d_lim_loss_50, 1),
+            "d_lim_loss_95": round(d_lim_loss_95, 1),
+            "d_lim_t_re": round(d_lim_t_re, 1),
             "water_loss_watt": round(sweat_rate, 1),
+            "water_loss": round(sw_tot_g, 1),
         }
     else:
         return {
             "t_re": t_re,
             "t_sk": t_sk,
             "t_cr": t_cr,
             "t_cr_eq": t_cr_eq,
@@ -3304,243 +3314,35 @@
     and JOS-2 model (https://doi.org/10.1016/j.buildenv.2013.04.013).
 
     To use this model, create an instance of the JOS3 class with optional body parameters
     such as body height, weight, age, sex, etc.
 
     Environmental conditions such as air temperature, mean radiant temperature, air velocity, etc.
     can be set using the setter methods. (ex. X.tdb, X.tr X.v)
-    If you want to set the different conditons in each body part, set them
-    as a 17 lengths of list, dictionaly, or numpy array format.
+    If you want to set the different conditions in each body part, set them
+    as a 17 lengths of list, dictionary, or numpy array format.
 
     List or numpy array format input must be 17 lengths and means the order of "head", "neck", "chest",
     "back", "pelvis", "left_shoulder", "left_arm", "left_hand", "right_shoulder", "right_arm",
     "right_hand", "left_thigh", "left_leg", "left_foot", "right_thigh", "right_leg" and "right_foot".
 
     The model output includes local and mean skin temperature, local core temperature,
-    local and mean skin wettedness, and heat loss from the skin etc. which can be accessed using getter methods.
+    local and mean skin wettedness, and heat loss from the skin etc.
+    The model output can be accessed using "dict_results()" method and be converted to a csv file
+    using "to_csv" method.
+    Each output parameter also can be accessed using getter methods.
     (ex. X.t_skin, X.t_skin_mean, X.t_core)
 
     If you use this package, please cite us as follows and mention the version of pythermalcomfort used:
     Y. Takahashi, A. Nomoto, S. Yoda, R. Hisayama, M. Ogata, Y. Ozeki, S. Tanabe,
     Thermoregulation Model JOS-3 with New Open Source Code, Energy & Buildings (2020),
     doi: https://doi.org/10.1016/j.enbuild.2020.110575
 
     Note: To maintain consistency in variable names for pythermalcomfort,
     some variable names differ from those used in the original paper.
-
-    Parameters
-    ----------
-    height : float, optional
-        body height, in [m]. The default is 1.72.
-    weight : float, optional
-        body weight, in [kg]. The default is 74.43.
-    fat : float, optional
-        fat percentage, in [%]. The default is 15.
-    age : int, optional
-        age, in [years]. The default is 20.
-    sex : str, optional
-        sex ("male" or "female"). The default is "male".
-    ci : float, optional
-        Cardiac index, in [L/min/m2]. The default is 2.6432.
-    bmr_equation : str, optional
-        The equation used to calculate basal metabolic rate (BMR). Choose a BMR equation.
-        The default is "harris-benedict" equation created uding Caucasian's data. (https://doi.org/10.1073/pnas.4.12.370)
-        If the Ganpule's equation (https://doi.org/10.1038/sj.ejcn.1602645) for Japanese people is used, input "japanese".
-    bsa_equation : str, optional
-        The equation used to calculate body surface area (bsa). Choose a bsa equation.
-        You can choose "dubois", "fujimoto", "kruazumi", or "takahira". The default is "dubois".
-        The body surface area can be calculated using the function
-        :py:meth:`pythermalcomfort.utilities.body_surface_area`.
-    ex_output : None, list or "all", optional
-        This is used when you want to display results other than the default output parameters (ex.skin temperature);
-        by default, JOS outputs only the most necessary parameters in order to reduce the computational load.
-        If the parameters other than the default output parameters are needed,
-        specify the list of the desired parameter names in string format like ["bf_skin", "bf_core", "t_artery"].
-        If you want to display all output results, set ex_output is "all".
-
-    Returns
-    -------
-    Q_total : total heat production of the whole body [W]
-    cardiac_output: cardiac output (the sum of the whole blood flow) [L/h]
-    cycle_time: the counts of executing one cycle calculation [-]
-    dt      : time step [sec]
-    pythermalcomfort_version: version of pythermalcomfort [-]
-    q_res   : heat loss by respiration [W]
-    q_skin  : total heat loss from the skin (each body part) [W]
-    simulation_time: simulation times [sec]
-    t_core  : core temperature (each body part) [°C]
-    t_skin  : skin temperature (each body part) [°C]
-    t_skin_mean: mean skin temperature [°C]
-    w       : skin wettedness (each body part) [-]
-    w_mean  : mean skin wettedness [-]
-    weight_loss_by_evap_and_res: weight loss by the evaporation and respiration of the whole body [g/sec]
-    OPTIONAL PARAMETERS : the paramters listed below are returned if ex_output = "all"
-    Q_bmr_core: core heat production by basal metabolism (each body part) [W]
-    Q_bmr_muscle: muscle heat production by basal metabolism (each body part) [W]
-    Q_bmr_skin: skin heat production by basal metabolism (each body part) [W]
-    Q_core  : core total heat production (each body part) [W]
-    Q_fat   : fat total heat production (each body part) [W]
-    Q_muscle: muscle total heat production (each body part) [W]
-    Q_nst   : core heat production by non-shivering thermogenesis (each body part) [W]
-    Q_shiv  : core or muscle heat production by shivering thermogenesis (each body part) [W]
-    Q_skin  : skin total heat production (each body part) [W]
-    Q_work  : core or muscle heat production by work (each body part) [W]
-    Ret     : total clothing evaporative heat resistance (each body part) [m2.kPa/W]
-    Rt      : total clothing heat resistance (each body part) [m2.K/W]
-    age     : age [years]
-    bf_ava_foot: AVA blood flow rate of one foot [L/h]
-    bf_ava_hand: AVA blood flow rate of one hand [L/h]
-    bf_core : core blood flow rate (each body part) [L/h]
-    bf_fat  : fat blood flow rate (each body part) [L/h]
-    bf_muscle: muscle blood flow rate (each body part) [L/h]
-    bf_skin : skin blood flow rate (each body part) [L/h]
-    bsa     : body surface area (each body part) [m2]
-    clo     : clothing insulation (each body part) [clo]
-    e_max   : maximum evaporative heat loss from the skin (each body part) [W]
-    e_skin  : evaporative heat loss from the skin (each body part) [W]
-    e_sweat : evaporative heat loss from the skin by only sweating (each body part) [W]
-    fat     : body fat rate [%]
-    height  : body height [m]
-    met_base_fat: fat heat production by basal metabolism (each body part) [W]
-    name    : name of the model [-]
-    par     : physical activity ratio [-]
-    q_res_latent: latent heat loss by respiration (each body part) [W]
-    q_res_sensible: sensible heat loss by respiration (each body part) [W]
-    q_skin_latent: latent heat loss from the skin (each body part) [W]
-    q_skin_sensible: sensible heat loss from the skin (each body part) [W]
-    rh      : relative humidity (each body part) [%]
-    sex     : sex [-]
-    t_artery: arterial temperature (each body part) [°C]
-    t_cb    : central blood temperature [°C]
-    t_core_set: skin set point temperature (each body part) [°C]
-    t_fat   : fat temperature (each body part) [°C]
-    t_muscle: muscle temperature (each body part) [°C]
-    t_skin_set: core set point temperature (each body part) [°C]
-    t_superficial_vein: superficial vein temperature (each body part) [°C]
-    t_vein  : vein temperature (each body part) [°C]
-    tdb     : dry bulb air temperature (each body part) [°C]
-    to      : operative temperature (each body part) [°C]
-    tr      : mean radiant temperature (each body part) [°C]
-    v       : air velocity (each body part) [m/s]
-    weight  : body weight [kg]
-
-
-    Examples
-    --------
-    Build a model and set a body built
-    Create an instance of the JOS3 class with optional body parameters such as body height, weight, age, sex, etc.
-
-    .. code-block:: python
-
-        >>> import numpy as np
-        >>> import pandas as pd
-        >>> import matplotlib.pyplot as plt
-        >>> import os
-        >>> from pythermalcomfort.models import JOS3
-        >>> from pythermalcomfort.jos3_functions.utilities import local_clo_typical_ensembles
-        >>>
-        >>> directory_name = "jos3_output_example"
-        >>> current_directory = os.getcwd()
-        >>> jos3_example_directory = os.path.join(current_directory, directory_name)
-        >>> if not os.path.exists(jos3_example_directory):
-        >>>     os.makedirs(jos3_example_directory)
-        >>>
-        >>> model = JOS3(
-        >>>     height=1.7,
-        >>>     weight=60,
-        >>>     fat=20,
-        >>>     age=30,
-        >>>     sex="male",
-        >>>     bmr_equation="japanese",
-        >>>     bsa_equation="fujimoto",
-        >>>     ex_output="all",
-        >>> )
-        >>> # Set environmental conditions such as air temperature, mean radiant temperature using the setter methods.
-        >>> # Set the first condition
-        >>> # Environmental parameters can be input as int, float, list, dict, numpy array format.
-        >>> model.tdb = 28  # Air temperature [°C]
-        >>> model.tr = 30  # Mean radiant temperature [°C]
-        >>> model.rh = 40  # Relative humidity [%]
-        >>> model.v = np.array( # Air velocity [m/s]
-        >>>     [
-        >>>         0.2,  # head
-        >>>         0.4,  # neck
-        >>>         0.4,  # chest
-        >>>         0.1,  # back
-        >>>         0.1,  # pelvis
-        >>>         0.4,  # left shoulder
-        >>>         0.4,  # left arm
-        >>>         0.4,  # left hand
-        >>>         0.4,  # right shoulder
-        >>>         0.4,  # right arm
-        >>>         0.4,  # right hand
-        >>>         0.1,  # left thigh
-        >>>         0.1,  # left leg
-        >>>         0.1,  # left foot
-        >>>         0.1,  # right thigh
-        >>>         0.1,  # right leg
-        >>>         0.1,  # right foot
-        >>>     ]
-        >>> )
-        >>> model.clo = local_clo_typical_ensembles["briefs, socks, undershirt, work jacket, work pants, safety shoes"]["local_body_part"]
-        >>> # par should be input as int, float.
-        >>> model.par = 1.2  # Physical activity ratio [-], assuming a sitting position
-        >>> # posture should be input as int (0, 1, or 2) or str ("standing", "sitting" or "lying").
-        >>> # (0="standing", 1="sitting" or 2="lying")
-        >>> model.posture = "sitting"  # Posture [-], assuming a sitting position
-        >>>
-        >>> # Run JOS-3 model
-        >>> model.simulate(
-        >>>     times=30,  # Number of loops of a simulation
-        >>>     dtime=60,  # Time delta [sec]. The default is 60.
-        >>> )  # Exposure time = 30 [loops] * 60 [sec] = 30 [min]
-        >>> # Set the next condition (You only need to change the parameters that you want to change)
-        >>> model.to = 20  # Change operative temperature
-        >>> model.v = { # Air velocity [m/s], assuming to use a desk fan
-        >>>     'head' : 0.2,
-        >>>     'neck' : 0.4,
-        >>>     'chest' : 0.4,
-        >>>     'back': 0.1,
-        >>>     'pelvis' : 0.1,
-        >>>     'left_shoulder' : 0.4,
-        >>>     'left_arm' : 0.4,
-        >>>     'left_hand' : 0.4,
-        >>>     'right_shoulder' : 0.4,
-        >>>     'right_arm' : 0.4,
-        >>>     'right_hand' : 0.4,
-        >>>     'left_thigh' : 0.1,
-        >>>     'left_leg' : 0.1,
-        >>>     'left_foot' : 0.1,
-        >>>     'right_thigh' : 0.1,
-        >>>     'right_leg' : 0.1,
-        >>>     'right_foot' : 0.1
-        >>>     }
-        >>> # Run JOS-3 model
-        >>> model.simulate(
-        >>>     times=60,  # Number of loops of a simulation
-        >>>     dtime=60,  # Time delta [sec]. The default is 60.
-        >>> )  # Additional exposure time = 60 [loops] * 60 [sec] = 60 [min]
-        >>> # Set the next condition (You only need to change the parameters that you want to change)
-        >>> model.tdb = 30  # Change air temperature [°C]
-        >>> model.tr = 35  # Change mean radiant temperature [°C]
-        >>> # Run JOS-3 model
-        >>> model.simulate(
-        >>>     times=30,  # Number of loops of a simulation
-        >>>     dtime=60,  # Time delta [sec]. The default is 60.
-        >>> )  # Additional exposure time = 30 [loops] * 60 [sec] = 30 [min]
-        >>> # Show the results
-        >>> df = pd.DataFrame(model.dict_results())  # Make pandas.DataFrame
-        >>> df[["t_skin_mean", "t_skin_head", "t_skin_chest", "t_skin_left_hand"]].plot()  # Plot time series of local skin temperature.
-        >>> plt.legend(["Mean", "Head", "Chest", "Left hand"])  # Reset the legends
-        >>> plt.ylabel("Skin temperature [°C]")  # Set y-label as 'Skin temperature [°C]'
-        >>> plt.xlabel("Time [min]")  # Set x-label as 'Time [min]'
-        >>> plt.savefig(os.path.join(jos3_example_directory, "jos3_example2_skin_temperatures.png"))  # Save plot at the current directory
-        >>> plt.show()  # Show the plot
-        >>> # Exporting the results as csv
-        >>> model.to_csv(os.path.join(jos3_example_directory, "jos3_example2 (all output).csv"))
     """
 
     def __init__(
         self,
         height=1.72,
         weight=74.43,
         fat=15,
@@ -3549,50 +3351,265 @@
         ci=2.59,
         bmr_equation="harris-benedict",
         bsa_equation="dubois",
         ex_output=None,
     ):
         """Initialize a new instance of JOS3 class, which is designed to model
         and simulate various physiological parameters related to human
-        thermoregulation. This class uses mathematical models to calculate and
-        predict body temperature, basal metabolic rate, body surface area, and
+        thermoregulation.
+
+        This class uses mathematical models to calculate and predict
+        body temperature, basal metabolic rate, body surface area, and
         other related parameters.
 
         Parameters
         ----------
-        height float, optional
-            Body height, in [m].
-            The default is 1.72.
+        height : float, optional
+            body height, in [m]. The default is 1.72.
         weight : float, optional
-            Body weight, in [kg]. The default is 74.43.
+            body weight, in [kg]. The default is 74.43.
         fat : float, optional
             fat percentage, in [%]. The default is 15.
         age : int, optional
             age, in [years]. The default is 20.
         sex : str, optional
             sex ("male" or "female"). The default is "male".
         ci : float, optional
             Cardiac index, in [L/min/m2]. The default is 2.6432.
         bmr_equation : str, optional
             The equation used to calculate basal metabolic rate (BMR). Choose a BMR equation.
-            The default is "harris-benedict" equation created uding Caucasian's data. (https://doi.org/10.1073/pnas.4.12.370)
-            If the Ganpule's equation (https://doi.org/10.1038/sj.ejcn.1602645) for Japanese people is used, input "japanese".
+            The default is "harris-benedict" equation created uding Caucasian's data. (DOI: doi.org/10.1073/pnas.4.12.370)
+            If the Ganpule's equation (DOI: doi.org/10.1038/sj.ejcn.1602645) for Japanese people is used, input "japanese".
         bsa_equation : str, optional
             The equation used to calculate body surface area (bsa). Choose a bsa equation.
             You can choose "dubois", "fujimoto", "kruazumi", or "takahira". The default is "dubois".
+            The body surface area can be calculated using the function
+            :py:meth:`pythermalcomfort.utilities.body_surface_area`.
         ex_output : None, list or "all", optional
             This is used when you want to display results other than the default output parameters (ex.skin temperature);
             by default, JOS outputs only the most necessary parameters in order to reduce the computational load.
             If the parameters other than the default output parameters are needed,
             specify the list of the desired parameter names in string format like ["bf_skin", "bf_core", "t_artery"].
             If you want to display all output results, set ex_output is "all".
 
+        Attributes
+        ----------
+        tdb : float or array-like
+            Dry bulb air temperature [°C].
+        tr : float or array-like
+            Mean radiant temperature [°C].
+        to : float or array-like
+            Operative temperature [°C].
+        v : float or array-like
+            Air speed [m/s].
+        rh : float or array-like
+            Relative humidity [%].
+        clo : float or array-like
+            Clothing insulation [clo].
+            Note: If you want to input clothing insulation to each body part,
+            it can be input using the dictionaly in "utilities.py" in "jos3_function" folder.
+            :py:meth:`pythermalcomfort.jos3_functions.utilities.local_clo_typical_ensembles`.
+        par : float
+            Physical activity ratio [-].
+            This equals the ratio of metabolic rate to basal metabolic rate.
+            The par of sitting quietly is 1.2.
+        posture : str
+            Body posture [-]. Choose a posture from standing, sitting or lying.
+        body_temp : numpy.ndarray (85,)
+            All segment temperatures of JOS-3
+
+        Methods
+        -------
+        simulate(times, dtime, output):
+            Run JOS-3 model for given times.
+        dict_results():
+            Get results as a dictionary with pandas.DataFrame values.
+        to_csv(path=None, folder=None, unit=True, meaning=True):
+            Export results as csv format.
+
         Returns
         -------
-        None.
+        cardiac_output: cardiac output (the sum of the whole blood flow) [L/h]
+        cycle_time: the counts of executing one cycle calculation [-]
+        dt      : time step [sec]
+        pythermalcomfort_version: version of pythermalcomfort [-]
+        q_res   : heat loss by respiration [W]
+        q_skin2env: total heat loss from the skin (each body part) [W]
+        q_thermogenesis_total: total thermogenesis of the whole body [W]
+        simulation_time: simulation times [sec]
+        t_core  : core temperature (each body part) [°C]
+        t_skin  : skin temperature (each body part) [°C]
+        t_skin_mean: mean skin temperature [°C]
+        w       : skin wettedness (each body part) [-]
+        w_mean  : mean skin wettedness [-]
+        weight_loss_by_evap_and_res: weight loss by the evaporation and respiration of the whole body [g/sec]
+        OPTIONAL PARAMETERS : the paramters listed below are returned if ex_output = "all"
+        age     : age [years]
+        bf_ava_foot: AVA blood flow rate of one foot [L/h]
+        bf_ava_hand: AVA blood flow rate of one hand [L/h]
+        bf_core : core blood flow rate (each body part) [L/h]
+        bf_fat  : fat blood flow rate (each body part) [L/h]
+        bf_muscle: muscle blood flow rate (each body part) [L/h]
+        bf_skin : skin blood flow rate (each body part) [L/h]
+        bsa     : body surface area (each body part) [m2]
+        clo     : clothing insulation (each body part) [clo]
+        e_max   : maximum evaporative heat loss from the skin (each body part) [W]
+        e_skin  : evaporative heat loss from the skin (each body part) [W]
+        e_sweat : evaporative heat loss from the skin by only sweating (each body part) [W]
+        fat     : body fat rate [%]
+        height  : body height [m]
+        name    : name of the model [-]
+        par     : physical activity ratio [-]
+        q_bmr_core: core thermogenesis by basal metabolism (each body part) [W]
+        q_bmr_fat: fat thermogenesis by basal metabolism (each body part) [W]
+        q_bmr_muscle: muscle thermogenesis by basal metabolism (each body part) [W]
+        q_bmr_skin: skin thermogenesis by basal metabolism (each body part) [W]
+        q_nst   : core thermogenesis by non-shivering (each body part) [W]
+        q_res_latent: latent heat loss by respiration (each body part) [W]
+        q_res_sensible: sensible heat loss by respiration (each body part) [W]
+        q_shiv  : core or muscle thermogenesis by shivering (each body part) [W]
+        q_skin2env_latent: latent heat loss from the skin (each body part) [W]
+        q_skin2env_sensible: sensible heat loss from the skin (each body part) [W]
+        q_thermogenesis_core: core total thermogenesis (each body part) [W]
+        q_thermogenesis_fat: fat total thermogenesis (each body part) [W]
+        q_thermogenesis_muscle: muscle total thermogenesis (each body part) [W]
+        q_thermogenesis_skin: skin total thermogenesis (each body part) [W]
+        q_work  : core or muscle thermogenesis by work (each body part) [W]
+        r_et    : total clothing evaporative heat resistance (each body part) [(m2*kPa)/W]
+        r_t     : total clothing heat resistance (each body part) [(m2*K)/W]
+        rh      : relative humidity (each body part) [%]
+        sex     : sex [-]
+        t_artery: arterial temperature (each body part) [°C]
+        t_cb    : central blood temperature [°C]
+        t_core_set: core set point temperature (each body part) [°C]
+        t_fat   : fat temperature (each body part) [°C]
+        t_muscle: muscle temperature (each body part) [°C]
+        t_skin_set: skin set point temperature (each body part) [°C]
+        t_superficial_vein: superficial vein temperature (each body part) [°C]
+        t_vein  : vein temperature (each body part) [°C]
+        tdb     : dry bulb air temperature (each body part) [°C]
+        to      : operative temperature (each body part) [°C]
+        tr      : mean radiant temperature (each body part) [°C]
+        v       : air velocity (each body part) [m/s]
+        weight  : body weight [kg]
+
+
+        Examples
+        --------
+        Build a model and set a body built
+        Create an instance of the JOS3 class with optional body parameters such as body height, weight, age, sex, etc.
+
+        .. code-block:: python
+
+            >>> import numpy as np
+            >>> import pandas as pd
+            >>> import matplotlib.pyplot as plt
+            >>> import os
+            >>> from pythermalcomfort.models import JOS3
+            >>> from pythermalcomfort.jos3_functions.utilities import local_clo_typical_ensembles
+            >>>
+            >>> directory_name = "jos3_output_example"
+            >>> current_directory = os.getcwd()
+            >>> jos3_example_directory = os.path.join(current_directory, directory_name)
+            >>> if not os.path.exists(jos3_example_directory):
+            >>>     os.makedirs(jos3_example_directory)
+            >>>
+            >>> model = JOS3(
+            >>>     height=1.7,
+            >>>     weight=60,
+            >>>     fat=20,
+            >>>     age=30,
+            >>>     sex="male",
+            >>>     bmr_equation="japanese",
+            >>>     bsa_equation="fujimoto",
+            >>>     ex_output="all",
+            >>> )
+            >>> # Set environmental conditions such as air temperature, mean radiant temperature using the setter methods.
+            >>> # Set the first condition
+            >>> # Environmental parameters can be input as int, float, list, dict, numpy array format.
+            >>> model.tdb = 28  # Air temperature [°C]
+            >>> model.tr = 30  # Mean radiant temperature [°C]
+            >>> model.rh = 40  # Relative humidity [%]
+            >>> model.v = np.array( # Air velocity [m/s]
+            >>>     [
+            >>>         0.2,  # head
+            >>>         0.4,  # neck
+            >>>         0.4,  # chest
+            >>>         0.1,  # back
+            >>>         0.1,  # pelvis
+            >>>         0.4,  # left shoulder
+            >>>         0.4,  # left arm
+            >>>         0.4,  # left hand
+            >>>         0.4,  # right shoulder
+            >>>         0.4,  # right arm
+            >>>         0.4,  # right hand
+            >>>         0.1,  # left thigh
+            >>>         0.1,  # left leg
+            >>>         0.1,  # left foot
+            >>>         0.1,  # right thigh
+            >>>         0.1,  # right leg
+            >>>         0.1,  # right foot
+            >>>     ]
+            >>> )
+            >>> model.clo = local_clo_typical_ensembles["briefs, socks, undershirt, work jacket, work pants, safety shoes"]["local_body_part"]
+            >>> # par should be input as int, float.
+            >>> model.par = 1.2  # Physical activity ratio [-], assuming a sitting position
+            >>> # posture should be input as int (0, 1, or 2) or str ("standing", "sitting" or "lying").
+            >>> # (0="standing", 1="sitting" or 2="lying")
+            >>> model.posture = "sitting"  # Posture [-], assuming a sitting position
+            >>>
+            >>> # Run JOS-3 model
+            >>> model.simulate(
+            >>>     times=30,  # Number of loops of a simulation
+            >>>     dtime=60,  # Time delta [sec]. The default is 60.
+            >>> )  # Exposure time = 30 [loops] * 60 [sec] = 30 [min]
+            >>> # Set the next condition (You only need to change the parameters that you want to change)
+            >>> model.to = 20  # Change operative temperature
+            >>> model.v = { # Air velocity [m/s], assuming to use a desk fan
+            >>>     'head' : 0.2,
+            >>>     'neck' : 0.4,
+            >>>     'chest' : 0.4,
+            >>>     'back': 0.1,
+            >>>     'pelvis' : 0.1,
+            >>>     'left_shoulder' : 0.4,
+            >>>     'left_arm' : 0.4,
+            >>>     'left_hand' : 0.4,
+            >>>     'right_shoulder' : 0.4,
+            >>>     'right_arm' : 0.4,
+            >>>     'right_hand' : 0.4,
+            >>>     'left_thigh' : 0.1,
+            >>>     'left_leg' : 0.1,
+            >>>     'left_foot' : 0.1,
+            >>>     'right_thigh' : 0.1,
+            >>>     'right_leg' : 0.1,
+            >>>     'right_foot' : 0.1
+            >>>     }
+            >>> # Run JOS-3 model
+            >>> model.simulate(
+            >>>     times=60,  # Number of loops of a simulation
+            >>>     dtime=60,  # Time delta [sec]. The default is 60.
+            >>> )  # Additional exposure time = 60 [loops] * 60 [sec] = 60 [min]
+            >>> # Set the next condition (You only need to change the parameters that you want to change)
+            >>> model.tdb = 30  # Change air temperature [°C]
+            >>> model.tr = 35  # Change mean radiant temperature [°C]
+            >>> # Run JOS-3 model
+            >>> model.simulate(
+            >>>     times=30,  # Number of loops of a simulation
+            >>>     dtime=60,  # Time delta [sec]. The default is 60.
+            >>> )  # Additional exposure time = 30 [loops] * 60 [sec] = 30 [min]
+            >>> # Show the results
+            >>> df = pd.DataFrame(model.dict_results())  # Make pandas.DataFrame
+            >>> df[["t_skin_mean", "t_skin_head", "t_skin_chest", "t_skin_left_hand"]].plot()  # Plot time series of local skin temperature.
+            >>> plt.legend(["Mean", "Head", "Chest", "Left hand"])  # Reset the legends
+            >>> plt.ylabel("Skin temperature [°C]")  # Set y-label as 'Skin temperature [°C]'
+            >>> plt.xlabel("Time [min]")  # Set x-label as 'Time [min]'
+            >>> plt.savefig(os.path.join(jos3_example_directory, "jos3_example2_skin_temperatures.png"))  # Save plot at the current directory
+            >>> plt.show()  # Show the plot
+            >>> # Exporting the results as csv
+            >>> model.to_csv(os.path.join(jos3_example_directory, "jos3_example2 (all output).csv"))
         """
 
         # Version of pythermalcomfort
         version_string = (
             __version__  # get the current version of pythermalcomfort package
         )
         version_number_string = re.findall("\d+\.\d+\.\d+", version_string)[0]
@@ -3639,15 +3656,15 @@
         self._va = np.ones(17) * 0.1  # Air velocity [m/s]
         self._clo = np.zeros(17)  # Clothing insulation
         self._iclo = np.ones(17) * 0.45  # Clothing vapor permeation efficiency [-]
         self._par = 1.25  # Physical activity ratio [-]
         self._posture = "standing"  # Body posture [-]
         self._hc = None  # Convective heat transfer coefficient
         self._hr = None  # Radiative heat transfer coefficient
-        self.ex_q = np.zeros(NUM_NODES)  # External heat production
+        self.ex_q = np.zeros(NUM_NODES)  # External heat gain
         self._t = dt.timedelta(0)  # Elapsed time
         self._cycle = 0  # Cycle time
         self.model_name = "JOS3"  # Model name
         self.options = {
             "nonshivering_thermogenesis": True,
             "cold_acclimated": False,
             "shivering_threshold": False,
@@ -3667,15 +3684,17 @@
         self._t = dt.timedelta(0)  # Elapsed time
         self._cycle = 0  # Cycle time
 
         # Reset set-point temperature and save the last model parameters
         dictout = self._reset_setpt()
         self._history.append(dictout)
 
-    def _calculate_operative_temp_when_pmv_is_zero(self, va=0.1, rh=50, met=1, clo=0):
+    def _calculate_operative_temp_when_pmv_is_zero(
+        self, va: float = 0.1, rh: float = 50, met: float = 1, clo: float = 0
+    ) -> float:
         """Calculate operative temperature [°C] when PMV=0.
 
         Parameters
         ----------
         va : float, optional
             Air velocity [m/s]. The default is 0.1.
         rh : float, optional
@@ -3778,15 +3797,15 @@
         The function then calculates the total heat loss and gains, including respiratory,
         sweating, and extra heat gain, and builds the matrices required
         to solve for the new body temperature.
 
         It then calculates the new body temperature by solving the matrices using numpy's linalg library.
 
         Finally, the function returns a dictionary of the simulation results.
-        The output parameters include cycle time, model time, t_skin_mean, t_skin, t_core, w_mean, w, weight_loss_by_evap_and_res, cardiac_output, Q_total, q_res, and q_skin.
+        The output parameters include cycle time, model time, t_skin_mean, t_skin, t_core, w_mean, w, weight_loss_by_evap_and_res, cardiac_output, q_thermogenesis_total, q_res, and q_skin_env.
 
         Additionally, if the _ex_output variable is set to "all" or is a list of keys,
         the function also returns a detailed dictionary of all the thermoregulation parameters
         and other variables used in the simulation.
 
         Parameters
         ----------
@@ -3944,35 +3963,45 @@
             q_nst = np.zeros(17)
 
         # ------------------------------------------------------------------
         # Thermogenesis
         # ------------------------------------------------------------------
 
         # Calculate local basal metabolic rate (BMR) [W]
-        m_base = threg.local_mbase(
+        q_bmr_local = threg.local_mbase(
             self._height,
             self._weight,
             self._age,
             self._sex,
             self._bmr_equation,
         )
         # Calculate overall basal metabolic rate (BMR) [W]
-        m_base_all = sum([m.sum() for m in m_base])
+        q_bmr_total = sum([m.sum() for m in q_bmr_local])
 
         # Calculate thermogenesis by work [W]
-        q_work = threg.local_q_work(m_base_all, self._par)
+        q_work = threg.local_q_work(q_bmr_total, self._par)
 
         # Calculate the sum of thermogenesis in core, muscle, fat, skin [W]
-        q_core, q_muscle, q_fat, q_skin = threg.sum_m(
-            m_base,
+        (
+            q_thermogenesis_core,
+            q_thermogenesis_muscle,
+            q_thermogenesis_fat,
+            q_thermogenesis_skin,
+        ) = threg.sum_m(
+            q_bmr_local,
             q_work,
             q_shiv,
             q_nst,
         )
-        qall = q_core.sum() + q_muscle.sum() + q_fat.sum() + q_skin.sum()
+        q_thermogenesis_total = (
+            q_thermogenesis_core.sum()
+            + q_thermogenesis_muscle.sum()
+            + q_thermogenesis_fat.sum()
+            + q_thermogenesis_skin.sum()
+        )
 
         # ------------------------------------------------------------------
         # Others
         # ------------------------------------------------------------------
         # Calculate blood flow in core, muscle, fat [L/h]
         bf_core, bf_muscle, bf_fat = threg.cr_ms_fat_blood_flow(
             q_work,
@@ -3982,18 +4011,20 @@
             self._bsa_equation,
             self._age,
             self._ci,
         )
 
         # Calculate heat loss by respiratory
         p_a = threg.antoine(self._ta) * self._rh / 100
-        res_sh, res_lh = threg.resp_heat_loss(self._ta[0], p_a[0], qall)
+        res_sh, res_lh = threg.resp_heat_loss(
+            self._ta[0], p_a[0], q_thermogenesis_total
+        )
 
         # Calculate sensible heat loss [W]
-        shlsk = (tsk - to) / r_t * self._bsa
+        shl_sk = (tsk - to) / r_t * self._bsa
 
         # Calculate cardiac output [L/h]
         co = threg.sum_bf(bf_core, bf_muscle, bf_fat, bf_skin, bf_ava_hand, bf_ava_foot)
 
         # Calculate weight loss rate by evaporation [g/sec]
         wlesk = (e_sweat + 0.06 * e_max) / 2418
         wleres = res_lh / 2418
@@ -4058,18 +4089,18 @@
 
         # Matrix Q = Matrix for heat generation rate from thermogenesis, respiratory, sweating,
         # and extra heat gain processes in different body parts.
 
         # Matrix Q [W] / [J/K] * [sec] = [-]
         # Thermogensis
         arr_q = np.zeros(NUM_NODES)
-        arr_q[INDEX["core"]] += q_core
-        arr_q[INDEX["muscle"]] += q_muscle[VINDEX["muscle"]]
-        arr_q[INDEX["fat"]] += q_fat[VINDEX["fat"]]
-        arr_q[INDEX["skin"]] += q_skin
+        arr_q[INDEX["core"]] += q_thermogenesis_core
+        arr_q[INDEX["muscle"]] += q_thermogenesis_muscle[VINDEX["muscle"]]
+        arr_q[INDEX["fat"]] += q_thermogenesis_fat[VINDEX["fat"]]
+        arr_q[INDEX["skin"]] += q_thermogenesis_skin
 
         # Respiratory [W]
         arr_q[INDEX["core"][2]] -= res_sh + res_lh  # chest core
 
         # Sweating [W]
         arr_q[INDEX["skin"]] -= e_sk
 
@@ -4104,17 +4135,17 @@
             dict_out["t_skin_mean"] = self.t_skin_mean
             dict_out["t_skin"] = self.t_skin
             dict_out["t_core"] = self.t_core
             dict_out["w_mean"] = np.average(wet, weights=_BSAst)
             dict_out["w"] = wet
             dict_out["weight_loss_by_evap_and_res"] = wlesk.sum() + wleres
             dict_out["cardiac_output"] = co
-            dict_out["Q_total"] = qall
+            dict_out["q_thermogenesis_total"] = q_thermogenesis_total
             dict_out["q_res"] = res_sh + res_lh
-            dict_out["q_skin"] = shlsk + e_sk
+            dict_out["q_skin2env"] = shl_sk + e_sk
 
         detail_out = {}
         if self._ex_output and output:
             detail_out["name"] = self.model_name
             detail_out["height"] = self._height
             detail_out["weight"] = self._weight
             detail_out["bsa"] = self._bsa
@@ -4126,16 +4157,16 @@
             detail_out["t_cb"] = self.t_cb
             detail_out["t_artery"] = self.t_artery
             detail_out["t_vein"] = self.t_vein
             detail_out["t_superficial_vein"] = self.t_superficial_vein
             detail_out["t_muscle"] = self.t_muscle
             detail_out["t_fat"] = self.t_fat
             detail_out["to"] = to
-            detail_out["Rt"] = r_t
-            detail_out["Ret"] = r_et
+            detail_out["r_t"] = r_t
+            detail_out["r_et"] = r_et
             detail_out["tdb"] = self._ta.copy()
             detail_out["tr"] = self._tr.copy()
             detail_out["rh"] = self._rh.copy()
             detail_out["v"] = self._va.copy()
             detail_out["par"] = self._par
             detail_out["clo"] = self._clo.copy()
             detail_out["e_skin"] = e_sk
@@ -4143,27 +4174,29 @@
             detail_out["e_sweat"] = e_sweat
             detail_out["bf_core"] = bf_core
             detail_out["bf_muscle"] = bf_muscle[VINDEX["muscle"]]
             detail_out["bf_fat"] = bf_fat[VINDEX["fat"]]
             detail_out["bf_skin"] = bf_skin
             detail_out["bf_ava_hand"] = bf_ava_hand
             detail_out["bf_ava_foot"] = bf_ava_foot
-            detail_out["Q_bmr_core"] = m_base[0]
-            detail_out["Q_bmr_muscle"] = m_base[1][VINDEX["muscle"]]
-            detail_out["met_base_fat"] = m_base[2][VINDEX["fat"]]
-            detail_out["Q_bmr_skin"] = m_base[3]
-            detail_out["Q_work"] = q_work
-            detail_out["Q_shiv"] = q_shiv
-            detail_out["Q_nst"] = q_nst
-            detail_out["Q_core"] = q_core
-            detail_out["Q_muscle"] = q_muscle[VINDEX["muscle"]]
-            detail_out["Q_fat"] = q_fat[VINDEX["fat"]]
-            detail_out["Q_skin"] = q_skin
-            dict_out["q_skin_sensible"] = shlsk
-            dict_out["q_skin_latent"] = e_sk
+            detail_out["q_bmr_core"] = q_bmr_local[0]
+            detail_out["q_bmr_muscle"] = q_bmr_local[1][VINDEX["muscle"]]
+            detail_out["q_bmr_fat"] = q_bmr_local[2][VINDEX["fat"]]
+            detail_out["q_bmr_skin"] = q_bmr_local[3]
+            detail_out["q_work"] = q_work
+            detail_out["q_shiv"] = q_shiv
+            detail_out["q_nst"] = q_nst
+            detail_out["q_thermogenesis_core"] = q_thermogenesis_core
+            detail_out["q_thermogenesis_muscle"] = q_thermogenesis_muscle[
+                VINDEX["muscle"]
+            ]
+            detail_out["q_thermogenesis_fat"] = q_thermogenesis_fat[VINDEX["fat"]]
+            detail_out["q_thermogenesis_skin"] = q_thermogenesis_skin
+            dict_out["q_skin2env_sensible"] = shl_sk
+            dict_out["q_skin2env_latent"] = e_sk
             dict_out["q_res_sensible"] = res_sh
             dict_out["q_res_latent"] = res_lh
 
         if self._ex_output == "all":
             dict_out.update(detail_out)
         elif isinstance(self._ex_output, list):  # if ex_out type is list
             out_keys = detail_out.keys()
@@ -4182,19 +4215,19 @@
         """
         if not self._history:
             print("The model has no data.")
             return None
 
         def check_word_contain(word, *args):
             """Check if word contains *args."""
-            boolfilter = False
+            bool_filter = False
             for arg in args:
                 if arg in word:
-                    boolfilter = True
-            return boolfilter
+                    bool_filter = True
+            return bool_filter
 
         # Set column titles
         # If the values are iter, add the body names as suffix words.
         # If the values are not iter and the single value data, convert it to iter.
         key2keys = {}  # Column keys
         for key, value in self._history[0].items():
             try:
@@ -4229,15 +4262,21 @@
 
         out_dict = dict(zip(data[0].keys(), [[] for _ in range(len(data[0].keys()))]))
         for row in data:
             for k in data[0].keys():
                 out_dict[k].append(row[k])
         return out_dict
 
-    def to_csv(self, path=None, folder=None, unit=True, meaning=True):
+    def to_csv(
+        self,
+        path: str = None,
+        folder: str = None,
+        unit: bool = True,
+        meaning: bool = True,
+    ) -> None:
         """Export results as csv format.
 
         Parameters
         ----------
         path : str, optional
             Output path. If you don't use the default file name, set a name.
             The default is None.
@@ -4246,37 +4285,41 @@
             set a only folder path.
             The default is None.
         unit : bool, optional
             Write units in csv file. The default is True.
         meaning : bool, optional
             Write meanings of the parameters in csv file. The default is True.
 
+        Returns
+        -------
+        None
+
         Examples
         ----------
         >>> from pythermalcomfort.models import JOS3
         >>> model = JOS3()
         >>> model.simulate(60)
         >>> model.to_csv()
         """
 
         # Use the model name and current time as default output file name
         if path is None:
-            nowtime = dt.datetime.now().strftime("%Y%m%d-%H%M%S")
-            path = "{}_{}.csv".format(self.model_name, nowtime)
+            now_time = dt.datetime.now().strftime("%Y%m%d-%H%M%S")
+            path = "{}_{}.csv".format(self.model_name, now_time)
             if folder:
                 os.makedirs(folder, exist_ok=True)
                 path = folder + os.sep + path
         elif not ((path[-4:] == ".csv") or (path[-4:] == ".txt")):
             path += ".csv"
 
         # Get simulation results as a dictionary
-        dictout = self.dict_results()
+        dict_out = self.dict_results()
 
         # Get column names, units and meanings
-        columns = [k for k in dictout.keys()]
+        columns = [k for k in dict_out.keys()]
         units = []
         meanings = []
         for col in columns:
             param, body_name = remove_body_name(col)
             if param in ALL_OUT_PARAMS:
                 u = ALL_OUT_PARAMS[param]["unit"]
                 units.append(u)
@@ -4296,23 +4339,20 @@
         with open(path, "wt", newline="", encoding="utf-8-sig") as f:
             writer = csv.writer(f)
             writer.writerow(list(columns))
             if unit:
                 writer.writerow(units)
             if meaning:
                 writer.writerow(meanings)
-            for i in range(len(dictout["cycle_time"])):
+            for i in range(len(dict_out["cycle_time"])):
                 row = []
                 for k in columns:
-                    row.append(dictout[k][i])
+                    row.append(dict_out[k][i])
                 writer.writerow(row)
 
-    # --------------------------------------------------------------------------
-    # Setter
-    # --------------------------------------------------------------------------
     def _set_ex_q(self, tissue, value):
         """Set extra heat gain by tissue name.
 
         Parameters
         ----------
         tissue : str
             Tissue name. "core", "skin", or "artery".... If you set value to
@@ -4324,57 +4364,43 @@
         -------
         array
             Extra heat gain of model.
         """
         self.ex_q[INDEX[tissue]] = value
         return self.ex_q
 
-    # --------------------------------------------------------------------------
-    # Setter & getter
-    # --------------------------------------------------------------------------
-
     @property
     def tdb(self):
-        """
-        Getter
+        """Dry-bulb air temperature. The setter accepts int, float, dict, list,
+        ndarray. The inputs are used to create a 17-element array. dict should
+        be passed with BODY_NAMES as keys.
+
         Returns
         -------
-        tdb : numpy.ndarray (17,)
-            Air temperature [°C].
+        ndarray
+            A NumPy array of shape (17,).
         """
         return self._ta
 
     @tdb.setter
     def tdb(self, inp):
         self._ta = _to17array(inp)
 
     @property
     def tr(self):
-        """
-        Getter
-        Returns
-        -------
-        tr : numpy.ndarray (17,)
-            Mean radiant temperature [°C].
-        """
+        """tr : numpy.ndarray (17,) Mean radiant temperature [°C]."""
         return self._tr
 
     @tr.setter
     def tr(self, inp):
         self._tr = _to17array(inp)
 
     @property
     def to(self):
-        """
-        Getter
-        Returns
-        -------
-        to : numpy.ndarray (17,)
-            Operative temperature [°C].
-        """
+        """to : numpy.ndarray (17,) Operative temperature [°C]."""
         hc = threg.fixed_hc(
             threg.conv_coef(
                 self._posture,
                 self._va,
                 self._ta,
                 self.t_skin,
             ),
@@ -4396,51 +4422,33 @@
     @to.setter
     def to(self, inp):
         self._ta = _to17array(inp)
         self._tr = _to17array(inp)
 
     @property
     def rh(self):
-        """
-        Getter
-        Returns
-        -------
-        rh : numpy.ndarray (17,)
-            Relative humidity [%].
-        """
+        """rh : numpy.ndarray (17,) Relative humidity [%]."""
         return self._rh
 
     @rh.setter
     def rh(self, inp):
         self._rh = _to17array(inp)
 
     @property
     def v(self):
-        """
-        Getter
-        Returns
-        -------
-        v : numpy.ndarray (17,)
-            Air velocity [m/s].
-        """
+        """v : numpy.ndarray (17,) Air velocity [m/s]."""
         return self._va
 
     @v.setter
     def v(self, inp):
         self._va = _to17array(inp)
 
     @property
     def posture(self):
-        """
-        Getter
-        Returns
-        -------
-        posture : str
-            Current JOS3 posture.
-        """
+        """posture : str Current JOS3 posture."""
         return self._posture
 
     @posture.setter
     def posture(self, inp):
         if inp == 0:
             self._posture = "standing"
         elif inp == 1:
@@ -4457,83 +4465,47 @@
         else:
             self._posture = "standing"
             print('posture must be 0="standing", 1="sitting" or 2="lying".')
             print('posture was set "standing".')
 
     @property
     def clo(self):
-        """
-        Getter
-        Returns
-        -------
-        clo : numpy.ndarray (17,)
-            Clothing insulation [clo].
-        """
+        """clo : numpy.ndarray (17,) Clothing insulation [clo]."""
         return self._clo
 
     @clo.setter
     def clo(self, inp):
         self._clo = _to17array(inp)
 
     @property
     def par(self):
-        """
-        Getter
-        Returns
-        -------
-        par : float
-            Physical activity ratio [-].
-            This equals the ratio of metabolic rate to basal metabolic rate.
-            par of sitting quietly is 1.2.
-        """
+        """par : float Physical activity ratio [-].This equals the ratio of metabolic rate to basal metabolic rate. par of sitting quietly is 1.2."""
         return self._par
 
     @par.setter
     def par(self, inp):
         self._par = inp
 
     @property
     def body_temp(self):
-        """
-        Getter
-        Returns
-        -------
-        bodytemp : numpy.ndarray (85,)
-            All segment temperatures of JOS-3
-        """
+        """body_temp : numpy.ndarray (85,) All segment temperatures of JOS-3"""
         return self._bodytemp
 
     @body_temp.setter
     def body_temp(self, inp):
         self._bodytemp = inp.copy()
 
-    # --------------------------------------------------------------------------
-    # Getter
-    # --------------------------------------------------------------------------
-
     @property
     def bsa(self):
-        """
-        Getter
-        Returns
-        -------
-        bsa : numpy.ndarray (17,)
-            Body surface areas by local body segments [m2].
-        """
+        """bsa : numpy.ndarray (17,) Body surface areas by local body segments [m2]."""
         return self._bsa.copy()
 
     @property
-    def r_dry(self):
-        """
-        Getter
-        Returns
-        -------
-        r_dry : numpy.ndarray (17,)
-            Dry heat resistances between the skin and ambience areas by local body segments [K.m2/W].
-        """
+    def r_t(self):
+        """r_t : numpy.ndarray (17,) Dry heat resistances between the skin and ambience areas by local body segments [(m2*K)/W]."""
         hc = threg.fixed_hc(
             threg.conv_coef(
                 self._posture,
                 self._va,
                 self._ta,
                 self.t_skin,
             ),
@@ -4543,197 +4515,108 @@
             threg.rad_coef(
                 self._posture,
             )
         )
         return threg.dry_r(hc, hr, self._clo)
 
     @property
-    def r_lat(self):
-        """
-        Getter
-        Returns
-        -------
-        r_lat : numpy.ndarray (17,)
-            w (Evaporative) heat resistances between the skin and ambience areas by local body segments [Pa.m2/W].
-        """
+    def r_et(self):
+        """r_et : numpy.ndarray (17,) w (Evaporative) heat resistances between the skin and ambience areas by local body segments [(m2*kPa)/W]."""
         hc = threg.fixed_hc(
             threg.conv_coef(
                 self._posture,
                 self._va,
                 self._ta,
                 self.t_skin,
             ),
             self._va,
         )
         return threg.wet_r(hc, self._clo, self._iclo)
 
     @property
     def w(self):
-        """
-        Getter
-        Returns
-        -------
-        w : numpy.ndarray (17,)
-            Skin wettedness on local body segments [-].
-        """
+        """w : numpy.ndarray (17,) Skin wettedness on local body segments [-]."""
         err_cr = self.t_core - self.setpt_cr
         err_sk = self.t_skin - self.setpt_sk
         wet, *_ = threg.evaporation(
-            err_cr, err_sk, self._ta, self._rh, self.r_lat, self._bsa_rate, self._age
+            err_cr, err_sk, self._ta, self._rh, self.r_et, self._bsa_rate, self._age
         )
         return wet
 
     @property
     def w_mean(self):
-        """
-        Getter
-        Returns
-        -------
-        w_mean : float
-            Mean skin wettedness of the whole body [-].
-        """
+        """w_mean : float Mean skin wettedness of the whole body [-]."""
         wet = self.w
         return np.average(wet, weights=_BSAst)
 
     @property
     def t_skin_mean(self):
-        """
-        Getter
-        Returns
-        -------
-        t_skin_mean : float
-            Mean skin temperature of the whole body [°C].
-        """
+        """t_skin_mean : float Mean skin temperature of the whole body [°C]."""
         return np.average(self._bodytemp[INDEX["skin"]], weights=_BSAst)
 
     @property
     def t_skin(self):
-        """
-        Getter
-        Returns
-        -------
-        t_skin : numpy.ndarray (17,)
-            Skin temperatures by the local body segments [°C].
-        """
+        """t_skin : numpy.ndarray (17,) Skin temperatures by the local body segments [°C]."""
         return self._bodytemp[INDEX["skin"]].copy()
 
     @property
     def t_core(self):
-        """
-        Getter
-        Returns
-        -------
-        t_core : numpy.ndarray (17,)
-            Skin temperatures by the local body segments [°C].
-        """
+        """t_core : numpy.ndarray (17,) Skin temperatures by the local body segments [°C]."""
         return self._bodytemp[INDEX["core"]].copy()
 
     @property
     def t_cb(self):
-        """
-        Getter
-        Returns
-        -------
-        t_cb : numpy.ndarray (1,)
-            Temperature at central blood pool [°C].
-        """
+        """t_cb : numpy.ndarray (1,) Temperature at central blood pool [°C]."""
         return self._bodytemp[0].copy()
 
     @property
     def t_artery(self):
-        """
-        Getter
-        Returns
-        -------
-        t_artery : numpy.ndarray (17,)
-            Arterial temperatures by the local body segments [°C].
-        """
+        """t_artery : numpy.ndarray (17,) Arterial temperatures by the local body segments [°C]."""
         return self._bodytemp[INDEX["artery"]].copy()
 
     @property
     def t_vein(self):
-        """
-        Getter
-        Returns
-        -------
-        t_vein : numpy.ndarray (17,)
-            Vein temperatures by the local body segments [°C].
-        """
+        """t_vein : numpy.ndarray (17,) Vein temperatures by the local body segments [°C]."""
         return self._bodytemp[INDEX["vein"]].copy()
 
     @property
     def t_superficial_vein(self):
-        """
-        Getter
-        Returns
-        -------
-        t_superficial_vein : numpy.ndarray (12,)
-            Superfical vein temperatures by the local body segments [°C].
-        """
+        """t_superficial_vein : numpy.ndarray (12,) Superficial vein temperatures by the local body segments [°C]."""
         return self._bodytemp[INDEX["sfvein"]].copy()
 
     @property
     def t_muscle(self):
-        """
-        Getter
-        Returns
-        -------
-        t_muscle : numpy.ndarray (2,)
-            Muscle temperatures of head and pelvis [°C].
-        """
+        """t_muscle : numpy.ndarray (2,) Muscle temperatures of head and pelvis [°C]."""
         return self._bodytemp[INDEX["muscle"]].copy()
 
     @property
     def t_fat(self):
-        """
-        Getter
-        Returns
-        -------
-        t_fat : numpy.ndarray (2,)
-            fat temperatures of head and pelvis  [°C].
-        """
+        """t_fat : numpy.ndarray (2,) fat temperatures of head and pelvis  [°C]."""
         return self._bodytemp[INDEX["fat"]].copy()
 
     @property
     def body_names(self):
-        """
-        Getter
-        Returns
-        -------
-        body_names : list
-            JOS3 body names
-        """
+        """body_names : list JOS3 body names"""
         return BODY_NAMES
 
     @property
     def results(self):
+        """Results of the model: dict."""
         return self.dict_results()
 
     @property
     def bmr(self):
-        """
-        Getter
-        Returns
-        -------
-        bmr : float
-            Basal metabolic rate [W/m2].
-        """
+        """bmr : float Basal metabolic rate [W/m2]."""
         tcr = threg.basal_met(
             self._height,
             self._weight,
             self._age,
             self._sex,
             self._bmr_equation,
         )
         return tcr / self.bsa.sum()
 
     @property
     def version(self):
-        """
-        Getter
-        Returns
-        -------
-        version : float
-            The current version of pythermalcomfort.
-        """
+        """version : float The current version of pythermalcomfort."""
 
         return self._version
```

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/optimized_functions.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/optimized_functions.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/psychrometrics.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/psychrometrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     ----------
     tdb: float
         air temperature, [°C]
 
     Returns
     -------
     p_sat: float
-        operative temperature, [Pa]
+        saturation vapor pressure, [Pa]
     """
 
     ta_k = tdb + c_to_k
     c1 = -5674.5359
     c2 = 6.3925247
     c3 = -0.9677843 * math.pow(10, -2)
     c4 = 0.62215701 * math.pow(10, -6)
```

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort/utilities.py` & `pythermalcomfort-2.8.0/src/pythermalcomfort/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,18 @@
         return 0.202 * (weight**0.425) * (height**0.725)
     elif formula == "takahira":
         return 0.2042 * (weight**0.425) * (height**0.725)
     elif formula == "fujimoto":
         return 0.1882 * (weight**0.444) * (height**0.663)
     elif formula == "kurazumi":
         return 0.2440 * (weight**0.383) * (height**0.693)
+    else:
+        raise ValueError(
+            f"This {formula} to calculate the body_surface_area does not exists."
+        )
 
 
 def f_svv(w, h, d):
     """Calculates the sky-vault view fraction.
 
     Parameters
     ----------
@@ -460,15 +464,15 @@
     "Trousers, long-sleeve shirt": 0.61,
     "Knee-length skirt, long-sleeve shirt, full slip": 0.67,
     "Sweat pants, long-sleeve sweatshirt": 0.74,
     "Jacket, Trousers, long-sleeve shirt": 0.96,
     "Typical winter indoor clothing": 1.0,
 }
 
-# Clo values of individual clothing elements. To calculate the total clothing insulation you need to add these values together.
+#: Clo values of individual clothing elements. To calculate the total clothing insulation you need to add these values together.
 clo_individual_garments = {
     "Metal chair": 0.00,
     "Bra": 0.01,
     "Wooden stool": 0.01,
     "Ankle socks": 0.02,
     "Shoes or sandals": 0.02,
     "Slippers": 0.03,
@@ -520,15 +524,15 @@
     "Long sleeve shirt (thick)": 0.36,
     "Single-breasted coat (thin)": 0.36,
     "Single-breasted coat (thick)": 0.44,
     "Double-breasted coat (thin)": 0.42,
     "Double-breasted coat (thick)": 0.48,
 }
 
-# This dictionary contains the reflection coefficients, Fr, for different special materials
+#: This dictionary contains the reflection coefficients, Fr, for different special materials
 f_r_garments = {
     "Cotton with aluminium paint": 0.42,
     "Viscose with glossy aluminium foil": 0.19,
     "Aramid (Kevlar) with glossy aluminium foil": 0.14,
     "Wool with glossy aluminium foil": 0.12,
     "Cotton with glossy aluminium foil": 0.04,
     "Viscose vacuum metallized with aluminium": 0.06,
```

### Comparing `pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/SOURCES.txt` & `pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 src/pythermalcomfort.egg-info/PKG-INFO
 src/pythermalcomfort.egg-info/SOURCES.txt
 src/pythermalcomfort.egg-info/dependency_links.txt
 src/pythermalcomfort.egg-info/entry_points.txt
 src/pythermalcomfort.egg-info/not-zip-safe
 src/pythermalcomfort.egg-info/requires.txt
 src/pythermalcomfort.egg-info/top_level.txt
+src/pythermalcomfort/jos3_functions/__init__.py
 src/pythermalcomfort/jos3_functions/construction.py
 src/pythermalcomfort/jos3_functions/matrix.py
 src/pythermalcomfort/jos3_functions/parameters.py
 src/pythermalcomfort/jos3_functions/thermoregulation.py
 src/pythermalcomfort/jos3_functions/utilities.py
 tests/test_jos3.py
 tests/test_models.py
```

### Comparing `pythermalcomfort-2.7.2/tests/test_models.py` & `pythermalcomfort-2.8.0/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import numpy as np
 import json
 import warnings
 import requests
+from itertools import product
 
 from pythermalcomfort.optimized_functions import pmv_ppd_optimized, utci_optimized
 from pythermalcomfort.models import (
     solar_gain,
     pmv_ppd,
     set_tmp,
     cooling_effect,
@@ -44,43 +45,46 @@
 from pythermalcomfort.utilities import (
     transpose_sharp_altitude,
     f_svv,
     clo_dynamic,
     running_mean_outdoor_temperature,
     units_converter,
     body_surface_area,
+    v_relative,
 )
 
 # get file containing validation tables
 url = "https://raw.githubusercontent.com/FedericoTartarini/validation-data-comfort-models/main/validation_data.json"
 resp = requests.get(url)
 reference_tables = json.loads(resp.text)
 
 # fmt: off
 data_test_set_ip = [  # I have commented the lines of code that don't pass the test
     {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 74.9},
+    {'tdb': 32, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 53.7},
+    {'tdb': 50, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 62.3},
     {'tdb': 59, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 66.5},
     {'tdb': 68, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 70.7},
     {'tdb': 86, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 79.6},
     {'tdb': 104, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 93.8},
     {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 10, 'met': 1, 'clo': 0.5, 'set': 74.0},
     {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 90, 'met': 1, 'clo': 0.5, 'set': 76.8},
     {'tdb': 77, 'tr': 77, 'v': 19.7 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 75.2},
     {'tdb': 77, 'tr': 77, 'v': 118.1 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 70.4},
     {'tdb': 77, 'tr': 77, 'v': 216.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 68.4},
     {'tdb': 77, 'tr': 77, 'v': 590.6 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 65.6},
     {'tdb': 77, 'tr': 50, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 59.6},
     {'tdb': 77, 'tr': 104, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 88.9},
+    {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.1, 'set': 69.3},
     {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 1, 'set': 81.0},
-    {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 2, 'set': 90.4},
+    {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 2, 'set': 90.3},
     {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 4, 'set': 99.7},
     {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 0.8, 'clo': 0.5, 'set': 73.9},
-    {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.1, 'set': 69.3},
-    {'tdb': 50, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 62.3},
-    {'tdb': 32, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 1, 'clo': 0.5, 'set': 53.7},
+    {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 2, 'clo': 0.5, 'set': 78.7},
+    {'tdb': 77, 'tr': 77, 'v': 29.5 / 60, 'rh': 50, 'met': 4, 'clo': 0.5, 'set': 86.8},
     ]
 
 data_test_pmv_ip = [  # I have commented the lines of code that don't pass the test
     {'tdb': 67.3, 'rh': 86, 'vr': 20 / 60, 'met': 1.1, 'clo': 1, 'pmv': -0.5, 'ppd': 10},
     {'tdb': 75.0, 'rh': 66, 'vr': 20 / 60, 'met': 1.1, 'clo': 1, 'pmv': 0.5, 'ppd': 10},
     {'tdb': 78.2, 'rh': 15, 'vr': 20 / 60, 'met': 1.1, 'clo': 1, 'pmv': 0.5, 'ppd': 10},
     {'tdb': 70.2, 'rh': 20, 'vr': 20 / 60, 'met': 1.1, 'clo': 1, 'pmv': -0.5, 'ppd': 10},
@@ -332,28 +336,25 @@
             clo=0.5,
             units="IP",
         )
     ) == 75.8
 
     for row in data_test_set_ip:
         assert (
-            abs(
-                set_tmp(
-                    row["tdb"],
-                    row["tr"],
-                    row["v"],
-                    row["rh"],
-                    row["met"],
-                    row["clo"],
-                    units="IP",
-                    limit_inputs=False,
-                )
-                - row["set"]
+            set_tmp(
+                row["tdb"],
+                row["tr"],
+                row["v"],
+                row["rh"],
+                row["met"],
+                row["clo"],
+                units="IP",
+                limit_inputs=False,
             )
-            < 0.11
+            == row["set"]
         )
 
     # checking that returns np.nan when outside standard applicability limits
     np.testing.assert_equal(
         set_tmp(
             [41, 20, 20, 20, 20, 39],
             [20, 41, 20, 20, 20, 39],
@@ -550,14 +551,71 @@
         "t_wb": 18.0,
         "t_dp": 13.8,
         "h": 50259.66,
     }
 
 
 def test_cooling_effect():
+
+    t_range = np.arange(10, 40, 10)
+    rh_range = np.arange(10, 75, 25)
+    v_range = np.arange(0.1, 4, 1)
+    all_combinations = list(product(t_range, rh_range, v_range))
+    results = [
+        0,
+        8.19,
+        10.94,
+        12.54,
+        0,
+        8.05,
+        10.77,
+        12.35,
+        0,
+        7.91,
+        10.6,
+        12.16,
+        0,
+        5.04,
+        6.62,
+        7.51,
+        0,
+        4.84,
+        6.37,
+        7.24,
+        0,
+        4.64,
+        6.12,
+        6.97,
+        0,
+        3.64,
+        4.32,
+        4.69,
+        0,
+        3.55,
+        4.25,
+        4.61,
+        0,
+        3.4,
+        4.1,
+        4.46,
+    ]
+    for ix, comb in enumerate(all_combinations):
+        pytest.approx(
+            cooling_effect(
+                tdb=comb[0],
+                tr=comb[0],
+                rh=comb[1],
+                vr=comb[2],
+                met=1,
+                clo=0.5,
+            )
+            == results[ix],
+            0.1,
+        )
+
     assert (cooling_effect(tdb=25, tr=25, vr=0.05, rh=50, met=1, clo=0.6)) == 0
     assert (cooling_effect(tdb=25, tr=25, vr=0.5, rh=50, met=1, clo=0.6)) == 2.17
     assert (cooling_effect(tdb=27, tr=25, vr=0.5, rh=50, met=1, clo=0.6)) == 1.85
     assert (cooling_effect(tdb=29, tr=25, vr=0.5, rh=50, met=1, clo=0.6)) == 1.63
     assert (cooling_effect(tdb=31, tr=25, vr=0.5, rh=50, met=1, clo=0.6)) == 1.42
     assert (cooling_effect(tdb=25, tr=27, vr=0.5, rh=50, met=1, clo=0.6)) == 2.44
     assert (cooling_effect(tdb=25, tr=29, vr=0.5, rh=50, met=1, clo=0.6)) == 2.81
@@ -601,14 +659,33 @@
         0.975312404754648,
     ]
     assert (units_converter(pressure=1, area=1 / 0.09, from_units="ip")) == [
         101325,
         1.0322474090590033,
     ]
 
+    expected_result = [25.0, 3.047]
+    assert np.allclose(units_converter("ip", tdb=77, v=10), expected_result, atol=0.01)
+
+    # Test case 2: Conversion from SI to IP for temperature and velocity
+    expected_result = [68, 6.562]
+    assert np.allclose(units_converter("si", tdb=20, v=2), expected_result, atol=0.01)
+
+    # Test case 3: Conversion from IP to SI for area and pressure
+    expected_result = [9.29, 1489477.5]
+    assert np.allclose(
+        units_converter("ip", area=100, pressure=14.7), expected_result, atol=0.01
+    )
+
+    # Test case 4: Conversion from SI to IP for area and pressure
+    expected_result = [538.199, 1]
+    assert np.allclose(
+        units_converter("si", area=50, pressure=101325), expected_result, atol=0.01
+    )
+
 
 def test_p_sat():
     assert (p_sat(tdb=25)) == 3169.2
     assert (p_sat(tdb=50)) == 12349.9
 
 
 def test_t_mrt():
@@ -861,14 +938,27 @@
 
 
 def test_clo_dynamic():
     assert (clo_dynamic(clo=1, met=1, standard="ASHRAE")) == 1
     assert (clo_dynamic(clo=1, met=0.5, standard="ASHRAE")) == 1
     assert (clo_dynamic(clo=2, met=0.5, standard="ASHRAE")) == 2
 
+    # Test ASHRAE standard
+    assert np.allclose(clo_dynamic(1.0, 1.0), np.array(1))
+    assert np.allclose(clo_dynamic(1.0, 1.2), np.array(1))
+    assert np.allclose(clo_dynamic(1.0, 2.0), np.array(0.8))
+
+    # Test ISO standard
+    assert np.allclose(clo_dynamic(1.0, 1.0, standard="ISO"), np.array(1))
+    assert np.allclose(clo_dynamic(1.0, 2.0, standard="ISO"), np.array(0.8))
+
+    # Test invalid standard input
+    with pytest.raises(ValueError):
+        clo_dynamic(1.0, 1.0, standard="invalid")
+
 
 def test_phs():
     assert phs(tdb=40, tr=40, rh=33.85, v=0.3, met=150, clo=0.5, posture=2) == {
         "d_lim_loss_50": 440.0,
         "d_lim_loss_95": 298.0,
         "d_lim_t_re": 480.0,
         "water_loss": 6166.4,
@@ -1063,14 +1153,20 @@
             phs(tdb=40, tr=40, rh=61, v=2, met=150, clo=0.5, posture=2),
             UserWarning,
         )
 
 
 def test_body_surface_area():
     assert body_surface_area(weight=80, height=1.8) == 1.9917607971689137
+    assert body_surface_area(70, 1.8, "dubois") == pytest.approx(1.88, rel=1e-2)
+    assert body_surface_area(75, 1.75, "takahira") == pytest.approx(1.91, rel=1e-2)
+    assert body_surface_area(80, 1.7, "fujimoto") == pytest.approx(1.872, rel=1e-2)
+    assert body_surface_area(85, 1.65, "kurazumi") == pytest.approx(1.89, rel=1e-2)
+    with pytest.raises(ValueError):
+        body_surface_area(70, 1.8, "invalid_formula")
 
 
 def test_t_o():
     assert t_o(25, 25, 0.1) == 25
     assert round(t_o(25, 30, 0.3), 2) == 26.83
     assert round(t_o(20, 30, 0.3), 2) == 23.66
     assert t_o(25, 25, 0.1, standard="ASHRAE") == 25
@@ -1223,7 +1319,27 @@
 
 
 def test_e_pmv():
     np.testing.assert_equal(
         e_pmv([24, 30], 30, vr=0.22, rh=50, met=1.4, clo=0.5, e_coefficient=0.6),
         [0.29, 0.91],
     )
+
+
+def test_v_relative():
+    # Test case when met is equal to or lower than 1
+    v = 2.0
+    met = 1.0
+    expected_result = v
+    assert np.allclose(v_relative(v, met), expected_result)
+
+    # Test case when met is greater than 1
+    v = np.array([1.0, 2.0, 3.0])
+    met = 2.0
+    expected_result = np.array([1.3, 2.3, 3.3])
+    assert np.allclose(v_relative(v, met), expected_result, atol=1e-6)
+
+    # Test case with negative values for v
+    v = -1.5
+    met = 1.5
+    expected_result = -1.5 + 0.3 * 0.5
+    assert np.allclose(v_relative(v, met), expected_result, atol=1e-6)
```

### Comparing `pythermalcomfort-2.7.2/tox.ini` & `pythermalcomfort-2.8.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 ; a generative tox configuration, see: https://tox.readthedocs.io/en/latest/config.html#generative-envlist
 
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py36,py37,py38,py39,py310},
+    {py38,py39,py310},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
-    py36: {env:TOXPYTHON:python3.6}
-    py37: {env:TOXPYTHON:python3.7}
     py39: {env:TOXPYTHON:python3.8}
-    {py39,docs}: {env:TOXPYTHON:python3.9}
-    py310: {env:TOXPYTHON:python3.10}
+    py39: {env:TOXPYTHON:python3.9}
+    {py310,docs}: {env:TOXPYTHON:python3.10}
     {bootstrap,clean,check,report,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop = false
```

