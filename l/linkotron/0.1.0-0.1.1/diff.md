# Comparing `tmp/linkotron-0.1.0.tar.gz` & `tmp/linkotron-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul  3 15:34:41 2023, max compression
+gzip compressed data, last modified: Mon Jul  3 15:53:52 2023, max compression
```

## Comparing `linkotron-0.1.0.tar` & `linkotron-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      391 2023-07-03 15:34:41.000000 linkotron-0.1.0/.coveragerc
--rw-r--r--   0        0        0      313 2023-07-03 15:34:41.000000 linkotron-0.1.0/.editorconfig
--rw-r--r--   0        0        0       30 2023-07-03 15:34:41.000000 linkotron-0.1.0/.flake8
--rw-r--r--   0        0        0     1794 2023-07-03 15:34:41.000000 linkotron-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      826 2023-07-03 15:34:41.000000 linkotron-0.1.0/RELEASING.md
--rw-r--r--   0        0        0      501 2023-07-03 15:34:41.000000 linkotron-0.1.0/tox.ini
--rw-r--r--   0        0        0     1134 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/labels.yml
--rw-r--r--   0        0        0      892 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      350 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/renovate.json
--rw-r--r--   0        0        0     1755 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      389 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      298 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      490 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1305 2023-07-03 15:34:41.000000 linkotron-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1704 2023-07-03 15:34:41.000000 linkotron-0.1.0/src/linkotron/__init__.py
--rw-r--r--   0        0        0      105 2023-07-03 15:34:41.000000 linkotron-0.1.0/src/linkotron/__main__.py
--rw-r--r--   0        0        0     1034 2023-07-03 15:34:41.000000 linkotron-0.1.0/src/linkotron/cli.py
--rw-r--r--   0        0        0        0 2023-07-03 15:34:41.000000 linkotron-0.1.0/src/linkotron/scripts/__init__.py
--rw-r--r--   0        0        0      575 2023-07-03 15:34:41.000000 linkotron-0.1.0/src/linkotron/scripts/run_command.py
--rw-r--r--   0        0        0        0 2023-07-03 15:34:41.000000 linkotron-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1374 2023-07-03 15:34:41.000000 linkotron-0.1.0/tests/test_linkotron.py
--rw-r--r--   0        0        0     3077 2023-07-03 15:34:41.000000 linkotron-0.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2023-07-03 15:34:41.000000 linkotron-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3582 2023-07-03 15:34:41.000000 linkotron-0.1.0/README.md
--rw-r--r--   0        0        0     1566 2023-07-03 15:34:41.000000 linkotron-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4877 2023-07-03 15:34:41.000000 linkotron-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      391 2023-07-03 15:53:52.000000 linkotron-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      313 2023-07-03 15:53:52.000000 linkotron-0.1.1/.editorconfig
+-rw-r--r--   0        0        0       30 2023-07-03 15:53:52.000000 linkotron-0.1.1/.flake8
+-rw-r--r--   0        0        0     1794 2023-07-03 15:53:52.000000 linkotron-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      826 2023-07-03 15:53:52.000000 linkotron-0.1.1/RELEASING.md
+-rw-r--r--   0        0        0      501 2023-07-03 15:53:52.000000 linkotron-0.1.1/tox.ini
+-rw-r--r--   0        0        0     1134 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/labels.yml
+-rw-r--r--   0        0        0      892 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      389 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      490 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1305 2023-07-03 15:53:52.000000 linkotron-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1704 2023-07-03 15:53:52.000000 linkotron-0.1.1/src/linkotron/__init__.py
+-rw-r--r--   0        0        0      105 2023-07-03 15:53:52.000000 linkotron-0.1.1/src/linkotron/__main__.py
+-rw-r--r--   0        0        0     1034 2023-07-03 15:53:52.000000 linkotron-0.1.1/src/linkotron/cli.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:53:52.000000 linkotron-0.1.1/src/linkotron/scripts/__init__.py
+-rw-r--r--   0        0        0      575 2023-07-03 15:53:52.000000 linkotron-0.1.1/src/linkotron/scripts/run_command.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:53:52.000000 linkotron-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1374 2023-07-03 15:53:52.000000 linkotron-0.1.1/tests/test_linkotron.py
+-rw-r--r--   0        0        0     3077 2023-07-03 15:53:52.000000 linkotron-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1079 2023-07-03 15:53:52.000000 linkotron-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3582 2023-07-03 15:53:52.000000 linkotron-0.1.1/README.md
+-rw-r--r--   0        0        0     1458 2023-07-03 15:53:52.000000 linkotron-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4768 2023-07-03 15:53:52.000000 linkotron-0.1.1/PKG-INFO
```

### Comparing `linkotron-0.1.0/.pre-commit-config.yaml` & `linkotron-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/RELEASING.md` & `linkotron-0.1.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/.github/labels.yml` & `linkotron-0.1.1/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/.github/release-drafter.yml` & `linkotron-0.1.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/.github/workflows/deploy.yml` & `linkotron-0.1.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/.github/workflows/release-drafter.yml` & `linkotron-0.1.1/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/.github/workflows/test.yml` & `linkotron-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/src/linkotron/__init__.py` & `linkotron-0.1.1/src/linkotron/__init__.py`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/src/linkotron/cli.py` & `linkotron-0.1.1/src/linkotron/cli.py`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/src/linkotron/scripts/run_command.py` & `linkotron-0.1.1/src/linkotron/scripts/run_command.py`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/tests/test_linkotron.py` & `linkotron-0.1.1/tests/test_linkotron.py`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/.gitignore` & `linkotron-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/LICENSE.txt` & `linkotron-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/README.md` & `linkotron-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `linkotron-0.1.0/pyproject.toml` & `linkotron-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -32,18 +32,14 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = [
   "version",
 ]
-dependencies = [
-  'pyperclip; platform_system == "Darwin"',
-  'pyperclip; platform_system == "Windows"',
-]
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-cov",
 ]
 [project.urls]
 Changelog = "https://github.com/hugovk/linkotron/releases"
```

### Comparing `linkotron-0.1.0/PKG-INFO` & `linkotron-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkotron
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI to format links
 Project-URL: Changelog, https://github.com/hugovk/linkotron/releases
 Project-URL: Homepage, https://github.com/hugovk/linkotron
 Project-URL: Source, https://github.com/hugovk/linkotron
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
@@ -18,16 +18,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: pyperclip; platform_system == 'Darwin'
-Requires-Dist: pyperclip; platform_system == 'Windows'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # linkotron
```

