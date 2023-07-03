# Comparing `tmp/cascade-config-0.3.0.tar.gz` & `tmp/cascade_config-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cascade-config-0.3.0.tar", last modified: Mon Nov 15 10:31:39 2021, max compression
+gzip compressed data, was "cascade_config-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cascade-config-0.3.0.tar` & `cascade_config-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0      852 2021-11-15 10:31:29.386444 cascade-config-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1886 2021-11-15 10:31:29.386444 cascade-config-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1881 2021-11-15 10:31:29.386444 cascade-config-0.3.0/.gitignore
--rw-r--r--   0        0        0      798 2021-11-15 10:31:29.386444 cascade-config-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2298 2021-11-15 10:31:29.386444 cascade-config-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2021-11-15 10:31:29.390444 cascade-config-0.3.0/LICENSE
--rw-r--r--   0        0        0     2218 2021-11-15 10:31:29.390444 cascade-config-0.3.0/README.md
--rw-r--r--   0        0        0     8351 2021-11-15 10:31:29.390444 cascade-config-0.3.0/cascade_config.py
--rw-r--r--   0        0        0      638 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/Makefile
--rw-r--r--   0        0        0      799 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/make.bat
--rw-r--r--   0        0        0       63 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/requirements.txt
--rw-r--r--   0        0        0       67 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/source/api.rst
--rw-r--r--   0        0        0       34 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     3356 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0       37 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/source/contributing.rst
--rw-r--r--   0        0        0      119 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0       20 2021-11-15 10:31:29.390444 cascade-config-0.3.0/docs/source/usage.rst
--rw-r--r--   0        0        0      787 2021-11-15 10:31:29.390444 cascade-config-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5003 2021-11-15 10:31:29.390444 cascade-config-0.3.0/tests/test_cascade_config.py
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 cascade-config-0.3.0/setup.py
--rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 cascade-config-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      609 2023-07-03 12:55:10.212758 cascade_config-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1842 2023-07-03 12:55:10.212758 cascade_config-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1881 2023-07-03 12:55:10.212758 cascade_config-0.3.1/.gitignore
+-rw-r--r--   0        0        0      132 2023-07-03 12:55:10.212758 cascade_config-0.3.1/.readthedocs.yml
+-rw-r--r--   0        0        0      926 2023-07-03 12:55:10.212758 cascade_config-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1973 2023-07-03 12:55:10.212758 cascade_config-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-07-03 12:55:10.212758 cascade_config-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2218 2023-07-03 12:55:10.212758 cascade_config-0.3.1/README.md
+-rw-r--r--   0        0        0     8668 2023-07-03 12:55:10.212758 cascade_config-0.3.1/cascade_config.py
+-rw-r--r--   0        0        0      638 2023-07-03 12:55:10.212758 cascade_config-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-07-03 12:55:10.212758 cascade_config-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0       67 2023-07-03 12:55:10.212758 cascade_config-0.3.1/docs/source/api.rst
+-rw-r--r--   0        0        0       34 2023-07-03 12:55:10.212758 cascade_config-0.3.1/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2913 2023-07-03 12:55:10.212758 cascade_config-0.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0       37 2023-07-03 12:55:10.212758 cascade_config-0.3.1/docs/source/contributing.rst
+-rw-r--r--   0        0        0      125 2023-07-03 12:55:10.212758 cascade_config-0.3.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1189 2023-07-03 12:55:10.212758 cascade_config-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5003 2023-07-03 12:55:10.212758 cascade_config-0.3.1/tests/test_cascade_config.py
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 cascade_config-0.3.1/PKG-INFO
```

### Comparing `cascade-config-0.3.0/.github/workflows/publish.yml` & `cascade_config-0.3.1/.github/workflows/publish.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 name: Publish to PyPI and GitHub release
 
 on:
-  push:
-    tags:
-    - 'v*'
+  release:
+    types: [created]
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v2
 
