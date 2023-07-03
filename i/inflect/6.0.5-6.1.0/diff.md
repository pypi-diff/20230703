# Comparing `tmp/inflect-6.0.5.tar.gz` & `tmp/inflect-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inflect-6.0.5.tar", last modified: Sun Jul  2 19:10:59 2023, max compression
+gzip compressed data, was "inflect-6.1.0.tar", last modified: Sun Jul  2 19:12:42 2023, max compression
```

## Comparing `inflect-6.0.5.tar` & `inflect-6.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.721276 inflect-6.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-02 19:10:39.000000 inflect-6.0.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 19:10:39.000000 inflect-6.0.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-02 19:10:39.000000 inflect-6.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.709276 inflect-6.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 19:10:39.000000 inflect-6.0.5/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-02 19:10:39.000000 inflect-6.0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.709276 inflect-6.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-02 19:10:39.000000 inflect-6.0.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 19:10:39.000000 inflect-6.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 19:10:39.000000 inflect-6.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 19:10:39.000000 inflect-6.0.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-02 19:10:39.000000 inflect-6.0.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-02 19:10:39.000000 inflect-6.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-07-02 19:10:59.721276 inflect-6.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19541 2023-07-02 19:10:39.000000 inflect-6.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.709276 inflect-6.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-02 19:10:39.000000 inflect-6.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 19:10:39.000000 inflect-6.0.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 19:10:39.000000 inflect-6.0.5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.713276 inflect-6.0.5/inflect/
--rw-r--r--   0 runner    (1001) docker     (123)   103763 2023-07-02 19:10:39.000000 inflect-6.0.5/inflect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:39.000000 inflect-6.0.5/inflect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.713276 inflect-6.0.5/inflect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 19:10:59.000000 inflect-6.0.5/inflect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-02 19:10:39.000000 inflect-6.0.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 19:10:39.000000 inflect-6.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-02 19:10:39.000000 inflect-6.0.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-02 19:10:59.721276 inflect-6.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:10:59.721276 inflect-6.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/inflections.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_an.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_ancient.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_herd.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_person.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_classical_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_compounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_inflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_numwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_pl_si.py
--rw-r--r--   0 runner    (1001) docker     (123)    46037 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-02 19:10:39.000000 inflect-6.0.5/tests/test_unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 19:10:39.000000 inflect-6.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:42.320695 inflect-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-02 19:12:21.000000 inflect-6.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 19:12:21.000000 inflect-6.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:42.320695 inflect-6.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 19:12:21.000000 inflect-6.1.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-02 19:12:21.000000 inflect-6.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:42.320695 inflect-6.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-02 19:12:21.000000 inflect-6.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 19:12:21.000000 inflect-6.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 19:12:21.000000 inflect-6.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 19:12:21.000000 inflect-6.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-02 19:12:21.000000 inflect-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-02 19:12:21.000000 inflect-6.1.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-02 19:12:42.320695 inflect-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-07-02 19:12:21.000000 inflect-6.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:42.320695 inflect-6.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-02 19:12:21.000000 inflect-6.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-02 19:12:21.000000 inflect-6.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 19:12:21.000000 inflect-6.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:42.320695 inflect-6.1.0/inflect/
+-rw-r--r--   0 runner    (1001) docker     (123)   103328 2023-07-02 19:12:21.000000 inflect-6.1.0/inflect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:21.000000 inflect-6.1.0/inflect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:42.320695 inflect-6.1.0/inflect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-02 19:12:42.000000 inflect-6.1.0/inflect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-02 19:12:42.000000 inflect-6.1.0/inflect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:12:42.000000 inflect-6.1.0/inflect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 19:12:42.000000 inflect-6.1.0/inflect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 19:12:42.000000 inflect-6.1.0/inflect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-02 19:12:21.000000 inflect-6.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-02 19:12:21.000000 inflect-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-02 19:12:21.000000 inflect-6.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-02 19:12:42.324695 inflect-6.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:12:42.320695 inflect-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/inflections.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_an.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_classical_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_classical_ancient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_classical_herd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_classical_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_classical_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_classical_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_compounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_inflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_numwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_pl_si.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46037 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-02 19:12:21.000000 inflect-6.1.0/tests/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-02 19:12:21.000000 inflect-6.1.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-02 19:12:21.000000 inflect-6.1.0/tox.ini
```

### Comparing `inflect-6.0.5/.github/workflows/main.yml` & `inflect-6.1.0/.github/workflows/main.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -35,57 +38,51 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
@@ -100,14 +97,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `inflect-6.0.5/CHANGES.rst` & `inflect-6.1.0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+v6.1.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v6.0.5
 ======
 
-* Pin to Pydantic 1 to avoid breaking in Pydantic 2.
+* #187: Pin to Pydantic 1 to avoid breaking in Pydantic 2.
 
 v6.0.4
 ======
 
 * Internal cleanup.
 
 v6.0.3
```

### Comparing `inflect-6.0.5/LICENSE` & `inflect-6.1.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `inflect-6.0.5/PKG-INFO` & `inflect-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.0.5
+Version: 6.1.0
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,28 +12,32 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/inflect.svg
    :target: https://pypi.org/project/inflect
 
 .. image:: https://img.shields.io/pypi/pyversions/inflect.svg
 
 .. image:: https://github.com/jaraco/inflect/workflows/tests/badge.svg
    :target: https://github.com/jaraco/inflect/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/inflect/badge/?version=latest
    :target: https://inflect.readthedocs.io/en/latest/?badge=latest
