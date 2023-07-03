# Comparing `tmp/target_permutation_importances-1.0.7.tar.gz` & `tmp/target_permutation_importances-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_permutation_importances-1.0.7.tar", max compression
+gzip compressed data, was "target_permutation_importances-1.0.8.tar", max compression
```

## Comparing `target_permutation_importances-1.0.7.tar` & `target_permutation_importances-1.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7450 2023-07-03 06:22:22.499940 target_permutation_importances-1.0.7/README.md
--rw-r--r--   0        0        0      995 2023-07-03 06:22:22.503941 target_permutation_importances-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     7363 2023-07-03 06:22:22.503941 target_permutation_importances-1.0.7/target_permutation_importances/__init__.py
--rw-r--r--   0        0        0     8043 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     7532 2023-07-03 06:51:37.433254 target_permutation_importances-1.0.8/README.md
+-rw-r--r--   0        0        0     1315 2023-07-03 06:51:37.437256 target_permutation_importances-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7363 2023-07-03 06:51:37.437256 target_permutation_importances-1.0.8/target_permutation_importances/__init__.py
+-rw-r--r--   0        0        0     8507 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.8/PKG-INFO
```

### Comparing `target_permutation_importances-1.0.7/README.md` & `target_permutation_importances-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Target Permutation Importances
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
 [![image](https://img.shields.io/pypi/v/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
 [![image](https://img.shields.io/pypi/pyversions/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
 [![Actions status](https://github.com/kingychiu/target-permutation-importances/workflows/CI/badge.svg)](https://github.com/kingychiu/target-permutation-importances/actions/workflows/main.yaml)
 
-
+[Source & Bug Report](https://github.com/kingychiu/target-permutation-importances)
 
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package
```

### Comparing `target_permutation_importances-1.0.7/pyproject.toml` & `target_permutation_importances-1.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [tool.poetry]
 name = "target-permutation-importances"
-version = "1.0.7"
+version = "1.0.8"
 description = "Compute (Target) Permutation Importances of a machine learning model"
 authors = ["Anthony Chiu <kingychiu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "target_permutation_importances"}]
+homepage = "https://github.com/kingychiu/target-permutation-importances"
+repository = "https://github.com/kingychiu/target-permutation-importances"
+documentation = "https://github.com/kingychiu/target-permutation-importances"
+keywords = ["feature selection", "feature ranking", "feature importances", "kaggle", "machine learning"]
 
 [project.urls]
-"Homepage" = "https://github.com/kingychiu/target-permutation-importances"
-"Bug Tracker" = "https://github.com/kingychiu/target-permutation-importances/issues"
+Repository = "https://github.com/kingychiu/target-permutation-importances" 
+Homepage = "https://github.com/kingychiu/target-permutation-importances"
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 numpy = "^1.21.0"
 pandas = "^1.5.3"
 tqdm = "^4.48.2"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.275"
```

### Comparing `target_permutation_importances-1.0.7/target_permutation_importances/__init__.py` & `target_permutation_importances-1.0.8/target_permutation_importances/__init__.py`

 * *Files identical despite different names*

### Comparing `target_permutation_importances-1.0.7/PKG-INFO` & `target_permutation_importances-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: target-permutation-importances
-Version: 1.0.7
+Version: 1.0.8
 Summary: Compute (Target) Permutation Importances of a machine learning model
+Home-page: https://github.com/kingychiu/target-permutation-importances
+Keywords: feature selection,feature ranking,feature importances,kaggle,machine learning
 Author: Anthony Chiu
 Author-email: kingychiu@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: tqdm (>=4.48.2,<5.0.0)
+Project-URL: Documentation, https://github.com/kingychiu/target-permutation-importances
+Project-URL: Repository, https://github.com/kingychiu/target-permutation-importances
 Description-Content-Type: text/markdown
 
 # Target Permutation Importances
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
 [![image](https://img.shields.io/pypi/v/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
 [![image](https://img.shields.io/pypi/pyversions/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
 [![Actions status](https://github.com/kingychiu/target-permutation-importances/workflows/CI/badge.svg)](https://github.com/kingychiu/target-permutation-importances/actions/workflows/main.yaml)
 
-
+[Source & Bug Report](https://github.com/kingychiu/target-permutation-importances)
 
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package
```