@@ -24,15 +23,7 @@
     - name: Build and publish to PyPI
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: |
         flit build
         twine upload dist/*
-
-    - name: Create GitHub Release
-      uses: docker://antonyurchenko/git-release:v4
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        DRAFT_RELEASE: "false"
-        PRE_RELEASE: "false"
-        CHANGELOG_FILE: "CHANGELOG.md"
```

### Comparing `cascade-config-0.3.0/.github/workflows/test.yml` & `cascade_config-0.3.1/.github/workflows/test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 name: Test Python package
 
-on: [push, pull_request]
+on:
+  push:
+    branches:
+      - main
+  pull_request:
 
 jobs:
   full_test:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v2
-      with:
-        python-version: 3.8
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install flit flake8
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-    - name: Lint with flake8
-      run: |
-        # stop the build if there are Python syntax errors or undefined names
-        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-    - name: Install with Flit
-      run: flit install
-    - name: Test with pytest
-      run: |
-        pytest --cov=cascade_config tests
-    - name: Uploade coverage reports to Codecov
-      uses: codecov/codecov-action@v1.0.12
+      - uses: actions/checkout@v2
+
+      - name: Set up Python 3.8
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.8
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install flit flake8
+
+      - name: Lint with flake8
+        run: |
+          # stop the build if there are Python syntax errors or undefined names
+          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
+          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+
+      - name: Install with Flit
+        run: flit install
+
+      - name: Test with pytest
+        run: |
+          pytest --cov=cascade_config tests
+
+      - name: Upload coverage reports to Codecov
+        uses: codecov/codecov-action@v3
 
   test_platforms:
-    runs-on: ${{ matrix.os }}
+    runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8]
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v2
+
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
+
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flit flake8
+
       - name: Lint with flake8
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+
       - name: Install project
         run: flit install
+
       - name: Test with pytest
         run: |
           pytest
```

### Comparing `cascade-config-0.3.0/.gitignore` & `cascade_config-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cascade-config-0.3.0/CHANGELOG.md` & `cascade_config-0.3.1/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 # Changelog
+
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.1] - 03/07/2023
+
+### Fixed
+
+- Fix previous broken build (did not include changes)
+
 ## [0.3.0] - 15/11/2021
+
+### Fixed
+
 - Fix parsing of empty dictionaries and `False` configuration values. These would
   previously be overridden by the downstream configuration.
 
 ## [0.2.0] - 28/09/2021
+
+### Added
+
 - Add none_overrides_value option. Before this change, None values would unexpectedly
   override previously configured values. Now, the previous value will be retained if
   newer values are None. The old behavior can be re-enabled with by setting the
   none_overrides_value argument of CascadeConfig to True.
 
 ## [0.1.0-a0] - 03/08/2020
+
+### Added
+
 - Initial release
```

### Comparing `cascade-config-0.3.0/CONTRIBUTING.md` & `cascade_config-0.3.1/CONTRIBUTING.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,48 +8,40 @@
 If you have an idea for a feature, use case to add or an approach for a bugfix,
 you are welcome to communicate it with the community by creating an issue in
 [GitHub issues](https://github.com/ralfg/cascade-config/issues).
 
 ## How to contribute
 
 - Fork [cascade-config](https://github.com/ralfg/cascade-config) on GitHub to
-make your changes.
+  make your changes.
 - Commit and push your changes to your
-[fork](https://help.github.com/articles/pushing-to-a-remote/).
+  [fork](https://help.github.com/articles/pushing-to-a-remote/).
 - Open a
-[pull request](https://help.github.com/articles/creating-a-pull-request/)
-with these changes. You pull request message ideally should include:
-   - A description of why the changes should be made.
-   - A description of the implementation of the changes.
-   - A description of how to test the changes.
+  [pull request](https://help.github.com/articles/creating-a-pull-request/)
+  with these changes. You pull request message ideally should include:
+  - A description of why the changes should be made.
+  - A description of the implementation of the changes.
+  - A description of how to test the changes.
 - The pull request should pass all the continuous integration tests which are
   automatically run by
   [GitHub Actions](https://github.com/ralfg/cascade-config/actions).
 
-
 ## Development setup
 
 1. Setup Python 3 and [Flit](https://flit.readthedocs.io/en/latest/)
 2. Clone the [cascade-config repository](https://github.com/ralfg/cascade-config) and
    run `flit install` to setup an editable version of cascade-config.
 
-
 ## Development workflow
 
 - When a new version is ready to be published:
 
-    1. Change the `__version__` in `cascade_config.py` following
-    [semantic versioning](https://semver.org/).
-    2. Update the documentation (`README.md` and `docs/source/usage.rst`) if required.
-    3. Update the changelog (if not already done) in `CHANGELOG.md` according to
-    [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
-    4. Commit all final changes to the `master` branch.
-    4. On `master`, set a new tag with the version number, e.g. `git tag v0.1.5`.
-    5. Push to GitHub, with the tag: `git push; git push --tags`.
-
-- When a new tag is pushed to (or made on) GitHub that matches `v*`, the
-following GitHub Actions are triggered:
-
-    1. The Python package is build and published to PyPI.
-    2. Using the [Git Release](https://github.com/marketplace/actions/git-release)
-    action, a new GitHub release is made with the changes that are listed in
-    `CHANGELOG.md`.
+  1. Change the `__version__` in `cascade_config.py` following
+     [semantic versioning](https://semver.org/).
+  2. Update the documentation (`README.md` and `docs/source/usage.rst`) if required.
+  3. Update the changelog (if not already done) in `CHANGELOG.md` according to
+     [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
+  4. Merge all final changes into the `main` branch.
+  5. Create a new GitHub release.
+
+- When a new GitHub release is created, the publish GitHub Action is triggered,
+  building the Python package is build and publishes it to PyPI.
```

### Comparing `cascade-config-0.3.0/LICENSE` & `cascade_config-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cascade-config-0.3.0/README.md` & `cascade_config-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cascade-config-0.3.0/cascade_config.py` & `cascade_config-0.3.1/cascade_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Cascading configuration from the CLI and config files."""
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 import json
 import os
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, Namespace
 from typing import Dict
 
@@ -51,51 +51,65 @@
         else:
             self._validation_schema = None
 
     def _update_dict_recursively(self, original: Dict, updater: Dict) -> Dict:
         """Update dictionary recursively."""
         for k, v in updater.items():
             if isinstance(v, dict):
-                original[k] = self._update_dict_recursively(original.get(k, {}), v)
+                if not v:  # v is not None, v is empty dictionary
+                    original[k] = dict()
+                else:
+                    original[k] = self._update_dict_recursively(original.get(k, {}), v)
+            elif isinstance(v, bool):
+                original[k] = v  # v is True or False
             elif v or k not in original:  # v is not None, or key does not exist yet
                 original[k] = v
-            elif self.none_overrides_value:  # v is None, but can override previous value
+            elif (
+                self.none_overrides_value
+            ):  # v is None, but can override previous value
                 original[k] = v
         return original
 
     def add_dict(self, *args, **kwargs):
         """
         Add dictionary configuration source to source list.
-        *args and **kwargs are passed to :class:`cascade_config.DictConfigSource()`.
+
+        ``*args`` and ``**kwargs`` are passed to :class:`cascade_config.DictConfigSource()`.
 
         """
         source = DictConfigSource(*args, **kwargs)
         self.sources.append(source)
 
     def add_argumentparser(self, *args, **kwargs):
         """
         Add argumentparser configuration source to source list.
-        *args and **kwargs are passed to :class:`cascade_config.ArgumentParserConfigSource()`.
+
+        ``*args`` and ``**kwargs`` are passed to
+        :class:`cascade_config.ArgumentParserConfigSource()`.
 
         """
         source = ArgumentParserConfigSource(*args, **kwargs)
         self.sources.append(source)
 
     def add_namespace(self, *args, **kwargs):
         """
         Add argparse Namespace configuration source to source list.
-        *args and **kwargs are passed to :class:`cascade_config.NamespaceConfigSource()`.
+
+        ``*args`` and ``**kwargs`` are passed to
+        :class:`cascade_config.NamespaceConfigSource()`.
         """
         source = NamespaceConfigSource(*args, **kwargs)
         self.sources.append(source)
 
     def add_json(self, *args, **kwargs):
         """
         Add JSON configuration source to source list.
-        *args and **kwargs are passed to :class:`cascade_config.JSONConfigSource()`.
+
+        ``*args`` and ``**kwargs`` are passed to
+        :class:`cascade_config.JSONConfigSource()`.
         """
         source = JSONConfigSource(*args, **kwargs)
         self.sources.append(source)
 
     def parse(self) -> Dict:
         """Parse all sources, cascade, validate, and return cascaded configuration."""
         config = dict()
```

### Comparing `cascade-config-0.3.0/docs/Makefile` & `cascade_config-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cascade-config-0.3.0/docs/make.bat` & `cascade_config-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cascade-config-0.3.0/tests/test_cascade_config.py` & `cascade_config-0.3.1/tests/test_cascade_config.py`

 * *Files identical despite different names*

### Comparing `cascade-config-0.3.0/PKG-INFO` & `cascade_config-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: cascade-config
-Version: 0.3.0
+Version: 0.3.1
 Summary: Cascading configuration from the CLI and config files.
-Home-page: https://github.com/RalfG/cascade-config
-Keywords: configuration, command line interface, configuration files, JSON
-Author: RalfG
-Author-email: ralf@gabriels.dev
+Keywords: configuration,command line interface,configuration files,JSON
+Author-email: Ralf Gabriels <ralf@gabriels.dev>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Dist: jsonschema>=3,<4
+Requires-Dist: jsonschema>=3
+Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: numpydoc>=1,<2 ; extra == "docs"
+Requires-Dist: recommonmark ; extra == "docs"
+Requires-Dist: sphinx-mdinclude ; extra == "docs"
+Requires-Dist: toml ; extra == "docs"
+Requires-Dist: semver>=2 ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme ; extra == "docs"
+Requires-Dist: sphinx-autobuild ; extra == "docs"
 Requires-Dist: pytest>=6,<7 ; extra == "test"
 Requires-Dist: pytest-cov>=2,<3 ; extra == "test"
-Provides-Extra: dev
+Project-URL: GitHub, https://github.com/RalfG/cascade-config
+Project-URL: ReadTheDocs, https://cascade-config.readthedocs.io/en/stable/
+Provides-Extra: docs
 Provides-Extra: test
 
 # cascade-config
 
 [![](https://flat.badgen.net/pypi/v/cascade-config?icon=pypi)](https://pypi.org/project/cascade-config)
 [![](https://flat.badgen.net/github/release/ralfg/cascade-config)](https://github.com/ralfg/cascade-config/releases)
 [![](https://flat.badgen.net/github/checks/ralfg/cascade-config/)](https://github.com/ralfg/cascade-config/actions)
```