```

### Comparing `inflect-6.0.5/README.rst` & `inflect-6.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/inflect.svg
 
 .. image:: https://github.com/jaraco/inflect/workflows/tests/badge.svg
    :target: https://github.com/jaraco/inflect/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/inflect/badge/?version=latest
    :target: https://inflect.readthedocs.io/en/latest/?badge=latest
```

### Comparing `inflect-6.0.5/docs/conf.py` & `inflect-6.1.0/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `inflect-6.0.5/inflect/__init__.py` & `inflect-6.1.0/inflect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1723,74 +1723,52 @@
 
 plverb_irregular_pres = {
     "am": "are",
     "are": "are",
     "is": "are",
     "was": "were",
     "were": "were",
-    "was": "were",
-    "have": "have",
     "have": "have",
     "has": "have",
     "do": "do",
-    "do": "do",
     "does": "do",
 }
 
 plverb_ambiguous_pres = {
     "act": "act",
-    "act": "act",
     "acts": "act",
     "blame": "blame",
-    "blame": "blame",
     "blames": "blame",
     "can": "can",
-    "can": "can",
-    "can": "can",
-    "must": "must",
-    "must": "must",
     "must": "must",
     "fly": "fly",
-    "fly": "fly",
     "flies": "fly",
     "copy": "copy",
-    "copy": "copy",
     "copies": "copy",
     "drink": "drink",
-    "drink": "drink",
     "drinks": "drink",
     "fight": "fight",
-    "fight": "fight",
     "fights": "fight",
     "fire": "fire",
-    "fire": "fire",
     "fires": "fire",
     "like": "like",
-    "like": "like",
     "likes": "like",
     "look": "look",
-    "look": "look",
     "looks": "look",
     "make": "make",
-    "make": "make",
     "makes": "make",
     "reach": "reach",
-    "reach": "reach",
     "reaches": "reach",
     "run": "run",
-    "run": "run",
     "runs": "run",
     "sink": "sink",
-    "sink": "sink",
     "sinks": "sink",
     "sleep": "sleep",
-    "sleep": "sleep",
     "sleeps": "sleep",
     "view": "view",
-    "view": "view",
     "views": "view",
 }
 
 plverb_ambiguous_pres_keys = re.compile(
     fr"^({enclose('|'.join(plverb_ambiguous_pres))})((\s.*)?)$", re.IGNORECASE
 )
 
@@ -3653,15 +3631,15 @@
                 post = nth[n % 100]
             except KeyError:
                 post = nth[n % 10]
             return f"{num}{post}"
         else:
             # Mad props to Damian Conway (?) whose ordinal()
             # algorithm is type-bendy enough to foil MyPy
-            str_num: str = num  # type:	ignore[assignment]
+            str_num: str = num  # type: ignore[assignment]
             mo = ordinal_suff.search(str_num)
             if mo:
                 post = ordinal[mo.group(1)]
                 rval = ordinal_suff.sub(post, str_num)
             else:
                 rval = f"{str_num}th"
             return rval
```

### Comparing `inflect-6.0.5/inflect.egg-info/PKG-INFO` & `inflect-6.1.0/inflect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.0.5
+Version: 6.1.0
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,28 +12,32 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/inflect.svg
    :target: https://pypi.org/project/inflect
 
 .. image:: https://img.shields.io/pypi/pyversions/inflect.svg
 
 .. image:: https://github.com/jaraco/inflect/workflows/tests/badge.svg
    :target: https://github.com/jaraco/inflect/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/inflect/badge/?version=latest
    :target: https://inflect.readthedocs.io/en/latest/?badge=latest
```

### Comparing `inflect-6.0.5/inflect.egg-info/SOURCES.txt` & `inflect-6.1.0/inflect.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .coveragerc
 .editorconfig
-.flake8
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
```

### Comparing `inflect-6.0.5/pytest.ini` & `inflect-6.1.0/pytest.ini`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 addopts=--doctest-modules
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `inflect-6.0.5/setup.cfg` & `inflect-6.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Text Processing :: Linguistic
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	pydantic >= 1.9.1, < 2
 keywords = plural inflect participle
 
 [options.packages.find]
 exclude = 
 	build*
@@ -33,23 +33,21 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	pygments
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
```

### Comparing `inflect-6.0.5/tests/inflections.txt` & `inflect-6.1.0/tests/inflections.txt`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_an.py` & `inflect-6.1.0/tests/test_an.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_classical_all.py` & `inflect-6.1.0/tests/test_classical_all.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_classical_ancient.py` & `inflect-6.1.0/tests/test_classical_ancient.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_classical_herd.py` & `inflect-6.1.0/tests/test_classical_herd.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_classical_names.py` & `inflect-6.1.0/tests/test_classical_names.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_classical_person.py` & `inflect-6.1.0/tests/test_classical_person.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_classical_zero.py` & `inflect-6.1.0/tests/test_classical_zero.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_compounds.py` & `inflect-6.1.0/tests/test_compounds.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_inflections.py` & `inflect-6.1.0/tests/test_inflections.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_join.py` & `inflect-6.1.0/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_numwords.py` & `inflect-6.1.0/tests/test_numwords.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tests/test_pwd.py` & `inflect-6.1.0/tests/test_pwd.py`

 * *Files identical despite different names*

### Comparing `inflect-6.0.5/tox.ini` & `inflect-6.1.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
@@ -21,14 +17,24 @@
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```

